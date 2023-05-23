# Comparing `tmp/qwak_sdk-0.5.3.tar.gz` & `tmp/qwak_sdk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_sdk-0.5.3.tar", max compression
+gzip compressed data, was "qwak_sdk-0.5.4.tar", max compression
```

## Comparing `qwak_sdk-0.5.3.tar` & `qwak_sdk-0.5.4.tar`

### file list

```diff
@@ -1,302 +1,302 @@
--rw-r--r--   0        0        0      183 2023-05-11 08:46:37.673262 qwak_sdk-0.5.3/README.md
--rw-r--r--   0        0        0     2607 2023-05-11 08:47:24.125490 qwak_sdk-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      134 2023-05-11 08:47:24.125490 qwak_sdk-0.5.3/qwak_sdk/__init__.py
--rw-r--r--   0        0        0     2039 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/cli.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/__init__.py
--rw-r--r--   0        0        0      327 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/admin_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/__init__.py
--rw-r--r--   0        0        0      467 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/__init__.py
--rw-r--r--   0        0        0      677 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/_logic.py
--rw-r--r--   0        0        0     1393 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
--rw-r--r--   0        0        0      796 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
--rw-r--r--   0        0        0      942 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/__init__.py
--rw-r--r--   0        0        0      367 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/config_base.py
--rw-r--r--   0        0        0      885 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
--rw-r--r--   0        0        0      886 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
--rw-r--r--   0        0        0     1626 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
--rw-r--r--   0        0        0      817 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
--rw-r--r--   0        0        0      340 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
--rw-r--r--   0        0        0      277 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/spec.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/__init__.py
--rw-r--r--   0        0        0       49 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
--rw-r--r--   0        0        0     3098 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/config.py
--rw-r--r--   0        0        0      646 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/__init__.py
--rw-r--r--   0        0        0     1359 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/_logic.py
--rw-r--r--   0        0        0      949 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/ui.py
--rw-r--r--   0        0        0      277 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/__init__.py
--rw-r--r--   0        0        0      857 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/automations_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/__init__.py
--rw-r--r--   0        0        0      235 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/_logic.py
--rw-r--r--   0        0        0      604 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/__init__.py
--rw-r--r--   0        0        0      346 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/executions_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/__init__.py
--rw-r--r--   0        0        0      330 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/_logic.py
--rw-r--r--   0        0        0      669 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/__init__.py
--rw-r--r--   0        0        0      252 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/_logic.py
--rw-r--r--   0        0        0      546 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/__init__.py
--rw-r--r--   0        0        0     1624 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/_logic.py
--rw-r--r--   0        0        0     1331 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/_logic.py
--rw-r--r--   0        0        0     1039 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/ui.py
--rw-r--r--   0        0        0     1002 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/feature_store_command_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/list/__init__.py
--rw-r--r--   0        0        0     4145 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/list/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/pause/__init__.py
--rw-r--r--   0        0        0      695 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/pause/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/__init__.py
--rw-r--r--   0        0        0    10893 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/_logic.py
--rw-r--r--   0        0        0     2822 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/resume/__init__.py
--rw-r--r--   0        0        0      700 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/resume/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/trigger/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/trigger/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/_logic/__init__.py
--rw-r--r--   0        0        0     2050 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/build_steps.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
--rw-r--r--   0        0        0     6185 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
--rw-r--r--   0        0        0     4383 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
--rw-r--r--   0        0        0     2908 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
--rw-r--r--   0        0        0     1369 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
--rw-r--r--   0        0        0     1435 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
--rw-r--r--   0        0        0      359 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
--rw-r--r--   0        0        0      975 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
--rw-r--r--   0        0        0      311 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
--rw-r--r--   0        0        0     9876 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/config/config_v1.py
--rw-r--r--   0        0        0      131 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
--rw-r--r--   0        0        0      881 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/step_description.py
--rw-r--r--   0        0        0       73 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
--rw-r--r--   0        0        0      189 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
--rw-r--r--   0        0        0     1872 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/context.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/__init__.py
--rw-r--r--   0        0        0      568 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
--rw-r--r--   0        0        0      745 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/__init__.py
--rw-r--r--   0        0        0      421 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
--rw-r--r--   0        0        0     1929 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      957 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     1917 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     2589 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     2025 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2232 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     4459 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
--rw-r--r--   0        0        0     5385 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
--rw-r--r--   0        0        0      274 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      611 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1605 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0    11882 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0      183 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
--rw-r--r--   0        0        0     2169 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
--rw-r--r--   0        0        0     1644 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/__init__.py
--rw-r--r--   0        0        0     1686 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
--rw-r--r--   0        0        0     1181 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
--rw-r--r--   0        0        0      188 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/text.py
--rw-r--r--   0        0        0     7125 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/build/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/__init__.py
--rw-r--r--   0        0        0      491 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/builds_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/__init__.py
--rw-r--r--   0        0        0      181 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/_logic.py
--rw-r--r--   0        0        0      518 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/logs/__init__.py
--rw-r--r--   0        0        0     1054 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/logs/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/__init__.py
--rw-r--r--   0        0        0      256 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/_logic.py
--rw-r--r--   0        0        0      973 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/create/__init__.py
--rw-r--r--   0        0        0     1335 2023-05-11 08:46:37.677262 qwak_sdk-0.5.3/qwak_sdk/commands/models/create/_logic.py
--rw-r--r--   0        0        0     1016 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/create/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/__init__.py
--rw-r--r--   0        0        0      186 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/_logic.py
--rw-r--r--   0        0        0      638 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
--rw-r--r--   0        0        0     1251 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
--rw-r--r--   0        0        0     2494 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
--rw-r--r--   0        0        0     8227 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
--rw-r--r--   0        0        0    13221 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
--rw-r--r--   0        0        0     3900 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
--rw-r--r--   0        0        0     5799 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
--rw-r--r--   0        0        0      770 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
--rw-r--r--   0        0        0     1067 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
--rw-r--r--   0        0        0     3166 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
--rw-r--r--   0        0        0      495 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      903 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3015 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
--rw-r--r--   0        0        0      500 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
--rw-r--r--   0        0        0      902 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
--rw-r--r--   0        0        0      907 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
--rw-r--r--   0        0        0     3621 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     4917 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
--rw-r--r--   0        0        0      905 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
--rw-r--r--   0        0        0     1500 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
--rw-r--r--   0        0        0     5381 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
--rw-r--r--   0        0        0     5773 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
--rw-r--r--   0        0        0     3036 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
--rw-r--r--   0        0        0     2083 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/__init__.py
--rw-r--r--   0        0        0      409 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/_logic.py
--rw-r--r--   0        0        0      828 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/ui.py
--rw-r--r--   0        0        0      789 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/execution_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/__init__.py
--rw-r--r--   0        0        0      533 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/_logic.py
--rw-r--r--   0        0        0     1435 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/__init__.py
--rw-r--r--   0        0        0      605 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/_logic.py
--rw-r--r--   0        0        0     5158 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/__init__.py
--rw-r--r--   0        0        0      480 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/_logic.py
--rw-r--r--   0        0        0      820 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/__init__.py
--rw-r--r--   0        0        0     1375 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
--rw-r--r--   0        0        0       35 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       84 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      164 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0   129370 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3610 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0     1030 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
--rw-r--r--   0        0        0       41 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0       74 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      161 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0    53393 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
--rw-r--r--   0        0        0     3967 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
--rw-r--r--   0        0        0      139 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      120 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
--rw-r--r--   0        0        0      140 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
--rw-r--r--   0        0        0     2169 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
--rw-r--r--   0        0        0      117 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
--rw-r--r--   0        0        0       61 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0      182 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
--rw-r--r--   0        0        0     3353 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      751 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
--rw-r--r--   0        0        0       68 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
--rw-r--r--   0        0        0      104 2023-05-11 08:46:37.681262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
--rw-r--r--   0        0        0      448 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
--rw-r--r--   0        0        0      752 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
--rw-r--r--   0        0        0     1906 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/init/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/list/__init__.py
--rw-r--r--   0        0        0      166 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/list/_logic.py
--rw-r--r--   0        0        0     1135 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/list/ui.py
--rw-r--r--   0        0        0     1241 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/models_command_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/__init__.py
--rw-r--r--   0        0        0     2678 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/_logic.py
--rw-r--r--   0        0        0     1378 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/logs/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/logs/ui.py
--rw-r--r--   0        0        0      693 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/runtime_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
--rw-r--r--   0        0        0     1811 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
--rw-r--r--   0        0        0     3160 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
--rw-r--r--   0        0        0     1212 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/__init__.py
--rw-r--r--   0        0        0      393 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/_logic.py
--rw-r--r--   0        0        0      622 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/__init__.py
--rw-r--r--   0        0        0      259 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/_logic.py
--rw-r--r--   0        0        0      691 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/__init__.py
--rw-r--r--   0        0        0      203 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/_logic.py
--rw-r--r--   0        0        0      557 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/__init__.py
--rw-r--r--   0        0        0      182 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/_logic.py
--rw-r--r--   0        0        0     1124 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/ui.py
--rw-r--r--   0        0        0      589 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/projects/projects_command_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/__init__.py
--rw-r--r--   0        0        0      141 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/_logic.py
--rw-r--r--   0        0        0      741 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/ui.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/__init__.py
--rw-r--r--   0        0        0      142 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/_logic.py
--rw-r--r--   0        0        0      574 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/ui.py
--rw-r--r--   0        0        0      502 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/secrets_commands_group.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/__init__.py
--rw-r--r--   0        0        0      149 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/_logic.py
--rw-r--r--   0        0        0      615 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/ui.py
--rw-r--r--   0        0        0      430 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/commands/ui_tools.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/__init__.py
--rw-r--r--   0        0        0      437 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/run_config/__init__.py
--rw-r--r--   0        0        0     3166 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/run_config/base.py
--rw-r--r--   0        0        0     6087 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/common/run_config/utils.py
--rw-r--r--   0        0        0      381 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0       48 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_command_exception.py
--rw-r--r--   0        0        0      133 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
--rw-r--r--   0        0        0      424 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      130 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0       48 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_resource_not_found.py
--rw-r--r--   0        0        0      746 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/__init__.py
--rw-r--r--   0        0        0     3164 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/file_registry.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/__init__.py
--rw-r--r--   0        0        0     4541 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/cli_tools.py
--rw-r--r--   0        0        0      488 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/config_handler.py
--rw-r--r--   0        0        0       71 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/__init__.py
--rw-r--r--   0        0        0     8869 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logging.yml
--rw-r--r--   0        0        0     1013 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/inner/tools/tracking.py
--rw-r--r--   0        0        0      136 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/main.py
--rw-r--r--   0        0        0        0 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/__init__.py
--rw-r--r--   0        0        0      287 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/colors.py
--rw-r--r--   0        0        0     2257 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/files.py
--rw-r--r--   0        0        0     5616 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/log_handling.py
--rw-r--r--   0        0        0     1168 2023-05-11 08:46:37.685262 qwak_sdk-0.5.3/qwak_sdk/tools/utils.py
--rw-r--r--   0        0        0     8325 1970-01-01 00:00:00.000000 qwak_sdk-0.5.3/setup.py
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 qwak_sdk-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      183 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/README.md
+-rw-r--r--   0        0        0     2608 2023-05-23 09:14:33.918873 qwak_sdk-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-05-23 09:14:33.918873 qwak_sdk-0.5.4/qwak_sdk/__init__.py
+-rw-r--r--   0        0        0     2039 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/qwak_sdk/cli.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/qwak_sdk/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.962545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/__init__.py
+-rw-r--r--   0        0        0      327 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/admin_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/__init__.py
+-rw-r--r--   0        0        0      467 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/api_keys_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/_logic.py
+-rw-r--r--   0        0        0     1393 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/_logic.py
+-rw-r--r--   0        0        0      942 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/config_base.py
+-rw-r--r--   0        0        0      885 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py
+-rw-r--r--   0        0        0     1626 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py
+-rw-r--r--   0        0        0      817 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py
+-rw-r--r--   0        0        0      340 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/route_config.py
+-rw-r--r--   0        0        0      277 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/spec.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/__init__.py
+-rw-r--r--   0        0        0     3326 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/config.py
+-rw-r--r--   0        0        0      646 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/parser.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/_logic.py
+-rw-r--r--   0        0        0      949 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/ui.py
+-rw-r--r--   0        0        0      277 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/autoscaling_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/__init__.py
+-rw-r--r--   0        0        0      857 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/automations_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/__init__.py
+-rw-r--r--   0        0        0      235 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/_logic.py
+-rw-r--r--   0        0        0      604 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/executions_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/_logic.py
+-rw-r--r--   0        0        0      669 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/_logic.py
+-rw-r--r--   0        0        0      546 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/__init__.py
+-rw-r--r--   0        0        0     1624 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/_logic.py
+-rw-r--r--   0        0        0     1331 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/_logic.py
+-rw-r--r--   0        0        0     1039 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/ui.py
+-rw-r--r--   0        0        0     1002 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/feature_store_command_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/list/__init__.py
+-rw-r--r--   0        0        0     4145 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/list/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/pause/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/pause/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/__init__.py
+-rw-r--r--   0        0        0    10893 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/_logic.py
+-rw-r--r--   0        0        0     2822 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/resume/__init__.py
+-rw-r--r--   0        0        0      700 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/resume/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/trigger/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/trigger/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/_logic/__init__.py
+-rw-r--r--   0        0        0     2050 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/build_steps.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/__init__.py
+-rw-r--r--   0        0        0     6185 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py
+-rw-r--r--   0        0        0     4383 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py
+-rw-r--r--   0        0        0     2908 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/logger.py
+-rw-r--r--   0        0        0     1369 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/messages.py
+-rw-r--r--   0        0        0     1435 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py
+-rw-r--r--   0        0        0      359 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/spinner.py
+-rw-r--r--   0        0        0      975 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py
+-rw-r--r--   0        0        0      311 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/utils.py
+-rw-r--r--   0        0        0     9258 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/config/config_v1.py
+-rw-r--r--   0        0        0      131 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/host_resource.py
+-rw-r--r--   0        0        0      881 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/step_description.py
+-rw-r--r--   0        0        0       73 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/temp_dir.py
+-rw-r--r--   0        0        0      189 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/upload_tag.py
+-rw-r--r--   0        0        0     1872 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/context.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/__init__.py
+-rw-r--r--   0        0        0      568 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py
+-rw-r--r--   0        0        0      745 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/__init__.py
+-rw-r--r--   0        0        0      421 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/__init__.py
+-rw-r--r--   0        0        0     1929 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     1917 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     2025 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2232 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     4459 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py
+-rw-r--r--   0        0        0     5385 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0      274 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      611 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1605 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0    11882 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0      183 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/__init__.py
+-rw-r--r--   0        0        0     2169 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py
+-rw-r--r--   0        0        0     1644 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/__init__.py
+-rw-r--r--   0        0        0     1686 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py
+-rw-r--r--   0        0        0     1181 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/step_decorator.py
+-rw-r--r--   0        0        0      188 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/text.py
+-rw-r--r--   0        0        0     6357 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/build/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/builds_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/_logic.py
+-rw-r--r--   0        0        0      518 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/logs/__init__.py
+-rw-r--r--   0        0        0     1054 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/logs/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/_logic.py
+-rw-r--r--   0        0        0      973 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/create/__init__.py
+-rw-r--r--   0        0        0     1335 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/create/_logic.py
+-rw-r--r--   0        0        0     1016 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/create/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/_logic.py
+-rw-r--r--   0        0        0      638 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/__init__.py
+-rw-r--r--   0        0        0     1251 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py
+-rw-r--r--   0        0        0     2494 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py
+-rw-r--r--   0        0        0     8227 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py
+-rw-r--r--   0        0        0    13221 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py
+-rw-r--r--   0        0        0     3900 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py
+-rw-r--r--   0        0        0     5799 2023-05-23 09:13:41.966545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py
+-rw-r--r--   0        0        0      770 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py
+-rw-r--r--   0        0        0     1067 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py
+-rw-r--r--   0        0        0     3166 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      903 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3015 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/ui.py
+-rw-r--r--   0        0        0      500 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/deploy_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/__init__.py
+-rw-r--r--   0        0        0      902 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py
+-rw-r--r--   0        0        0      907 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     3621 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     4917 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/__init__.py
+-rw-r--r--   0        0        0      905 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py
+-rw-r--r--   0        0        0     1500 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py
+-rw-r--r--   0        0        0     5381 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/__init__.py
+-rw-r--r--   0        0        0     5773 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py
+-rw-r--r--   0        0        0     3036 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py
+-rw-r--r--   0        0        0     2083 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/_logic.py
+-rw-r--r--   0        0        0      828 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/ui.py
+-rw-r--r--   0        0        0      789 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/execution_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/__init__.py
+-rw-r--r--   0        0        0      533 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/_logic.py
+-rw-r--r--   0        0        0     1435 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/__init__.py
+-rw-r--r--   0        0        0      605 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/_logic.py
+-rw-r--r--   0        0        0     5158 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/__init__.py
+-rw-r--r--   0        0        0      480 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/_logic.py
+-rw-r--r--   0        0        0      820 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/__init__.py
+-rw-r--r--   0        0        0     1375 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0   129370 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3610 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0     1030 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0    53393 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv
+-rw-r--r--   0        0        0     3967 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/conda.yml
+-rw-r--r--   0        0        0     2169 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.test_directory}}/test_qwak_model.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/conda.yml
+-rw-r--r--   0        0        0     3353 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py
+-rw-r--r--   0        0        0      448 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/__init__.py
+-rw-r--r--   0        0        0      752 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py
+-rw-r--r--   0        0        0     1906 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/init/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/list/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/list/_logic.py
+-rw-r--r--   0        0        0     1135 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/list/ui.py
+-rw-r--r--   0        0        0     1241 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/models_command_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/_logic.py
+-rw-r--r--   0        0        0     1378 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/logs/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/logs/ui.py
+-rw-r--r--   0        0        0      693 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/runtime_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.970545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/__init__.py
+-rw-r--r--   0        0        0     1811 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py
+-rw-r--r--   0        0        0     3160 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py
+-rw-r--r--   0        0        0     1212 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/__init__.py
+-rw-r--r--   0        0        0      393 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/_logic.py
+-rw-r--r--   0        0        0      622 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/_logic.py
+-rw-r--r--   0        0        0      691 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/_logic.py
+-rw-r--r--   0        0        0      557 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/_logic.py
+-rw-r--r--   0        0        0     1124 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/ui.py
+-rw-r--r--   0        0        0      589 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/projects/projects_command_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/__init__.py
+-rw-r--r--   0        0        0      141 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/_logic.py
+-rw-r--r--   0        0        0      741 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/ui.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/_logic.py
+-rw-r--r--   0        0        0      574 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/ui.py
+-rw-r--r--   0        0        0      502 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/secrets_commands_group.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/_logic.py
+-rw-r--r--   0        0        0      615 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/ui.py
+-rw-r--r--   0        0        0      430 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/commands/ui_tools.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/run_config/__init__.py
+-rw-r--r--   0        0        0     3166 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/run_config/base.py
+-rw-r--r--   0        0        0     6087 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/common/run_config/utils.py
+-rw-r--r--   0        0        0      381 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_command_exception.py
+-rw-r--r--   0        0        0      133 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_deploy_new_build_failed.py
+-rw-r--r--   0        0        0      424 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      130 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0       48 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_resource_not_found.py
+-rw-r--r--   0        0        0      746 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/__init__.py
+-rw-r--r--   0        0        0     3164 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/file_registry.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/__init__.py
+-rw-r--r--   0        0        0     4541 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/cli_tools.py
+-rw-r--r--   0        0        0      488 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/config_handler.py
+-rw-r--r--   0        0        0       71 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/__init__.py
+-rw-r--r--   0        0        0     8869 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logging.yml
+-rw-r--r--   0        0        0     1013 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/inner/tools/tracking.py
+-rw-r--r--   0        0        0      136 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/main.py
+-rw-r--r--   0        0        0        0 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/colors.py
+-rw-r--r--   0        0        0     2257 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/files.py
+-rw-r--r--   0        0        0     5616 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/log_handling.py
+-rw-r--r--   0        0        0     1168 2023-05-23 09:13:41.974545 qwak_sdk-0.5.4/qwak_sdk/tools/utils.py
+-rw-r--r--   0        0        0     8327 1970-01-01 00:00:00.000000 qwak_sdk-0.5.4/setup.py
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 qwak_sdk-0.5.4/PKG-INFO
```

### Comparing `qwak_sdk-0.5.3/pyproject.toml` & `qwak_sdk-0.5.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-sdk"
-version = "0.5.3"
+version = "0.5.4"
 description = "Qwak SDK and CLI for qwak models"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak_sdk"},
 ]
@@ -23,24 +23,24 @@
 "Home page" = "https://www.qwak.com/"
 
 [tool.poetry.scripts]
 qwak = "qwak_sdk.main:qwak_cli"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-qwak-core = "==0.0.53"
-qwak-inference = "==0.1.1"
+qwak-core = "==0.0.69"
+qwak-inference = "==0.1.2"
 tabulate = ">=0.8.0"
 python-json-logger = ">=2.0.2"
 pydantic = "*"
 yaspin = ">=2.0.0"
 assertpy = "^1.1"
 cookiecutter = "*"
 gitpython = ">=2.1.0"
-boto3 = { version="^1.24.89", optional=true } # Inference dependencies
+boto3 = { version="^1.24.116", optional=true } # Inference dependencies
 pandas = [ # Inference dependencies
     {version="<1.4", python=">=3.7.1,<3.8", optional=true},
     {version=">=1.4.3,<2.0.0", python=">=3.8,<3.10", optional=true}
 ]
 joblib = { version="^1.1.0", optional=true } # Inference dependencies
 pyarrow = { version=">=6.0.0, <11.0.0", optional=true } # Inference dependencies
```

### Comparing `qwak_sdk-0.5.3/qwak_sdk/cli.py` & `qwak_sdk-0.5.4/qwak_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/generate/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/generate/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/admin/apikeys/revoke/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/admin/apikeys/revoke/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/parser.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/audience_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/conditions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/audience/_logic/config/v1/config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/config.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from enum import Enum
 from typing import List
 
 from _qwak_proto.qwak.auto_scaling.v1.auto_scaling_pb2 import (
     AGGREGATION_TYPE_AVERAGE,
     AGGREGATION_TYPE_MAX,
     AGGREGATION_TYPE_MIN,
+    AGGREGATION_TYPE_P50,
+    AGGREGATION_TYPE_P90,
+    AGGREGATION_TYPE_P95,
+    AGGREGATION_TYPE_P99,
     AGGREGATION_TYPE_SUM,
     METRIC_TYPE_CPU,
     METRIC_TYPE_GPU,
     METRIC_TYPE_LATENCY,
     METRIC_TYPE_MEMORY,
     AutoScalingConfig,
     PrometheusTrigger,
@@ -28,14 +32,18 @@
 
 
 class AggregationType(Enum):
     avg = AGGREGATION_TYPE_AVERAGE
     max = AGGREGATION_TYPE_MAX
     min = AGGREGATION_TYPE_MIN
     sum = AGGREGATION_TYPE_SUM
+    p50 = AGGREGATION_TYPE_P50
+    p90 = AGGREGATION_TYPE_P90
+    p95 = AGGREGATION_TYPE_P95
+    p99 = AGGREGATION_TYPE_P99
 
 
 @dataclass
 class AutoScaling:
     @dataclass
     class Triggers:
         @dataclass
```

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/_logic/config/parser.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/_logic/config/parser.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/auto_scalling/attach/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/auto_scalling/attach/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/automations/automations_commands_group.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/automations/automations_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/automations/delete/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/automations/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/automations/executions/list/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/automations/executions/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/automations/list/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/automations/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/automations/register/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/automations/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/delete/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/feature_store_command_group.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/feature_store_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/list/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/pause/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/pause/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/register/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/register/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/resume/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/resume/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/feature_store/trigger/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/feature_store/trigger/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/_logic/variations.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/build_steps.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/build_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/build_run_handlers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/cli_ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/logger.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/messages.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/messages.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/notifier_impl.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/client_logs/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/config/config_v1.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/config/config_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from _qwak_proto.qwak.builds.builds_pb2 import (
     BuildConfiguration,
     BuildEnvironment,
     BuildModelUri,
     BuildPropertiesProto,
     CondaBuild,
     DockerBuild,
-    LocalBuild,
     PoetryBuild,
     PythonBuild,
     RemoteBuild,
     RemoteBuildResources,
     Step,
     VirtualEnvironmentBuild,
 )
@@ -80,19 +79,15 @@
     ConfigCliMap("base_image", "build_env.docker.base_image", validate_string),
     ConfigCliMap("param_list", "build_env.docker.params", validate_list_of_strings),
     ConfigCliMap("env_vars", "build_env.docker.env_vars", validate_list_of_strings),
     ConfigCliMap("cache", "build_env.docker.cache", validate_bool),
     ConfigCliMap(
         "iam_role_arn", "build_env.docker.assumed_iam_role_arn", validate_string
     ),
-    # LocalConf
-    ConfigCliMap("push", "build_env.docker.push", validate_bool),
-    ConfigCliMap("aws_profile", "build_env.local.aws_profile", validate_string),
     # RemoteConf
-    ConfigCliMap("remote", "build_env.remote.is_remote", validate_bool),
     ConfigCliMap("cpus", "build_env.remote.resources.cpus", validate_float),
     ConfigCliMap("memory", "build_env.remote.resources.memory", validate_string),
     ConfigCliMap("gpu_type", "build_env.remote.resources.gpu_type", validate_string),
     ConfigCliMap("gpu_amount", "build_env.remote.resources.gpu_amount", validate_int),
     # Verbosity level
     ConfigCliMap("verbose", "verbose", validate_int),
     ConfigCliMap("deploy", "deploy", validate_bool),
@@ -152,15 +147,14 @@
             env_vars: Optional[Union[List[str], Dict[str, str], Tuple]] = field(
                 default_factory=list
             )
             assumed_iam_role_arn: str = field(default=None)
             params: Optional[List[str]] = field(default_factory=list)
             no_cache: bool = field(default=False)
             cache: bool = field(default=True)
-            push: bool = field(default=True)
 
         @protobuf_factory(
             PythonBuild, exclude_fields=["git_credentials_secret", "git_credentials"]
         )
         @dataclass
         class PythonEnv:
             @protobuf_factory(PoetryBuild)
@@ -181,27 +175,20 @@
                 requirements_txt: Optional[str] = field(default=None)
 
             git_credentials: Optional[str] = field(default=None)
             git_credentials_secret: Optional[str] = field(default=None)
             poetry: PoetryType = field(default=None)
             conda: CondaType = field(default=None)
             virtualenv: VirtualenvType = field(default=None)
-            qwak_sdk_extra_index_url: str = field(default=None)
             dependency_file_path: Optional[str] = field(default=None)
 
             def __post_init__(self):
                 if not (self.poetry or self.conda or self.virtualenv):
                     self.conda = self.CondaType("conda.yml")
 
-        @protobuf_factory(LocalBuild)
-        @dataclass
-        class LocalConf:
-            no_push: bool = field(default=False)  # Deprecated
-            aws_profile: str = field(default=None)
-
         @protobuf_factory(RemoteBuild)
         @dataclass
         class RemoteConf:
             @protobuf_factory(RemoteBuildResources)
             @dataclass
             class RemoteBuildResources:
                 cpus: Optional[float] = field(default=None)
@@ -212,15 +199,14 @@
             is_remote: bool = field(default=True)
             resources: RemoteBuildResources = field(
                 default_factory=RemoteBuildResources
             )
 
         docker: DockerConf = field(default_factory=DockerConf)
         python_env: PythonEnv = field(default_factory=PythonEnv)
-        local: LocalConf = field(default_factory=LocalConf)
         remote: RemoteConf = field(default_factory=RemoteConf)
 
     build_properties: BuildProperties = field(default_factory=BuildProperties)
     build_env: Optional[BuildEnv] = field(default_factory=BuildEnv)
     pre_build: Optional[BuildEnv] = field(default=None)
     post_build: Optional[BuildEnv] = field(default=None)
     step: Step = field(default_factory=Step)
```

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/constant/step_description.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/constant/step_description.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/context.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/context.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/notifier_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/fetch_model_step/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/a_fetch_model_code/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/b_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/build_polling_status.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/phase/c_deploy/deploy_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/_logic/util/step_decorator.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/_logic/util/step_decorator.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/build/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/build/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,20 +36,14 @@
     "-T",
     "--tags",
     required=False,
     multiple=True,
     help="A tag for the model build",
 )
 @click.option(
-    "--remote/--no-remote",
-    help=f"Whether to use remote mode."
-    f"\n[Default: {ConfigV1.BuildEnv.RemoteConf.is_remote}]",
-    default=None,
-)
-@click.option(
     "--git-credentials",
     required=False,
     metavar="USERNAME:ACCESS_TOKEN",
     help="Access credentials for private repositories listed in the python dependencies file",
 )
 @click.option(
     "--git-branch",
@@ -109,31 +103,19 @@
 @click.option(
     "--iam-role-arn",
     required=False,
     type=str,
     help="[REMOTE BUILD] Custom IAM Role ARN.",
 )
 @click.option(
-    "--push/--no-push",
-    default=None,
-    help="[LOCAL BUILD] Whether to push the model to the registry."
-    "\n[Default: Push enabled",
-)
-@click.option(
     "--cache/--no-cache",
     default=None,
     help="Disable docker build cache. [Default: Cache enabled]",
 )
 @click.option(
-    "--aws-profile",
-    required=False,
-    help="[LOCAL BUILD] AWS Profile to use for s3 operations."
-    f"\n[Default: {ConfigV1.BuildEnv.LocalConf.aws_profile}]",
-)
-@click.option(
     "-v",
     "--verbose",
     count=True,
     default=None,
     help="Log verbosity level - v: INFO, vv: DEBUG [default: WARNING], Default ERROR",
 )
 @click.option(
@@ -141,20 +123,14 @@
     help="Used for customizing the docker container image built for train, build and deploy."
     "Docker images should be based on qwak images, The entrypoint or cmd of the docker "
     "image should not be changed."
     f"\n[Default: {ConfigV1.BuildEnv.DockerConf.base_image}]",
     required=False,
 )
 @click.option(
-    "--qwak-sdk-extra-index-url",
-    required=False,
-    help="Extra index url to install from the Qwak-SDK on remote (enables running dev versions on remote build"
-    ", it's required to upload the dev version to the index url of course)",
-)
-@click.option(
     "-f",
     "--from-file",
     help="Build by run_config file, Command arguments will overwrite any run_config.",
     required=False,
     type=click.Path(exists=True, resolve_path=True, dir_okay=False),
 )
 @click.option(
```

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/cancel/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/logs/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/builds/status/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/builds/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/create/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/create/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/create/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/delete/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/advance_deployment_options_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/base_deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deploy_config.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_message_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_response_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/deployment_size_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/get_latest_successful_build.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/batch/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/batch/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/advanced_deployment_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/realtime/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/deploy_executor.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/_logic/serving_strategy_mapper.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/deploy/streaming/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/request_undeploy.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/deployments/undeploy/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/deployments/undeploy/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/cancel/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/cancel/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/execution_commands_group.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/execution_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/report/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/report/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/start/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/start/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/executions/status/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/executions/status/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/initialize_model_structure.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/churn/{{cookiecutter.model_directory}}/tests/it/test_churn.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/data.csv`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/credit_risk/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/general/{{cookiecutter.model_directory}}/{{cookiecutter.main_directory}}/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/main/model.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/_logic/template/titanic_poetry/{{cookiecutter.model_directory}}/tests/it/test_titanic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/init/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/init/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/list/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/models_command_group.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/models_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/_logic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/_logic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/feedback/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/feedback/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/logs/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/logs/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/runtime_commands_group.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/runtime_commands_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/execute_runtime_update_traffic.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/_logic/variations.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/traffic_update/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/traffic_update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/models/runtime/update/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/models/runtime/update/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/projects/create/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/projects/create/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/projects/delete/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/projects/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/projects/list/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/projects/list/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/projects/projects_command_group.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/projects/projects_command_group.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/secrets/delete/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/secrets/delete/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/secrets/get/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/secrets/get/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/commands/secrets/set/ui.py` & `qwak_sdk-0.5.4/qwak_sdk/commands/secrets/set/ui.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/common/run_config/base.py` & `qwak_sdk-0.5.4/qwak_sdk/common/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/common/run_config/utils.py` & `qwak_sdk-0.5.4/qwak_sdk/common/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/exceptions/qwak_suggestion_exception.py` & `qwak_sdk-0.5.4/qwak_sdk/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/inner/file_registry.py` & `qwak_sdk-0.5.4/qwak_sdk/inner/file_registry.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/inner/tools/cli_tools.py` & `qwak_sdk-0.5.4/qwak_sdk/inner/tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logger.py` & `qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/inner/tools/logger/logging.yml` & `qwak_sdk-0.5.4/qwak_sdk/inner/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/inner/tools/tracking.py` & `qwak_sdk-0.5.4/qwak_sdk/inner/tools/tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/tools/files.py` & `qwak_sdk-0.5.4/qwak_sdk/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/tools/log_handling.py` & `qwak_sdk-0.5.4/qwak_sdk/tools/log_handling.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/qwak_sdk/tools/utils.py` & `qwak_sdk-0.5.4/qwak_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_sdk-0.5.3/setup.py` & `qwak_sdk-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,39 +123,39 @@
 
 install_requires = \
 ['assertpy>=1.1,<2.0',
  'cookiecutter',
  'gitpython>=2.1.0',
  'pydantic',
  'python-json-logger>=2.0.2',
- 'qwak-core==0.0.53',
- 'qwak-inference==0.1.1',
+ 'qwak-core==0.0.69',
+ 'qwak-inference==0.1.2',
  'tabulate>=0.8.0',
  'yaspin>=2.0.0']
 
 extras_require = \
-{'batch': ['boto3>=1.24.89,<2.0.0',
+{'batch': ['boto3>=1.24.116,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
            'pyarrow>=6.0.0,<11.0.0'],
  'batch:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                      'pandas<1.4'],
  'batch:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                'pandas>=1.4.3,<2.0.0'],
- 'feedback': ['boto3>=1.24.89,<2.0.0', 'joblib>=1.1.0,<2.0.0'],
+ 'feedback': ['boto3>=1.24.116,<2.0.0', 'joblib>=1.1.0,<2.0.0'],
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
  'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['qwak = qwak_sdk.main:qwak_cli']}
 
 setup_kwargs = {
     'name': 'qwak-sdk',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'Qwak SDK and CLI for qwak models',
     'long_description': '# Qwak SDK\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_sdk-0.5.3/PKG-INFO` & `qwak_sdk-0.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: Qwak SDK and CLI for qwak models
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,25 +16,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: batch
 Provides-Extra: feedback
 Requires-Dist: assertpy (>=1.1,<2.0)
-Requires-Dist: boto3 (>=1.24.89,<2.0.0) ; extra == "batch" or extra == "feedback"
+Requires-Dist: boto3 (>=1.24.116,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: cookiecutter
 Requires-Dist: gitpython (>=2.1.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
 Requires-Dist: pydantic
 Requires-Dist: python-json-logger (>=2.0.2)
-Requires-Dist: qwak-core (==0.0.53)
-Requires-Dist: qwak-inference (==0.1.1)
+Requires-Dist: qwak-core (==0.0.69)
+Requires-Dist: qwak-inference (==0.1.2)
 Requires-Dist: tabulate (>=0.8.0)
 Requires-Dist: yaspin (>=2.0.0)
 Project-URL: Home page, https://www.qwak.com/
 Description-Content-Type: text/markdown
 
 # Qwak SDK
```

