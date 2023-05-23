# Comparing `tmp/buz-1.9.0rc1.tar.gz` & `tmp/buz-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buz-1.9.0rc1.tar", max compression
+gzip compressed data, was "buz-2.0.0rc1.tar", max compression
```

## Comparing `buz-1.9.0rc1.tar` & `buz-2.0.0rc1.tar`

### file list

```diff
@@ -1,101 +1,129 @@
--rw-r--r--   0        0        0     1062 2022-11-15 14:44:53.618677 buz-1.9.0rc1/LICENSE
--rw-r--r--   0        0        0      104 2022-11-15 14:44:53.618677 buz-1.9.0rc1/README.md
--rw-r--r--   0        0        0     1389 2022-11-15 14:44:53.618677 buz-1.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0      109 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/__init__.py
--rw-r--r--   0        0        0      302 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/__init__.py
--rw-r--r--   0        0        0      680 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/base_command_handler.py
--rw-r--r--   0        0        0      193 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/command.py
--rw-r--r--   0        0        0      175 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/command_bus.py
--rw-r--r--   0        0        0      316 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/command_handler.py
--rw-r--r--   0        0        0      370 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/__init__.py
--rw-r--r--   0        0        0      709 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      385 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1031 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      266 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/sync/__init__.py
--rw-r--r--   0        0        0      401 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/sync/more_than_one_command_handler_related_exception.py
--rw-r--r--   0        0        0     1115 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/sync/sync_command_bus.py
--rw-r--r--   0        0        0      256 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/__init__.py
--rw-r--r--   0        0        0      645 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/base_subscriber.py
--rw-r--r--   0        0        0      189 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/event.py
--rw-r--r--   0        0        0      293 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/event_bus.py
--rw-r--r--   0        0        0      656 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/__init__.py
--rw-r--r--   0        0        0      263 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/__init__.py
--rw-r--r--   0        0        0      179 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
--rw-r--r--   0        0        0      756 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
--rw-r--r--   0        0        0      215 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/event_not_published_exception.py
--rw-r--r--   0        0        0      302 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/event_restore_exception.py
--rw-r--r--   0        0        0      258 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/execution_strategy/__init__.py
--rw-r--r--   0        0        0      192 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
--rw-r--r--   0        0        0      429 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
--rw-r--r--   0        0        0     5529 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/kombu_consumer.py
--rw-r--r--   0        0        0     3251 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/kombu_event_bus.py
--rw-r--r--   0        0        0      285 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/publish_strategy/__init__.py
--rw-r--r--   0        0        0      382 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
--rw-r--r--   0        0        0      309 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
--rw-r--r--   0        0        0      894 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/__init__.py
--rw-r--r--   0        0        0      361 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/consume_retrier.py
--rw-r--r--   0        0        0      229 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/consumed_event_retry.py
--rw-r--r--   0        0        0      449 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
--rw-r--r--   0        0        0     1332 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
--rw-r--r--   0        0        0      230 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
--rw-r--r--   0        0        0      993 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py
--rw-r--r--   0        0        0      241 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/reject_callback.py
--rw-r--r--   0        0        0     1236 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
--rw-r--r--   0        0        0       75 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/serializer_enum.py
--rw-r--r--   0        0        0      695 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py
--rw-r--r--   0        0        0      704 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/worker.py
--rw-r--r--   0        0        0      773 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/__init__.py
--rw-r--r--   0        0        0      651 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/base_consume_middleware.py
--rw-r--r--   0        0        0      531 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/base_publish_middleware.py
--rw-r--r--   0        0        0      363 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/consume_middleware.py
--rw-r--r--   0        0        0     1021 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
--rw-r--r--   0        0        0      315 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/publish_middleware.py
--rw-r--r--   0        0        0      949 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
--rw-r--r--   0        0        0      303 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/subscriber.py
--rw-r--r--   0        0        0       91 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/sync/__init__.py
--rw-r--r--   0        0        0     1413 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/sync/sync_event_bus.py
--rw-r--r--   0        0        0     1209 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/__init__.py
--rw-r--r--   0        0        0      506 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
--rw-r--r--   0        0        0      779 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
--rw-r--r--   0        0        0      515 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py
--rw-r--r--   0        0        0      860 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record.py
--rw-r--r--   0        0        0      281 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record_stream_finder.py
--rw-r--r--   0        0        0      708 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
--rw-r--r--   0        0        0      509 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_repository.py
--rw-r--r--   0        0        0       89 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_sorting_criteria.py
--rw-r--r--   0        0        0      903 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
--rw-r--r--   0        0        0     2416 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
--rw-r--r--   0        0        0      272 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/handler.py
--rw-r--r--   0        0        0      293 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/__init__.py
--rw-r--r--   0        0        0      206 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/handler_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/locator.py
--rw-r--r--   0        0        0      206 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/message_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/__init__.py
--rw-r--r--   0        0        0     3517 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/container_locator.py
--rw-r--r--   0        0        0      246 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/handler_already_registered_exception.py
--rw-r--r--   0        0        0      240 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/handler_not_found_exception.py
--rw-r--r--   0        0        0      235 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
--rw-r--r--   0        0        0      370 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/__init__.py
--rw-r--r--   0        0        0      245 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/handler_already_registered_exception.py
--rw-r--r--   0        0        0      234 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/handler_not_registered_exception.py
--rw-r--r--   0        0        0     2082 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/instance_locator.py
--rw-r--r--   0        0        0     1359 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/message.py
--rw-r--r--   0        0        0      176 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/middleware/__init__.py
--rw-r--r--   0        0        0       54 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/middleware/middleware.py
--rw-r--r--   0        0        0     1002 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/middleware/middleware_chain_builder.py
--rw-r--r--   0        0        0        0 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/py.typed
--rw-r--r--   0        0        0      320 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/__init__.py
--rw-r--r--   0        0        0      627 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/base_query_handler.py
--rw-r--r--   0        0        0      364 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/__init__.py
--rw-r--r--   0        0        0      783 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      400 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1052 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      189 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query.py
--rw-r--r--   0        0        0      189 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query_bus.py
--rw-r--r--   0        0        0      328 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query_handler.py
--rw-r--r--   0        0        0      153 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query_response.py
--rw-r--r--   0        0        0      250 2022-11-15 14:44:53.622677 buz-1.9.0rc1/src/buz/query/sync/__init__.py
--rw-r--r--   0        0        0      375 2022-11-15 14:44:53.622677 buz-1.9.0rc1/src/buz/query/sync/more_than_one_query_handler_related_exception.py
--rw-r--r--   0        0        0     1104 2022-11-15 14:44:53.622677 buz-1.9.0rc1/src/buz/query/sync/sync_query_bus.py
--rw-r--r--   0        0        0     1422 2022-11-15 14:45:18.261402 buz-1.9.0rc1/setup.py
--rw-r--r--   0        0        0     1178 2022-11-15 14:45:18.261790 buz-1.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-23 06:51:27.083614 buz-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      104 2023-05-23 06:51:27.083614 buz-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     1329 2023-05-23 06:51:27.083614 buz-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/__init__.py
+-rw-r--r--   0        0        0      271 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/__init__.py
+-rw-r--r--   0        0        0      709 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/base_command_handler.py
+-rw-r--r--   0        0        0      181 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/command_bus.py
+-rw-r--r--   0        0        0      330 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/command_handler.py
+-rw-r--r--   0        0        0      409 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      788 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      449 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1147 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      134 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1239 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py
+-rw-r--r--   0        0        0      193 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/command.py
+-rw-r--r--   0        0        0      554 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/more_than_one_command_handler_related_exception.py
+-rw-r--r--   0        0        0      268 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/base_command_handler.py
+-rw-r--r--   0        0        0      175 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/command_bus.py
+-rw-r--r--   0        0        0      316 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/command_handler.py
+-rw-r--r--   0        0        0      406 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      774 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      420 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1133 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      133 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1153 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/self_process/self_process_command_bus.py
+-rw-r--r--   0        0        0      133 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/synced_async/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/command/synchronous/synced_async/synced_async_command_bus.py
+-rw-r--r--   0        0        0      256 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/base_subscriber.py
+-rw-r--r--   0        0        0      189 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/event.py
+-rw-r--r--   0        0        0      293 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/event_bus.py
+-rw-r--r--   0        0        0      656 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/kombu/__init__.py
+-rw-r--r--   0        0        0      263 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/kombu/consume_strategy/__init__.py
+-rw-r--r--   0        0        0      179 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
+-rw-r--r--   0        0        0      756 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
+-rw-r--r--   0        0        0      215 2023-05-23 06:51:27.083614 buz-2.0.0rc1/src/buz/event/kombu/event_not_published_exception.py
+-rw-r--r--   0        0        0      302 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/event_restore_exception.py
+-rw-r--r--   0        0        0      258 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/execution_strategy/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
+-rw-r--r--   0        0        0      429 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
+-rw-r--r--   0        0        0     5529 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/kombu_consumer.py
+-rw-r--r--   0        0        0     3251 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/kombu_event_bus.py
+-rw-r--r--   0        0        0      285 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/publish_strategy/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
+-rw-r--r--   0        0        0      309 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
+-rw-r--r--   0        0        0      894 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/__init__.py
+-rw-r--r--   0        0        0      361 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/consume_retrier.py
+-rw-r--r--   0        0        0      229 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/consumed_event_retry.py
+-rw-r--r--   0        0        0      449 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
+-rw-r--r--   0        0        0     1332 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
+-rw-r--r--   0        0        0      230 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
+-rw-r--r--   0        0        0      993 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py
+-rw-r--r--   0        0        0      241 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/reject_callback.py
+-rw-r--r--   0        0        0     1236 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
+-rw-r--r--   0        0        0       75 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/serializer_enum.py
+-rw-r--r--   0        0        0      695 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py
+-rw-r--r--   0        0        0      742 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/kombu/worker.py
+-rw-r--r--   0        0        0      773 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/base_consume_middleware.py
+-rw-r--r--   0        0        0      531 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/base_publish_middleware.py
+-rw-r--r--   0        0        0      363 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/consume_middleware.py
+-rw-r--r--   0        0        0     1021 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      315 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/publish_middleware.py
+-rw-r--r--   0        0        0      949 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      303 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/subscriber.py
+-rw-r--r--   0        0        0       91 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/sync/__init__.py
+-rw-r--r--   0        0        0     1413 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/sync/sync_event_bus.py
+-rw-r--r--   0        0        0     1209 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/__init__.py
+-rw-r--r--   0        0        0      506 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
+-rw-r--r--   0        0        0      779 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
+-rw-r--r--   0        0        0      515 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py
+-rw-r--r--   0        0        0      860 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_record.py
+-rw-r--r--   0        0        0      281 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_record_stream_finder.py
+-rw-r--r--   0        0        0      708 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
+-rw-r--r--   0        0        0      509 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_repository.py
+-rw-r--r--   0        0        0       89 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_sorting_criteria.py
+-rw-r--r--   0        0        0      903 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
+-rw-r--r--   0        0        0     2415 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
+-rw-r--r--   0        0        0      272 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/handler.py
+-rw-r--r--   0        0        0      293 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/handler_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      512 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/locator.py
+-rw-r--r--   0        0        0      206 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/message_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      512 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/pypendency/__init__.py
+-rw-r--r--   0        0        0     3517 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/pypendency/container_locator.py
+-rw-r--r--   0        0        0      246 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/pypendency/handler_already_registered_exception.py
+-rw-r--r--   0        0        0      240 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/pypendency/handler_not_found_exception.py
+-rw-r--r--   0        0        0      235 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
+-rw-r--r--   0        0        0      370 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/sync/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/sync/handler_already_registered_exception.py
+-rw-r--r--   0        0        0      234 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/sync/handler_not_registered_exception.py
+-rw-r--r--   0        0        0     2082 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/locator/sync/instance_locator.py
+-rw-r--r--   0        0        0     1359 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/message.py
+-rw-r--r--   0        0        0      176 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/middleware/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/middleware/middleware.py
+-rw-r--r--   0        0        0     1002 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/middleware/middleware_chain_builder.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/py.typed
+-rw-r--r--   0        0        0      274 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/__init__.py
+-rw-r--r--   0        0        0      247 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/__init__.py
+-rw-r--r--   0        0        0      675 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/base_query_handler.py
+-rw-r--r--   0        0        0      404 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      874 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      462 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1148 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      195 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/query_bus.py
+-rw-r--r--   0        0        0      334 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/query_handler.py
+-rw-r--r--   0        0        0      126 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1223 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py
+-rw-r--r--   0        0        0      516 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/more_than_one_query_handler_related_exception.py
+-rw-r--r--   0        0        0      189 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/query.py
+-rw-r--r--   0        0        0      153 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/query_response.py
+-rw-r--r--   0        0        0      244 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/__init__.py
+-rw-r--r--   0        0        0      674 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/base_query_handler.py
+-rw-r--r--   0        0        0      400 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/middleware/__init__.py
+-rw-r--r--   0        0        0      846 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      433 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1095 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      189 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/query_bus.py
+-rw-r--r--   0        0        0      328 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/query_handler.py
+-rw-r--r--   0        0        0      125 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/self_process/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py
+-rw-r--r--   0        0        0      125 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/synced_async/__init__.py
+-rw-r--r--   0        0        0      470 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/query/synchronous/synced_async/synced_async_query_bus.py
+-rw-r--r--   0        0        0       77 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/wrapper/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/wrapper/async_to_sync.py
+-rw-r--r--   0        0        0      266 2023-05-23 06:51:27.087614 buz-2.0.0rc1/src/buz/wrapper/event_loop.py
+-rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 buz-2.0.0rc1/PKG-INFO
```

### Comparing `buz-1.9.0rc1/LICENSE` & `buz-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/pyproject.toml` & `buz-2.0.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 [tool.poetry]
 name = "buz"
-version = "1.9.0rc1"
+version = "2.0.0rc1"
 description = "Buz is a set of light, simple and extensible implementations of event, command and query buses."
 readme = "README.md"
 authors = ["Luis Pintado Lozano <luis.pintado.lozano@gmail.com>"]
+maintainers = ["Fever - Platform Squad <platform@feverup.com>"]
 license = "MIT License"
 classifiers=[
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Typing :: Typed",
-]
+    ]
 include = ["py.typed"]
 
 [tool.poetry.dependencies]
-python = "^3.6.9"
-pypendency = { version = "~0.1.0", optional = true }
-dataclasses = {version = "~0.8", python = "<3.7.0"}
+python = "^3.8.0"
+pypendency = { version = "~0.3.0", optional = true }
 kombu = { version = ">= 4.6.11", optional = true }
 
 [tool.poetry.dev-dependencies]
-black = "^21.5b1"
-mypy = "^0.812"
-tox = "^3.23.1"
-flake8 = "^3.9.2"
-tox-pyenv = "^1.1.0"
+black = "^23.3"
+mypy = "^1.2"
+flake8 = "^5.0.4"
 
 [tool.poetry.extras]
 pypendency = ["pypendency"]
 kombu = ["kombu"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target_version = ['py36', 'py37', 'py38', 'py39']
+target_version = ['py38', 'py39']
 include = '\.pyi?$'
 exclude = '''
-/(
-  | \.git
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-)/
-'''
+    /(
+      | \.git
+      | \.mypy_cache
+      | \.tox
+      | \.venv
+    )/
+    '''
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `buz-1.9.0rc1/src/buz/command/base_command_handler.py` & `buz-2.0.0rc1/src/buz/command/asynchronous/base_command_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Type, get_type_hints
 
 from buz.command import Command
-from buz.command import CommandHandler
+from buz.command.asynchronous.command_handler import CommandHandler
 
 
 class BaseCommandHandler(CommandHandler):
     @classmethod
     def fqn(cls) -> str:
         return f"command_handler.{cls.__module__}.{cls.__name__}"
```

### Comparing `buz-1.9.0rc1/src/buz/command/middleware/base_handle_middleware.py` & `buz-2.0.0rc1/src/buz/command/synchronous/middleware/base_handle_middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
 
-from buz.command import Command, CommandHandler
-from buz.command.middleware import HandleMiddleware, HandleCallable
+from buz.command import Command
+from buz.command.synchronous import CommandHandler
+from buz.command.synchronous.middleware.handle_middleware import HandleMiddleware, HandleCallable
 
 
 class BaseHandleMiddleware(HandleMiddleware):
     def on_handle(self, command: Command, command_handler: CommandHandler, handle: HandleCallable) -> None:
         self._before_on_handle(command, command_handler)
         handle(command, command_handler)
         self._after_on_handle(command, command_handler)
```

### Comparing `buz-1.9.0rc1/src/buz/command/middleware/handle_middleware_chain_resolver.py` & `buz-2.0.0rc1/src/buz/command/asynchronous/self_process/self_process_command_bus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-from typing import List
+from typing import List, Optional
 
-from buz.command import Command, CommandHandler
-from buz.command.middleware import HandleMiddleware, HandleCallable
-from buz.middleware import MiddlewareChainBuilder
-
-
-class HandleMiddlewareChainResolver:
-    def __init__(self, middlewares: List[HandleMiddleware]):
-        self.__middlewares = middlewares
-        self.__middleware_chain_builder: MiddlewareChainBuilder[
-            HandleCallable, HandleMiddleware
-        ] = MiddlewareChainBuilder(middlewares)
-
-    def resolve(self, command: Command, command_handler: CommandHandler, handle: HandleCallable) -> None:
-        chain_callable: HandleCallable = self.__middleware_chain_builder.get_chain_callable(
-            handle, self.__get_middleware_callable
-        )
-        chain_callable(command, command_handler)
+from buz.command import Command
+from buz.command.asynchronous import CommandBus
+from buz.command.asynchronous import CommandHandler
+from buz.command.asynchronous.middleware import HandleMiddleware, HandleMiddlewareChainResolver
+from buz.command import MoreThanOneCommandHandlerRelatedException
 
-    def __get_middleware_callable(self, middleware: HandleMiddleware, next_callable: HandleCallable) -> HandleCallable:
-        return lambda command, command_handler: middleware.on_handle(command, command_handler, next_callable)
+from buz.locator import Locator
+
+
+class SelfProcessCommandBus(CommandBus):
+    def __init__(
+        self,
+        locator: Locator[Command, CommandHandler],
+        middlewares: Optional[List[HandleMiddleware]] = None,
+    ):
+        self.__locator = locator
+        self.__handle_middleware_chain_resolver = HandleMiddlewareChainResolver(middlewares or [])
+
+    async def handle(self, command: Command) -> None:
+        command_handlers = self.__locator.get(command)
+
+        if len(command_handlers) > 1:
+            raise MoreThanOneCommandHandlerRelatedException(command, command_handlers)
+
+        command_handler = command_handlers[0]
+        await self.__handle_middleware_chain_resolver.resolve(command, command_handler, self.__perform_handle)
+
+    @staticmethod
+    async def __perform_handle(command: Command, command_handler: CommandHandler) -> None:
+        await command_handler.handle(command)
```

### Comparing `buz-1.9.0rc1/src/buz/command/sync/sync_command_bus.py` & `buz-2.0.0rc1/src/buz/query/asynchronous/self_process/self_process_query_bus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import List, Optional
 
-from buz.command import CommandBus, Command, CommandHandler
-from buz.command.middleware import HandleMiddleware, HandleMiddlewareChainResolver
-from buz.command.sync import MoreThanOneCommandHandlerRelatedException
 from buz.locator import Locator
+from buz.query import Query, QueryResponse
+from buz.query.asynchronous import QueryBus
+from buz.query.asynchronous import QueryHandler
+from buz.query.asynchronous.middleware import HandleMiddleware, HandleMiddlewareChainResolver
+from buz.query import MoreThanOneQueryHandlerRelatedException
 
 
-class SyncCommandBus(CommandBus):
+class SelfProcessQueryBus(QueryBus):
     def __init__(
         self,
-        locator: Locator[Command, CommandHandler],
+        locator: Locator[Query, QueryHandler],
         middlewares: Optional[List[HandleMiddleware]] = None,
     ):
         self.__locator = locator
         self.__handle_middleware_chain_resolver = HandleMiddlewareChainResolver(middlewares or [])
 
-    def handle(self, command: Command) -> None:
-        command_handlers = self.__locator.get(command)
+    async def handle(self, query: Query) -> QueryResponse:
+        query_handlers = self.__locator.get(query)
 
-        if len(command_handlers) > 1:
-            raise MoreThanOneCommandHandlerRelatedException(command, command_handlers)
+        if len(query_handlers) > 1:
+            raise MoreThanOneQueryHandlerRelatedException(query, query_handlers)
 
-        command_handler = command_handlers[0]
-        self.__handle_middleware_chain_resolver.resolve(command, command_handler, self.__perform_handle)
+        query_handler = query_handlers[0]
+        return await self.__handle_middleware_chain_resolver.resolve(query, query_handler, self.__perform_handle)
 
-    def __perform_handle(self, command: Command, command_handler: CommandHandler) -> None:
-        command_handler.handle(command)
+    @staticmethod
+    async def __perform_handle(query: Query, query_handler: QueryHandler) -> QueryResponse:
+        return await query_handler.handle(query)
```

### Comparing `buz-1.9.0rc1/src/buz/event/base_subscriber.py` & `buz-2.0.0rc1/src/buz/event/base_subscriber.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/__init__.py` & `buz-2.0.0rc1/src/buz/event/kombu/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py` & `buz-2.0.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/kombu_consumer.py` & `buz-2.0.0rc1/src/buz/event/kombu/kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/kombu_event_bus.py` & `buz-2.0.0rc1/src/buz/event/kombu/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/retry/__init__.py` & `buz-2.0.0rc1/src/buz/event/kombu/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py` & `buz-2.0.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py` & `buz-2.0.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py` & `buz-2.0.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py` & `buz-2.0.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/middleware/__init__.py` & `buz-2.0.0rc1/src/buz/event/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/middleware/base_consume_middleware.py` & `buz-2.0.0rc1/src/buz/event/middleware/base_consume_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/middleware/base_publish_middleware.py` & `buz-2.0.0rc1/src/buz/event/middleware/base_publish_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py` & `buz-2.0.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py` & `buz-2.0.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/sync/sync_event_bus.py` & `buz-2.0.0rc1/src/buz/event/sync/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/__init__.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_record.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py` & `buz-2.0.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self.__logger = logger
         self.__max_retries = max_retries
 
     def start(self) -> None:
         criteria = OutboxCriteria(delivered_at=None, order_by=OutboxSortingCriteria.CREATED_AT, delivery_paused=False)
 
         for outbox_record in self.__outbox_record_stream_finder.find(criteria):
-
             try:
                 event = self.__outbox_record_to_event_translator.translate(outbox_record)
 
                 self.__event_bus.publish(event)
                 outbox_record.mark_as_delivered()
 
             except (MessageFqnNotFoundException, EventNotPublishedException) as e:
```

### Comparing `buz-1.9.0rc1/src/buz/locator/locator.py` & `buz-2.0.0rc1/src/buz/locator/locator.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/locator/pypendency/__init__.py` & `buz-2.0.0rc1/src/buz/locator/pypendency/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/locator/pypendency/container_locator.py` & `buz-2.0.0rc1/src/buz/locator/pypendency/container_locator.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/locator/sync/instance_locator.py` & `buz-2.0.0rc1/src/buz/locator/sync/instance_locator.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/message.py` & `buz-2.0.0rc1/src/buz/message.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/middleware/middleware_chain_builder.py` & `buz-2.0.0rc1/src/buz/middleware/middleware_chain_builder.py`

 * *Files identical despite different names*

### Comparing `buz-1.9.0rc1/src/buz/query/middleware/base_handle_middleware.py` & `buz-2.0.0rc1/src/buz/query/synchronous/middleware/base_handle_middleware.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
 
-from buz.query import Query, QueryHandler, QueryResponse
-from buz.query.middleware import HandleMiddleware, HandleCallable
+from buz.query import Query, QueryResponse
+from buz.query.synchronous import QueryHandler
+from buz.query.synchronous.middleware.handle_middleware import HandleMiddleware, HandleCallable
 
 
 class BaseHandleMiddleware(HandleMiddleware):
     def on_handle(self, query: Query, query_handler: QueryHandler, handle: HandleCallable) -> QueryResponse:
         self._before_on_handle(query, query_handler)
         query_response = handle(query, query_handler)
         return self._after_on_handle(query, query_handler, query_response)
```

### Comparing `buz-1.9.0rc1/src/buz/query/middleware/handle_middleware_chain_resolver.py` & `buz-2.0.0rc1/src/buz/query/synchronous/middleware/handle_middleware_chain_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List
 
 from buz.middleware import MiddlewareChainBuilder
-from buz.query import Query, QueryHandler, QueryResponse
-from buz.query.middleware import HandleMiddleware, HandleCallable
+from buz.query import Query, QueryResponse
+from buz.query.synchronous import QueryHandler
+from buz.query.synchronous.middleware import HandleMiddleware, HandleCallable
 
 
 class HandleMiddlewareChainResolver:
     def __init__(self, middlewares: List[HandleMiddleware]):
         self.__middlewares = middlewares
         self.__middleware_chain_builder: MiddlewareChainBuilder[
             HandleCallable, HandleMiddleware
@@ -14,11 +15,10 @@
 
     def resolve(self, query: Query, query_handler: QueryHandler, handle: HandleCallable) -> QueryResponse:
         chain_callable: HandleCallable = self.__middleware_chain_builder.get_chain_callable(
             handle, self.__get_middleware_callable
         )
         return chain_callable(query, query_handler)
 
-    def __get_middleware_callable(
-        self, middleware: HandleMiddleware, handle_callable: HandleCallable
-    ) -> HandleCallable:
+    @staticmethod
+    def __get_middleware_callable(middleware: HandleMiddleware, handle_callable: HandleCallable) -> HandleCallable:
         return lambda query, query_handler: middleware.on_handle(query, query_handler, handle_callable)
```

### Comparing `buz-1.9.0rc1/src/buz/query/sync/sync_query_bus.py` & `buz-2.0.0rc1/src/buz/query/synchronous/self_process/self_process_query_bus.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import List, Optional
 
 from buz.locator import Locator
-from buz.query import QueryBus, Query, QueryHandler, QueryResponse
-from buz.query.middleware import HandleMiddleware, HandleMiddlewareChainResolver
-from buz.query.sync import MoreThanOneQueryHandlerRelatedException
+from buz.query import Query, QueryResponse
+from buz.query.synchronous.middleware import HandleMiddleware, HandleMiddlewareChainResolver
+from buz.query import MoreThanOneQueryHandlerRelatedException
+from buz.query.synchronous import QueryBus, QueryHandler
 
 
-class SyncQueryBus(QueryBus):
+class SelfProcessQueryBus(QueryBus):
     def __init__(
         self,
         locator: Locator[Query, QueryHandler],
         middlewares: Optional[List[HandleMiddleware]] = None,
     ):
         self.__locator = locator
         self.__handle_middleware_chain_resolver = HandleMiddlewareChainResolver(middlewares or [])
@@ -20,9 +21,10 @@
 
         if len(query_handlers) > 1:
             raise MoreThanOneQueryHandlerRelatedException(query, query_handlers)
 
         query_handler = query_handlers[0]
         return self.__handle_middleware_chain_resolver.resolve(query, query_handler, self.__perform_handle)
 
-    def __perform_handle(self, query: Query, query_handler: QueryHandler) -> QueryResponse:
+    @staticmethod
+    def __perform_handle(query: Query, query_handler: QueryHandler) -> QueryResponse:
         return query_handler.handle(query)
```

### Comparing `buz-1.9.0rc1/PKG-INFO` & `buz-2.0.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: buz
-Version: 1.9.0rc1
+Version: 2.0.0rc1
 Summary: Buz is a set of light, simple and extensible implementations of event, command and query buses.
 License: MIT
 Author: Luis Pintado Lozano
 Author-email: luis.pintado.lozano@gmail.com
-Requires-Python: >=3.6.9,<4.0.0
+Maintainer: Fever - Platform Squad
+Maintainer-email: platform@feverup.com
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Provides-Extra: kombu
 Provides-Extra: pypendency
-Requires-Dist: dataclasses (>=0.8,<0.9); python_full_version < "3.7.0"
-Requires-Dist: kombu (>=4.6.11); extra == "kombu"
-Requires-Dist: pypendency (>=0.1.0,<0.2.0); extra == "pypendency"
+Requires-Dist: kombu (>=4.6.11) ; extra == "kombu"
+Requires-Dist: pypendency (>=0.3.0,<0.4.0) ; extra == "pypendency"
 Description-Content-Type: text/markdown
 
 # Buz
 
 Buz is a set of light, simple and extensible implementations of event, command and query buses.
```

