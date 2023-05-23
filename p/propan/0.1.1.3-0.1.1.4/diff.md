# Comparing `tmp/propan-0.1.1.3.tar.gz` & `tmp/propan-0.1.1.4.tar.gz`

## Comparing `propan-0.1.1.3.tar` & `propan-0.1.1.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 propan-0.1.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.3/SECURITY.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 propan-0.1.1.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.3/examples/redis/pattern.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/__about__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/__main__.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/log/logging.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/redis.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.3/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.3/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.3/LICENSE
--rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 propan-0.1.1.3/README.md
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.3/pyproject.toml
--rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 propan-0.1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 propan-0.1.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.1.4/SECURITY.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.1.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.1.4/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.1.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 propan-0.1.1.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.1.4/examples/redis/pattern.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/__about__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/__main__.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/log/logging.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/test/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/test/redis.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.1.4/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.1.4/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.1.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.1.4/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.1.4/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.1.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.1.4/LICENSE
+-rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 propan-0.1.1.4/README.md
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 propan-0.1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 propan-0.1.1.4/PKG-INFO
```

### Comparing `propan-0.1.1.3/CONTRIBUTING.md` & `propan-0.1.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/SECURITY.md` & `propan-0.1.1.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/.github/workflows/documentation.yml` & `propan-0.1.1.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/.github/workflows/publish_coverage.yml` & `propan-0.1.1.4/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/.github/workflows/publish_pypi.yml` & `propan-0.1.1.4/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/.github/workflows/tests.yml` & `propan-0.1.1.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/3_lifespan_events.py` & `propan-0.1.1.4/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/4_cli_attributes_promotion.py` & `propan-0.1.1.4/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/5_publishing.py` & `propan-0.1.1.4/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/6_arguments_casting.py` & `propan-0.1.1.4/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/7_handler_errors_processing.py` & `propan-0.1.1.4/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/dependencies/1_dependency_injection.py` & `propan-0.1.1.4/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.1.4/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.1.4/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.1.4/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.1.4/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/dependencies/7_annotated.py` & `propan-0.1.1.4/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/quart.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.1.4/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/rabbit/direct.py` & `propan-0.1.1.4/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/rabbit/fanout.py` & `propan-0.1.1.4/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/rabbit/header.py` & `propan-0.1.1.4/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/rabbit/topic.py` & `propan-0.1.1.4/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/redis/direct.py` & `propan-0.1.1.4/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/examples/redis/pattern.py` & `propan-0.1.1.4/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/__init__.py` & `propan-0.1.1.4/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/annotations.py` & `propan-0.1.1.4/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/types.py` & `propan-0.1.1.4/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/push_back_watcher.py` & `propan-0.1.1.4/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/model/broker_usecase.py` & `propan-0.1.1.4/propan/brokers/model/broker_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,23 +201,23 @@
             func: Callable[[PropanMessage], Awaitable[T]]
         ) -> Callable[[PropanMessage], Awaitable[T]]:
             @wraps(func)
             async def wrapper(message: PropanMessage) -> T:
                 log_context = self._get_log_context(message=message, **broker_args)
 
                 with context.scope("log_context", log_context):
-                    self._log("Received")
+                    self._log("Received", extra=log_context)
 
                     try:
                         r = await func(message)
                     except Exception as e:
                         self._log(repr(e), logging.ERROR)
                         raise e
                     else:
-                        self._log("Processed")
+                        self._log("Processed", extra=log_context)
                         return r
 
             return wrapper
 
         return decor
 
     def _log(
```

### Comparing `propan-0.1.1.3/propan/brokers/model/schemas.py` & `propan-0.1.1.4/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/model/utils.py` & `propan-0.1.1.4/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/nats/nats_broker.py` & `propan-0.1.1.4/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.1.4/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.1.4/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/nats/schemas.py` & `propan-0.1.1.4/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.1.4/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         )
 
         if self._channel is None:  # pragma: no branch
             max_consumers = self._max_consumers
             self._channel = await connection.channel()
 
             if max_consumers:
-                self._log(f"Set max consumers to {max_consumers}")
+                c = self._get_log_context(None, RabbitQueue(""), RabbitExchange(""))
+                self._log(f"Set max consumers to {max_consumers}", extra=c)
                 await self._channel.set_qos(prefetch_count=int(self._max_consumers))
 
         return connection
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
```

### Comparing `propan-0.1.1.3/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.1.4/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/rabbit/schemas.py` & `propan-0.1.1.4/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/redis/redis_broker.py` & `propan-0.1.1.4/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.1.4/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/brokers/redis/schemas.py` & `propan-0.1.1.4/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/app.py` & `propan-0.1.1.4/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/main.py` & `propan-0.1.1.4/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/startproject/core.py` & `propan-0.1.1.4/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/startproject/async_app/app.py` & `propan-0.1.1.4/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/startproject/async_app/core.py` & `propan-0.1.1.4/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/startproject/async_app/nats.py` & `propan-0.1.1.4/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.1.4/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/startproject/async_app/redis.py` & `propan-0.1.1.4/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/supervisors/basereload.py` & `propan-0.1.1.4/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/supervisors/multiprocess.py` & `propan-0.1.1.4/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/supervisors/utils.py` & `propan-0.1.1.4/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/supervisors/watchfiles.py` & `propan-0.1.1.4/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/utils/imports.py` & `propan-0.1.1.4/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/utils/logs.py` & `propan-0.1.1.4/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/cli/utils/parser.py` & `propan-0.1.1.4/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/fastapi/core/route.py` & `propan-0.1.1.4/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/fastapi/core/router.py` & `propan-0.1.1.4/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/fastapi/rabbit/router.pyi` & `propan-0.1.1.4/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/fastapi/redis/router.pyi` & `propan-0.1.1.4/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/log/formatter.py` & `propan-0.1.1.4/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/log/logging.py` & `propan-0.1.1.4/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/test/rabbit.py` & `propan-0.1.1.4/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/test/redis.py` & `propan-0.1.1.4/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/test/utils.py` & `propan-0.1.1.4/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/utils/functions.py` & `propan-0.1.1.4/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/utils/context/main.py` & `propan-0.1.1.4/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/propan/utils/context/types.py` & `propan-0.1.1.4/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/LICENSE` & `propan-0.1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/README.md` & `propan-0.1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/pyproject.toml` & `propan-0.1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.1.3/PKG-INFO` & `propan-0.1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.1.3
+Version: 0.1.1.4
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.1.3 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.1.4 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
```

