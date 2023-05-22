# Comparing `tmp/azure-eventgrid-4.9.0b1.zip` & `tmp/azure-eventgrid-4.9.1.zip`

## zipinfo {}

```diff
@@ -1,107 +1,107 @@
-Zip file size: 122484 bytes, number of entries: 105
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/
--rw-rw-r--  2.0 unx    25940 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/README.md
--rw-rw-r--  2.0 unx     6037 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/migration_guide.md
--rw-rw-r--  2.0 unx       38 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/setup.cfg
--rw-rw-r--  2.0 unx     2504 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/setup.py
--rw-rw-r--  2.0 unx    40731 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/PKG-INFO
--rw-rw-r--  2.0 unx     1073 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/LICENSE
--rw-rw-r--  2.0 unx     8379 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx      155 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/MANIFEST.in
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/eventgrid/
--rw-rw-r--  2.0 unx       80 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/eventgrid/aio/
--rw-rw-r--  2.0 unx      494 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_version.py
--rw-rw-r--  2.0 unx     6841 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_helpers.py
--rw-rw-r--  2.0 unx     5298 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_models.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/py.typed
--rw-rw-r--  2.0 unx     1535 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_signature_credential_policy.py
--rw-rw-r--  2.0 unx      663 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/__init__.py
--rw-rw-r--  2.0 unx     9830 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_publisher_client.py
--rw-rw-r--  2.0 unx     2130 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_policies.py
--rw-rw-r--  2.0 unx    15251 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_event_mappings.py
--rw-rw-r--  2.0 unx     1526 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_messaging_shared.py
--rw-rw-r--  2.0 unx      548 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_constants.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/
--rw-rw-r--  2.0 unx     2245 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/_configuration.py
--rw-rw-r--  2.0 unx     3272 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/_event_grid_publisher_client.py
--rw-rw-r--  2.0 unx      675 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/__init__.py
--rw-rw-r--  2.0 unx     1150 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/__init__.py
--rw-rw-r--  2.0 unx     7641 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/_request_builders_py3.py
--rw-rw-r--  2.0 unx     7546 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/_request_builders.py
--rw-rw-r--  2.0 unx     2085 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx     3231 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_event_grid_publisher_client.py
--rw-rw-r--  2.0 unx      574 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     1648 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_event_grid_publisher_client_async.py
--rw-rw-r--  2.0 unx     2085 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_configuration_async.py
--rw-rw-r--  2.0 unx     6344 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/_models_py3.py
--rw-rw-r--  2.0 unx     5926 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/_models.py
--rw-rw-r--  2.0 unx      755 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/__init__.py
--rw-rw-r--  2.0 unx      269 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/aio/__init__.py
--rw-rw-r--  2.0 unx    10173 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/azure/eventgrid/aio/_publisher_client_async.py
--rw-rw-r--  2.0 unx        1 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx    40731 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx       41 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     3904 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/not-zip-safe
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     3194 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/_mocks.py
--rw-rw-r--  2.0 unx     4779 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_cncf_events_async.py
--rw-rw-r--  2.0 unx     5671 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_serialization.py
--rw-rw-r--  2.0 unx     4413 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_cncf_events.py
--rw-rw-r--  2.0 unx     2599 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_cloud_event_tracing.py
--rw-rw-r--  2.0 unx    15315 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_eg_publisher_client.py
--rw-rw-r--  2.0 unx     3560 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_exceptions.py
--rw-rw-r--  2.0 unx     2270 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/eventgrid_preparer.py
--rw-rw-r--  2.0 unx    14718 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_eg_publisher_client_async.py
--rw-rw-r--  2.0 unx    11071 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_eg_event_get_bytes.py
--rw-rw-r--  2.0 unx     3756 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/test_exceptions_async.py
--rw-rw-r--  2.0 unx     2275 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/conftest.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     2849 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/tests/perfstress_tests/send.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/sync_samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/consume_samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/publish_samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/async_samples/
--rw-rw-r--  2.0 unx     1402 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
--rw-rw-r--  2.0 unx     1567 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
--rw-rw-r--  2.0 unx     1770 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_to_channel.py
--rw-rw-r--  2.0 unx     1223 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_generate_sas.py
--rw-rw-r--  2.0 unx     1591 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_cloud_event_using_dict.py
--rw-rw-r--  2.0 unx     1500 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
--rw-rw-r--  2.0 unx     2079 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_event_using_dict.py
--rw-rw-r--  2.0 unx     1998 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_authentication.py
--rw-rw-r--  2.0 unx     1472 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_cncf_cloud_events.py
--rw-rw-r--  2.0 unx     1136 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_consume_custom_payload.py
--rw-rw-r--  2.0 unx     1713 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
--rw-rw-r--  2.0 unx     1810 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/
--rw-rw-r--  2.0 unx     1479 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/consume_samples/consume_eventgrid_events_from_service_bus_queue.py
--rw-rw-r--  2.0 unx     1461 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/consume_samples/consume_cloud_events_from_storage_queue.py
--rw-rw-r--  2.0 unx     1527 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/consume_samples/consume_cloud_events_from_eventhub.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Apr-07 17:51 azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/EventGridTrigger1/
--rw-rw-r--  2.0 unx      566 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/EventGridTrigger1/__init__.py
--rw-rw-r--  2.0 unx     2179 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/publish_samples/publish_event_grid_events_to_custom_topic_sample.py
--rw-rw-r--  2.0 unx     2268 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/publish_samples/publish_cloud_events_to_custom_topic_sample.py
--rw-rw-r--  2.0 unx     2432 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/publish_samples/publish_with_shared_access_signature_sample.py
--rw-rw-r--  2.0 unx     2125 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/publish_samples/publish_custom_schema_events_to_topic_sample.py
--rw-rw-r--  2.0 unx     2249 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/publish_samples/publish_cloud_events_to_domain_topic_sample.py
--rw-rw-r--  2.0 unx     1946 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_to_channel_async.py
--rw-rw-r--  2.0 unx     2209 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_event_using_dict_async.py
--rw-rw-r--  2.0 unx     1943 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
--rw-rw-r--  2.0 unx     1998 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
--rw-rw-r--  2.0 unx     2225 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_authentication_async.py
--rw-rw-r--  2.0 unx     1719 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
--rw-rw-r--  2.0 unx     1788 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
--rw-rw-r--  2.0 unx     1993 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
--rw-rw-r--  2.0 unx     1695 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
--rw-rw-r--  2.0 unx     1638 b- defN 22-Apr-07 17:50 azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_cncf_cloud_events_async.py
-105 files, 360527 bytes uncompressed, 100946 bytes compressed:  72.0%
+Zip file size: 121602 bytes, number of entries: 105
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/
+-rw-rw-r--  2.0 unx     6037 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/migration_guide.md
+-rw-rw-r--  2.0 unx     2467 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/setup.py
+-rw-rw-r--  2.0 unx    25941 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/README.md
+-rw-rw-r--  2.0 unx     8661 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/CHANGELOG.md
+-rw-rw-r--  2.0 unx       38 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/setup.cfg
+-rw-rw-r--  2.0 unx     1073 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/LICENSE
+-rw-rw-r--  2.0 unx      155 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/MANIFEST.in
+-rw-rw-r--  2.0 unx    35366 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/publish_samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/
+-rw-rw-r--  2.0 unx     2249 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/publish_samples/publish_cloud_events_to_domain_topic_sample.py
+-rw-rw-r--  2.0 unx     2179 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/publish_samples/publish_event_grid_events_to_custom_topic_sample.py
+-rw-rw-r--  2.0 unx     2432 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/publish_samples/publish_with_shared_access_signature_sample.py
+-rw-rw-r--  2.0 unx     2125 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/publish_samples/publish_custom_schema_events_to_topic_sample.py
+-rw-rw-r--  2.0 unx     2268 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/publish_samples/publish_cloud_events_to_custom_topic_sample.py
+-rw-rw-r--  2.0 unx     2225 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_authentication_async.py
+-rw-rw-r--  2.0 unx     1671 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
+-rw-rw-r--  2.0 unx     1946 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_to_channel_async.py
+-rw-rw-r--  2.0 unx     1640 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_cncf_cloud_events_async.py
+-rw-rw-r--  2.0 unx     1895 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
+-rw-rw-r--  2.0 unx     1647 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
+-rw-rw-r--  2.0 unx     2161 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_event_using_dict_async.py
+-rw-rw-r--  2.0 unx     1945 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
+-rw-rw-r--  2.0 unx     1950 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
+-rw-rw-r--  2.0 unx     1740 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/
+-rw-rw-r--  2.0 unx     1479 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/consume_eventgrid_events_from_service_bus_queue.py
+-rw-rw-r--  2.0 unx     1527 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/consume_cloud_events_from_eventhub.py
+-rw-rw-r--  2.0 unx     1461 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/consume_cloud_events_from_storage_queue.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/EventGridTrigger1/
+-rw-rw-r--  2.0 unx      566 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/EventGridTrigger1/__init__.py
+-rw-rw-r--  2.0 unx     1713 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
+-rw-rw-r--  2.0 unx     1810 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
+-rw-rw-r--  2.0 unx     1136 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_consume_custom_payload.py
+-rw-rw-r--  2.0 unx     1500 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
+-rw-rw-r--  2.0 unx     1402 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
+-rw-rw-r--  2.0 unx     1998 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_authentication.py
+-rw-rw-r--  2.0 unx     2079 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_event_using_dict.py
+-rw-rw-r--  2.0 unx     1591 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_cloud_event_using_dict.py
+-rw-rw-r--  2.0 unx     1567 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
+-rw-rw-r--  2.0 unx     1223 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_generate_sas.py
+-rw-rw-r--  2.0 unx     1474 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_cncf_cloud_events.py
+-rw-rw-r--  2.0 unx     1770 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_to_channel.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/
+-rw-rw-r--  2.0 unx       80 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/
+-rw-rw-r--  2.0 unx     6841 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_helpers.py
+-rw-rw-r--  2.0 unx     1535 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_signature_credential_policy.py
+-rw-rw-r--  2.0 unx    15651 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_event_mappings.py
+-rw-rw-r--  2.0 unx     9924 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_publisher_client.py
+-rw-rw-r--  2.0 unx      548 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_constants.py
+-rw-rw-r--  2.0 unx      492 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_version.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/py.typed
+-rw-rw-r--  2.0 unx     1526 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_messaging_shared.py
+-rw-rw-r--  2.0 unx      663 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/__init__.py
+-rw-rw-r--  2.0 unx     5298 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_models.py
+-rw-rw-r--  2.0 unx     2130 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_policies.py
+-rw-rw-r--  2.0 unx    10267 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/aio/_publisher_client_async.py
+-rw-rw-r--  2.0 unx      269 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/aio/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/
+-rw-rw-r--  2.0 unx     2245 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/_configuration.py
+-rw-rw-r--  2.0 unx     3272 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/_event_grid_publisher_client.py
+-rw-rw-r--  2.0 unx      675 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/__init__.py
+-rw-rw-r--  2.0 unx     1648 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_event_grid_publisher_client_async.py
+-rw-rw-r--  2.0 unx     2085 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_configuration_async.py
+-rw-rw-r--  2.0 unx     2085 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     3231 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_event_grid_publisher_client.py
+-rw-rw-r--  2.0 unx      574 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     6344 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/_models_py3.py
+-rw-rw-r--  2.0 unx      755 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx     5926 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/_models.py
+-rw-rw-r--  2.0 unx     7641 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/_request_builders_py3.py
+-rw-rw-r--  2.0 unx     7546 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/_request_builders.py
+-rw-rw-r--  2.0 unx     1150 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/__init__.py
+-rw-rw-r--  2.0 unx     3904 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx       40 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/requires.txt
+-rw-rw-r--  2.0 unx    35366 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/azure_eventgrid.egg-info/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx    15315 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_eg_publisher_client.py
+-rw-rw-r--  2.0 unx     4413 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_cncf_events.py
+-rw-rw-r--  2.0 unx     3256 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/_mocks.py
+-rw-rw-r--  2.0 unx    11071 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_eg_event_get_bytes.py
+-rw-rw-r--  2.0 unx    14718 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_eg_publisher_client_async.py
+-rw-rw-r--  2.0 unx     5672 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_serialization.py
+-rw-rw-r--  2.0 unx     4779 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_cncf_events_async.py
+-rw-rw-r--  2.0 unx     3756 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_exceptions_async.py
+-rw-rw-r--  2.0 unx     3560 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_exceptions.py
+-rw-rw-r--  2.0 unx     2275 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/conftest.py
+-rw-rw-r--  2.0 unx     2643 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/test_cloud_event_tracing.py
+-rw-rw-r--  2.0 unx     2270 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/eventgrid_preparer.py
+-rw-rw-r--  2.0 unx     2847 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/perfstress_tests/send.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 22:50 azure-eventgrid-4.9.1/tests/perfstress_tests/__init__.py
+105 files, 350401 bytes uncompressed, 100484 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,316 +1,316 @@
-Filename: azure-eventgrid-4.9.0b1/
+Filename: azure-eventgrid-4.9.1/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/
+Filename: azure-eventgrid-4.9.1/samples/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/
+Filename: azure-eventgrid-4.9.1/azure/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/
+Filename: azure-eventgrid-4.9.1/tests/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/README.md
+Filename: azure-eventgrid-4.9.1/migration_guide.md
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/migration_guide.md
+Filename: azure-eventgrid-4.9.1/setup.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/setup.cfg
+Filename: azure-eventgrid-4.9.1/README.md
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/setup.py
+Filename: azure-eventgrid-4.9.1/CHANGELOG.md
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/PKG-INFO
+Filename: azure-eventgrid-4.9.1/setup.cfg
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/LICENSE
+Filename: azure-eventgrid-4.9.1/LICENSE
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/CHANGELOG.md
+Filename: azure-eventgrid-4.9.1/MANIFEST.in
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/MANIFEST.in
+Filename: azure-eventgrid-4.9.1/PKG-INFO
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/
+Filename: azure-eventgrid-4.9.1/samples/publish_samples/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/aio/
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_version.py
+Filename: azure-eventgrid-4.9.1/samples/publish_samples/publish_cloud_events_to_domain_topic_sample.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_helpers.py
+Filename: azure-eventgrid-4.9.1/samples/publish_samples/publish_event_grid_events_to_custom_topic_sample.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_models.py
+Filename: azure-eventgrid-4.9.1/samples/publish_samples/publish_with_shared_access_signature_sample.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/py.typed
+Filename: azure-eventgrid-4.9.1/samples/publish_samples/publish_custom_schema_events_to_topic_sample.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_signature_credential_policy.py
+Filename: azure-eventgrid-4.9.1/samples/publish_samples/publish_cloud_events_to_custom_topic_sample.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_authentication_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_publisher_client.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_policies.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_to_channel_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_event_mappings.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_cncf_cloud_events_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_messaging_shared.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_constants.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_event_using_dict_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/_configuration.py
+Filename: azure-eventgrid-4.9.1/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/_event_grid_publisher_client.py
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/consume_eventgrid_events_from_service_bus_queue.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/consume_cloud_events_from_eventhub.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/_request_builders_py3.py
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/consume_cloud_events_from_storage_queue.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/_request_builders.py
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/EventGridTrigger1/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_configuration.py
+Filename: azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/EventGridTrigger1/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_event_grid_publisher_client.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_event_grid_publisher_client_async.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_consume_custom_payload.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_configuration_async.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/_models_py3.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/_models.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_authentication.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_event_using_dict.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/aio/__init__.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_cloud_event_using_dict.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure/eventgrid/aio/_publisher_client_async.py
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/dependency_links.txt
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_generate_sas.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/PKG-INFO
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_cncf_cloud_events.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/requires.txt
+Filename: azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_to_channel.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/top_level.txt
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/SOURCES.txt
+Filename: azure-eventgrid-4.9.1/azure/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/not-zip-safe
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/aio/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/perfstress_tests/
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/_mocks.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_helpers.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_cncf_events_async.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_signature_credential_policy.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_serialization.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_event_mappings.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_cncf_events.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_publisher_client.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_cloud_event_tracing.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_constants.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_eg_publisher_client.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_version.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_exceptions.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/py.typed
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/eventgrid_preparer.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_messaging_shared.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_eg_publisher_client_async.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_eg_event_get_bytes.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_models.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/test_exceptions_async.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_policies.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/conftest.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/aio/_publisher_client_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/perfstress_tests/__init__.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/aio/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/tests/perfstress_tests/send.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/publish_samples/
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/_configuration.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/_event_grid_publisher_client.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_event_grid_publisher_client_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_to_channel.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_configuration_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_generate_sas.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_cloud_event_using_dict.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_event_grid_publisher_client.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_event_using_dict.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_authentication.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_cncf_cloud_events.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/_models.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_consume_custom_payload.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/_request_builders_py3.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/_request_builders.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
+Filename: azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/__init__.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/consume_eventgrid_events_from_service_bus_queue.py
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/consume_cloud_events_from_storage_queue.py
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/consume_cloud_events_from_eventhub.py
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/EventGridTrigger1/
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/requires.txt
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/EventGridTrigger1/__init__.py
+Filename: azure-eventgrid-4.9.1/azure_eventgrid.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/publish_samples/publish_event_grid_events_to_custom_topic_sample.py
+Filename: azure-eventgrid-4.9.1/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/publish_samples/publish_cloud_events_to_custom_topic_sample.py
+Filename: azure-eventgrid-4.9.1/tests/test_eg_publisher_client.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/publish_samples/publish_with_shared_access_signature_sample.py
+Filename: azure-eventgrid-4.9.1/tests/test_cncf_events.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/publish_samples/publish_custom_schema_events_to_topic_sample.py
+Filename: azure-eventgrid-4.9.1/tests/_mocks.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/publish_samples/publish_cloud_events_to_domain_topic_sample.py
+Filename: azure-eventgrid-4.9.1/tests/test_eg_event_get_bytes.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_to_channel_async.py
+Filename: azure-eventgrid-4.9.1/tests/test_eg_publisher_client_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_event_using_dict_async.py
+Filename: azure-eventgrid-4.9.1/tests/test_serialization.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
+Filename: azure-eventgrid-4.9.1/tests/test_cncf_events_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
+Filename: azure-eventgrid-4.9.1/tests/test_exceptions_async.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_authentication_async.py
+Filename: azure-eventgrid-4.9.1/tests/test_exceptions.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
+Filename: azure-eventgrid-4.9.1/tests/conftest.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
+Filename: azure-eventgrid-4.9.1/tests/test_cloud_event_tracing.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
+Filename: azure-eventgrid-4.9.1/tests/eventgrid_preparer.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
+Filename: azure-eventgrid-4.9.1/tests/perfstress_tests/send.py
 Comment: 
 
-Filename: azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_cncf_cloud_events_async.py
+Filename: azure-eventgrid-4.9.1/tests/perfstress_tests/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-eventgrid-4.9.0b1/README.md` & `azure-eventgrid-4.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended on 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
-* Python 3.6 or later is required to use this package.
+* Python 3.7 or later is required to use this package.
 * You must have an [Azure subscription][azure_subscription] and an Event Grid Topic resource to use this package. Follow this [step-by-step tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart-portal) to register the Event Grid resource provider and create Event Grid topics using the [Azure portal](https://portal.azure.com/). There is a [similar tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart) using [Azure CLI](https://docs.microsoft.com/cli/azure).
 
 
 ### Install the package
 Install the Azure Event Grid client library for Python with [pip][pip]:
 
 ```bash
@@ -327,15 +327,15 @@
 
     ## deserialize payload into a list of typed Events
     events = [EventGridEvent.from_dict(json.loads(next(msg.body).decode('utf-8'))) for msg in payload]
 ```
 
 ## Distributed Tracing with EventGrid
 
-You can use opentelemetry for Python as usual with EventGrid since it's compatible with azure-core tracing integration.
+You can use OpenTelemetry for Python as usual with EventGrid since it's compatible with azure-core tracing integration.
 
 Here is an example of using OpenTelemetry to trace sending a CloudEvent.
 
 First, set OpenTelemetry as enabled tracing plugin for EventGrid.
 
 ```python
 from azure.core.settings import settings
@@ -347,15 +347,15 @@
 Regular open telemetry usage from here. See [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-python) for details.
 This example uses a simple console exporter to export the traces. Any exporter can be used here including `azure-monitor-opentelemetry-exporter`, `jaeger`, `zipkin` etc.
 
 ```python
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-from opentelemetry.sdk.trace.export import SimpleSpanProcessor  # this requires opentelemtry >= 1.0.0
+from opentelemetry.sdk.trace.export import SimpleSpanProcessor  # this requires opentelemetry >= 1.0.0
 
 # Simple console exporter
 exporter = ConsoleSpanExporter()
 
 trace.set_tracer_provider(TracerProvider())
 tracer = trace.get_tracer(__name__)
 trace.get_tracer_provider().add_span_processor(
```

## Comparing `azure-eventgrid-4.9.0b1/migration_guide.md` & `azure-eventgrid-4.9.1/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/setup.py` & `azure-eventgrid-4.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,30 +43,29 @@
     long_description=readme + '\n\n' + changelog,
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         'samples',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
     ]),
     install_requires=[
-        'msrest>=0.6.21',
-        'azure-core<2.0.0,>=1.18.0',
+        'msrest>=0.7.1',
+        'azure-core<2.0.0,>=1.24.0',
     ],
 )
```

## Comparing `azure-eventgrid-4.9.0b1/PKG-INFO` & `azure-eventgrid-4.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,721 +1,734 @@
 Metadata-Version: 2.1
 Name: azure-eventgrid
-Version: 4.9.0b1
+Version: 4.9.1
 Summary: Microsoft Azure Event Grid Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: # Azure Event Grid client library for Python
-        
-        Azure Event Grid is a fully-managed intelligent event routing service that allows for uniform event consumption using a publish-subscribe model.
-        
-        [Source code][python-eg-src] | [Package (PyPI)][python-eg-pypi] | [API reference documentation][python-eg-ref-docs] | [Product documentation][python-eg-product-docs] | [Samples][python-eg-samples] | [Changelog][python-eg-changelog]
-        
-        ## _Disclaimer_
-        
-        _Azure SDK Python packages support for Python 2.7 has ended on 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
-        
-        ## Getting started
-        
-        ### Prerequisites
-        * Python 3.6 or later is required to use this package.
-        * You must have an [Azure subscription][azure_subscription] and an Event Grid Topic resource to use this package. Follow this [step-by-step tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart-portal) to register the Event Grid resource provider and create Event Grid topics using the [Azure portal](https://portal.azure.com/). There is a [similar tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart) using [Azure CLI](https://docs.microsoft.com/cli/azure).
-        
-        
-        ### Install the package
-        Install the Azure Event Grid client library for Python with [pip][pip]:
-        
-        ```bash
-        pip install azure-eventgrid
-        ```
-        
-        * An existing Event Grid topic or domain is required. You can create the resource using [Azure Portal][azure_portal_create_EG_resource] or [Azure CLI][azure_cli_link]
-        
-        If you use Azure CLI, replace `<resource-group-name>` and `<resource-name>` with your own unique names.
-        
-        #### Create an Event Grid Topic
-        
-        ```
-        az eventgrid topic --create --location <location> --resource-group <resource-group-name> --name <resource-name>
-        ```
-        
-        #### Create an Event Grid Domain
-        
-        ```
-        az eventgrid domain --create --location <location> --resource-group <resource-group-name> --name <resource-name>
-        ```
-        
-        ### Authenticate the client
-        In order to interact with the Event Grid service, you will need to create an instance of a client.
-        An **endpoint** and **credential** are necessary to instantiate the client object.
-        
-        #### Using Azure Active Directory (AAD)
-        
-        Azure Event Grid provides integration with Azure Active Directory (Azure AD) for identity-based authentication of requests. With Azure AD, you can use role-based access control (RBAC) to grant access to your Azure Event Grid resources to users, groups, or applications.
-        
-        To send events to a topic or domain with a `TokenCredential`, the authenticated identity should have the "EventGrid Data Sender" role assigned.
-        
-        With the `azure-identity` package, you can seamlessly authorize requests in both development and production environments. To learn more about Azure Active Directory, see the [`azure-identity` README](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/identity/azure-identity/README.md).
-        
-        For example, you can use `DefaultAzureCredential` to construct a client which will authenticate using Azure Active Directory:
-        
-        ```Python
-        from azure.identity import DefaultAzureCredential
-        from azure.eventgrid import EventGridPublisherClient, EventGridEvent
-        
-        event = EventGridEvent(
-            data={"team": "azure-sdk"},
-            subject="Door1",
-            event_type="Azure.Sdk.Demo",
-            data_version="2.0"
-        )
-        
-        credential = DefaultAzureCredential()
-        endpoint = os.environ["EG_TOPIC_HOSTNAME"]
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        #### Looking up the endpoint
-        You can find the topic endpoint within the Event Grid Topic resource on the Azure portal. This will look like:
-        `"https://<event-grid-topic-name>.<topic-location>.eventgrid.azure.net/api/events"`
-        
-        #### Create the client with AzureKeyCredential
-        
-        To use an Access key as the `credential` parameter,
-        pass the key as a string into an instance of [AzureKeyCredential][azure-key-credential].
-        
-        > **Note:** The Access Key may be found in the azure portal in the "Access Keys" menu of the Event Grid Topic resource.  They may also be obtained via the azure CLI, or the `azure-mgmt-eventgrid` library. A guide for getting access keys can be found [here](https://docs.microsoft.com/azure/event-grid/get-access-keys).
-        
-        ```python
-        from azure.core.credentials import AzureKeyCredential
-        from azure.eventgrid import EventGridPublisherClient
-        
-        endpoint = "https://<name>.<region>.eventgrid.azure.net/api/events"
-        credential = AzureKeyCredential("<access_key>")
-        eg_publisher_client = EventGridPublisherClient(endpoint, credential)
-        ```
-        > **Note:** A client may also be authenticated via SAS signature, using the `AzureSasCredential`. A sample demonstrating this, is available [here][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async]).
-        
-        > **Note:** The `generate_sas` method can be used to generate a shared access signature. A sample demonstrating this can be seen [here][python-eg-generate-sas].
-        
-        ## Key concepts
-        
-        ### Topic
-        A **[topic](https://docs.microsoft.com/azure/event-grid/concepts#topics)** is a channel within the EventGrid service to send events. The event schema that a topic accepts is decided at topic creation time. If events of a schema type are sent to a topic that requires a different schema type, errors will be raised.
-        
-        ### Domain
-        An event **[domain](https://docs.microsoft.com/azure/event-grid/event-domains)** is a management tool for large numbers of Event Grid topics related to the same application. They allow you to publish events to thousands of topics. Domains also give you authorization and authentication control over each topic. For more information, visit [Event domain overview](https://docs.microsoft.com/azure/event-grid/event-domains).
-        
-        When you create an event domain, a publishing endpoint for this domain is made available to you. This process is similar to creating an Event Grid Topic. The only difference is that, when publishing to a domain, you must specify the topic within the domain that you'd like the event to be delivered to.
-        
-        ### Event schemas
-        An **[event](https://docs.microsoft.com/azure/event-grid/concepts#events)** is the smallest amount of information that fully describes something that happened in the system. When a custom topic or domain is created, you must specify the schema that will be used when publishing events.
-        
-        Event Grid supports multiple schemas for encoding events.
-        
-        #### Event Grid schema
-        While you may configure your topic to use a [custom schema](https://docs.microsoft.com/azure/event-grid/input-mappings), it is more common to use the already-defined Event Grid schema. See the specifications and requirements [here](https://docs.microsoft.com/azure/event-grid/event-schema).
-        
-        #### CloudEvents v1.0 schema
-        Another option is to use the CloudEvents v1.0 schema. [CloudEvents](https://cloudevents.io/) is a Cloud Native Computing Foundation project which produces a specification for describing event data in a common way. The service summary of CloudEvents can be found [here](https://docs.microsoft.com/azure/event-grid/cloud-event-schema).
-        
-        ### EventGridPublisherClient
-        `EventGridPublisherClient` provides operations to send event data to a topic hostname specified during client initialization.
-        
-        Regardless of the schema that your topic or domain is configured to use, `EventGridPublisherClient` will be used to publish events to it. Use the `send` method publishing events.
-        
-        The following formats of events are allowed to be sent:
-        - A list or a single instance of strongly typed EventGridEvents.
-        - A dict representation of a serialized EventGridEvent object.
-        - A list or a single instance of strongly typed CloudEvents.
-        - A dict representation of a serialized CloudEvent object.
-        
-        - A dict representation of any Custom Schema.
-        
-        Please have a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples) for detailed examples.
-        
-        
-         **Note:** It is important to know if your topic supports CloudEvents or EventGridEvents before publishing. If you send to a topic that does not support the schema of the event you are sending, send() will throw an exception.
-        
-        ### System Topics
-        A **[system topic](https://docs.microsoft.com/azure/event-grid/system-topics)** in Event Grid represents one or more events published by Azure services such as Azure Storage or Azure Event Hubs. For example, a system topic may represent all blob events or only blob creation and blob deletion events published for a specific storage account.
-        
-        The names of the various event types for the system events published to Azure Event Grid are available in `azure.eventgrid.SystemEventNames`.
-        For complete list of recognizable system topics, visit [System Topics](https://docs.microsoft.com/azure/event-grid/system-topics).
-        
-         For more information about the key concepts on Event Grid, see [Concepts in Azure Event Grid][publisher-service-doc].
-        
-        ## Event Grid on Kubernetes with Azure Arc
-        
-        Event Grid on Kubernetes with Azure Arc is an offering that allows you to run Event Grid on your own Kubernetes cluster. This capability is enabled by the use of Azure Arc enabled Kubernetes. Through Azure Arc enabled Kubernetes, a supported Kubernetes cluster connects to Azure. Once connected, you are able to install Event Grid on it. Learn more about it [here](https://docs.microsoft.com/azure/event-grid/kubernetes/overview).
-        
-        ### Support for CNCF Cloud Events
-        
-        Starting with v4.7.0, this package also supports publishing a CNCF cloud event from https://pypi.org/project/cloudevents/. You would be able to pass a CloudEvent object from this library to the `send` API.
-        
-        ```python
-        
-        from cloudevents.http import CloudEvent
-        
-        event = CloudEvent(...)
-        
-        client.send(event)
-        ```
-        
-        ## Examples
-        
-        The following sections provide several code snippets covering some of the most common Event Grid tasks, including:
-        
-        * [Send an Event Grid Event](#send-an-event-grid-event)
-        * [Send a Cloud Event](#send-a-cloud-event)
-        * [Send Multiple Events](#send-multiple-events)
-        * [Send events as Dictionaries](#send-events-as-dictionaries)
-        * [Consume a payload from storage queue](#consume-from-storage-queue)
-        * [Consume from ServiceBus](#consume-from-servicebus)
-        
-        ### Send an Event Grid Event
-        
-        This example publishes an Event Grid event.
-        
-        ```Python
-        import os
-        from azure.core.credentials import AzureKeyCredential
-        from azure.eventgrid import EventGridPublisherClient, EventGridEvent
-        
-        key = os.environ["EG_ACCESS_KEY"]
-        endpoint = os.environ["EG_TOPIC_HOSTNAME"]
-        
-        event = EventGridEvent(
-            data={"team": "azure-sdk"},
-            subject="Door1",
-            event_type="Azure.Sdk.Demo",
-            data_version="2.0"
-        )
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        ### Send a Cloud Event
-        
-        This example publishes a Cloud event.
-        
-        ```Python
-        import os
-        from azure.core.credentials import AzureKeyCredential
-        from azure.core.messaging import CloudEvent
-        from azure.eventgrid import EventGridPublisherClient
-        
-        key = os.environ["CLOUD_ACCESS_KEY"]
-        endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
-        
-        event = CloudEvent(
-            type="Azure.Sdk.Sample",
-            source="https://egsample.dev/sampleevent",
-            data={"team": "azure-sdk"}
-        )
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        ### Send Multiple events
-        
-        It is possible to send events as a batch when sending multiple events to a topic or a domain. This example sends a list of CloudEvents using the send method.
-        
-        **WARNING:** When sending a list of multiple events at one time, iterating over and sending each event will not result in optimal performance. For best performance, it is highly recommended to send a list of events.
-        
-        ```Python
-        import os
-        from azure.core.credentials import AzureKeyCredential
-        from azure.core.messaging import CloudEvent
-        from azure.eventgrid import EventGridPublisherClient
-        
-        key = os.environ["CLOUD_ACCESS_KEY"]
-        endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
-        
-        event0 = CloudEvent(
-            type="Azure.Sdk.Sample",
-            source="https://egsample.dev/sampleevent",
-            data={"team": "azure-sdk"}
-        )
-        event1 = CloudEvent(
-            type="Azure.Sdk.Sample",
-            source="https://egsample.dev/sampleevent",
-            data={"team2": "azure-eventgrid"}
-        )
-        
-        events = [event0, event1]
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(events)
-        ```
-        
-        ### Send events as dictionaries
-        
-        A dict representation of respective serialized models can also be used to publish CloudEvent(s) or EventGridEvent(s) apart from the strongly typed objects.
-        
-        Use a dict-like representation to send to a topic with custom schema as shown below.
-        
-        ```Python
-        import os
-        import uuid
-        import datetime as dt
-        from msrest.serialization import UTC
-        from azure.core.credentials import AzureKeyCredential
-        from azure.eventgrid import EventGridPublisherClient
-        
-        key = os.environ["CUSTOM_SCHEMA_ACCESS_KEY"]
-        endpoint = os.environ["CUSTOM_SCHEMA_TOPIC_HOSTNAME"]
-        
-        event = custom_schema_event = {
-            "customSubject": "sample",
-            "customEventType": "sample.event",
-            "customDataVersion": "2.0",
-            "customId": uuid.uuid4(),
-            "customEventTime": dt.datetime.now(UTC()).isoformat(),
-            "customData": "sample data"
-            }
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        ### Consume from storage queue
-        
-        This example consumes a message received from storage queue and deserializes it to a CloudEvent object.
-        
-        ```Python
-        from azure.core.messaging import CloudEvent
-        from azure.storage.queue import QueueServiceClient, BinaryBase64DecodePolicy
-        import os
-        import json
-        
-        # all types of CloudEvents below produce same DeserializedEvent
-        connection_str = os.environ['STORAGE_QUEUE_CONN_STR']
-        queue_name = os.environ['STORAGE_QUEUE_NAME']
-        
-        with QueueServiceClient.from_connection_string(connection_str) as qsc:
-            payload =  qsc.get_queue_client(
-                queue=queue_name,
-                message_decode_policy=BinaryBase64DecodePolicy()
-                ).peek_messages()
-        
-            ## deserialize payload into a list of typed Events
-            events = [CloudEvent.from_dict(json.loads(msg.content)) for msg in payload]
-        ```
-        
-        ### Consume from servicebus
-        
-        This example consumes a payload message received from ServiceBus and deserializes it to an EventGridEvent object.
-        
-        ```Python
-        from azure.eventgrid import EventGridEvent
-        from azure.servicebus import ServiceBusClient
-        import os
-        import json
-        
-        # all types of EventGridEvents below produce same DeserializedEvent
-        connection_str = os.environ['SERVICE_BUS_CONN_STR']
-        queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
-        
-        with ServiceBusClient.from_connection_string(connection_str) as sb_client:
-            payload =  sb_client.get_queue_receiver(queue_name).receive_messages()
-        
-            ## deserialize payload into a list of typed Events
-            events = [EventGridEvent.from_dict(json.loads(next(msg.body).decode('utf-8'))) for msg in payload]
-        ```
-        
-        ## Distributed Tracing with EventGrid
-        
-        You can use opentelemetry for Python as usual with EventGrid since it's compatible with azure-core tracing integration.
-        
-        Here is an example of using OpenTelemetry to trace sending a CloudEvent.
-        
-        First, set OpenTelemetry as enabled tracing plugin for EventGrid.
-        
-        ```python
-        from azure.core.settings import settings
-        from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
-        
-        settings.tracing_implementation = OpenTelemetrySpan
-        ```
-        
-        Regular open telemetry usage from here. See [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-python) for details.
-        This example uses a simple console exporter to export the traces. Any exporter can be used here including `azure-monitor-opentelemetry-exporter`, `jaeger`, `zipkin` etc.
-        
-        ```python
-        from opentelemetry import trace
-        from opentelemetry.sdk.trace import TracerProvider
-        from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-        from opentelemetry.sdk.trace.export import SimpleSpanProcessor  # this requires opentelemtry >= 1.0.0
-        
-        # Simple console exporter
-        exporter = ConsoleSpanExporter()
-        
-        trace.set_tracer_provider(TracerProvider())
-        tracer = trace.get_tracer(__name__)
-        trace.get_tracer_provider().add_span_processor(
-            SimpleSpanProcessor(exporter)
-        )
-        ```
-        
-        Once the `tracer` and `exporter` are set, please follow the example below to start collecting traces while using the `send` method from the `EventGridPublisherClient` to send a CloudEvent object.
-        
-        ```python
-        import os
-        from azure.eventgrid import EventGridPublisherClient
-        from azure.core.messaging import CloudEvent
-        from azure.core.credentials import AzureKeyCredential
-        
-        hostname = os.environ['CLOUD_TOPIC_HOSTNAME']
-        key = AzureKeyCredential(os.environ['CLOUD_ACCESS_KEY'])
-        cloud_event = CloudEvent(
-            source = 'demo',
-            type = 'sdk.demo',
-            data = {'test': 'hello'},
-        )
-        with tracer.start_as_current_span(name="MyApplication"):
-            client = EventGridPublisherClient(hostname, key)
-            client.send(cloud_event)
-        ```
-        
-        ## Troubleshooting
-        
-        - Enable `azure.eventgrid` logger to collect traces from the library.
-        
-        ### General
-        Event Grid client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-        
-        ### Logging
-        This library uses the standard
-        [logging][python_logging] library for logging.
-        Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO
-        level.
-        
-        ### Optional Configuration
-        
-        Optional keyword arguments can be passed in at the client and per-operation level.
-        The azure-core [reference documentation][azure_core_ref_docs]
-        describes available configurations for retries, logging, transport protocols, and more.
-        
-        ## Next steps
-        
-        The following section provides several code snippets illustrating common patterns used in the Event Grid Python API.
-        
-        ### More sample code
-        
-        These code samples show common champion scenario operations with the Azure Event Grid client library.
-        
-        * Generate Shared Access Signature: [sample_generate_sas.py][python-eg-generate-sas]
-        
-        * Authenticate the client: [sample_authentication.py][python-eg-auth] ([async_version][python-eg-auth-async])
-        
-        * Publish events to a topic using SAS: [sample_publish_events_to_a_topic_using_sas_credential_async.py][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async])
-        * Publish Event Grid Events to a topic: [sample_publish_eg_events_to_a_topic.py][python-eg-sample-eg-event] ([async_version][python-eg-sample-eg-event-async])
-        * Publish EventGrid Events to a domain topic: [sample_publish_eg_events_to_a_domain_topic.py][python-eg-sample-eg-event-to-domain] ([async_version][python-eg-sample-eg-event-to-domain-async])
-        * Publish a Cloud Event: [sample_publish_events_using_cloud_events_1.0_schema.py][python-eg-sample-send-cloudevent] ([async_version][python-eg-sample-send-cloudevent-async])
-        * Publish a Custom Schema: [sample_publish_custom_schema_to_a_topic.py][python-eg-publish-custom-schema] ([async_version][python-eg-publish-custom-schema-async])
-        
-        The following samples cover publishing and consuming `dict` representations of EventGridEvents and CloudEvents.
-        * Publish EventGridEvent as dict like representation: [sample_publish_eg_event_using_dict.py][python-eg-sample-send-eg-as-dict] ([async_version][python-eg-sample-send-eg-as-dict-async])
-        
-        * Publish CloudEvent as dict like representation: [sample_publish_cloud_event_using_dict.py][python-eg-sample-send-cloudevent-as-dict] ([async_version][python-eg-sample-send-cloudevent-as-dict-async])
-        
-        * Consume a Custom Payload of raw cloudevent data: [sample_consume_custom_payload.py][python-eg-sample-consume-custom-payload]
-        
-        More samples can be found [here][python-eg-samples].
-        
-        * More samples related to the send scenario can be seen [here][python-eg-publish-samples].
-        * To see more samples related to consuming a payload from different messaging services as a typed object, please visit [Consume Samples][python-eg-consume-samples]
-        
-        ### Additional documentation
-        
-        For more extensive documentation on Azure Event Grid, see the [Event Grid documentation][python-eg-product-docs] on docs.microsoft.com.
-        
-        ## Contributing
-        This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
-        
-        When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
-        
-        This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
-        
-        <!-- LINKS -->
-        
-        [azure_cli_link]: https://pypi.org/project/azure-cli/
-        [python-eg-src]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/
-        [python-eg-pypi]: https://pypi.org/project/azure-eventgrid
-        [python-eg-product-docs]: https://docs.microsoft.com/azure/event-grid/overview
-        [python-eg-ref-docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-eventgrid/latest/index.html
-        [publisher-service-doc]: https://docs.microsoft.com/azure/event-grid/concepts
-        [python-eg-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples
-        [python-eg-changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/CHANGELOG.md
-        [pip]: https://pypi.org/project/pip/
-        
-        [azure_portal_create_EG_resource]: https://ms.portal.azure.com/#blade/HubsExtension/BrowseResource/resourceType/Microsoft.EventGrid%2Ftopics
-        [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
-        [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
-        [python_logging]: https://docs.python.org/3/library/logging.html
-        [azure_core_ref_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core#configurations
-        [azure_subscription]: https://azure.microsoft.com/free/
-        
-        [python-eg-auth]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_authentication.py
-        [python-eg-generate-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_generate_sas.py
-        [python-eg-sample-send-using-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
-        [python-eg-sample-eg-event]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
-        [python-eg-sample-eg-event-to-domain]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
-        [python-eg-sample-send-cloudevent]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
-        [python-eg-publish-custom-schema]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
-        [python-eg-sample-send-eg-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_event_using_dict.py
-        [python-eg-sample-send-cloudevent-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_cloud_event_using_dict.py
-        
-        [python-eg-auth-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_authentication_async.py
-        [python-eg-sample-send-using-sas-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
-        [python-eg-sample-eg-event-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
-        [python-eg-sample-eg-event-to-domain-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
-        [python-eg-sample-send-cloudevent-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
-        [python-eg-publish-custom-schema-async]:https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
-        [python-eg-sample-send-eg-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_event_using_dict_async.py
-        [python-eg-sample-send-cloudevent-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
-        
-        [python-eg-publish-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/publish_samples
-        [python-eg-consume-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/consume_samples
-        [python-eg-sample-consume-custom-payload]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_consume_custom_payload.py
-        
-        [cla]: https://cla.microsoft.com
-        [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
-        [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
-        [coc_contact]: mailto:opencode@microsoft.com
-        
-        
-        # Release History
-        
-        ## 4.9.0b1 (2022-04-07)
-        
-        ### Features Added
-        
-        - Added support for publishing events to a channel.
-        
-        ## 4.8.0 (2022-04-06)
-        
-        - This version and all future versions will require Python 3.6+. Python 2.7 is no longer supported.
-        
-        ### Features Added
-        
-        - Added new enum values to `SystemEventNames` related to health care APIs.
-        
-        ## 4.7.1 (2021-11-18)
-        
-        ### Bugs Fixed
-        
-        - The `send` API will raise on exceptions.
-        
-        ## 4.7.0 (2021-11-09)
-        
-        ### Features Added
-        
-        - Added support for publishing native CNCF cloudevents (https://pypi.org/project/cloudevents/).
-        
-        ## 4.6.0 (2021-10-05)
-        
-        ### Features Added
-        
-        - Added new enum values to `SystemEvents`.
-        
-        ## 4.5.0 (2021-08-10)
-        
-        ### Features Added
-        
-        - Added a new enum value `Microsoft.ContainerService.NewKubernetesVersionAvailable` to `SystemEvents`.
-        - Added a `from_json` method which now accepts storage QueueMessage, eventhub's EventData or ServiceBusMessage or simply json bytes to return an `EventGridEvent`
-        
-        ## 4.4.0 (2021-07-19)
-        
-        - Bumped `msrest` dependency to `0.6.21` to align with mgmt package.
-        
-        ### Features Added
-        
-        - `EventGridPublisherClient` now supports Azure Active Directory (AAD) for authentication.
-        
-        ## 4.3.0 (2021-06-09)
-        
-          **New Features**
-          - Added new event names related to blob inventory to the `SystemEventNames` enum.
-        
-          **Bug Fixes**
-          - Replaced the `ServiceBusDeadletterMessagesAvailableWithNoListenerEventName` with the right value.
-        
-        ## 4.2.0 (2021-05-12)
-        
-          **New Features**
-          - Added new event names to the `SystemEventNames` enum.
-        
-        ## 4.1.1 (2021-04-07)
-        
-          **Bug Fixes**
-          - Improved the `repr` on `EventGridEvent` to show more meaningful text.
-        
-        ## 4.1.0 (2021-03-23)
-        
-          **New Features**
-          - Added new SystemEventNames `AcsChatThreadParticipantRemovedEventName`, `AcsChatThreadParticipantAddedEventName` and `AcsRecordingFileStatusUpdatedEventName`.
-        
-        ## 4.0.0 (2021-03-09)
-        
-          **Note:** This is the first stable release of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid. Users migrating from `v1.x` are advised to view the [migration guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/migration_guide.md).
-        
-          **New Features**
-          - `azure-eventgrid` package now supports `azure.core.messaging.CloudEvent` which honors the CNCF CloudEvent spec.
-          - `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping for system events.
-          - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and Custom schema events.
-        
-          **Breaking Changes**
-          - `azure.eventgrid.models` namespace along with all the models in it are now removed.:
-              - JSON documentation on the events is available here: https://docs.microsoft.com/azure/event-grid/system-topics
-              - `azure.eventgrid.SystemEventNames` provides the list of available events name for easy switching.
-          - `azure.eventgrid.event_grid_client.EventGridClient` is now removed in favor of `azure.eventgrid.EventGridPublisherClient`.
-          - `azure.eventgrid.event_grid_client.EventGridClientConfiguration` is now removed.
-        
-        
-        ## 2.0.0 (2021-03-09)
-        
-          **Disclaimer:** v2.0.0 is functionally equivalent to v4.0.0. Users are advised to use v4.0.0 instead of this.
-        
-          **Breaking Changes**
-          - `~azure.eventgrid.CloudEvent` is now removed in favor of `~azure.core.messaging.CloudEvent`.
-          - All the `SystemEventNames` related to Azure Communication Service starting with `ACS****` are renamed to `Acs***` to honor pascal case.
-        
-          **Features**
-          - Added support for two new `SystemEvents` - `ServiceBusDeadletterMessagesAvailablePeriodicNotificationsEventData` and `ServiceBusActiveMessagesAvailablePeriodicNotificationsEventData`
-        
-        ## 2.0.0b5 (2021-02-10)
-        
-          **Breaking Changes**
-          - `EventGridSharedAccessSignatureCredential` is deprecated in favor of `AzureSasCredential`.
-          - `azure.eventgrid.models` namespace along with all the models in it are now removed. `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping.
-          - `topic_hostname` is renamed to `endpoint` in the `EventGridPublisherClient`.
-          - `azure.eventgrid.generate_shared_access_signature` method is now renamed to `generate_sas`.
-          - `EventGridConsumer`is now removed. Please see the samples to see how events can be deserialized.
-          - `CustomEvent` model is removed. Dictionaries must be used to send a custom schema.
-        
-          **Bug Fixes**
-          - `EventGridEvent` has two additional required positional parameters namely, `data` and `data_version`.
-          - `EventGridPublisherClient` now appropriately throws a `ValueError` if an invalid credential is passed during initialization.
-        
-        ## 2.0.0b4 (2020-11-11)
-        
-          **Bug Fixes**
-          - `TypeError` is raised when bytes are passed to an `EventGridEvent`.
-        
-        ## 2.0.0b3 (2020-10-05)
-        
-          **Feature**
-          - Added support for Keyvault Event Types
-          - Added distributed tracing support for CloudEvents
-        
-        ## 2.0.0b2 (2020-09-24)
-        
-          **Features**
-          - Added support for Azure Communication Services event types.
-        
-        ## 2.0.0b1 (2020-09-08)
-        
-          **Features**
-          - Version (2.0.0b1) is the first preview of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid.
-          For more information about this, and preview releases of other Azure SDK libraries, please visit https://azure.github.io/azure-sdk/releases/latest/python.html.
-          - Added Support for `CloudEvents`.
-          - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and CustomEvents.
-          - Implements the `EventGridConsumer` for the consume flow of the events.
-        
-        ## 1.3.0 (2019-05-20)
-        
-          - Event Schemas for new event types from IotHub, Media Services,
-            Container Registry, Maps, and AppConfiguration services.
-        
-        ## 1.2.0 (2018-08-28)
-        
-          - Event Schemas for new events (IotHub DeviceConnected and
-            DeviceDisconnected events, Resource events related to actions), and
-            breaking changes to the schema for IotHub DeviceCreated event and
-            IotHub DeviceDeleted event.
-        
-        ## 1.1.0 (2018-05-24)
-        
-          - Event Schemas for EventGrid subscription validation event, Azure
-            Media events, and ServiceBus events.
-        
-        ## 1.0.0 (2018-04-26)
-        
-        **General Breaking changes**
-        
-        This version uses a next-generation code generator that *might*
-        introduce breaking changes.
-        
-          - Model signatures now use only keyword-argument syntax. All
-            positional arguments must be re-written as keyword-arguments. To
-            keep auto-completion in most cases, models are now generated for
-            Python 2 and Python 3. Python 3 uses the "*" syntax for
-            keyword-only arguments.
-          - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to
-            improve the behavior when unrecognized enum values are encountered.
-            While this is not a breaking change, the distinctions are important,
-            and are documented here:
-            <https://docs.python.org/3/library/enum.html#others> At a glance:
-              - "is" should not be used at all.
-              - "format" will return the string value, where "%s" string
-                formatting will return `NameOfEnum.stringvalue`. Format syntax
-                should be prefered.
-          - New Long Running Operation:
-              - Return type changes from
-                `msrestazure.azure_operation.AzureOperationPoller` to
-                `msrest.polling.LROPoller`. External API is the same.
-              - Return type is now **always** a `msrest.polling.LROPoller`,
-                regardless of the optional parameters used.
-              - The behavior has changed when using `raw=True`. Instead of
-                returning the initial call result as `ClientRawResponse`,
-                without polling, now this returns an LROPoller. After polling,
-                the final resource will be returned as a `ClientRawResponse`.
-              - New `polling` parameter. The default behavior is
-                `Polling=True` which will poll using ARM algorithm. When
-                `Polling=False`, the response of the initial call will be
-                returned without polling.
-              - `polling` parameter accepts instances of subclasses of
-                `msrest.polling.PollingMethod`.
-              - `add_done_callback` will no longer raise if called after
-                polling is finished, but will instead execute the callback right
-                away.
-        
-        **Features**
-        
-          - Client class can be used as a context manager to keep the underlying
-            HTTP session open for performance
-          - Support for consuming Azure Container Registry events and Azure IoT
-            Hub events published to Event Grid.
-        
-        ## 0.1.0 (2018-01-30)
-        
-          - Initial Release
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Azure Event Grid client library for Python
+
+Azure Event Grid is a fully-managed intelligent event routing service that allows for uniform event consumption using a publish-subscribe model.
+
+[Source code][python-eg-src] | [Package (PyPI)][python-eg-pypi] | [API reference documentation][python-eg-ref-docs] | [Product documentation][python-eg-product-docs] | [Samples][python-eg-samples] | [Changelog][python-eg-changelog]
+
+## _Disclaimer_
+
+_Azure SDK Python packages support for Python 2.7 has ended on 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
+
+## Getting started
+
+### Prerequisites
+* Python 3.7 or later is required to use this package.
+* You must have an [Azure subscription][azure_subscription] and an Event Grid Topic resource to use this package. Follow this [step-by-step tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart-portal) to register the Event Grid resource provider and create Event Grid topics using the [Azure portal](https://portal.azure.com/). There is a [similar tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart) using [Azure CLI](https://docs.microsoft.com/cli/azure).
+
+
+### Install the package
+Install the Azure Event Grid client library for Python with [pip][pip]:
+
+```bash
+pip install azure-eventgrid
+```
+
+* An existing Event Grid topic or domain is required. You can create the resource using [Azure Portal][azure_portal_create_EG_resource] or [Azure CLI][azure_cli_link]
+
+If you use Azure CLI, replace `<resource-group-name>` and `<resource-name>` with your own unique names.
+
+#### Create an Event Grid Topic
+
+```
+az eventgrid topic --create --location <location> --resource-group <resource-group-name> --name <resource-name>
+```
+
+#### Create an Event Grid Domain
+
+```
+az eventgrid domain --create --location <location> --resource-group <resource-group-name> --name <resource-name>
+```
+
+### Authenticate the client
+In order to interact with the Event Grid service, you will need to create an instance of a client.
+An **endpoint** and **credential** are necessary to instantiate the client object.
+
+#### Using Azure Active Directory (AAD)
+
+Azure Event Grid provides integration with Azure Active Directory (Azure AD) for identity-based authentication of requests. With Azure AD, you can use role-based access control (RBAC) to grant access to your Azure Event Grid resources to users, groups, or applications.
+
+To send events to a topic or domain with a `TokenCredential`, the authenticated identity should have the "EventGrid Data Sender" role assigned.
+
+With the `azure-identity` package, you can seamlessly authorize requests in both development and production environments. To learn more about Azure Active Directory, see the [`azure-identity` README](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/identity/azure-identity/README.md).
+
+For example, you can use `DefaultAzureCredential` to construct a client which will authenticate using Azure Active Directory:
+
+```Python
+from azure.identity import DefaultAzureCredential
+from azure.eventgrid import EventGridPublisherClient, EventGridEvent
+
+event = EventGridEvent(
+    data={"team": "azure-sdk"},
+    subject="Door1",
+    event_type="Azure.Sdk.Demo",
+    data_version="2.0"
+)
+
+credential = DefaultAzureCredential()
+endpoint = os.environ["EG_TOPIC_HOSTNAME"]
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+#### Looking up the endpoint
+You can find the topic endpoint within the Event Grid Topic resource on the Azure portal. This will look like:
+`"https://<event-grid-topic-name>.<topic-location>.eventgrid.azure.net/api/events"`
+
+#### Create the client with AzureKeyCredential
+
+To use an Access key as the `credential` parameter,
+pass the key as a string into an instance of [AzureKeyCredential][azure-key-credential].
+
+> **Note:** The Access Key may be found in the azure portal in the "Access Keys" menu of the Event Grid Topic resource.  They may also be obtained via the azure CLI, or the `azure-mgmt-eventgrid` library. A guide for getting access keys can be found [here](https://docs.microsoft.com/azure/event-grid/get-access-keys).
+
+```python
+from azure.core.credentials import AzureKeyCredential
+from azure.eventgrid import EventGridPublisherClient
+
+endpoint = "https://<name>.<region>.eventgrid.azure.net/api/events"
+credential = AzureKeyCredential("<access_key>")
+eg_publisher_client = EventGridPublisherClient(endpoint, credential)
+```
+> **Note:** A client may also be authenticated via SAS signature, using the `AzureSasCredential`. A sample demonstrating this, is available [here][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async]).
+
+> **Note:** The `generate_sas` method can be used to generate a shared access signature. A sample demonstrating this can be seen [here][python-eg-generate-sas].
+
+## Key concepts
+
+### Topic
+A **[topic](https://docs.microsoft.com/azure/event-grid/concepts#topics)** is a channel within the EventGrid service to send events. The event schema that a topic accepts is decided at topic creation time. If events of a schema type are sent to a topic that requires a different schema type, errors will be raised.
+
+### Domain
+An event **[domain](https://docs.microsoft.com/azure/event-grid/event-domains)** is a management tool for large numbers of Event Grid topics related to the same application. They allow you to publish events to thousands of topics. Domains also give you authorization and authentication control over each topic. For more information, visit [Event domain overview](https://docs.microsoft.com/azure/event-grid/event-domains).
+
+When you create an event domain, a publishing endpoint for this domain is made available to you. This process is similar to creating an Event Grid Topic. The only difference is that, when publishing to a domain, you must specify the topic within the domain that you'd like the event to be delivered to.
+
+### Event schemas
+An **[event](https://docs.microsoft.com/azure/event-grid/concepts#events)** is the smallest amount of information that fully describes something that happened in the system. When a custom topic or domain is created, you must specify the schema that will be used when publishing events.
+
+Event Grid supports multiple schemas for encoding events.
+
+#### Event Grid schema
+While you may configure your topic to use a [custom schema](https://docs.microsoft.com/azure/event-grid/input-mappings), it is more common to use the already-defined Event Grid schema. See the specifications and requirements [here](https://docs.microsoft.com/azure/event-grid/event-schema).
+
+#### CloudEvents v1.0 schema
+Another option is to use the CloudEvents v1.0 schema. [CloudEvents](https://cloudevents.io/) is a Cloud Native Computing Foundation project which produces a specification for describing event data in a common way. The service summary of CloudEvents can be found [here](https://docs.microsoft.com/azure/event-grid/cloud-event-schema).
+
+### EventGridPublisherClient
+`EventGridPublisherClient` provides operations to send event data to a topic hostname specified during client initialization.
+
+Regardless of the schema that your topic or domain is configured to use, `EventGridPublisherClient` will be used to publish events to it. Use the `send` method publishing events.
+
+The following formats of events are allowed to be sent:
+- A list or a single instance of strongly typed EventGridEvents.
+- A dict representation of a serialized EventGridEvent object.
+- A list or a single instance of strongly typed CloudEvents.
+- A dict representation of a serialized CloudEvent object.
+
+- A dict representation of any Custom Schema.
+
+Please have a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples) for detailed examples.
+
+
+ **Note:** It is important to know if your topic supports CloudEvents or EventGridEvents before publishing. If you send to a topic that does not support the schema of the event you are sending, send() will throw an exception.
+
+### System Topics
+A **[system topic](https://docs.microsoft.com/azure/event-grid/system-topics)** in Event Grid represents one or more events published by Azure services such as Azure Storage or Azure Event Hubs. For example, a system topic may represent all blob events or only blob creation and blob deletion events published for a specific storage account.
+
+The names of the various event types for the system events published to Azure Event Grid are available in `azure.eventgrid.SystemEventNames`.
+For complete list of recognizable system topics, visit [System Topics](https://docs.microsoft.com/azure/event-grid/system-topics).
+
+ For more information about the key concepts on Event Grid, see [Concepts in Azure Event Grid][publisher-service-doc].
+
+## Event Grid on Kubernetes with Azure Arc
+
+Event Grid on Kubernetes with Azure Arc is an offering that allows you to run Event Grid on your own Kubernetes cluster. This capability is enabled by the use of Azure Arc enabled Kubernetes. Through Azure Arc enabled Kubernetes, a supported Kubernetes cluster connects to Azure. Once connected, you are able to install Event Grid on it. Learn more about it [here](https://docs.microsoft.com/azure/event-grid/kubernetes/overview).
+
+### Support for CNCF Cloud Events
+
+Starting with v4.7.0, this package also supports publishing a CNCF cloud event from https://pypi.org/project/cloudevents/. You would be able to pass a CloudEvent object from this library to the `send` API.
+
+```python
+
+from cloudevents.http import CloudEvent
+
+event = CloudEvent(...)
+
+client.send(event)
+```
+
+## Examples
+
+The following sections provide several code snippets covering some of the most common Event Grid tasks, including:
+
+* [Send an Event Grid Event](#send-an-event-grid-event)
+* [Send a Cloud Event](#send-a-cloud-event)
+* [Send Multiple Events](#send-multiple-events)
+* [Send events as Dictionaries](#send-events-as-dictionaries)
+* [Consume a payload from storage queue](#consume-from-storage-queue)
+* [Consume from ServiceBus](#consume-from-servicebus)
+
+### Send an Event Grid Event
+
+This example publishes an Event Grid event.
+
+```Python
+import os
+from azure.core.credentials import AzureKeyCredential
+from azure.eventgrid import EventGridPublisherClient, EventGridEvent
+
+key = os.environ["EG_ACCESS_KEY"]
+endpoint = os.environ["EG_TOPIC_HOSTNAME"]
+
+event = EventGridEvent(
+    data={"team": "azure-sdk"},
+    subject="Door1",
+    event_type="Azure.Sdk.Demo",
+    data_version="2.0"
+)
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+### Send a Cloud Event
+
+This example publishes a Cloud event.
+
+```Python
+import os
+from azure.core.credentials import AzureKeyCredential
+from azure.core.messaging import CloudEvent
+from azure.eventgrid import EventGridPublisherClient
+
+key = os.environ["CLOUD_ACCESS_KEY"]
+endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
+
+event = CloudEvent(
+    type="Azure.Sdk.Sample",
+    source="https://egsample.dev/sampleevent",
+    data={"team": "azure-sdk"}
+)
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+### Send Multiple events
+
+It is possible to send events as a batch when sending multiple events to a topic or a domain. This example sends a list of CloudEvents using the send method.
+
+**WARNING:** When sending a list of multiple events at one time, iterating over and sending each event will not result in optimal performance. For best performance, it is highly recommended to send a list of events.
+
+```Python
+import os
+from azure.core.credentials import AzureKeyCredential
+from azure.core.messaging import CloudEvent
+from azure.eventgrid import EventGridPublisherClient
+
+key = os.environ["CLOUD_ACCESS_KEY"]
+endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
+
+event0 = CloudEvent(
+    type="Azure.Sdk.Sample",
+    source="https://egsample.dev/sampleevent",
+    data={"team": "azure-sdk"}
+)
+event1 = CloudEvent(
+    type="Azure.Sdk.Sample",
+    source="https://egsample.dev/sampleevent",
+    data={"team2": "azure-eventgrid"}
+)
+
+events = [event0, event1]
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(events)
+```
+
+### Send events as dictionaries
+
+A dict representation of respective serialized models can also be used to publish CloudEvent(s) or EventGridEvent(s) apart from the strongly typed objects.
+
+Use a dict-like representation to send to a topic with custom schema as shown below.
+
+```Python
+import os
+import uuid
+import datetime as dt
+from msrest.serialization import UTC
+from azure.core.credentials import AzureKeyCredential
+from azure.eventgrid import EventGridPublisherClient
+
+key = os.environ["CUSTOM_SCHEMA_ACCESS_KEY"]
+endpoint = os.environ["CUSTOM_SCHEMA_TOPIC_HOSTNAME"]
+
+event = custom_schema_event = {
+    "customSubject": "sample",
+    "customEventType": "sample.event",
+    "customDataVersion": "2.0",
+    "customId": uuid.uuid4(),
+    "customEventTime": dt.datetime.now(UTC()).isoformat(),
+    "customData": "sample data"
+    }
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+### Consume from storage queue
+
+This example consumes a message received from storage queue and deserializes it to a CloudEvent object.
+
+```Python
+from azure.core.messaging import CloudEvent
+from azure.storage.queue import QueueServiceClient, BinaryBase64DecodePolicy
+import os
+import json
+
+# all types of CloudEvents below produce same DeserializedEvent
+connection_str = os.environ['STORAGE_QUEUE_CONN_STR']
+queue_name = os.environ['STORAGE_QUEUE_NAME']
+
+with QueueServiceClient.from_connection_string(connection_str) as qsc:
+    payload =  qsc.get_queue_client(
+        queue=queue_name,
+        message_decode_policy=BinaryBase64DecodePolicy()
+        ).peek_messages()
+
+    ## deserialize payload into a list of typed Events
+    events = [CloudEvent.from_dict(json.loads(msg.content)) for msg in payload]
+```
+
+### Consume from servicebus
+
+This example consumes a payload message received from ServiceBus and deserializes it to an EventGridEvent object.
+
+```Python
+from azure.eventgrid import EventGridEvent
+from azure.servicebus import ServiceBusClient
+import os
+import json
+
+# all types of EventGridEvents below produce same DeserializedEvent
+connection_str = os.environ['SERVICE_BUS_CONN_STR']
+queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
+
+with ServiceBusClient.from_connection_string(connection_str) as sb_client:
+    payload =  sb_client.get_queue_receiver(queue_name).receive_messages()
+
+    ## deserialize payload into a list of typed Events
+    events = [EventGridEvent.from_dict(json.loads(next(msg.body).decode('utf-8'))) for msg in payload]
+```
+
+## Distributed Tracing with EventGrid
+
+You can use OpenTelemetry for Python as usual with EventGrid since it's compatible with azure-core tracing integration.
+
+Here is an example of using OpenTelemetry to trace sending a CloudEvent.
+
+First, set OpenTelemetry as enabled tracing plugin for EventGrid.
+
+```python
+from azure.core.settings import settings
+from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
+
+settings.tracing_implementation = OpenTelemetrySpan
+```
+
+Regular open telemetry usage from here. See [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-python) for details.
+This example uses a simple console exporter to export the traces. Any exporter can be used here including `azure-monitor-opentelemetry-exporter`, `jaeger`, `zipkin` etc.
+
+```python
+from opentelemetry import trace
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.export import ConsoleSpanExporter
+from opentelemetry.sdk.trace.export import SimpleSpanProcessor  # this requires opentelemetry >= 1.0.0
+
+# Simple console exporter
+exporter = ConsoleSpanExporter()
+
+trace.set_tracer_provider(TracerProvider())
+tracer = trace.get_tracer(__name__)
+trace.get_tracer_provider().add_span_processor(
+    SimpleSpanProcessor(exporter)
+)
+```
+
+Once the `tracer` and `exporter` are set, please follow the example below to start collecting traces while using the `send` method from the `EventGridPublisherClient` to send a CloudEvent object.
+
+```python
+import os
+from azure.eventgrid import EventGridPublisherClient
+from azure.core.messaging import CloudEvent
+from azure.core.credentials import AzureKeyCredential
+
+hostname = os.environ['CLOUD_TOPIC_HOSTNAME']
+key = AzureKeyCredential(os.environ['CLOUD_ACCESS_KEY'])
+cloud_event = CloudEvent(
+    source = 'demo',
+    type = 'sdk.demo',
+    data = {'test': 'hello'},
+)
+with tracer.start_as_current_span(name="MyApplication"):
+    client = EventGridPublisherClient(hostname, key)
+    client.send(cloud_event)
+```
+
+## Troubleshooting
+
+- Enable `azure.eventgrid` logger to collect traces from the library.
+
+### General
+Event Grid client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
+
+### Logging
+This library uses the standard
+[logging][python_logging] library for logging.
+Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO
+level.
+
+### Optional Configuration
+
+Optional keyword arguments can be passed in at the client and per-operation level.
+The azure-core [reference documentation][azure_core_ref_docs]
+describes available configurations for retries, logging, transport protocols, and more.
+
+## Next steps
+
+The following section provides several code snippets illustrating common patterns used in the Event Grid Python API.
+
+### More sample code
+
+These code samples show common champion scenario operations with the Azure Event Grid client library.
+
+* Generate Shared Access Signature: [sample_generate_sas.py][python-eg-generate-sas]
+
+* Authenticate the client: [sample_authentication.py][python-eg-auth] ([async_version][python-eg-auth-async])
+
+* Publish events to a topic using SAS: [sample_publish_events_to_a_topic_using_sas_credential_async.py][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async])
+* Publish Event Grid Events to a topic: [sample_publish_eg_events_to_a_topic.py][python-eg-sample-eg-event] ([async_version][python-eg-sample-eg-event-async])
+* Publish EventGrid Events to a domain topic: [sample_publish_eg_events_to_a_domain_topic.py][python-eg-sample-eg-event-to-domain] ([async_version][python-eg-sample-eg-event-to-domain-async])
+* Publish a Cloud Event: [sample_publish_events_using_cloud_events_1.0_schema.py][python-eg-sample-send-cloudevent] ([async_version][python-eg-sample-send-cloudevent-async])
+* Publish a Custom Schema: [sample_publish_custom_schema_to_a_topic.py][python-eg-publish-custom-schema] ([async_version][python-eg-publish-custom-schema-async])
+
+The following samples cover publishing and consuming `dict` representations of EventGridEvents and CloudEvents.
+* Publish EventGridEvent as dict like representation: [sample_publish_eg_event_using_dict.py][python-eg-sample-send-eg-as-dict] ([async_version][python-eg-sample-send-eg-as-dict-async])
+
+* Publish CloudEvent as dict like representation: [sample_publish_cloud_event_using_dict.py][python-eg-sample-send-cloudevent-as-dict] ([async_version][python-eg-sample-send-cloudevent-as-dict-async])
+
+* Consume a Custom Payload of raw cloudevent data: [sample_consume_custom_payload.py][python-eg-sample-consume-custom-payload]
+
+More samples can be found [here][python-eg-samples].
+
+* More samples related to the send scenario can be seen [here][python-eg-publish-samples].
+* To see more samples related to consuming a payload from different messaging services as a typed object, please visit [Consume Samples][python-eg-consume-samples]
+
+### Additional documentation
+
+For more extensive documentation on Azure Event Grid, see the [Event Grid documentation][python-eg-product-docs] on docs.microsoft.com.
+
+## Contributing
+This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
+
+When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
+
+<!-- LINKS -->
+
+[azure_cli_link]: https://pypi.org/project/azure-cli/
+[python-eg-src]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/
+[python-eg-pypi]: https://pypi.org/project/azure-eventgrid
+[python-eg-product-docs]: https://docs.microsoft.com/azure/event-grid/overview
+[python-eg-ref-docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-eventgrid/latest/index.html
+[publisher-service-doc]: https://docs.microsoft.com/azure/event-grid/concepts
+[python-eg-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples
+[python-eg-changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/CHANGELOG.md
+[pip]: https://pypi.org/project/pip/
+
+[azure_portal_create_EG_resource]: https://ms.portal.azure.com/#blade/HubsExtension/BrowseResource/resourceType/Microsoft.EventGrid%2Ftopics
+[azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
+[azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
+[python_logging]: https://docs.python.org/3/library/logging.html
+[azure_core_ref_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core#configurations
+[azure_subscription]: https://azure.microsoft.com/free/
+
+[python-eg-auth]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_authentication.py
+[python-eg-generate-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_generate_sas.py
+[python-eg-sample-send-using-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
+[python-eg-sample-eg-event]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
+[python-eg-sample-eg-event-to-domain]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
+[python-eg-sample-send-cloudevent]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
+[python-eg-publish-custom-schema]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
+[python-eg-sample-send-eg-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_event_using_dict.py
+[python-eg-sample-send-cloudevent-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_cloud_event_using_dict.py
+
+[python-eg-auth-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_authentication_async.py
+[python-eg-sample-send-using-sas-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
+[python-eg-sample-eg-event-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
+[python-eg-sample-eg-event-to-domain-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
+[python-eg-sample-send-cloudevent-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
+[python-eg-publish-custom-schema-async]:https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
+[python-eg-sample-send-eg-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_event_using_dict_async.py
+[python-eg-sample-send-cloudevent-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
+
+[python-eg-publish-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/publish_samples
+[python-eg-consume-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/consume_samples
+[python-eg-sample-consume-custom-payload]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_consume_custom_payload.py
+
+[cla]: https://cla.microsoft.com
+[code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
+[coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
+[coc_contact]: mailto:opencode@microsoft.com
+
+
+# Release History
+
+## 4.9.1 (2022-11-08)
+
+- This version and all future versions will require Python 3.7+.
+
+### Features Added
+
+- Added new enum values to `SystemEventNames` related to health care APIs.
+
+## 4.9.0 (2022-07-05)
+
+### Features Added
+
+- Added support for publishing events to a channel.
+
+## 4.9.0b1 (2022-04-07)
+
+### Features Added
+
+- Added support for publishing events to a channel.
+
+## 4.8.0 (2022-04-06)
+
+- This version and all future versions will require Python 3.6+. Python 2.7 is no longer supported.
+
+### Features Added
+
+- Added new enum values to `SystemEventNames` related to health care APIs.
+
+## 4.7.1 (2021-11-18)
+
+### Bugs Fixed
+
+- The `send` API will raise on exceptions.
+
+## 4.7.0 (2021-11-09)
+
+### Features Added
+
+- Added support for publishing native CNCF cloudevents (https://pypi.org/project/cloudevents/).
+
+## 4.6.0 (2021-10-05)
+
+### Features Added
+
+- Added new enum values to `SystemEvents`.
+
+## 4.5.0 (2021-08-10)
+
+### Features Added
+
+- Added a new enum value `Microsoft.ContainerService.NewKubernetesVersionAvailable` to `SystemEvents`.
+- Added a `from_json` method which now accepts storage QueueMessage, eventhub's EventData or ServiceBusMessage or simply json bytes to return an `EventGridEvent`
+
+## 4.4.0 (2021-07-19)
+
+- Bumped `msrest` dependency to `0.6.21` to align with mgmt package.
+
+### Features Added
+
+- `EventGridPublisherClient` now supports Azure Active Directory (AAD) for authentication.
+
+## 4.3.0 (2021-06-09)
+
+  **New Features**
+  - Added new event names related to blob inventory to the `SystemEventNames` enum.
+
+  **Bug Fixes**
+  - Replaced the `ServiceBusDeadletterMessagesAvailableWithNoListenerEventName` with the right value.
+
+## 4.2.0 (2021-05-12)
+
+  **New Features**
+  - Added new event names to the `SystemEventNames` enum.
+
+## 4.1.1 (2021-04-07)
+
+  **Bug Fixes**
+  - Improved the `repr` on `EventGridEvent` to show more meaningful text.
+
+## 4.1.0 (2021-03-23)
+
+  **New Features**
+  - Added new SystemEventNames `AcsChatThreadParticipantRemovedEventName`, `AcsChatThreadParticipantAddedEventName` and `AcsRecordingFileStatusUpdatedEventName`.
+
+## 4.0.0 (2021-03-09)
+
+  **Note:** This is the first stable release of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid. Users migrating from `v1.x` are advised to view the [migration guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/migration_guide.md).
+
+  **New Features**
+  - `azure-eventgrid` package now supports `azure.core.messaging.CloudEvent` which honors the CNCF CloudEvent spec.
+  - `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping for system events.
+  - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and Custom schema events.
+
+  **Breaking Changes**
+  - `azure.eventgrid.models` namespace along with all the models in it are now removed.:
+      - JSON documentation on the events is available here: https://docs.microsoft.com/azure/event-grid/system-topics
+      - `azure.eventgrid.SystemEventNames` provides the list of available events name for easy switching.
+  - `azure.eventgrid.event_grid_client.EventGridClient` is now removed in favor of `azure.eventgrid.EventGridPublisherClient`.
+  - `azure.eventgrid.event_grid_client.EventGridClientConfiguration` is now removed.
+
+
+## 2.0.0 (2021-03-09)
+
+  **Disclaimer:** v2.0.0 is functionally equivalent to v4.0.0. Users are advised to use v4.0.0 instead of this.
+
+  **Breaking Changes**
+  - `~azure.eventgrid.CloudEvent` is now removed in favor of `~azure.core.messaging.CloudEvent`.
+  - All the `SystemEventNames` related to Azure Communication Service starting with `ACS****` are renamed to `Acs***` to honor pascal case.
+
+  **Features**
+  - Added support for two new `SystemEvents` - `ServiceBusDeadletterMessagesAvailablePeriodicNotificationsEventData` and `ServiceBusActiveMessagesAvailablePeriodicNotificationsEventData`
+
+## 2.0.0b5 (2021-02-10)
+
+  **Breaking Changes**
+  - `EventGridSharedAccessSignatureCredential` is deprecated in favor of `AzureSasCredential`.
+  - `azure.eventgrid.models` namespace along with all the models in it are now removed. `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping.
+  - `topic_hostname` is renamed to `endpoint` in the `EventGridPublisherClient`.
+  - `azure.eventgrid.generate_shared_access_signature` method is now renamed to `generate_sas`.
+  - `EventGridConsumer`is now removed. Please see the samples to see how events can be deserialized.
+  - `CustomEvent` model is removed. Dictionaries must be used to send a custom schema.
+
+  **Bug Fixes**
+  - `EventGridEvent` has two additional required positional parameters namely, `data` and `data_version`.
+  - `EventGridPublisherClient` now appropriately throws a `ValueError` if an invalid credential is passed during initialization.
+
+## 2.0.0b4 (2020-11-11)
+
+  **Bug Fixes**
+  - `TypeError` is raised when bytes are passed to an `EventGridEvent`.
+
+## 2.0.0b3 (2020-10-05)
+
+  **Feature**
+  - Added support for Keyvault Event Types
+  - Added distributed tracing support for CloudEvents
+
+## 2.0.0b2 (2020-09-24)
+
+  **Features**
+  - Added support for Azure Communication Services event types.
+
+## 2.0.0b1 (2020-09-08)
+
+  **Features**
+  - Version (2.0.0b1) is the first preview of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid.
+  For more information about this, and preview releases of other Azure SDK libraries, please visit https://azure.github.io/azure-sdk/releases/latest/python.html.
+  - Added Support for `CloudEvents`.
+  - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and CustomEvents.
+  - Implements the `EventGridConsumer` for the consume flow of the events.
+
+## 1.3.0 (2019-05-20)
+
+  - Event Schemas for new event types from IotHub, Media Services,
+    Container Registry, Maps, and AppConfiguration services.
+
+## 1.2.0 (2018-08-28)
+
+  - Event Schemas for new events (IotHub DeviceConnected and
+    DeviceDisconnected events, Resource events related to actions), and
+    breaking changes to the schema for IotHub DeviceCreated event and
+    IotHub DeviceDeleted event.
+
+## 1.1.0 (2018-05-24)
+
+  - Event Schemas for EventGrid subscription validation event, Azure
+    Media events, and ServiceBus events.
+
+## 1.0.0 (2018-04-26)
+
+**General Breaking changes**
+
+This version uses a next-generation code generator that *might*
+introduce breaking changes.
+
+  - Model signatures now use only keyword-argument syntax. All
+    positional arguments must be re-written as keyword-arguments. To
+    keep auto-completion in most cases, models are now generated for
+    Python 2 and Python 3. Python 3 uses the "*" syntax for
+    keyword-only arguments.
+  - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to
+    improve the behavior when unrecognized enum values are encountered.
+    While this is not a breaking change, the distinctions are important,
+    and are documented here:
+    <https://docs.python.org/3/library/enum.html#others> At a glance:
+      - "is" should not be used at all.
+      - "format" will return the string value, where "%s" string
+        formatting will return `NameOfEnum.stringvalue`. Format syntax
+        should be preferred.
+  - New Long Running Operation:
+      - Return type changes from
+        `msrestazure.azure_operation.AzureOperationPoller` to
+        `msrest.polling.LROPoller`. External API is the same.
+      - Return type is now **always** a `msrest.polling.LROPoller`,
+        regardless of the optional parameters used.
+      - The behavior has changed when using `raw=True`. Instead of
+        returning the initial call result as `ClientRawResponse`,
+        without polling, now this returns an LROPoller. After polling,
+        the final resource will be returned as a `ClientRawResponse`.
+      - New `polling` parameter. The default behavior is
+        `Polling=True` which will poll using ARM algorithm. When
+        `Polling=False`, the response of the initial call will be
+        returned without polling.
+      - `polling` parameter accepts instances of subclasses of
+        `msrest.polling.PollingMethod`.
+      - `add_done_callback` will no longer raise if called after
+        polling is finished, but will instead execute the callback right
+        away.
+
+**Features**
+
+  - Client class can be used as a context manager to keep the underlying
+    HTTP session open for performance
+  - Support for consuming Azure Container Registry events and Azure IoT
+    Hub events published to Event Grid.
+
+## 0.1.0 (2018-01-30)
+
+  - Initial Release
```

## Comparing `azure-eventgrid-4.9.0b1/LICENSE` & `azure-eventgrid-4.9.1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/CHANGELOG.md` & `azure-eventgrid-4.9.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Release History
 
+## 4.9.1 (2022-11-08)
+
+- This version and all future versions will require Python 3.7+.
+
+### Features Added
+
+- Added new enum values to `SystemEventNames` related to health care APIs.
+
+## 4.9.0 (2022-07-05)
+
+### Features Added
+
+- Added support for publishing events to a channel.
+
 ## 4.9.0b1 (2022-04-07)
 
 ### Features Added
 
 - Added support for publishing events to a channel.
 
 ## 4.8.0 (2022-04-06)
@@ -170,15 +184,15 @@
     improve the behavior when unrecognized enum values are encountered.
     While this is not a breaking change, the distinctions are important,
     and are documented here:
     <https://docs.python.org/3/library/enum.html#others> At a glance:
       - "is" should not be used at all.
       - "format" will return the string value, where "%s" string
         formatting will return `NameOfEnum.stringvalue`. Format syntax
-        should be prefered.
+        should be preferred.
   - New Long Running Operation:
       - Return type changes from
         `msrestazure.azure_operation.AzureOperationPoller` to
         `msrest.polling.LROPoller`. External API is the same.
       - Return type is now **always** a `msrest.polling.LROPoller`,
         regardless of the optional parameters used.
       - The behavior has changed when using `raw=True`. Instead of
```

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_helpers.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_helpers.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_models.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_models.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_signature_credential_policy.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_signature_credential_policy.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/__init__.py` & `azure-eventgrid-4.9.1/azure/eventgrid/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_publisher_client.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_publisher_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     List[EventGridEvent],
     List[Dict],
 ]
 
 ListEventType = Union[List[CloudEvent], List[EventGridEvent], List[Dict]]
 
 
-class EventGridPublisherClient(object):
+class EventGridPublisherClient(object): # pylint: disable=client-accepts-api-version-keyword
     """EventGridPublisherClient publishes events to an EventGrid topic or domain.
     It can be used to publish either an EventGridEvent, a CloudEvent or a Custom Schema.
 
     :param str endpoint: The topic endpoint to send the events to.
     :param credential: The credential object used for authentication which
      implements SAS key authentication or SAS token authentication or a TokenCredential.
     :type credential: ~azure.core.credentials.AzureKeyCredential or ~azure.core.credentials.AzureSasCredential or
@@ -188,15 +188,16 @@
 
         :param events: A single instance or a list of dictionaries/CloudEvent/EventGridEvent to be sent.
         :type events: ~azure.core.messaging.CloudEvent or ~azure.eventgrid.EventGridEvent or dict or
          List[~azure.core.messaging.CloudEvent] or List[~azure.eventgrid.EventGridEvent] or List[dict]
         :keyword str content_type: The type of content to be used to send the events.
          Has default value "application/json; charset=utf-8" for EventGridEvents,
          with "cloudevents-batch+json" for CloudEvents
-        :keyword str channel_name: Optional. Used to specify the name of event channel when publishing to partner.
+        :keyword channel_name: Optional. Used to specify the name of event channel when publishing to partner.
+        :paramtype channel_name: str or None
          namespaces with partner topic. For more details, visit
          https://docs.microsoft.com/azure/event-grid/partner-events-overview
         :rtype: None
         """
         if not isinstance(events, list):
             events = cast(ListEventType, [events])
         content_type = kwargs.pop("content_type", "application/json; charset=utf-8")
```

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_policies.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _LOGGER = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from azure.core.pipeline import PipelineRequest
 
 
 class CloudEventDistributedTracingPolicy(SansIOHTTPPolicy):
-    """CloudEventDistributedTracingPolicy is a policy which adds distributed tracing informatiom
+    """CloudEventDistributedTracingPolicy is a policy which adds distributed tracing information
     to a batch of cloud events. It does so by copying the `traceparent` and `tracestate` properties
     from the HTTP request into the individual events as extension properties.
     This will only happen in the case where an event does not have a `traceparent` defined already. This
     allows events to explicitly set a traceparent and tracestate which would be respected during "multi-hop
     transmission".
     See https://github.com/cloudevents/spec/blob/master/extensions/distributed-tracing.md
     for more information on distributed tracing and cloud events.
```

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_event_mappings.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_event_mappings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 
 # THE VALUES IN THE ENUM ARE AUTO-GENERATED. DO NOT EDIT THIS MANUALLY.
 # --------------------------------------------------------------------------------------------
 from enum import Enum
+from azure.core import CaseInsensitiveEnumMeta
 
 # pylint: disable=line-too-long
-
-class SystemEventNames(str, Enum):
+# pylint: disable=enum-must-be-uppercase
+class SystemEventNames(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """
     This enum represents the names of the various event types for the system events published to
     Azure Event Grid. To check the list of recognizable system topics,
     visit https://docs.microsoft.com/azure/event-grid/system-topics.
     """
     # These names at the top are 'corrected' aliases of duplicate values that appear below, which are
     # deprecated but maintained for backwards compatibility.
@@ -137,14 +138,20 @@
 
     ContainerRegistryImagePushedEventName = 'Microsoft.ContainerRegistry.ImagePushed'
 
     ContainerServiceNewKubernetesVersionAvailableEventName = 'Microsoft.ContainerService.NewKubernetesVersionAvailable'
 
     EventHubCaptureFileCreatedEventName = 'Microsoft.EventHub.CaptureFileCreated'
 
+    # spell-checker:ignore Dicom
+    HealthcareDicomImageCreatedEventName = 'Microsoft.HealthcareApis.DicomImageCreated'
+
+    HealthcareDicomImageDeletedEventName = 'Microsoft.HealthcareApis.DicomImageDeleted'
+
+    # spell-checker:ignore Fhir
     HealthcareFhirResourceCreatedEventName = 'Microsoft.HealthcareApis.FhirResourceCreated'
 
     HealthcareFhirResourceDeletedEventName = 'Microsoft.HealthcareApis.FhirResourceDeleted'
 
     HealthcareFhirResourceUpdatedEventName = 'Microsoft.HealthcareApis.FhirResourceUpdated'
 
     IotHubDeviceConnectedEventName = 'Microsoft.Devices.DeviceConnected'
@@ -193,14 +200,15 @@
 
     MapsGeofenceResultEventName = 'Microsoft.Maps.GeofenceResult'
 
     MediaJobCanceledEventName = 'Microsoft.Media.JobCanceled'
 
     MediaJobCancelingEventName = 'Microsoft.Media.JobCanceling'
 
+    # spell-checker:ignore Errored
     MediaJobErroredEventName = 'Microsoft.Media.JobErrored'
 
     MediaJobFinishedEventName = 'Microsoft.Media.JobFinished'
 
     MediaJobOutputCanceledEventName = 'Microsoft.Media.JobOutputCanceled'
 
     MediaJobOutputCancelingEventName = 'Microsoft.Media.JobOutputCanceling'
```

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_messaging_shared.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_messaging_shared.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_constants.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/_configuration.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/_event_grid_publisher_client.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/_event_grid_publisher_client.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/__init__.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/__init__.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/_request_builders_py3.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/_request_builders_py3.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/rest/_request_builders.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/rest/_request_builders.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_configuration.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_configuration_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_event_grid_publisher_client.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_event_grid_publisher_client.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/__init__.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_event_grid_publisher_client_async.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_event_grid_publisher_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/aio/_configuration_async.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/_models_py3.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/_models.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/_generated/models/__init__.py` & `azure-eventgrid-4.9.1/azure/eventgrid/_generated/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/azure/eventgrid/aio/_publisher_client_async.py` & `azure-eventgrid-4.9.1/azure/eventgrid/aio/_publisher_client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 SendType = Union[
     CloudEvent, EventGridEvent, Dict, List[CloudEvent], List[EventGridEvent], List[Dict]
 ]
 
 ListEventType = Union[List[CloudEvent], List[EventGridEvent], List[Dict]]
 
 
-class EventGridPublisherClient:
+class EventGridPublisherClient: # pylint: disable=client-accepts-api-version-keyword
     """Asynchronous EventGridPublisherClient publishes events to an EventGrid topic or domain.
     It can be used to publish either an EventGridEvent, a CloudEvent or a Custom Schema.
 
     :param str endpoint: The topic endpoint to send the events to.
     :param credential: The credential object used for authentication which implements
      SAS key authentication or SAS token authentication or an AsyncTokenCredential.
     :type credential: ~azure.core.credentials.AzureKeyCredential or ~azure.core.credentials.AzureSasCredential or
@@ -183,15 +183,16 @@
 
         :param events: A single instance or a list of dictionaries/CloudEvent/EventGridEvent to be sent.
         :type events: ~azure.core.messaging.CloudEvent or ~azure.eventgrid.EventGridEvent or dict or
          List[~azure.core.messaging.CloudEvent] or List[~azure.eventgrid.EventGridEvent] or List[dict]
         :keyword str content_type: The type of content to be used to send the events.
          Has default value "application/json; charset=utf-8" for EventGridEvents,
          with "cloudevents-batch+json" for CloudEvents
-        :keyword str channel_name: Optional. Used to specify the name of event channel when publishing to partner
+        :keyword channel_name: Optional. Used to specify the name of event channel when publishing to partner
+        :paramtype channel_name: str or None
          namespaces with partner topic. For more details, visit
          https://docs.microsoft.com/azure/event-grid/partner-events-overview
         :rtype: None
         """
         if not isinstance(events, list):
             events = cast(ListEventType, [events])
         content_type = kwargs.pop("content_type", "application/json; charset=utf-8")
```

## Comparing `azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/PKG-INFO` & `azure-eventgrid-4.9.1/azure_eventgrid.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,721 +1,734 @@
 Metadata-Version: 2.1
 Name: azure-eventgrid
-Version: 4.9.0b1
+Version: 4.9.1
 Summary: Microsoft Azure Event Grid Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: # Azure Event Grid client library for Python
-        
-        Azure Event Grid is a fully-managed intelligent event routing service that allows for uniform event consumption using a publish-subscribe model.
-        
-        [Source code][python-eg-src] | [Package (PyPI)][python-eg-pypi] | [API reference documentation][python-eg-ref-docs] | [Product documentation][python-eg-product-docs] | [Samples][python-eg-samples] | [Changelog][python-eg-changelog]
-        
-        ## _Disclaimer_
-        
-        _Azure SDK Python packages support for Python 2.7 has ended on 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
-        
-        ## Getting started
-        
-        ### Prerequisites
-        * Python 3.6 or later is required to use this package.
-        * You must have an [Azure subscription][azure_subscription] and an Event Grid Topic resource to use this package. Follow this [step-by-step tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart-portal) to register the Event Grid resource provider and create Event Grid topics using the [Azure portal](https://portal.azure.com/). There is a [similar tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart) using [Azure CLI](https://docs.microsoft.com/cli/azure).
-        
-        
-        ### Install the package
-        Install the Azure Event Grid client library for Python with [pip][pip]:
-        
-        ```bash
-        pip install azure-eventgrid
-        ```
-        
-        * An existing Event Grid topic or domain is required. You can create the resource using [Azure Portal][azure_portal_create_EG_resource] or [Azure CLI][azure_cli_link]
-        
-        If you use Azure CLI, replace `<resource-group-name>` and `<resource-name>` with your own unique names.
-        
-        #### Create an Event Grid Topic
-        
-        ```
-        az eventgrid topic --create --location <location> --resource-group <resource-group-name> --name <resource-name>
-        ```
-        
-        #### Create an Event Grid Domain
-        
-        ```
-        az eventgrid domain --create --location <location> --resource-group <resource-group-name> --name <resource-name>
-        ```
-        
-        ### Authenticate the client
-        In order to interact with the Event Grid service, you will need to create an instance of a client.
-        An **endpoint** and **credential** are necessary to instantiate the client object.
-        
-        #### Using Azure Active Directory (AAD)
-        
-        Azure Event Grid provides integration with Azure Active Directory (Azure AD) for identity-based authentication of requests. With Azure AD, you can use role-based access control (RBAC) to grant access to your Azure Event Grid resources to users, groups, or applications.
-        
-        To send events to a topic or domain with a `TokenCredential`, the authenticated identity should have the "EventGrid Data Sender" role assigned.
-        
-        With the `azure-identity` package, you can seamlessly authorize requests in both development and production environments. To learn more about Azure Active Directory, see the [`azure-identity` README](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/identity/azure-identity/README.md).
-        
-        For example, you can use `DefaultAzureCredential` to construct a client which will authenticate using Azure Active Directory:
-        
-        ```Python
-        from azure.identity import DefaultAzureCredential
-        from azure.eventgrid import EventGridPublisherClient, EventGridEvent
-        
-        event = EventGridEvent(
-            data={"team": "azure-sdk"},
-            subject="Door1",
-            event_type="Azure.Sdk.Demo",
-            data_version="2.0"
-        )
-        
-        credential = DefaultAzureCredential()
-        endpoint = os.environ["EG_TOPIC_HOSTNAME"]
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        #### Looking up the endpoint
-        You can find the topic endpoint within the Event Grid Topic resource on the Azure portal. This will look like:
-        `"https://<event-grid-topic-name>.<topic-location>.eventgrid.azure.net/api/events"`
-        
-        #### Create the client with AzureKeyCredential
-        
-        To use an Access key as the `credential` parameter,
-        pass the key as a string into an instance of [AzureKeyCredential][azure-key-credential].
-        
-        > **Note:** The Access Key may be found in the azure portal in the "Access Keys" menu of the Event Grid Topic resource.  They may also be obtained via the azure CLI, or the `azure-mgmt-eventgrid` library. A guide for getting access keys can be found [here](https://docs.microsoft.com/azure/event-grid/get-access-keys).
-        
-        ```python
-        from azure.core.credentials import AzureKeyCredential
-        from azure.eventgrid import EventGridPublisherClient
-        
-        endpoint = "https://<name>.<region>.eventgrid.azure.net/api/events"
-        credential = AzureKeyCredential("<access_key>")
-        eg_publisher_client = EventGridPublisherClient(endpoint, credential)
-        ```
-        > **Note:** A client may also be authenticated via SAS signature, using the `AzureSasCredential`. A sample demonstrating this, is available [here][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async]).
-        
-        > **Note:** The `generate_sas` method can be used to generate a shared access signature. A sample demonstrating this can be seen [here][python-eg-generate-sas].
-        
-        ## Key concepts
-        
-        ### Topic
-        A **[topic](https://docs.microsoft.com/azure/event-grid/concepts#topics)** is a channel within the EventGrid service to send events. The event schema that a topic accepts is decided at topic creation time. If events of a schema type are sent to a topic that requires a different schema type, errors will be raised.
-        
-        ### Domain
-        An event **[domain](https://docs.microsoft.com/azure/event-grid/event-domains)** is a management tool for large numbers of Event Grid topics related to the same application. They allow you to publish events to thousands of topics. Domains also give you authorization and authentication control over each topic. For more information, visit [Event domain overview](https://docs.microsoft.com/azure/event-grid/event-domains).
-        
-        When you create an event domain, a publishing endpoint for this domain is made available to you. This process is similar to creating an Event Grid Topic. The only difference is that, when publishing to a domain, you must specify the topic within the domain that you'd like the event to be delivered to.
-        
-        ### Event schemas
-        An **[event](https://docs.microsoft.com/azure/event-grid/concepts#events)** is the smallest amount of information that fully describes something that happened in the system. When a custom topic or domain is created, you must specify the schema that will be used when publishing events.
-        
-        Event Grid supports multiple schemas for encoding events.
-        
-        #### Event Grid schema
-        While you may configure your topic to use a [custom schema](https://docs.microsoft.com/azure/event-grid/input-mappings), it is more common to use the already-defined Event Grid schema. See the specifications and requirements [here](https://docs.microsoft.com/azure/event-grid/event-schema).
-        
-        #### CloudEvents v1.0 schema
-        Another option is to use the CloudEvents v1.0 schema. [CloudEvents](https://cloudevents.io/) is a Cloud Native Computing Foundation project which produces a specification for describing event data in a common way. The service summary of CloudEvents can be found [here](https://docs.microsoft.com/azure/event-grid/cloud-event-schema).
-        
-        ### EventGridPublisherClient
-        `EventGridPublisherClient` provides operations to send event data to a topic hostname specified during client initialization.
-        
-        Regardless of the schema that your topic or domain is configured to use, `EventGridPublisherClient` will be used to publish events to it. Use the `send` method publishing events.
-        
-        The following formats of events are allowed to be sent:
-        - A list or a single instance of strongly typed EventGridEvents.
-        - A dict representation of a serialized EventGridEvent object.
-        - A list or a single instance of strongly typed CloudEvents.
-        - A dict representation of a serialized CloudEvent object.
-        
-        - A dict representation of any Custom Schema.
-        
-        Please have a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples) for detailed examples.
-        
-        
-         **Note:** It is important to know if your topic supports CloudEvents or EventGridEvents before publishing. If you send to a topic that does not support the schema of the event you are sending, send() will throw an exception.
-        
-        ### System Topics
-        A **[system topic](https://docs.microsoft.com/azure/event-grid/system-topics)** in Event Grid represents one or more events published by Azure services such as Azure Storage or Azure Event Hubs. For example, a system topic may represent all blob events or only blob creation and blob deletion events published for a specific storage account.
-        
-        The names of the various event types for the system events published to Azure Event Grid are available in `azure.eventgrid.SystemEventNames`.
-        For complete list of recognizable system topics, visit [System Topics](https://docs.microsoft.com/azure/event-grid/system-topics).
-        
-         For more information about the key concepts on Event Grid, see [Concepts in Azure Event Grid][publisher-service-doc].
-        
-        ## Event Grid on Kubernetes with Azure Arc
-        
-        Event Grid on Kubernetes with Azure Arc is an offering that allows you to run Event Grid on your own Kubernetes cluster. This capability is enabled by the use of Azure Arc enabled Kubernetes. Through Azure Arc enabled Kubernetes, a supported Kubernetes cluster connects to Azure. Once connected, you are able to install Event Grid on it. Learn more about it [here](https://docs.microsoft.com/azure/event-grid/kubernetes/overview).
-        
-        ### Support for CNCF Cloud Events
-        
-        Starting with v4.7.0, this package also supports publishing a CNCF cloud event from https://pypi.org/project/cloudevents/. You would be able to pass a CloudEvent object from this library to the `send` API.
-        
-        ```python
-        
-        from cloudevents.http import CloudEvent
-        
-        event = CloudEvent(...)
-        
-        client.send(event)
-        ```
-        
-        ## Examples
-        
-        The following sections provide several code snippets covering some of the most common Event Grid tasks, including:
-        
-        * [Send an Event Grid Event](#send-an-event-grid-event)
-        * [Send a Cloud Event](#send-a-cloud-event)
-        * [Send Multiple Events](#send-multiple-events)
-        * [Send events as Dictionaries](#send-events-as-dictionaries)
-        * [Consume a payload from storage queue](#consume-from-storage-queue)
-        * [Consume from ServiceBus](#consume-from-servicebus)
-        
-        ### Send an Event Grid Event
-        
-        This example publishes an Event Grid event.
-        
-        ```Python
-        import os
-        from azure.core.credentials import AzureKeyCredential
-        from azure.eventgrid import EventGridPublisherClient, EventGridEvent
-        
-        key = os.environ["EG_ACCESS_KEY"]
-        endpoint = os.environ["EG_TOPIC_HOSTNAME"]
-        
-        event = EventGridEvent(
-            data={"team": "azure-sdk"},
-            subject="Door1",
-            event_type="Azure.Sdk.Demo",
-            data_version="2.0"
-        )
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        ### Send a Cloud Event
-        
-        This example publishes a Cloud event.
-        
-        ```Python
-        import os
-        from azure.core.credentials import AzureKeyCredential
-        from azure.core.messaging import CloudEvent
-        from azure.eventgrid import EventGridPublisherClient
-        
-        key = os.environ["CLOUD_ACCESS_KEY"]
-        endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
-        
-        event = CloudEvent(
-            type="Azure.Sdk.Sample",
-            source="https://egsample.dev/sampleevent",
-            data={"team": "azure-sdk"}
-        )
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        ### Send Multiple events
-        
-        It is possible to send events as a batch when sending multiple events to a topic or a domain. This example sends a list of CloudEvents using the send method.
-        
-        **WARNING:** When sending a list of multiple events at one time, iterating over and sending each event will not result in optimal performance. For best performance, it is highly recommended to send a list of events.
-        
-        ```Python
-        import os
-        from azure.core.credentials import AzureKeyCredential
-        from azure.core.messaging import CloudEvent
-        from azure.eventgrid import EventGridPublisherClient
-        
-        key = os.environ["CLOUD_ACCESS_KEY"]
-        endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
-        
-        event0 = CloudEvent(
-            type="Azure.Sdk.Sample",
-            source="https://egsample.dev/sampleevent",
-            data={"team": "azure-sdk"}
-        )
-        event1 = CloudEvent(
-            type="Azure.Sdk.Sample",
-            source="https://egsample.dev/sampleevent",
-            data={"team2": "azure-eventgrid"}
-        )
-        
-        events = [event0, event1]
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(events)
-        ```
-        
-        ### Send events as dictionaries
-        
-        A dict representation of respective serialized models can also be used to publish CloudEvent(s) or EventGridEvent(s) apart from the strongly typed objects.
-        
-        Use a dict-like representation to send to a topic with custom schema as shown below.
-        
-        ```Python
-        import os
-        import uuid
-        import datetime as dt
-        from msrest.serialization import UTC
-        from azure.core.credentials import AzureKeyCredential
-        from azure.eventgrid import EventGridPublisherClient
-        
-        key = os.environ["CUSTOM_SCHEMA_ACCESS_KEY"]
-        endpoint = os.environ["CUSTOM_SCHEMA_TOPIC_HOSTNAME"]
-        
-        event = custom_schema_event = {
-            "customSubject": "sample",
-            "customEventType": "sample.event",
-            "customDataVersion": "2.0",
-            "customId": uuid.uuid4(),
-            "customEventTime": dt.datetime.now(UTC()).isoformat(),
-            "customData": "sample data"
-            }
-        
-        credential = AzureKeyCredential(key)
-        client = EventGridPublisherClient(endpoint, credential)
-        
-        client.send(event)
-        ```
-        
-        ### Consume from storage queue
-        
-        This example consumes a message received from storage queue and deserializes it to a CloudEvent object.
-        
-        ```Python
-        from azure.core.messaging import CloudEvent
-        from azure.storage.queue import QueueServiceClient, BinaryBase64DecodePolicy
-        import os
-        import json
-        
-        # all types of CloudEvents below produce same DeserializedEvent
-        connection_str = os.environ['STORAGE_QUEUE_CONN_STR']
-        queue_name = os.environ['STORAGE_QUEUE_NAME']
-        
-        with QueueServiceClient.from_connection_string(connection_str) as qsc:
-            payload =  qsc.get_queue_client(
-                queue=queue_name,
-                message_decode_policy=BinaryBase64DecodePolicy()
-                ).peek_messages()
-        
-            ## deserialize payload into a list of typed Events
-            events = [CloudEvent.from_dict(json.loads(msg.content)) for msg in payload]
-        ```
-        
-        ### Consume from servicebus
-        
-        This example consumes a payload message received from ServiceBus and deserializes it to an EventGridEvent object.
-        
-        ```Python
-        from azure.eventgrid import EventGridEvent
-        from azure.servicebus import ServiceBusClient
-        import os
-        import json
-        
-        # all types of EventGridEvents below produce same DeserializedEvent
-        connection_str = os.environ['SERVICE_BUS_CONN_STR']
-        queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
-        
-        with ServiceBusClient.from_connection_string(connection_str) as sb_client:
-            payload =  sb_client.get_queue_receiver(queue_name).receive_messages()
-        
-            ## deserialize payload into a list of typed Events
-            events = [EventGridEvent.from_dict(json.loads(next(msg.body).decode('utf-8'))) for msg in payload]
-        ```
-        
-        ## Distributed Tracing with EventGrid
-        
-        You can use opentelemetry for Python as usual with EventGrid since it's compatible with azure-core tracing integration.
-        
-        Here is an example of using OpenTelemetry to trace sending a CloudEvent.
-        
-        First, set OpenTelemetry as enabled tracing plugin for EventGrid.
-        
-        ```python
-        from azure.core.settings import settings
-        from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
-        
-        settings.tracing_implementation = OpenTelemetrySpan
-        ```
-        
-        Regular open telemetry usage from here. See [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-python) for details.
-        This example uses a simple console exporter to export the traces. Any exporter can be used here including `azure-monitor-opentelemetry-exporter`, `jaeger`, `zipkin` etc.
-        
-        ```python
-        from opentelemetry import trace
-        from opentelemetry.sdk.trace import TracerProvider
-        from opentelemetry.sdk.trace.export import ConsoleSpanExporter
-        from opentelemetry.sdk.trace.export import SimpleSpanProcessor  # this requires opentelemtry >= 1.0.0
-        
-        # Simple console exporter
-        exporter = ConsoleSpanExporter()
-        
-        trace.set_tracer_provider(TracerProvider())
-        tracer = trace.get_tracer(__name__)
-        trace.get_tracer_provider().add_span_processor(
-            SimpleSpanProcessor(exporter)
-        )
-        ```
-        
-        Once the `tracer` and `exporter` are set, please follow the example below to start collecting traces while using the `send` method from the `EventGridPublisherClient` to send a CloudEvent object.
-        
-        ```python
-        import os
-        from azure.eventgrid import EventGridPublisherClient
-        from azure.core.messaging import CloudEvent
-        from azure.core.credentials import AzureKeyCredential
-        
-        hostname = os.environ['CLOUD_TOPIC_HOSTNAME']
-        key = AzureKeyCredential(os.environ['CLOUD_ACCESS_KEY'])
-        cloud_event = CloudEvent(
-            source = 'demo',
-            type = 'sdk.demo',
-            data = {'test': 'hello'},
-        )
-        with tracer.start_as_current_span(name="MyApplication"):
-            client = EventGridPublisherClient(hostname, key)
-            client.send(cloud_event)
-        ```
-        
-        ## Troubleshooting
-        
-        - Enable `azure.eventgrid` logger to collect traces from the library.
-        
-        ### General
-        Event Grid client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
-        
-        ### Logging
-        This library uses the standard
-        [logging][python_logging] library for logging.
-        Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO
-        level.
-        
-        ### Optional Configuration
-        
-        Optional keyword arguments can be passed in at the client and per-operation level.
-        The azure-core [reference documentation][azure_core_ref_docs]
-        describes available configurations for retries, logging, transport protocols, and more.
-        
-        ## Next steps
-        
-        The following section provides several code snippets illustrating common patterns used in the Event Grid Python API.
-        
-        ### More sample code
-        
-        These code samples show common champion scenario operations with the Azure Event Grid client library.
-        
-        * Generate Shared Access Signature: [sample_generate_sas.py][python-eg-generate-sas]
-        
-        * Authenticate the client: [sample_authentication.py][python-eg-auth] ([async_version][python-eg-auth-async])
-        
-        * Publish events to a topic using SAS: [sample_publish_events_to_a_topic_using_sas_credential_async.py][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async])
-        * Publish Event Grid Events to a topic: [sample_publish_eg_events_to_a_topic.py][python-eg-sample-eg-event] ([async_version][python-eg-sample-eg-event-async])
-        * Publish EventGrid Events to a domain topic: [sample_publish_eg_events_to_a_domain_topic.py][python-eg-sample-eg-event-to-domain] ([async_version][python-eg-sample-eg-event-to-domain-async])
-        * Publish a Cloud Event: [sample_publish_events_using_cloud_events_1.0_schema.py][python-eg-sample-send-cloudevent] ([async_version][python-eg-sample-send-cloudevent-async])
-        * Publish a Custom Schema: [sample_publish_custom_schema_to_a_topic.py][python-eg-publish-custom-schema] ([async_version][python-eg-publish-custom-schema-async])
-        
-        The following samples cover publishing and consuming `dict` representations of EventGridEvents and CloudEvents.
-        * Publish EventGridEvent as dict like representation: [sample_publish_eg_event_using_dict.py][python-eg-sample-send-eg-as-dict] ([async_version][python-eg-sample-send-eg-as-dict-async])
-        
-        * Publish CloudEvent as dict like representation: [sample_publish_cloud_event_using_dict.py][python-eg-sample-send-cloudevent-as-dict] ([async_version][python-eg-sample-send-cloudevent-as-dict-async])
-        
-        * Consume a Custom Payload of raw cloudevent data: [sample_consume_custom_payload.py][python-eg-sample-consume-custom-payload]
-        
-        More samples can be found [here][python-eg-samples].
-        
-        * More samples related to the send scenario can be seen [here][python-eg-publish-samples].
-        * To see more samples related to consuming a payload from different messaging services as a typed object, please visit [Consume Samples][python-eg-consume-samples]
-        
-        ### Additional documentation
-        
-        For more extensive documentation on Azure Event Grid, see the [Event Grid documentation][python-eg-product-docs] on docs.microsoft.com.
-        
-        ## Contributing
-        This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
-        
-        When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
-        
-        This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
-        
-        <!-- LINKS -->
-        
-        [azure_cli_link]: https://pypi.org/project/azure-cli/
-        [python-eg-src]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/
-        [python-eg-pypi]: https://pypi.org/project/azure-eventgrid
-        [python-eg-product-docs]: https://docs.microsoft.com/azure/event-grid/overview
-        [python-eg-ref-docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-eventgrid/latest/index.html
-        [publisher-service-doc]: https://docs.microsoft.com/azure/event-grid/concepts
-        [python-eg-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples
-        [python-eg-changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/CHANGELOG.md
-        [pip]: https://pypi.org/project/pip/
-        
-        [azure_portal_create_EG_resource]: https://ms.portal.azure.com/#blade/HubsExtension/BrowseResource/resourceType/Microsoft.EventGrid%2Ftopics
-        [azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
-        [azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
-        [python_logging]: https://docs.python.org/3/library/logging.html
-        [azure_core_ref_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core#configurations
-        [azure_subscription]: https://azure.microsoft.com/free/
-        
-        [python-eg-auth]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_authentication.py
-        [python-eg-generate-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_generate_sas.py
-        [python-eg-sample-send-using-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
-        [python-eg-sample-eg-event]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
-        [python-eg-sample-eg-event-to-domain]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
-        [python-eg-sample-send-cloudevent]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
-        [python-eg-publish-custom-schema]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
-        [python-eg-sample-send-eg-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_event_using_dict.py
-        [python-eg-sample-send-cloudevent-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_cloud_event_using_dict.py
-        
-        [python-eg-auth-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_authentication_async.py
-        [python-eg-sample-send-using-sas-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
-        [python-eg-sample-eg-event-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
-        [python-eg-sample-eg-event-to-domain-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
-        [python-eg-sample-send-cloudevent-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
-        [python-eg-publish-custom-schema-async]:https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
-        [python-eg-sample-send-eg-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_event_using_dict_async.py
-        [python-eg-sample-send-cloudevent-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
-        
-        [python-eg-publish-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/publish_samples
-        [python-eg-consume-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/consume_samples
-        [python-eg-sample-consume-custom-payload]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_consume_custom_payload.py
-        
-        [cla]: https://cla.microsoft.com
-        [code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
-        [coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
-        [coc_contact]: mailto:opencode@microsoft.com
-        
-        
-        # Release History
-        
-        ## 4.9.0b1 (2022-04-07)
-        
-        ### Features Added
-        
-        - Added support for publishing events to a channel.
-        
-        ## 4.8.0 (2022-04-06)
-        
-        - This version and all future versions will require Python 3.6+. Python 2.7 is no longer supported.
-        
-        ### Features Added
-        
-        - Added new enum values to `SystemEventNames` related to health care APIs.
-        
-        ## 4.7.1 (2021-11-18)
-        
-        ### Bugs Fixed
-        
-        - The `send` API will raise on exceptions.
-        
-        ## 4.7.0 (2021-11-09)
-        
-        ### Features Added
-        
-        - Added support for publishing native CNCF cloudevents (https://pypi.org/project/cloudevents/).
-        
-        ## 4.6.0 (2021-10-05)
-        
-        ### Features Added
-        
-        - Added new enum values to `SystemEvents`.
-        
-        ## 4.5.0 (2021-08-10)
-        
-        ### Features Added
-        
-        - Added a new enum value `Microsoft.ContainerService.NewKubernetesVersionAvailable` to `SystemEvents`.
-        - Added a `from_json` method which now accepts storage QueueMessage, eventhub's EventData or ServiceBusMessage or simply json bytes to return an `EventGridEvent`
-        
-        ## 4.4.0 (2021-07-19)
-        
-        - Bumped `msrest` dependency to `0.6.21` to align with mgmt package.
-        
-        ### Features Added
-        
-        - `EventGridPublisherClient` now supports Azure Active Directory (AAD) for authentication.
-        
-        ## 4.3.0 (2021-06-09)
-        
-          **New Features**
-          - Added new event names related to blob inventory to the `SystemEventNames` enum.
-        
-          **Bug Fixes**
-          - Replaced the `ServiceBusDeadletterMessagesAvailableWithNoListenerEventName` with the right value.
-        
-        ## 4.2.0 (2021-05-12)
-        
-          **New Features**
-          - Added new event names to the `SystemEventNames` enum.
-        
-        ## 4.1.1 (2021-04-07)
-        
-          **Bug Fixes**
-          - Improved the `repr` on `EventGridEvent` to show more meaningful text.
-        
-        ## 4.1.0 (2021-03-23)
-        
-          **New Features**
-          - Added new SystemEventNames `AcsChatThreadParticipantRemovedEventName`, `AcsChatThreadParticipantAddedEventName` and `AcsRecordingFileStatusUpdatedEventName`.
-        
-        ## 4.0.0 (2021-03-09)
-        
-          **Note:** This is the first stable release of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid. Users migrating from `v1.x` are advised to view the [migration guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/migration_guide.md).
-        
-          **New Features**
-          - `azure-eventgrid` package now supports `azure.core.messaging.CloudEvent` which honors the CNCF CloudEvent spec.
-          - `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping for system events.
-          - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and Custom schema events.
-        
-          **Breaking Changes**
-          - `azure.eventgrid.models` namespace along with all the models in it are now removed.:
-              - JSON documentation on the events is available here: https://docs.microsoft.com/azure/event-grid/system-topics
-              - `azure.eventgrid.SystemEventNames` provides the list of available events name for easy switching.
-          - `azure.eventgrid.event_grid_client.EventGridClient` is now removed in favor of `azure.eventgrid.EventGridPublisherClient`.
-          - `azure.eventgrid.event_grid_client.EventGridClientConfiguration` is now removed.
-        
-        
-        ## 2.0.0 (2021-03-09)
-        
-          **Disclaimer:** v2.0.0 is functionally equivalent to v4.0.0. Users are advised to use v4.0.0 instead of this.
-        
-          **Breaking Changes**
-          - `~azure.eventgrid.CloudEvent` is now removed in favor of `~azure.core.messaging.CloudEvent`.
-          - All the `SystemEventNames` related to Azure Communication Service starting with `ACS****` are renamed to `Acs***` to honor pascal case.
-        
-          **Features**
-          - Added support for two new `SystemEvents` - `ServiceBusDeadletterMessagesAvailablePeriodicNotificationsEventData` and `ServiceBusActiveMessagesAvailablePeriodicNotificationsEventData`
-        
-        ## 2.0.0b5 (2021-02-10)
-        
-          **Breaking Changes**
-          - `EventGridSharedAccessSignatureCredential` is deprecated in favor of `AzureSasCredential`.
-          - `azure.eventgrid.models` namespace along with all the models in it are now removed. `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping.
-          - `topic_hostname` is renamed to `endpoint` in the `EventGridPublisherClient`.
-          - `azure.eventgrid.generate_shared_access_signature` method is now renamed to `generate_sas`.
-          - `EventGridConsumer`is now removed. Please see the samples to see how events can be deserialized.
-          - `CustomEvent` model is removed. Dictionaries must be used to send a custom schema.
-        
-          **Bug Fixes**
-          - `EventGridEvent` has two additional required positional parameters namely, `data` and `data_version`.
-          - `EventGridPublisherClient` now appropriately throws a `ValueError` if an invalid credential is passed during initialization.
-        
-        ## 2.0.0b4 (2020-11-11)
-        
-          **Bug Fixes**
-          - `TypeError` is raised when bytes are passed to an `EventGridEvent`.
-        
-        ## 2.0.0b3 (2020-10-05)
-        
-          **Feature**
-          - Added support for Keyvault Event Types
-          - Added distributed tracing support for CloudEvents
-        
-        ## 2.0.0b2 (2020-09-24)
-        
-          **Features**
-          - Added support for Azure Communication Services event types.
-        
-        ## 2.0.0b1 (2020-09-08)
-        
-          **Features**
-          - Version (2.0.0b1) is the first preview of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid.
-          For more information about this, and preview releases of other Azure SDK libraries, please visit https://azure.github.io/azure-sdk/releases/latest/python.html.
-          - Added Support for `CloudEvents`.
-          - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and CustomEvents.
-          - Implements the `EventGridConsumer` for the consume flow of the events.
-        
-        ## 1.3.0 (2019-05-20)
-        
-          - Event Schemas for new event types from IotHub, Media Services,
-            Container Registry, Maps, and AppConfiguration services.
-        
-        ## 1.2.0 (2018-08-28)
-        
-          - Event Schemas for new events (IotHub DeviceConnected and
-            DeviceDisconnected events, Resource events related to actions), and
-            breaking changes to the schema for IotHub DeviceCreated event and
-            IotHub DeviceDeleted event.
-        
-        ## 1.1.0 (2018-05-24)
-        
-          - Event Schemas for EventGrid subscription validation event, Azure
-            Media events, and ServiceBus events.
-        
-        ## 1.0.0 (2018-04-26)
-        
-        **General Breaking changes**
-        
-        This version uses a next-generation code generator that *might*
-        introduce breaking changes.
-        
-          - Model signatures now use only keyword-argument syntax. All
-            positional arguments must be re-written as keyword-arguments. To
-            keep auto-completion in most cases, models are now generated for
-            Python 2 and Python 3. Python 3 uses the "*" syntax for
-            keyword-only arguments.
-          - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to
-            improve the behavior when unrecognized enum values are encountered.
-            While this is not a breaking change, the distinctions are important,
-            and are documented here:
-            <https://docs.python.org/3/library/enum.html#others> At a glance:
-              - "is" should not be used at all.
-              - "format" will return the string value, where "%s" string
-                formatting will return `NameOfEnum.stringvalue`. Format syntax
-                should be prefered.
-          - New Long Running Operation:
-              - Return type changes from
-                `msrestazure.azure_operation.AzureOperationPoller` to
-                `msrest.polling.LROPoller`. External API is the same.
-              - Return type is now **always** a `msrest.polling.LROPoller`,
-                regardless of the optional parameters used.
-              - The behavior has changed when using `raw=True`. Instead of
-                returning the initial call result as `ClientRawResponse`,
-                without polling, now this returns an LROPoller. After polling,
-                the final resource will be returned as a `ClientRawResponse`.
-              - New `polling` parameter. The default behavior is
-                `Polling=True` which will poll using ARM algorithm. When
-                `Polling=False`, the response of the initial call will be
-                returned without polling.
-              - `polling` parameter accepts instances of subclasses of
-                `msrest.polling.PollingMethod`.
-              - `add_done_callback` will no longer raise if called after
-                polling is finished, but will instead execute the callback right
-                away.
-        
-        **Features**
-        
-          - Client class can be used as a context manager to keep the underlying
-            HTTP session open for performance
-          - Support for consuming Azure Container Registry events and Azure IoT
-            Hub events published to Event Grid.
-        
-        ## 0.1.0 (2018-01-30)
-        
-          - Initial Release
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Azure Event Grid client library for Python
+
+Azure Event Grid is a fully-managed intelligent event routing service that allows for uniform event consumption using a publish-subscribe model.
+
+[Source code][python-eg-src] | [Package (PyPI)][python-eg-pypi] | [API reference documentation][python-eg-ref-docs] | [Product documentation][python-eg-product-docs] | [Samples][python-eg-samples] | [Changelog][python-eg-changelog]
+
+## _Disclaimer_
+
+_Azure SDK Python packages support for Python 2.7 has ended on 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
+
+## Getting started
+
+### Prerequisites
+* Python 3.7 or later is required to use this package.
+* You must have an [Azure subscription][azure_subscription] and an Event Grid Topic resource to use this package. Follow this [step-by-step tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart-portal) to register the Event Grid resource provider and create Event Grid topics using the [Azure portal](https://portal.azure.com/). There is a [similar tutorial](https://docs.microsoft.com/azure/event-grid/custom-event-quickstart) using [Azure CLI](https://docs.microsoft.com/cli/azure).
+
+
+### Install the package
+Install the Azure Event Grid client library for Python with [pip][pip]:
+
+```bash
+pip install azure-eventgrid
+```
+
+* An existing Event Grid topic or domain is required. You can create the resource using [Azure Portal][azure_portal_create_EG_resource] or [Azure CLI][azure_cli_link]
+
+If you use Azure CLI, replace `<resource-group-name>` and `<resource-name>` with your own unique names.
+
+#### Create an Event Grid Topic
+
+```
+az eventgrid topic --create --location <location> --resource-group <resource-group-name> --name <resource-name>
+```
+
+#### Create an Event Grid Domain
+
+```
+az eventgrid domain --create --location <location> --resource-group <resource-group-name> --name <resource-name>
+```
+
+### Authenticate the client
+In order to interact with the Event Grid service, you will need to create an instance of a client.
+An **endpoint** and **credential** are necessary to instantiate the client object.
+
+#### Using Azure Active Directory (AAD)
+
+Azure Event Grid provides integration with Azure Active Directory (Azure AD) for identity-based authentication of requests. With Azure AD, you can use role-based access control (RBAC) to grant access to your Azure Event Grid resources to users, groups, or applications.
+
+To send events to a topic or domain with a `TokenCredential`, the authenticated identity should have the "EventGrid Data Sender" role assigned.
+
+With the `azure-identity` package, you can seamlessly authorize requests in both development and production environments. To learn more about Azure Active Directory, see the [`azure-identity` README](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/identity/azure-identity/README.md).
+
+For example, you can use `DefaultAzureCredential` to construct a client which will authenticate using Azure Active Directory:
+
+```Python
+from azure.identity import DefaultAzureCredential
+from azure.eventgrid import EventGridPublisherClient, EventGridEvent
+
+event = EventGridEvent(
+    data={"team": "azure-sdk"},
+    subject="Door1",
+    event_type="Azure.Sdk.Demo",
+    data_version="2.0"
+)
+
+credential = DefaultAzureCredential()
+endpoint = os.environ["EG_TOPIC_HOSTNAME"]
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+#### Looking up the endpoint
+You can find the topic endpoint within the Event Grid Topic resource on the Azure portal. This will look like:
+`"https://<event-grid-topic-name>.<topic-location>.eventgrid.azure.net/api/events"`
+
+#### Create the client with AzureKeyCredential
+
+To use an Access key as the `credential` parameter,
+pass the key as a string into an instance of [AzureKeyCredential][azure-key-credential].
+
+> **Note:** The Access Key may be found in the azure portal in the "Access Keys" menu of the Event Grid Topic resource.  They may also be obtained via the azure CLI, or the `azure-mgmt-eventgrid` library. A guide for getting access keys can be found [here](https://docs.microsoft.com/azure/event-grid/get-access-keys).
+
+```python
+from azure.core.credentials import AzureKeyCredential
+from azure.eventgrid import EventGridPublisherClient
+
+endpoint = "https://<name>.<region>.eventgrid.azure.net/api/events"
+credential = AzureKeyCredential("<access_key>")
+eg_publisher_client = EventGridPublisherClient(endpoint, credential)
+```
+> **Note:** A client may also be authenticated via SAS signature, using the `AzureSasCredential`. A sample demonstrating this, is available [here][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async]).
+
+> **Note:** The `generate_sas` method can be used to generate a shared access signature. A sample demonstrating this can be seen [here][python-eg-generate-sas].
+
+## Key concepts
+
+### Topic
+A **[topic](https://docs.microsoft.com/azure/event-grid/concepts#topics)** is a channel within the EventGrid service to send events. The event schema that a topic accepts is decided at topic creation time. If events of a schema type are sent to a topic that requires a different schema type, errors will be raised.
+
+### Domain
+An event **[domain](https://docs.microsoft.com/azure/event-grid/event-domains)** is a management tool for large numbers of Event Grid topics related to the same application. They allow you to publish events to thousands of topics. Domains also give you authorization and authentication control over each topic. For more information, visit [Event domain overview](https://docs.microsoft.com/azure/event-grid/event-domains).
+
+When you create an event domain, a publishing endpoint for this domain is made available to you. This process is similar to creating an Event Grid Topic. The only difference is that, when publishing to a domain, you must specify the topic within the domain that you'd like the event to be delivered to.
+
+### Event schemas
+An **[event](https://docs.microsoft.com/azure/event-grid/concepts#events)** is the smallest amount of information that fully describes something that happened in the system. When a custom topic or domain is created, you must specify the schema that will be used when publishing events.
+
+Event Grid supports multiple schemas for encoding events.
+
+#### Event Grid schema
+While you may configure your topic to use a [custom schema](https://docs.microsoft.com/azure/event-grid/input-mappings), it is more common to use the already-defined Event Grid schema. See the specifications and requirements [here](https://docs.microsoft.com/azure/event-grid/event-schema).
+
+#### CloudEvents v1.0 schema
+Another option is to use the CloudEvents v1.0 schema. [CloudEvents](https://cloudevents.io/) is a Cloud Native Computing Foundation project which produces a specification for describing event data in a common way. The service summary of CloudEvents can be found [here](https://docs.microsoft.com/azure/event-grid/cloud-event-schema).
+
+### EventGridPublisherClient
+`EventGridPublisherClient` provides operations to send event data to a topic hostname specified during client initialization.
+
+Regardless of the schema that your topic or domain is configured to use, `EventGridPublisherClient` will be used to publish events to it. Use the `send` method publishing events.
+
+The following formats of events are allowed to be sent:
+- A list or a single instance of strongly typed EventGridEvents.
+- A dict representation of a serialized EventGridEvent object.
+- A list or a single instance of strongly typed CloudEvents.
+- A dict representation of a serialized CloudEvent object.
+
+- A dict representation of any Custom Schema.
+
+Please have a look at the [samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples) for detailed examples.
+
+
+ **Note:** It is important to know if your topic supports CloudEvents or EventGridEvents before publishing. If you send to a topic that does not support the schema of the event you are sending, send() will throw an exception.
+
+### System Topics
+A **[system topic](https://docs.microsoft.com/azure/event-grid/system-topics)** in Event Grid represents one or more events published by Azure services such as Azure Storage or Azure Event Hubs. For example, a system topic may represent all blob events or only blob creation and blob deletion events published for a specific storage account.
+
+The names of the various event types for the system events published to Azure Event Grid are available in `azure.eventgrid.SystemEventNames`.
+For complete list of recognizable system topics, visit [System Topics](https://docs.microsoft.com/azure/event-grid/system-topics).
+
+ For more information about the key concepts on Event Grid, see [Concepts in Azure Event Grid][publisher-service-doc].
+
+## Event Grid on Kubernetes with Azure Arc
+
+Event Grid on Kubernetes with Azure Arc is an offering that allows you to run Event Grid on your own Kubernetes cluster. This capability is enabled by the use of Azure Arc enabled Kubernetes. Through Azure Arc enabled Kubernetes, a supported Kubernetes cluster connects to Azure. Once connected, you are able to install Event Grid on it. Learn more about it [here](https://docs.microsoft.com/azure/event-grid/kubernetes/overview).
+
+### Support for CNCF Cloud Events
+
+Starting with v4.7.0, this package also supports publishing a CNCF cloud event from https://pypi.org/project/cloudevents/. You would be able to pass a CloudEvent object from this library to the `send` API.
+
+```python
+
+from cloudevents.http import CloudEvent
+
+event = CloudEvent(...)
+
+client.send(event)
+```
+
+## Examples
+
+The following sections provide several code snippets covering some of the most common Event Grid tasks, including:
+
+* [Send an Event Grid Event](#send-an-event-grid-event)
+* [Send a Cloud Event](#send-a-cloud-event)
+* [Send Multiple Events](#send-multiple-events)
+* [Send events as Dictionaries](#send-events-as-dictionaries)
+* [Consume a payload from storage queue](#consume-from-storage-queue)
+* [Consume from ServiceBus](#consume-from-servicebus)
+
+### Send an Event Grid Event
+
+This example publishes an Event Grid event.
+
+```Python
+import os
+from azure.core.credentials import AzureKeyCredential
+from azure.eventgrid import EventGridPublisherClient, EventGridEvent
+
+key = os.environ["EG_ACCESS_KEY"]
+endpoint = os.environ["EG_TOPIC_HOSTNAME"]
+
+event = EventGridEvent(
+    data={"team": "azure-sdk"},
+    subject="Door1",
+    event_type="Azure.Sdk.Demo",
+    data_version="2.0"
+)
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+### Send a Cloud Event
+
+This example publishes a Cloud event.
+
+```Python
+import os
+from azure.core.credentials import AzureKeyCredential
+from azure.core.messaging import CloudEvent
+from azure.eventgrid import EventGridPublisherClient
+
+key = os.environ["CLOUD_ACCESS_KEY"]
+endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
+
+event = CloudEvent(
+    type="Azure.Sdk.Sample",
+    source="https://egsample.dev/sampleevent",
+    data={"team": "azure-sdk"}
+)
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+### Send Multiple events
+
+It is possible to send events as a batch when sending multiple events to a topic or a domain. This example sends a list of CloudEvents using the send method.
+
+**WARNING:** When sending a list of multiple events at one time, iterating over and sending each event will not result in optimal performance. For best performance, it is highly recommended to send a list of events.
+
+```Python
+import os
+from azure.core.credentials import AzureKeyCredential
+from azure.core.messaging import CloudEvent
+from azure.eventgrid import EventGridPublisherClient
+
+key = os.environ["CLOUD_ACCESS_KEY"]
+endpoint = os.environ["CLOUD_TOPIC_HOSTNAME"]
+
+event0 = CloudEvent(
+    type="Azure.Sdk.Sample",
+    source="https://egsample.dev/sampleevent",
+    data={"team": "azure-sdk"}
+)
+event1 = CloudEvent(
+    type="Azure.Sdk.Sample",
+    source="https://egsample.dev/sampleevent",
+    data={"team2": "azure-eventgrid"}
+)
+
+events = [event0, event1]
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(events)
+```
+
+### Send events as dictionaries
+
+A dict representation of respective serialized models can also be used to publish CloudEvent(s) or EventGridEvent(s) apart from the strongly typed objects.
+
+Use a dict-like representation to send to a topic with custom schema as shown below.
+
+```Python
+import os
+import uuid
+import datetime as dt
+from msrest.serialization import UTC
+from azure.core.credentials import AzureKeyCredential
+from azure.eventgrid import EventGridPublisherClient
+
+key = os.environ["CUSTOM_SCHEMA_ACCESS_KEY"]
+endpoint = os.environ["CUSTOM_SCHEMA_TOPIC_HOSTNAME"]
+
+event = custom_schema_event = {
+    "customSubject": "sample",
+    "customEventType": "sample.event",
+    "customDataVersion": "2.0",
+    "customId": uuid.uuid4(),
+    "customEventTime": dt.datetime.now(UTC()).isoformat(),
+    "customData": "sample data"
+    }
+
+credential = AzureKeyCredential(key)
+client = EventGridPublisherClient(endpoint, credential)
+
+client.send(event)
+```
+
+### Consume from storage queue
+
+This example consumes a message received from storage queue and deserializes it to a CloudEvent object.
+
+```Python
+from azure.core.messaging import CloudEvent
+from azure.storage.queue import QueueServiceClient, BinaryBase64DecodePolicy
+import os
+import json
+
+# all types of CloudEvents below produce same DeserializedEvent
+connection_str = os.environ['STORAGE_QUEUE_CONN_STR']
+queue_name = os.environ['STORAGE_QUEUE_NAME']
+
+with QueueServiceClient.from_connection_string(connection_str) as qsc:
+    payload =  qsc.get_queue_client(
+        queue=queue_name,
+        message_decode_policy=BinaryBase64DecodePolicy()
+        ).peek_messages()
+
+    ## deserialize payload into a list of typed Events
+    events = [CloudEvent.from_dict(json.loads(msg.content)) for msg in payload]
+```
+
+### Consume from servicebus
+
+This example consumes a payload message received from ServiceBus and deserializes it to an EventGridEvent object.
+
+```Python
+from azure.eventgrid import EventGridEvent
+from azure.servicebus import ServiceBusClient
+import os
+import json
+
+# all types of EventGridEvents below produce same DeserializedEvent
+connection_str = os.environ['SERVICE_BUS_CONN_STR']
+queue_name = os.environ['SERVICE_BUS_QUEUE_NAME']
+
+with ServiceBusClient.from_connection_string(connection_str) as sb_client:
+    payload =  sb_client.get_queue_receiver(queue_name).receive_messages()
+
+    ## deserialize payload into a list of typed Events
+    events = [EventGridEvent.from_dict(json.loads(next(msg.body).decode('utf-8'))) for msg in payload]
+```
+
+## Distributed Tracing with EventGrid
+
+You can use OpenTelemetry for Python as usual with EventGrid since it's compatible with azure-core tracing integration.
+
+Here is an example of using OpenTelemetry to trace sending a CloudEvent.
+
+First, set OpenTelemetry as enabled tracing plugin for EventGrid.
+
+```python
+from azure.core.settings import settings
+from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
+
+settings.tracing_implementation = OpenTelemetrySpan
+```
+
+Regular open telemetry usage from here. See [OpenTelemetry](https://github.com/open-telemetry/opentelemetry-python) for details.
+This example uses a simple console exporter to export the traces. Any exporter can be used here including `azure-monitor-opentelemetry-exporter`, `jaeger`, `zipkin` etc.
+
+```python
+from opentelemetry import trace
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.export import ConsoleSpanExporter
+from opentelemetry.sdk.trace.export import SimpleSpanProcessor  # this requires opentelemetry >= 1.0.0
+
+# Simple console exporter
+exporter = ConsoleSpanExporter()
+
+trace.set_tracer_provider(TracerProvider())
+tracer = trace.get_tracer(__name__)
+trace.get_tracer_provider().add_span_processor(
+    SimpleSpanProcessor(exporter)
+)
+```
+
+Once the `tracer` and `exporter` are set, please follow the example below to start collecting traces while using the `send` method from the `EventGridPublisherClient` to send a CloudEvent object.
+
+```python
+import os
+from azure.eventgrid import EventGridPublisherClient
+from azure.core.messaging import CloudEvent
+from azure.core.credentials import AzureKeyCredential
+
+hostname = os.environ['CLOUD_TOPIC_HOSTNAME']
+key = AzureKeyCredential(os.environ['CLOUD_ACCESS_KEY'])
+cloud_event = CloudEvent(
+    source = 'demo',
+    type = 'sdk.demo',
+    data = {'test': 'hello'},
+)
+with tracer.start_as_current_span(name="MyApplication"):
+    client = EventGridPublisherClient(hostname, key)
+    client.send(cloud_event)
+```
+
+## Troubleshooting
+
+- Enable `azure.eventgrid` logger to collect traces from the library.
+
+### General
+Event Grid client library will raise exceptions defined in [Azure Core][azure_core_exceptions].
+
+### Logging
+This library uses the standard
+[logging][python_logging] library for logging.
+Basic information about HTTP sessions (URLs, headers, etc.) is logged at INFO
+level.
+
+### Optional Configuration
+
+Optional keyword arguments can be passed in at the client and per-operation level.
+The azure-core [reference documentation][azure_core_ref_docs]
+describes available configurations for retries, logging, transport protocols, and more.
+
+## Next steps
+
+The following section provides several code snippets illustrating common patterns used in the Event Grid Python API.
+
+### More sample code
+
+These code samples show common champion scenario operations with the Azure Event Grid client library.
+
+* Generate Shared Access Signature: [sample_generate_sas.py][python-eg-generate-sas]
+
+* Authenticate the client: [sample_authentication.py][python-eg-auth] ([async_version][python-eg-auth-async])
+
+* Publish events to a topic using SAS: [sample_publish_events_to_a_topic_using_sas_credential_async.py][python-eg-sample-send-using-sas] ([async_version][python-eg-sample-send-using-sas-async])
+* Publish Event Grid Events to a topic: [sample_publish_eg_events_to_a_topic.py][python-eg-sample-eg-event] ([async_version][python-eg-sample-eg-event-async])
+* Publish EventGrid Events to a domain topic: [sample_publish_eg_events_to_a_domain_topic.py][python-eg-sample-eg-event-to-domain] ([async_version][python-eg-sample-eg-event-to-domain-async])
+* Publish a Cloud Event: [sample_publish_events_using_cloud_events_1.0_schema.py][python-eg-sample-send-cloudevent] ([async_version][python-eg-sample-send-cloudevent-async])
+* Publish a Custom Schema: [sample_publish_custom_schema_to_a_topic.py][python-eg-publish-custom-schema] ([async_version][python-eg-publish-custom-schema-async])
+
+The following samples cover publishing and consuming `dict` representations of EventGridEvents and CloudEvents.
+* Publish EventGridEvent as dict like representation: [sample_publish_eg_event_using_dict.py][python-eg-sample-send-eg-as-dict] ([async_version][python-eg-sample-send-eg-as-dict-async])
+
+* Publish CloudEvent as dict like representation: [sample_publish_cloud_event_using_dict.py][python-eg-sample-send-cloudevent-as-dict] ([async_version][python-eg-sample-send-cloudevent-as-dict-async])
+
+* Consume a Custom Payload of raw cloudevent data: [sample_consume_custom_payload.py][python-eg-sample-consume-custom-payload]
+
+More samples can be found [here][python-eg-samples].
+
+* More samples related to the send scenario can be seen [here][python-eg-publish-samples].
+* To see more samples related to consuming a payload from different messaging services as a typed object, please visit [Consume Samples][python-eg-consume-samples]
+
+### Additional documentation
+
+For more extensive documentation on Azure Event Grid, see the [Event Grid documentation][python-eg-product-docs] on docs.microsoft.com.
+
+## Contributing
+This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [cla.microsoft.com][cla].
+
+When you submit a pull request, a CLA-bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct][code_of_conduct]. For more information see the [Code of Conduct FAQ][coc_faq] or contact [opencode@microsoft.com][coc_contact] with any additional questions or comments.
+
+<!-- LINKS -->
+
+[azure_cli_link]: https://pypi.org/project/azure-cli/
+[python-eg-src]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/
+[python-eg-pypi]: https://pypi.org/project/azure-eventgrid
+[python-eg-product-docs]: https://docs.microsoft.com/azure/event-grid/overview
+[python-eg-ref-docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-eventgrid/latest/index.html
+[publisher-service-doc]: https://docs.microsoft.com/azure/event-grid/concepts
+[python-eg-samples]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/samples
+[python-eg-changelog]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/eventgrid/azure-eventgrid/CHANGELOG.md
+[pip]: https://pypi.org/project/pip/
+
+[azure_portal_create_EG_resource]: https://ms.portal.azure.com/#blade/HubsExtension/BrowseResource/resourceType/Microsoft.EventGrid%2Ftopics
+[azure-key-credential]: https://aka.ms/azsdk/python/core/azurekeycredential
+[azure_core_exceptions]: https://aka.ms/azsdk/python/core/docs#module-azure.core.exceptions
+[python_logging]: https://docs.python.org/3/library/logging.html
+[azure_core_ref_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core#configurations
+[azure_subscription]: https://azure.microsoft.com/free/
+
+[python-eg-auth]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_authentication.py
+[python-eg-generate-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_generate_sas.py
+[python-eg-sample-send-using-sas]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py
+[python-eg-sample-eg-event]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_topic.py
+[python-eg-sample-eg-event-to-domain]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_events_to_a_domain.py
+[python-eg-sample-send-cloudevent]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py
+[python-eg-publish-custom-schema]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py
+[python-eg-sample-send-eg-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_eg_event_using_dict.py
+[python-eg-sample-send-cloudevent-as-dict]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_publish_cloud_event_using_dict.py
+
+[python-eg-auth-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_authentication_async.py
+[python-eg-sample-send-using-sas-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py
+[python-eg-sample-eg-event-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py
+[python-eg-sample-eg-event-to-domain-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py
+[python-eg-sample-send-cloudevent-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py
+[python-eg-publish-custom-schema-async]:https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py
+[python-eg-sample-send-eg-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_eg_event_using_dict_async.py
+[python-eg-sample-send-cloudevent-as-dict-async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/async_samples/sample_publish_cloud_event_using_dict_async.py
+
+[python-eg-publish-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/publish_samples
+[python-eg-consume-samples]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/consume_samples
+[python-eg-sample-consume-custom-payload]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/samples/sync_samples/sample_consume_custom_payload.py
+
+[cla]: https://cla.microsoft.com
+[code_of_conduct]: https://opensource.microsoft.com/codeofconduct/
+[coc_faq]: https://opensource.microsoft.com/codeofconduct/faq/
+[coc_contact]: mailto:opencode@microsoft.com
+
+
+# Release History
+
+## 4.9.1 (2022-11-08)
+
+- This version and all future versions will require Python 3.7+.
+
+### Features Added
+
+- Added new enum values to `SystemEventNames` related to health care APIs.
+
+## 4.9.0 (2022-07-05)
+
+### Features Added
+
+- Added support for publishing events to a channel.
+
+## 4.9.0b1 (2022-04-07)
+
+### Features Added
+
+- Added support for publishing events to a channel.
+
+## 4.8.0 (2022-04-06)
+
+- This version and all future versions will require Python 3.6+. Python 2.7 is no longer supported.
+
+### Features Added
+
+- Added new enum values to `SystemEventNames` related to health care APIs.
+
+## 4.7.1 (2021-11-18)
+
+### Bugs Fixed
+
+- The `send` API will raise on exceptions.
+
+## 4.7.0 (2021-11-09)
+
+### Features Added
+
+- Added support for publishing native CNCF cloudevents (https://pypi.org/project/cloudevents/).
+
+## 4.6.0 (2021-10-05)
+
+### Features Added
+
+- Added new enum values to `SystemEvents`.
+
+## 4.5.0 (2021-08-10)
+
+### Features Added
+
+- Added a new enum value `Microsoft.ContainerService.NewKubernetesVersionAvailable` to `SystemEvents`.
+- Added a `from_json` method which now accepts storage QueueMessage, eventhub's EventData or ServiceBusMessage or simply json bytes to return an `EventGridEvent`
+
+## 4.4.0 (2021-07-19)
+
+- Bumped `msrest` dependency to `0.6.21` to align with mgmt package.
+
+### Features Added
+
+- `EventGridPublisherClient` now supports Azure Active Directory (AAD) for authentication.
+
+## 4.3.0 (2021-06-09)
+
+  **New Features**
+  - Added new event names related to blob inventory to the `SystemEventNames` enum.
+
+  **Bug Fixes**
+  - Replaced the `ServiceBusDeadletterMessagesAvailableWithNoListenerEventName` with the right value.
+
+## 4.2.0 (2021-05-12)
+
+  **New Features**
+  - Added new event names to the `SystemEventNames` enum.
+
+## 4.1.1 (2021-04-07)
+
+  **Bug Fixes**
+  - Improved the `repr` on `EventGridEvent` to show more meaningful text.
+
+## 4.1.0 (2021-03-23)
+
+  **New Features**
+  - Added new SystemEventNames `AcsChatThreadParticipantRemovedEventName`, `AcsChatThreadParticipantAddedEventName` and `AcsRecordingFileStatusUpdatedEventName`.
+
+## 4.0.0 (2021-03-09)
+
+  **Note:** This is the first stable release of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid. Users migrating from `v1.x` are advised to view the [migration guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/eventgrid/azure-eventgrid/migration_guide.md).
+
+  **New Features**
+  - `azure-eventgrid` package now supports `azure.core.messaging.CloudEvent` which honors the CNCF CloudEvent spec.
+  - `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping for system events.
+  - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and Custom schema events.
+
+  **Breaking Changes**
+  - `azure.eventgrid.models` namespace along with all the models in it are now removed.:
+      - JSON documentation on the events is available here: https://docs.microsoft.com/azure/event-grid/system-topics
+      - `azure.eventgrid.SystemEventNames` provides the list of available events name for easy switching.
+  - `azure.eventgrid.event_grid_client.EventGridClient` is now removed in favor of `azure.eventgrid.EventGridPublisherClient`.
+  - `azure.eventgrid.event_grid_client.EventGridClientConfiguration` is now removed.
+
+
+## 2.0.0 (2021-03-09)
+
+  **Disclaimer:** v2.0.0 is functionally equivalent to v4.0.0. Users are advised to use v4.0.0 instead of this.
+
+  **Breaking Changes**
+  - `~azure.eventgrid.CloudEvent` is now removed in favor of `~azure.core.messaging.CloudEvent`.
+  - All the `SystemEventNames` related to Azure Communication Service starting with `ACS****` are renamed to `Acs***` to honor pascal case.
+
+  **Features**
+  - Added support for two new `SystemEvents` - `ServiceBusDeadletterMessagesAvailablePeriodicNotificationsEventData` and `ServiceBusActiveMessagesAvailablePeriodicNotificationsEventData`
+
+## 2.0.0b5 (2021-02-10)
+
+  **Breaking Changes**
+  - `EventGridSharedAccessSignatureCredential` is deprecated in favor of `AzureSasCredential`.
+  - `azure.eventgrid.models` namespace along with all the models in it are now removed. `azure.eventgrid.SystemEventNames` can be used to get the event model type mapping.
+  - `topic_hostname` is renamed to `endpoint` in the `EventGridPublisherClient`.
+  - `azure.eventgrid.generate_shared_access_signature` method is now renamed to `generate_sas`.
+  - `EventGridConsumer`is now removed. Please see the samples to see how events can be deserialized.
+  - `CustomEvent` model is removed. Dictionaries must be used to send a custom schema.
+
+  **Bug Fixes**
+  - `EventGridEvent` has two additional required positional parameters namely, `data` and `data_version`.
+  - `EventGridPublisherClient` now appropriately throws a `ValueError` if an invalid credential is passed during initialization.
+
+## 2.0.0b4 (2020-11-11)
+
+  **Bug Fixes**
+  - `TypeError` is raised when bytes are passed to an `EventGridEvent`.
+
+## 2.0.0b3 (2020-10-05)
+
+  **Feature**
+  - Added support for Keyvault Event Types
+  - Added distributed tracing support for CloudEvents
+
+## 2.0.0b2 (2020-09-24)
+
+  **Features**
+  - Added support for Azure Communication Services event types.
+
+## 2.0.0b1 (2020-09-08)
+
+  **Features**
+  - Version (2.0.0b1) is the first preview of our efforts to create a user-friendly and Pythonic client library for Azure EventGrid.
+  For more information about this, and preview releases of other Azure SDK libraries, please visit https://azure.github.io/azure-sdk/releases/latest/python.html.
+  - Added Support for `CloudEvents`.
+  - Implements the `EventGridPublisherClient` for the publish flow for EventGrid Events, CloudEvents and CustomEvents.
+  - Implements the `EventGridConsumer` for the consume flow of the events.
+
+## 1.3.0 (2019-05-20)
+
+  - Event Schemas for new event types from IotHub, Media Services,
+    Container Registry, Maps, and AppConfiguration services.
+
+## 1.2.0 (2018-08-28)
+
+  - Event Schemas for new events (IotHub DeviceConnected and
+    DeviceDisconnected events, Resource events related to actions), and
+    breaking changes to the schema for IotHub DeviceCreated event and
+    IotHub DeviceDeleted event.
+
+## 1.1.0 (2018-05-24)
+
+  - Event Schemas for EventGrid subscription validation event, Azure
+    Media events, and ServiceBus events.
+
+## 1.0.0 (2018-04-26)
+
+**General Breaking changes**
+
+This version uses a next-generation code generator that *might*
+introduce breaking changes.
+
+  - Model signatures now use only keyword-argument syntax. All
+    positional arguments must be re-written as keyword-arguments. To
+    keep auto-completion in most cases, models are now generated for
+    Python 2 and Python 3. Python 3 uses the "*" syntax for
+    keyword-only arguments.
+  - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to
+    improve the behavior when unrecognized enum values are encountered.
+    While this is not a breaking change, the distinctions are important,
+    and are documented here:
+    <https://docs.python.org/3/library/enum.html#others> At a glance:
+      - "is" should not be used at all.
+      - "format" will return the string value, where "%s" string
+        formatting will return `NameOfEnum.stringvalue`. Format syntax
+        should be preferred.
+  - New Long Running Operation:
+      - Return type changes from
+        `msrestazure.azure_operation.AzureOperationPoller` to
+        `msrest.polling.LROPoller`. External API is the same.
+      - Return type is now **always** a `msrest.polling.LROPoller`,
+        regardless of the optional parameters used.
+      - The behavior has changed when using `raw=True`. Instead of
+        returning the initial call result as `ClientRawResponse`,
+        without polling, now this returns an LROPoller. After polling,
+        the final resource will be returned as a `ClientRawResponse`.
+      - New `polling` parameter. The default behavior is
+        `Polling=True` which will poll using ARM algorithm. When
+        `Polling=False`, the response of the initial call will be
+        returned without polling.
+      - `polling` parameter accepts instances of subclasses of
+        `msrest.polling.PollingMethod`.
+      - `add_done_callback` will no longer raise if called after
+        polling is finished, but will instead execute the callback right
+        away.
+
+**Features**
+
+  - Client class can be used as a context manager to keep the underlying
+    HTTP session open for performance
+  - Support for consuming Azure Container Registry events and Azure IoT
+    Hub events published to Event Grid.
+
+## 0.1.0 (2018-01-30)
+
+  - Initial Release
```

## Comparing `azure-eventgrid-4.9.0b1/azure_eventgrid.egg-info/SOURCES.txt` & `azure-eventgrid-4.9.1/azure_eventgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/_mocks.py` & `azure-eventgrid-4.9.1/tests/_mocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "time":"2020-08-07T02:06:08.11969Z",
     "specversion":"1.0"
 }
 cloud_custom_string = json.dumps(cloud_custom_dict)
 cloud_custom_bytes = cloud_custom_string.encode("utf-8")
 
 # storage eg event
+# spell-checker:ignore swpill eventgridegsub egtopicsamplesub
 eg_storage_dict = {
     "id":"bbab6625-dc56-4b22-abeb-afcc72e5290c",
     "subject":"/blobServices/default/containers/oc2d2817345i200097container/blobs/oc2d2817345i20002296blob",
     "data":{
         "api":"PutBlockList",
         "clientRequestId":"6d79dbfb-0e37-4fc4-981f-442c9ca65760",
         "requestId":"831e1650-001e-001b-66ab-eeb76e000000",
```

## Comparing `azure-eventgrid-4.9.0b1/tests/test_cncf_events_async.py` & `azure-eventgrid-4.9.1/tests/test_cncf_events_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/test_serialization.py` & `azure-eventgrid-4.9.1/tests/test_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         with pytest.raises(TypeError):
             eg_event = EventGridEvent(
                     subject="sample",
                     event_type="Sample.EventGrid.Event",
                     data_version="2.0"
                     )
 
-    def test_import_from_sytem_events(self):
+    def test_import_from_system_events(self):
         var = SystemEventNames.AcsChatMemberAddedToThreadWithUserEventName 
         assert var == "Microsoft.Communication.ChatMemberAddedToThreadWithUser"
         assert SystemEventNames.KeyVaultKeyNearExpiryEventName == "Microsoft.KeyVault.KeyNearExpiry"
         var = SystemEventNames.ServiceBusActiveMessagesAvailableWithNoListenersEventName
         assert var == "Microsoft.ServiceBus.ActiveMessagesAvailableWithNoListeners"
         var = SystemEventNames.AcsChatThreadParticipantAddedEventName
         assert var == "Microsoft.Communication.ChatThreadParticipantAdded"
```

## Comparing `azure-eventgrid-4.9.0b1/tests/test_cncf_events.py` & `azure-eventgrid-4.9.1/tests/test_cncf_events.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/test_cloud_event_tracing.py` & `azure-eventgrid-4.9.1/tests/test_cloud_event_tracing.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 )
 from azure.core.pipeline.transport import HttpRequest
 from azure.core.messaging import CloudEvent
 from azure.eventgrid._policies import CloudEventDistributedTracingPolicy
 from _mocks import (
     cloud_storage_dict
 )
-
+# spell-checker:disable
 _content_type = "application/cloudevents-batch+json; charset=utf-8"
 _traceparent_value = "00-4bf92f3577b34da6a3ce929d0e0e4736-00f067aa0ba902b7-01"
 _tracestate_value = "rojo=00-4bf92f3577b34da6a3ce929d0e0e4736-00f067aa0ba902b7-01,congo=lZWRzIHRoNhcm5hbCBwbGVhc3VyZS4"
-
+# spell-chcker:enable
 
 class EventGridSerializationTests(object):
 
     def test_cloud_event_policy_copies(self):
         policy = CloudEventDistributedTracingPolicy()
 
         body = json.dumps([cloud_storage_dict])
```

## Comparing `azure-eventgrid-4.9.0b1/tests/test_eg_publisher_client.py` & `azure-eventgrid-4.9.1/tests/test_eg_publisher_client.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/test_exceptions.py` & `azure-eventgrid-4.9.1/tests/test_exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/eventgrid_preparer.py` & `azure-eventgrid-4.9.1/tests/eventgrid_preparer.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/test_eg_publisher_client_async.py` & `azure-eventgrid-4.9.1/tests/test_eg_publisher_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/test_eg_event_get_bytes.py` & `azure-eventgrid-4.9.1/tests/test_eg_event_get_bytes.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/test_exceptions_async.py` & `azure-eventgrid-4.9.1/tests/test_exceptions_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/conftest.py` & `azure-eventgrid-4.9.1/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/tests/perfstress_tests/send.py` & `azure-eventgrid-4.9.1/tests/perfstress_tests/send.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,24 @@
         await self.async_publisher_client.close()
         await super().close()
 
     def run_sync(self):
         """The synchronous perf test.
         
         Try to keep this minimal and focused. Using only a single client API.
-        Avoid putting any ancilliary logic (e.g. generating UUIDs), and put this in the setup/init instead
+        Avoid putting any ancillary logic (e.g. generating UUIDs), and put this in the setup/init instead
         so that we're only measuring the client API call.
         """
         self.publisher_client.send(self.event_list)
 
     async def run_async(self):
         """The asynchronous perf test.
         
         Try to keep this minimal and focused. Using only a single client API.
-        Avoid putting any ancilliary logic (e.g. generating UUIDs), and put this in the setup/init instead
+        Avoid putting any ancillary logic (e.g. generating UUIDs), and put this in the setup/init instead
         so that we're only measuring the client API call.
         """
         await self.async_publisher_client.send(self.event_list)
 
     @staticmethod
     def add_arguments(parser):
         super(EventGridPerfTest, EventGridPerfTest).add_arguments(parser)
```

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_events_to_a_topic.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_events_to_a_topic.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_events_using_cloud_events_1.0_schema.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_to_channel.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_to_channel.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_generate_sas.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_generate_sas.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_cloud_event_using_dict.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_cloud_event_using_dict.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_events_to_a_topic_using_sas_credential.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_event_using_dict.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_event_using_dict.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_authentication.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_cncf_cloud_events.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_cncf_cloud_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 client = EventGridPublisherClient(endpoint, credential)
 
 client.send([
     CloudEvent(
         attributes={
             "type": "cloudevent",
             "source": "/cncf/cloud/event/1.0",
-            "subject": "testingcncfevent"
+            "subject": "testing-cncf-event"
         },
         data=b'This is a cncf cloud event.',
     )
 ])
```

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_consume_custom_payload.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_consume_custom_payload.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_eg_events_to_a_domain.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_eg_events_to_a_domain.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py` & `azure-eventgrid-4.9.1/samples/sync_samples/sample_publish_custom_schema_to_a_topic.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/consume_samples/consume_eventgrid_events_from_service_bus_queue.py` & `azure-eventgrid-4.9.1/samples/consume_samples/consume_eventgrid_events_from_service_bus_queue.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/consume_samples/consume_cloud_events_from_storage_queue.py` & `azure-eventgrid-4.9.1/samples/consume_samples/consume_cloud_events_from_storage_queue.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/consume_samples/consume_cloud_events_from_eventhub.py` & `azure-eventgrid-4.9.1/samples/consume_samples/consume_cloud_events_from_eventhub.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/consume_samples/functionsapp/EventGridTrigger1/__init__.py` & `azure-eventgrid-4.9.1/samples/consume_samples/functionsapp/EventGridTrigger1/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/publish_samples/publish_event_grid_events_to_custom_topic_sample.py` & `azure-eventgrid-4.9.1/samples/publish_samples/publish_event_grid_events_to_custom_topic_sample.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/publish_samples/publish_cloud_events_to_custom_topic_sample.py` & `azure-eventgrid-4.9.1/samples/publish_samples/publish_cloud_events_to_custom_topic_sample.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/publish_samples/publish_with_shared_access_signature_sample.py` & `azure-eventgrid-4.9.1/samples/publish_samples/publish_with_shared_access_signature_sample.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/publish_samples/publish_custom_schema_events_to_topic_sample.py` & `azure-eventgrid-4.9.1/samples/publish_samples/publish_custom_schema_events_to_topic_sample.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/publish_samples/publish_cloud_events_to_domain_topic_sample.py` & `azure-eventgrid-4.9.1/samples/publish_samples/publish_cloud_events_to_domain_topic_sample.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_to_channel_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_to_channel_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_event_using_dict_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_event_using_dict_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,9 +53,8 @@
     }
 
     async with client:	
         await client.send([event0, event1])
     # [END publish_eg_event_dict_async]
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish())
+    asyncio.run(publish())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_cloud_event_using_dict_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
-FILE: sample_publish_cloud_event_using_dict_async.py
+FILE: sample_publish_events_using_cloud_events_1.0_schema_async.py
 DESCRIPTION:
-    These samples demonstrate creating a list of CloudEvents using dict representations
-    and sending then as a list.
+    These samples demonstrate creating a list of CloudEvents and sending then as a list.
 USAGE:
-    python sample_publish_cloud_event_using_dict_async.py
+    python sample_publish_events_using_cloud_events_1.0_schema_async.py
     Set the environment variables with your own values before running the sample:
     1) EVENTGRID_CLOUD_EVENT_TOPIC_KEY - The access key of your eventgrid account.
     2) EVENTGRID_CLOUD_EVENT_TOPIC_ENDPOINT - The topic hostname. Typically it exists in the format
     "https://<YOUR-TOPIC-NAME>.<REGION-NAME>.eventgrid.azure.net/api/events".
 """
+# [START publish_cloud_event_to_topic_async]
 import os
 import asyncio
 from azure.core.messaging import CloudEvent
 from azure.eventgrid.aio import EventGridPublisherClient
 from azure.core.credentials import AzureKeyCredential
 
 topic_key = os.environ["EVENTGRID_CLOUD_EVENT_TOPIC_KEY"]
 endpoint = os.environ["EVENTGRID_CLOUD_EVENT_TOPIC_ENDPOINT"]
 
 async def publish():
     credential = AzureKeyCredential(topic_key)
     client = EventGridPublisherClient(endpoint, credential)
 
-    # [START publish_cloud_event_dict_async]
-    async with client:
-        await client.send([
-            {
-                "type": "Contoso.Items.ItemReceived",
-                "source": "/contoso/items",	
-                "data": {	
-                    "itemSku": "Contoso Item SKU #1"	
-                },	
-                "subject": "Door1",	
-                "specversion": "1.0",	
-                "id": "randomclouduuid11"
-            }
-        ])
-    # [END publish_cloud_event_dict_async]
+    await client.send([
+        CloudEvent(
+            type="Contoso.Items.ItemReceived",
+            source="/contoso/items",
+            data={
+                "itemSku": "Contoso Item SKU #1"
+            },
+            subject="Door1"
+        )
+    ])
+# [END publish_cloud_event_to_topic_async]
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish())
+    asyncio.run(publish())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_custom_schema_to_a_topic_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,9 +45,8 @@
     async with client:
         # publish list of events
         await client.send(custom_schema_event)
     
     # [END publish_custom_schema_async]
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish_event())
+    asyncio.run(publish_event())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_authentication_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_events_to_a_topic_using_sas_credential_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,9 +36,8 @@
                 },
                 subject="Door1",
                 data_version="2.0"
             )
         ])
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish())
+    asyncio.run(publish())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_events_using_cloud_events_1.0_schema_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_cncf_cloud_events_async.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
-FILE: sample_publish_events_using_cloud_events_1.0_schema_async.py
+FILE: sample_publish_cncf_cloud_events_async.py
 DESCRIPTION:
-    These samples demonstrate creating a list of CloudEvents and sending then as a list.
+    This sample demonstrates creating sending a cloud event from the CNCF library.
 USAGE:
-    python sample_publish_events_using_cloud_events_1.0_schema_async.py
+    python sample_publish_cncf_cloud_events_async.py
     Set the environment variables with your own values before running the sample:
     1) EVENTGRID_CLOUD_EVENT_TOPIC_KEY - The access key of your eventgrid account.
     2) EVENTGRID_CLOUD_EVENT_TOPIC_ENDPOINT - The topic hostname. Typically it exists in the format
     "https://<YOUR-TOPIC-NAME>.<REGION-NAME>.eventgrid.azure.net/api/events".
 """
-# [START publish_cloud_event_to_topic_async]
 import os
 import asyncio
-from azure.core.messaging import CloudEvent
 from azure.eventgrid.aio import EventGridPublisherClient
 from azure.core.credentials import AzureKeyCredential
+from cloudevents.http import CloudEvent
 
 topic_key = os.environ["EVENTGRID_CLOUD_EVENT_TOPIC_KEY"]
 endpoint = os.environ["EVENTGRID_CLOUD_EVENT_TOPIC_ENDPOINT"]
 
+
 async def publish():
+    
     credential = AzureKeyCredential(topic_key)
     client = EventGridPublisherClient(endpoint, credential)
-
     await client.send([
         CloudEvent(
-            type="Contoso.Items.ItemReceived",
-            source="/contoso/items",
-            data={
-                "itemSku": "Contoso Item SKU #1"
+            attributes={
+                "type": "cloudevent",
+                "source": "/cncf/cloud/event/1.0",
+                "subject": "testing-cncf-event"
             },
-            subject="Door1"
+            data=b'This is a cncf cloud event.',
         )
     ])
-# [END publish_cloud_event_to_topic_async]
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish())
+    asyncio.run(publish())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_events_to_a_domain_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,9 +46,8 @@
             },
             subject="Door1",
             data_version="2.0"
         )
     ])
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish())
+    asyncio.run(publish())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_eg_events_to_a_topic_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,8 @@
             subject="Door1",
             data_version="2.0"
         )
     ])
 # [END publish_eg_event_to_topic_async]
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(publish())
+    asyncio.run(publish())
```

## Comparing `azure-eventgrid-4.9.0b1/samples/async_samples/sample_publish_cncf_cloud_events_async.py` & `azure-eventgrid-4.9.1/samples/async_samples/sample_publish_cloud_event_using_dict_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
-FILE: sample_publish_cncf_cloud_events_async.py
+FILE: sample_publish_cloud_event_using_dict_async.py
 DESCRIPTION:
-    This sample demonstrates creating sending a cloud event from the CNCF library.
+    These samples demonstrate creating a list of CloudEvents using dict representations
+    and sending then as a list.
 USAGE:
-    python sample_publish_cncf_cloud_events_async.py
+    python sample_publish_cloud_event_using_dict_async.py
     Set the environment variables with your own values before running the sample:
     1) EVENTGRID_CLOUD_EVENT_TOPIC_KEY - The access key of your eventgrid account.
     2) EVENTGRID_CLOUD_EVENT_TOPIC_ENDPOINT - The topic hostname. Typically it exists in the format
     "https://<YOUR-TOPIC-NAME>.<REGION-NAME>.eventgrid.azure.net/api/events".
 """
 import os
 import asyncio
+from azure.core.messaging import CloudEvent
 from azure.eventgrid.aio import EventGridPublisherClient
 from azure.core.credentials import AzureKeyCredential
-from cloudevents.http import CloudEvent
 
 topic_key = os.environ["EVENTGRID_CLOUD_EVENT_TOPIC_KEY"]
 endpoint = os.environ["EVENTGRID_CLOUD_EVENT_TOPIC_ENDPOINT"]
 
-
 async def publish():
-    
     credential = AzureKeyCredential(topic_key)
     client = EventGridPublisherClient(endpoint, credential)
-    await client.send([
-        CloudEvent(
-            attributes={
-                "type": "cloudevent",
-                "source": "/cncf/cloud/event/1.0",
-                "subject": "testingcncfevent"
-            },
-            data=b'This is a cncf cloud event.',
-        )
-    ])
+
+    # [START publish_cloud_event_dict_async]
+    async with client:
+        await client.send([
+            {
+                "type": "Contoso.Items.ItemReceived",
+                "source": "/contoso/items",	
+                "data": {	
+                    "itemSku": "Contoso Item SKU #1"	
+                },	
+                "subject": "Door1",	
+                "specversion": "1.0",	
+                "id": "randomclouduuid11"
+            }
+        ])
+    # [END publish_cloud_event_dict_async]
 
 if __name__ == '__main__':
     asyncio.run(publish())
```

