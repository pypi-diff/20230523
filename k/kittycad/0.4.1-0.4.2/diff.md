# Comparing `tmp/kittycad-0.4.1.tar.gz` & `tmp/kittycad-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kittycad-0.4.1.tar", max compression
+gzip compressed data, was "kittycad-0.4.2.tar", max compression
```

## Comparing `kittycad-0.4.1.tar` & `kittycad-0.4.2.tar`

### file list

```diff
@@ -1,271 +1,276 @@
--rw-r--r--   0        0        0     1065 2023-05-08 21:32:05.549300 kittycad-0.4.1/LICENSE
--rw-r--r--   0        0        0      875 2023-05-08 21:32:05.549300 kittycad-0.4.1/README.md
--rw-r--r--   0        0        0       48 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/__init__.py
--rw-r--r--   0        0        0       47 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/ai/__init__.py
--rw-r--r--   0        0        0     3781 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/ai/create_image_to_3d.py
--rw-r--r--   0        0        0     3559 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/ai/create_text_to_3d.py
--rw-r--r--   0        0        0      199 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/__init__.py
--rw-r--r--   0        0        0     3110 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_api_call.py
--rw-r--r--   0        0        0     2799 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_api_call_for_user.py
--rw-r--r--   0        0        0     3243 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_api_call_metrics.py
--rw-r--r--   0        0        0     6149 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/get_async_operation.py
--rw-r--r--   0        0        0     4236 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/list_api_calls.py
--rw-r--r--   0        0        0     5005 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/list_api_calls_for_user.py
--rw-r--r--   0        0        0     4815 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/list_async_operations.py
--rw-r--r--   0        0        0     4351 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_calls/user_list_api_calls.py
--rw-r--r--   0        0        0      352 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/__init__.py
--rw-r--r--   0        0        0     2573 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/create_api_token_for_user.py
--rw-r--r--   0        0        0     2879 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/delete_api_token_for_user.py
--rw-r--r--   0        0        0     2784 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/get_api_token_for_user.py
--rw-r--r--   0        0        0     4284 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/api_tokens/list_api_tokens_for_user.py
--rw-r--r--   0        0        0      116 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/__init__.py
--rw-r--r--   0        0        0     2597 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/apps_github_callback.py
--rw-r--r--   0        0        0     2911 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/apps_github_consent.py
--rw-r--r--   0        0        0     2338 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/apps/apps_github_webhook.py
--rw-r--r--   0        0        0      156 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/beta/__init__.py
--rw-r--r--   0        0        0      118 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/constant/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/constant/get_physics_constant.py
--rw-r--r--   0        0        0      142 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/drawing/__init__.py
--rw-r--r--   0        0        0     2786 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/drawing/cmd.py
--rw-r--r--   0        0        0     2684 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/drawing/cmd_batch.py
--rw-r--r--   0        0        0      161 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/executor/__init__.py
--rw-r--r--   0        0        0     1781 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/executor/create_executor_term.py
--rw-r--r--   0        0        0     3195 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/executor/create_file_execution.py
--rw-r--r--   0        0        0      233 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/__init__.py
--rw-r--r--   0        0        0     3871 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_center_of_mass.py
--rw-r--r--   0        0        0     4461 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_conversion.py
--rw-r--r--   0        0        0     1962 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0     4276 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_density.py
--rw-r--r--   0        0        0     4294 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_mass.py
--rw-r--r--   0        0        0     3855 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_surface_area.py
--rw-r--r--   0        0        0     3785 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/create_file_volume.py
--rw-r--r--   0        0        0     1341 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/file/get_file_conversion_with_base64_helper.py
--rw-r--r--   0        0        0      133 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/auth_email.py
--rw-r--r--   0        0        0     3220 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/auth_email_callback.py
--rw-r--r--   0        0        0     2139 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/hidden/logout.py
--rw-r--r--   0        0        0      105 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/__init__.py
--rw-r--r--   0        0        0     2383 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_ai_plugin_manifest.py
--rw-r--r--   0        0        0     2629 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_metadata.py
--rw-r--r--   0        0        0     2564 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_openai_schema.py
--rw-r--r--   0        0        0     2193 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/get_schema.py
--rw-r--r--   0        0        0     2245 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/meta/ping.py
--rw-r--r--   0        0        0      123 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/oauth2/__init__.py
--rw-r--r--   0        0        0      117 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/__init__.py
--rw-r--r--   0        0        0     2956 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/create_payment_information_for_user.py
--rw-r--r--   0        0        0     2638 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/create_payment_intent_for_user.py
--rw-r--r--   0        0        0     2431 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/delete_payment_information_for_user.py
--rw-r--r--   0        0        0     2486 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/delete_payment_method_for_user.py
--rw-r--r--   0        0        0     2655 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/get_payment_balance_for_user.py
--rw-r--r--   0        0        0     2681 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/get_payment_information_for_user.py
--rw-r--r--   0        0        0     2616 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/list_invoices_for_user.py
--rw-r--r--   0        0        0     2684 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/list_payment_methods_for_user.py
--rw-r--r--   0        0        0     2954 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/update_payment_information_for_user.py
--rw-r--r--   0        0        0     2483 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/payments/validate_customer_tax_information_for_user.py
--rw-r--r--   0        0        0      101 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/__init__.py
--rw-r--r--   0        0        0     3966 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_acceleration_unit_conversion.py
--rw-r--r--   0        0        0     3784 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_angle_unit_conversion.py
--rw-r--r--   0        0        0     4051 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_angular_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3758 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_area_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_charge_unit_conversion.py
--rw-r--r--   0        0        0     3990 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_concentration_unit_conversion.py
--rw-r--r--   0        0        0     4082 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_data_unit_conversion.py
--rw-r--r--   0        0        0     3834 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_density_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_energy_unit_conversion.py
--rw-r--r--   0        0        0     3782 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_force_unit_conversion.py
--rw-r--r--   0        0        0     3938 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_illuminance_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_length_unit_conversion.py
--rw-r--r--   0        0        0     4230 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
--rw-r--r--   0        0        0     3971 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_mass_unit_conversion.py
--rw-r--r--   0        0        0     3918 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
--rw-r--r--   0        0        0     3955 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
--rw-r--r--   0        0        0     3848 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_metric_power_unit_conversion.py
--rw-r--r--   0        0        0     3782 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_power_unit_conversion.py
--rw-r--r--   0        0        0     3860 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_pressure_unit_conversion.py
--rw-r--r--   0        0        0     3886 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_radiation_unit_conversion.py
--rw-r--r--   0        0        0     3990 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_radioactivity_unit_conversion.py
--rw-r--r--   0        0        0     3919 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_solid_angle_unit_conversion.py
--rw-r--r--   0        0        0     3938 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_temperature_unit_conversion.py
--rw-r--r--   0        0        0     3756 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_time_unit_conversion.py
--rw-r--r--   0        0        0     3860 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_velocity_unit_conversion.py
--rw-r--r--   0        0        0     3834 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_voltage_unit_conversion.py
--rw-r--r--   0        0        0     3808 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/unit/get_volume_unit_conversion.py
--rw-r--r--   0        0        0      297 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/users/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-08 21:32:06.305308 kittycad-0.4.1/kittycad/api/users/delete_user_self.py
--rw-r--r--   0        0        0     2757 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_session_for_user.py
--rw-r--r--   0        0        0     3061 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user.py
--rw-r--r--   0        0        0     3185 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_extended.py
--rw-r--r--   0        0        0     2480 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_front_hash_self.py
--rw-r--r--   0        0        0     2506 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_onboarding_self.py
--rw-r--r--   0        0        0     2523 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_self.py
--rw-r--r--   0        0        0     2629 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/get_user_self_extended.py
--rw-r--r--   0        0        0     4105 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/list_users.py
--rw-r--r--   0        0        0     4187 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/list_users_extended.py
--rw-r--r--   0        0        0     2779 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/api/users/update_user_self.py
--rw-r--r--   0        0        0     2297 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/client.py
--rw-r--r--   0        0        0     5250 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/client_test.py
--rw-r--r--   0        0        0   127516 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/examples_test.py
--rw-r--r--   0        0        0     7838 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/__init__.py
--rw-r--r--   0        0        0      322 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/account_provider.py
--rw-r--r--   0        0        0     2249 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_api.py
--rw-r--r--   0        0        0      242 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_api_type.py
--rw-r--r--   0        0        0     2440 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_auth.py
--rw-r--r--   0        0        0      413 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_auth_type.py
--rw-r--r--   0        0        0      287 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_http_auth_type.py
--rw-r--r--   0        0        0     4685 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/ai_plugin_manifest.py
--rw-r--r--   0        0        0     1720 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_query_group.py
--rw-r--r--   0        0        0      777 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_query_group_by.py
--rw-r--r--   0        0        0      620 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_status.py
--rw-r--r--   0        0        0     8266 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_with_price.py
--rw-r--r--   0        0        0     2128 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_call_with_price_results_page.py
--rw-r--r--   0        0        0     3278 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_token.py
--rw-r--r--   0        0        0     2004 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/api_token_results_page.py
--rw-r--r--   0        0        0     1447 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/app_client_info.py
--rw-r--r--   0        0        0     5747 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call.py
--rw-r--r--   0        0        0    34040 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call_output.py
--rw-r--r--   0        0        0     2066 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call_results_page.py
--rw-r--r--   0        0        0      648 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/async_api_call_type.py
--rw-r--r--   0        0        0     2127 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/billing_info.py
--rw-r--r--   0        0        0     1479 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/cache_metadata.py
--rw-r--r--   0        0        0     3353 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/card_details.py
--rw-r--r--   0        0        0     2697 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/cluster.py
--rw-r--r--   0        0        0      229 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/code_language.py
--rw-r--r--   0        0        0     2244 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/code_output.py
--rw-r--r--   0        0        0     1732 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/commit.py
--rw-r--r--   0        0        0    14343 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/connection.py
--rw-r--r--   0        0        0    13513 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/country_code.py
--rw-r--r--   0        0        0      507 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/created_at_sort_mode.py
--rw-r--r--   0        0        0     8623 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/currency.py
--rw-r--r--   0        0        0     4298 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/customer.py
--rw-r--r--   0        0        0     4306 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/customer_balance.py
--rw-r--r--   0        0        0     2412 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/device_access_token_request_form.py
--rw-r--r--   0        0        0     1580 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/device_auth_request_form.py
--rw-r--r--   0        0        0     1606 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/device_auth_verify_params.py
--rw-r--r--   0        0        0    21264 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/docker_system_info.py
--rw-r--r--   0        0        0     3553 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd.py
--rw-r--r--   0        0        0       75 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd_id.py
--rw-r--r--   0        0        0     2441 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd_req.py
--rw-r--r--   0        0        0     1746 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_cmd_req_batch.py
--rw-r--r--   0        0        0     2393 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_error.py
--rw-r--r--   0        0        0     1869 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_outcome.py
--rw-r--r--   0        0        0     1505 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/drawing_outcomes.py
--rw-r--r--   0        0        0     1789 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/email_authentication_form.py
--rw-r--r--   0        0        0     3847 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/engine_metadata.py
--rw-r--r--   0        0        0      269 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/environment.py
--rw-r--r--   0        0        0     1930 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/error.py
--rw-r--r--   0        0        0     2715 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/executor_metadata.py
--rw-r--r--   0        0        0     6069 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/extended_user.py
--rw-r--r--   0        0        0     2060 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/extended_user_results_page.py
--rw-r--r--   0        0        0     5700 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_center_of_mass.py
--rw-r--r--   0        0        0     6060 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_conversion.py
--rw-r--r--   0        0        0     5725 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_density.py
--rw-r--r--   0        0        0     1369 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_export_format.py
--rw-r--r--   0        0        0     1306 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_import_format.py
--rw-r--r--   0        0        0     5707 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_mass.py
--rw-r--r--   0        0        0     5522 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_surface_area.py
--rw-r--r--   0        0        0     1513 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_system_metadata.py
--rw-r--r--   0        0        0     5428 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/file_volume.py
--rw-r--r--   0        0        0     2304 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/gateway.py
--rw-r--r--   0        0        0      187 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/image_type.py
--rw-r--r--   0        0        0     2228 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/index_info.py
--rw-r--r--   0        0        0     8273 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/invoice.py
--rw-r--r--   0        0        0     2888 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/invoice_line_item.py
--rw-r--r--   0        0        0      563 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/invoice_status.py
--rw-r--r--   0        0        0     2666 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream.py
--rw-r--r--   0        0        0     1907 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream_api_stats.py
--rw-r--r--   0        0        0     2212 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream_config.py
--rw-r--r--   0        0        0     3174 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/jetstream_stats.py
--rw-r--r--   0        0        0     2125 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/leaf_node.py
--rw-r--r--   0        0        0     1337 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/mesh.py
--rw-r--r--   0        0        0     1923 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/meta_cluster_info.py
--rw-r--r--   0        0        0     5025 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/metadata.py
--rw-r--r--   0        0        0     1788 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/method.py
--rw-r--r--   0        0        0     3081 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/new_address.py
--rw-r--r--   0        0        0     2038 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/o_auth2_client_info.py
--rw-r--r--   0        0        0      415 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/o_auth2_grant_type.py
--rw-r--r--   0        0        0     2501 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/onboarding.py
--rw-r--r--   0        0        0     1646 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/output_file.py
--rw-r--r--   0        0        0     1527 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_intent.py
--rw-r--r--   0        0        0     3753 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_method.py
--rw-r--r--   0        0        0     2267 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_method_card_checks.py
--rw-r--r--   0        0        0      294 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/payment_method_type.py
--rw-r--r--   0        0        0     5424 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/physics_constant.py
--rw-r--r--   0        0        0     4448 2023-05-08 21:32:06.309308 kittycad-0.4.1/kittycad/models/physics_constant_name.py
--rw-r--r--   0        0        0     2809 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/plugins_info.py
--rw-r--r--   0        0        0     1498 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/point_e_metadata.py
--rw-r--r--   0        0        0     1432 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/pong.py
--rw-r--r--   0        0        0     4187 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/registry_service_config.py
--rw-r--r--   0        0        0     2034 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/runtime.py
--rw-r--r--   0        0        0     3638 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/session.py
--rw-r--r--   0        0        0      214 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_cgroup_driver_enum.py
--rw-r--r--   0        0        0      175 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_cgroup_version_enum.py
--rw-r--r--   0        0        0     1663 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_default_address_pools.py
--rw-r--r--   0        0        0      213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/system_info_isolation_enum.py
--rw-r--r--   0        0        0     6317 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_acceleration_conversion.py
--rw-r--r--   0        0        0      642 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_acceleration_format.py
--rw-r--r--   0        0        0     6226 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angle_conversion.py
--rw-r--r--   0        0        0      916 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angle_format.py
--rw-r--r--   0        0        0     6360 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angular_velocity_conversion.py
--rw-r--r--   0        0        0      754 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_angular_velocity_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_area_conversion.py
--rw-r--r--   0        0        0      888 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_area_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_charge_conversion.py
--rw-r--r--   0        0        0      380 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_charge_format.py
--rw-r--r--   0        0        0     6330 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_concentration_conversion.py
--rw-r--r--   0        0        0      752 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_concentration_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_conversion.py
--rw-r--r--   0        0        0      539 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_format.py
--rw-r--r--   0        0        0     6377 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_conversion.py
--rw-r--r--   0        0        0      656 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_format.py
--rw-r--r--   0        0        0     6252 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_density_conversion.py
--rw-r--r--   0        0        0     1488 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_density_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_energy_conversion.py
--rw-r--r--   0        0        0     1162 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_energy_format.py
--rw-r--r--   0        0        0     6226 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_force_conversion.py
--rw-r--r--   0        0        0      645 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_force_format.py
--rw-r--r--   0        0        0     6304 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_illuminance_conversion.py
--rw-r--r--   0        0        0      584 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_illuminance_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_length_conversion.py
--rw-r--r--   0        0        0     2187 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_length_format.py
--rw-r--r--   0        0        0     6442 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_field_strength_conversion.py
--rw-r--r--   0        0        0      402 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_field_strength_format.py
--rw-r--r--   0        0        0     6321 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_flux_conversion.py
--rw-r--r--   0        0        0      389 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_magnetic_flux_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_mass_conversion.py
--rw-r--r--   0        0        0     1094 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_mass_format.py
--rw-r--r--   0        0        0     3438 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power.py
--rw-r--r--   0        0        0     6259 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power_conversion.py
--rw-r--r--   0        0        0     6287 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power_cubed_conversion.py
--rw-r--r--   0        0        0     6297 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_metric_power_squared_conversion.py
--rw-r--r--   0        0        0     6226 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_power_conversion.py
--rw-r--r--   0        0        0      468 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_power_format.py
--rw-r--r--   0        0        0     6265 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_pressure_conversion.py
--rw-r--r--   0        0        0      725 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_pressure_format.py
--rw-r--r--   0        0        0     6278 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radiation_conversion.py
--rw-r--r--   0        0        0      586 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radiation_format.py
--rw-r--r--   0        0        0     6330 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radioactivity_conversion.py
--rw-r--r--   0        0        0      570 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_radioactivity_format.py
--rw-r--r--   0        0        0     6295 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_solid_angle_conversion.py
--rw-r--r--   0        0        0      500 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_solid_angle_format.py
--rw-r--r--   0        0        0     6304 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_temperature_conversion.py
--rw-r--r--   0        0        0      674 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_temperature_format.py
--rw-r--r--   0        0        0     6213 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_time_conversion.py
--rw-r--r--   0        0        0      902 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_time_format.py
--rw-r--r--   0        0        0     6265 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_velocity_conversion.py
--rw-r--r--   0        0        0      753 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_velocity_format.py
--rw-r--r--   0        0        0     6252 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_voltage_conversion.py
--rw-r--r--   0        0        0      452 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_voltage_format.py
--rw-r--r--   0        0        0     6239 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_volume_conversion.py
--rw-r--r--   0        0        0     3286 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/unit_volume_format.py
--rw-r--r--   0        0        0     2577 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/update_user.py
--rw-r--r--   0        0        0     5084 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/user.py
--rw-r--r--   0        0        0     1942 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/user_results_page.py
--rw-r--r--   0        0        0       67 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/uuid.py
--rw-r--r--   0        0        0     3448 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/models/verification_token.py
--rw-r--r--   0        0        0       26 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/py.typed
--rw-r--r--   0        0        0     1049 2023-05-08 21:32:06.313308 kittycad-0.4.1/kittycad/types.py
--rw-r--r--   0        0        0     2472 2023-05-08 21:32:06.313308 kittycad-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-23 21:26:44.314666 kittycad-0.4.2/LICENSE
+-rw-r--r--   0        0        0      875 2023-05-23 21:26:44.314666 kittycad-0.4.2/README.md
+-rw-r--r--   0        0        0       48 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/ai/__init__.py
+-rw-r--r--   0        0        0     3781 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/ai/create_image_to_3d.py
+-rw-r--r--   0        0        0     3559 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/ai/create_text_to_3d.py
+-rw-r--r--   0        0        0      199 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/__init__.py
+-rw-r--r--   0        0        0     3110 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_api_call.py
+-rw-r--r--   0        0        0     2799 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_api_call_for_user.py
+-rw-r--r--   0        0        0     3243 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_api_call_metrics.py
+-rw-r--r--   0        0        0     6149 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/get_async_operation.py
+-rw-r--r--   0        0        0     4236 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/list_api_calls.py
+-rw-r--r--   0        0        0     5005 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/list_api_calls_for_user.py
+-rw-r--r--   0        0        0     4815 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/list_async_operations.py
+-rw-r--r--   0        0        0     4351 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_calls/user_list_api_calls.py
+-rw-r--r--   0        0        0      352 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/__init__.py
+-rw-r--r--   0        0        0     2573 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/create_api_token_for_user.py
+-rw-r--r--   0        0        0     2879 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/delete_api_token_for_user.py
+-rw-r--r--   0        0        0     2784 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/get_api_token_for_user.py
+-rw-r--r--   0        0        0     4284 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/api_tokens/list_api_tokens_for_user.py
+-rw-r--r--   0        0        0      116 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/__init__.py
+-rw-r--r--   0        0        0     2597 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/apps_github_callback.py
+-rw-r--r--   0        0        0     2911 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/apps_github_consent.py
+-rw-r--r--   0        0        0     2338 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/apps/apps_github_webhook.py
+-rw-r--r--   0        0        0      156 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/beta/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/constant/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/constant/get_physics_constant.py
+-rw-r--r--   0        0        0      161 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/executor/__init__.py
+-rw-r--r--   0        0        0     1781 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/executor/create_executor_term.py
+-rw-r--r--   0        0        0     3195 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/executor/create_file_execution.py
+-rw-r--r--   0        0        0      233 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/__init__.py
+-rw-r--r--   0        0        0     4635 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_center_of_mass.py
+-rw-r--r--   0        0        0     4461 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_conversion.py
+-rw-r--r--   0        0        0     1962 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0     5162 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_density.py
+-rw-r--r--   0        0        0     5290 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_mass.py
+-rw-r--r--   0        0        0     4559 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_surface_area.py
+-rw-r--r--   0        0        0     4487 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/create_file_volume.py
+-rw-r--r--   0        0        0     1341 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/file/get_file_conversion_with_base64_helper.py
+-rw-r--r--   0        0        0      133 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/auth_email.py
+-rw-r--r--   0        0        0     3220 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/auth_email_callback.py
+-rw-r--r--   0        0        0     2139 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/hidden/logout.py
+-rw-r--r--   0        0        0      105 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/meta/__init__.py
+-rw-r--r--   0        0        0     2383 2023-05-23 21:26:45.182695 kittycad-0.4.2/kittycad/api/meta/get_ai_plugin_manifest.py
+-rw-r--r--   0        0        0     2629 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/get_metadata.py
+-rw-r--r--   0        0        0     2564 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/get_openai_schema.py
+-rw-r--r--   0        0        0     2193 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/get_schema.py
+-rw-r--r--   0        0        0     2245 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/meta/ping.py
+-rw-r--r--   0        0        0      144 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/__init__.py
+-rw-r--r--   0        0        0     2794 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/cmd.py
+-rw-r--r--   0        0        0     2701 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/cmd_batch.py
+-rw-r--r--   0        0        0     1995 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/modeling/modeling_commands_ws.py
+-rw-r--r--   0        0        0      123 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/oauth2/__init__.py
+-rw-r--r--   0        0        0      117 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/__init__.py
+-rw-r--r--   0        0        0     2956 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/create_payment_information_for_user.py
+-rw-r--r--   0        0        0     2638 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/create_payment_intent_for_user.py
+-rw-r--r--   0        0        0     2431 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/delete_payment_information_for_user.py
+-rw-r--r--   0        0        0     2486 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/delete_payment_method_for_user.py
+-rw-r--r--   0        0        0     2655 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/get_payment_balance_for_user.py
+-rw-r--r--   0        0        0     2681 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/get_payment_information_for_user.py
+-rw-r--r--   0        0        0     2616 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/list_invoices_for_user.py
+-rw-r--r--   0        0        0     2684 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/list_payment_methods_for_user.py
+-rw-r--r--   0        0        0     2954 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/update_payment_information_for_user.py
+-rw-r--r--   0        0        0     2483 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/payments/validate_customer_tax_information_for_user.py
+-rw-r--r--   0        0        0      101 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/__init__.py
+-rw-r--r--   0        0        0     3966 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_acceleration_unit_conversion.py
+-rw-r--r--   0        0        0     3784 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_angle_unit_conversion.py
+-rw-r--r--   0        0        0     4051 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_angular_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3758 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_area_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_charge_unit_conversion.py
+-rw-r--r--   0        0        0     3990 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_concentration_unit_conversion.py
+-rw-r--r--   0        0        0     4082 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_data_unit_conversion.py
+-rw-r--r--   0        0        0     3834 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_density_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_energy_unit_conversion.py
+-rw-r--r--   0        0        0     3782 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_force_unit_conversion.py
+-rw-r--r--   0        0        0     3938 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_illuminance_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_length_unit_conversion.py
+-rw-r--r--   0        0        0     4230 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py
+-rw-r--r--   0        0        0     3971 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_magnetic_flux_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_mass_unit_conversion.py
+-rw-r--r--   0        0        0     3918 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py
+-rw-r--r--   0        0        0     3955 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_metric_power_squared_unit_conversion.py
+-rw-r--r--   0        0        0     3848 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_metric_power_unit_conversion.py
+-rw-r--r--   0        0        0     3782 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_power_unit_conversion.py
+-rw-r--r--   0        0        0     3860 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_pressure_unit_conversion.py
+-rw-r--r--   0        0        0     3886 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_radiation_unit_conversion.py
+-rw-r--r--   0        0        0     3990 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_radioactivity_unit_conversion.py
+-rw-r--r--   0        0        0     3919 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_solid_angle_unit_conversion.py
+-rw-r--r--   0        0        0     3938 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_temperature_unit_conversion.py
+-rw-r--r--   0        0        0     3756 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_time_unit_conversion.py
+-rw-r--r--   0        0        0     3860 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_velocity_unit_conversion.py
+-rw-r--r--   0        0        0     3834 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_voltage_unit_conversion.py
+-rw-r--r--   0        0        0     3808 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/unit/get_volume_unit_conversion.py
+-rw-r--r--   0        0        0      297 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/delete_user_self.py
+-rw-r--r--   0        0        0     2757 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_session_for_user.py
+-rw-r--r--   0        0        0     3061 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user.py
+-rw-r--r--   0        0        0     3185 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_extended.py
+-rw-r--r--   0        0        0     2480 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_front_hash_self.py
+-rw-r--r--   0        0        0     2506 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_onboarding_self.py
+-rw-r--r--   0        0        0     2523 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_self.py
+-rw-r--r--   0        0        0     2629 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/get_user_self_extended.py
+-rw-r--r--   0        0        0     4105 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/list_users.py
+-rw-r--r--   0        0        0     4187 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/list_users_extended.py
+-rw-r--r--   0        0        0     2779 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/api/users/update_user_self.py
+-rw-r--r--   0        0        0     2297 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/client.py
+-rw-r--r--   0        0        0     5250 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/client_test.py
+-rw-r--r--   0        0        0   129480 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/examples_test.py
+-rw-r--r--   0        0        0     7966 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/__init__.py
+-rw-r--r--   0        0        0      322 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/account_provider.py
+-rw-r--r--   0        0        0     2249 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_api.py
+-rw-r--r--   0        0        0      242 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_api_type.py
+-rw-r--r--   0        0        0     2440 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_auth.py
+-rw-r--r--   0        0        0      413 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_auth_type.py
+-rw-r--r--   0        0        0      287 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_http_auth_type.py
+-rw-r--r--   0        0        0     4685 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/ai_plugin_manifest.py
+-rw-r--r--   0        0        0     1720 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_query_group.py
+-rw-r--r--   0        0        0      777 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_query_group_by.py
+-rw-r--r--   0        0        0      620 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_status.py
+-rw-r--r--   0        0        0     8574 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_with_price.py
+-rw-r--r--   0        0        0     2128 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_call_with_price_results_page.py
+-rw-r--r--   0        0        0     3455 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_token.py
+-rw-r--r--   0        0        0     2004 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/api_token_results_page.py
+-rw-r--r--   0        0        0     1447 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/app_client_info.py
+-rw-r--r--   0        0        0     5909 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call.py
+-rw-r--r--   0        0        0    34857 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call_output.py
+-rw-r--r--   0        0        0     2066 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call_results_page.py
+-rw-r--r--   0        0        0      648 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/async_api_call_type.py
+-rw-r--r--   0        0        0     2127 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/billing_info.py
+-rw-r--r--   0        0        0     1479 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/cache_metadata.py
+-rw-r--r--   0        0        0     3353 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/card_details.py
+-rw-r--r--   0        0        0     2697 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/cluster.py
+-rw-r--r--   0        0        0      229 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/code_language.py
+-rw-r--r--   0        0        0     2244 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/code_output.py
+-rw-r--r--   0        0        0     1732 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/commit.py
+-rw-r--r--   0        0        0    14343 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/connection.py
+-rw-r--r--   0        0        0    13513 2023-05-23 21:26:45.186695 kittycad-0.4.2/kittycad/models/country_code.py
+-rw-r--r--   0        0        0      507 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/created_at_sort_mode.py
+-rw-r--r--   0        0        0     8623 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/currency.py
+-rw-r--r--   0        0        0     4298 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/customer.py
+-rw-r--r--   0        0        0     4468 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/customer_balance.py
+-rw-r--r--   0        0        0     2412 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/device_access_token_request_form.py
+-rw-r--r--   0        0        0     1580 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/device_auth_request_form.py
+-rw-r--r--   0        0        0     1606 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/device_auth_verify_params.py
+-rw-r--r--   0        0        0    21264 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/docker_system_info.py
+-rw-r--r--   0        0        0     1789 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/email_authentication_form.py
+-rw-r--r--   0        0        0     3847 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/engine_metadata.py
+-rw-r--r--   0        0        0      529 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/environment.py
+-rw-r--r--   0        0        0     1930 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/error.py
+-rw-r--r--   0        0        0     2715 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/executor_metadata.py
+-rw-r--r--   0        0        0     6069 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/extended_user.py
+-rw-r--r--   0        0        0     2060 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/extended_user_results_page.py
+-rw-r--r--   0        0        0     1940 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/extrude.py
+-rw-r--r--   0        0        0     5862 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_center_of_mass.py
+-rw-r--r--   0        0        0     6222 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_conversion.py
+-rw-r--r--   0        0        0     5887 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_density.py
+-rw-r--r--   0        0        0     1369 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_export_format.py
+-rw-r--r--   0        0        0     1306 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_import_format.py
+-rw-r--r--   0        0        0     5869 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_mass.py
+-rw-r--r--   0        0        0     5684 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_surface_area.py
+-rw-r--r--   0        0        0     1513 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_system_metadata.py
+-rw-r--r--   0        0        0     5590 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/file_volume.py
+-rw-r--r--   0        0        0     2304 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/gateway.py
+-rw-r--r--   0        0        0      187 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/image_type.py
+-rw-r--r--   0        0        0     2228 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/index_info.py
+-rw-r--r--   0        0        0     8273 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/invoice.py
+-rw-r--r--   0        0        0     2888 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/invoice_line_item.py
+-rw-r--r--   0        0        0      563 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/invoice_status.py
+-rw-r--r--   0        0        0     2666 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream.py
+-rw-r--r--   0        0        0     1907 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream_api_stats.py
+-rw-r--r--   0        0        0     2212 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream_config.py
+-rw-r--r--   0        0        0     3174 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/jetstream_stats.py
+-rw-r--r--   0        0        0     2125 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/leaf_node.py
+-rw-r--r--   0        0        0     2007 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/line3d.py
+-rw-r--r--   0        0        0     1337 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/mesh.py
+-rw-r--r--   0        0        0     1923 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/meta_cluster_info.py
+-rw-r--r--   0        0        0     5025 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/metadata.py
+-rw-r--r--   0        0        0     1788 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/method.py
+-rw-r--r--   0        0        0     1726 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd.py
+-rw-r--r--   0        0        0       76 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd_id.py
+-rw-r--r--   0        0        0     2456 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd_req.py
+-rw-r--r--   0        0        0     1752 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_cmd_req_batch.py
+-rw-r--r--   0        0        0     2399 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_error.py
+-rw-r--r--   0        0        0     1878 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_outcome.py
+-rw-r--r--   0        0        0     1511 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/modeling_outcomes.py
+-rw-r--r--   0        0        0     3081 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/new_address.py
+-rw-r--r--   0        0        0     2038 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/o_auth2_client_info.py
+-rw-r--r--   0        0        0      415 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/o_auth2_grant_type.py
+-rw-r--r--   0        0        0     2509 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/onboarding.py
+-rw-r--r--   0        0        0     1646 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/output_file.py
+-rw-r--r--   0        0        0     1527 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_intent.py
+-rw-r--r--   0        0        0     3753 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_method.py
+-rw-r--r--   0        0        0     2267 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_method_card_checks.py
+-rw-r--r--   0        0        0      294 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/payment_method_type.py
+-rw-r--r--   0        0        0     5586 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/physics_constant.py
+-rw-r--r--   0        0        0     4448 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/physics_constant_name.py
+-rw-r--r--   0        0        0     2809 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/plugins_info.py
+-rw-r--r--   0        0        0     1530 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/point2d.py
+-rw-r--r--   0        0        0     1691 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/point3d.py
+-rw-r--r--   0        0        0     1498 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/point_e_metadata.py
+-rw-r--r--   0        0        0     1432 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/pong.py
+-rw-r--r--   0        0        0     4187 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/registry_service_config.py
+-rw-r--r--   0        0        0     2034 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/runtime.py
+-rw-r--r--   0        0        0     3855 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/session.py
+-rw-r--r--   0        0        0      214 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_cgroup_driver_enum.py
+-rw-r--r--   0        0        0      175 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_cgroup_version_enum.py
+-rw-r--r--   0        0        0     1663 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_default_address_pools.py
+-rw-r--r--   0        0        0      213 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/system_info_isolation_enum.py
+-rw-r--r--   0        0        0     6479 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_acceleration_conversion.py
+-rw-r--r--   0        0        0      642 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_acceleration_format.py
+-rw-r--r--   0        0        0     6388 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angle_conversion.py
+-rw-r--r--   0        0        0      916 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angle_format.py
+-rw-r--r--   0        0        0     6522 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angular_velocity_conversion.py
+-rw-r--r--   0        0        0      754 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_angular_velocity_format.py
+-rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_area_conversion.py
+-rw-r--r--   0        0        0      888 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_area_format.py
+-rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_charge_conversion.py
+-rw-r--r--   0        0        0      380 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_charge_format.py
+-rw-r--r--   0        0        0     6492 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_concentration_conversion.py
+-rw-r--r--   0        0        0      752 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_concentration_format.py
+-rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_conversion.py
+-rw-r--r--   0        0        0      539 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_format.py
+-rw-r--r--   0        0        0     6539 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_conversion.py
+-rw-r--r--   0        0        0      656 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_format.py
+-rw-r--r--   0        0        0     6414 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_density_conversion.py
+-rw-r--r--   0        0        0     1488 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_density_format.py
+-rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_energy_conversion.py
+-rw-r--r--   0        0        0     1162 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_energy_format.py
+-rw-r--r--   0        0        0     6388 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_force_conversion.py
+-rw-r--r--   0        0        0      645 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_force_format.py
+-rw-r--r--   0        0        0     6466 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_illuminance_conversion.py
+-rw-r--r--   0        0        0      584 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_illuminance_format.py
+-rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_length_conversion.py
+-rw-r--r--   0        0        0     2187 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_length_format.py
+-rw-r--r--   0        0        0     6604 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_field_strength_conversion.py
+-rw-r--r--   0        0        0      402 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_field_strength_format.py
+-rw-r--r--   0        0        0     6483 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_flux_conversion.py
+-rw-r--r--   0        0        0      389 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_magnetic_flux_format.py
+-rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_mass_conversion.py
+-rw-r--r--   0        0        0     1094 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_mass_format.py
+-rw-r--r--   0        0        0     3438 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power.py
+-rw-r--r--   0        0        0     6421 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power_conversion.py
+-rw-r--r--   0        0        0     6449 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power_cubed_conversion.py
+-rw-r--r--   0        0        0     6459 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_metric_power_squared_conversion.py
+-rw-r--r--   0        0        0     6388 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_power_conversion.py
+-rw-r--r--   0        0        0      468 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_power_format.py
+-rw-r--r--   0        0        0     6427 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_pressure_conversion.py
+-rw-r--r--   0        0        0      725 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_pressure_format.py
+-rw-r--r--   0        0        0     6440 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_radiation_conversion.py
+-rw-r--r--   0        0        0      586 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_radiation_format.py
+-rw-r--r--   0        0        0     6492 2023-05-23 21:26:45.190695 kittycad-0.4.2/kittycad/models/unit_radioactivity_conversion.py
+-rw-r--r--   0        0        0      570 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_radioactivity_format.py
+-rw-r--r--   0        0        0     6457 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_solid_angle_conversion.py
+-rw-r--r--   0        0        0      500 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_solid_angle_format.py
+-rw-r--r--   0        0        0     6466 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_temperature_conversion.py
+-rw-r--r--   0        0        0      674 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_temperature_format.py
+-rw-r--r--   0        0        0     6375 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_time_conversion.py
+-rw-r--r--   0        0        0      902 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_time_format.py
+-rw-r--r--   0        0        0     6427 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_velocity_conversion.py
+-rw-r--r--   0        0        0      753 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_velocity_format.py
+-rw-r--r--   0        0        0     6414 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_voltage_conversion.py
+-rw-r--r--   0        0        0      452 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_voltage_format.py
+-rw-r--r--   0        0        0     6401 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_volume_conversion.py
+-rw-r--r--   0        0        0     3286 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/unit_volume_format.py
+-rw-r--r--   0        0        0     2577 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/update_user.py
+-rw-r--r--   0        0        0     5084 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/user.py
+-rw-r--r--   0        0        0     1942 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/user_results_page.py
+-rw-r--r--   0        0        0       67 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/uuid.py
+-rw-r--r--   0        0        0     3448 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/models/verification_token.py
+-rw-r--r--   0        0        0       26 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/py.typed
+-rw-r--r--   0        0        0     1049 2023-05-23 21:26:45.194695 kittycad-0.4.2/kittycad/types.py
+-rw-r--r--   0        0        0     2472 2023-05-23 21:26:45.194695 kittycad-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 kittycad-0.4.2/PKG-INFO
```

### Comparing `kittycad-0.4.1/LICENSE` & `kittycad-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/README.md` & `kittycad-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/ai/create_image_to_3d.py` & `kittycad-0.4.2/kittycad/api/ai/create_image_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/ai/create_text_to_3d.py` & `kittycad-0.4.2/kittycad/api/ai/create_text_to_3d.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/get_api_call.py` & `kittycad-0.4.2/kittycad/api/api_calls/get_api_call.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/get_api_call_for_user.py` & `kittycad-0.4.2/kittycad/api/api_calls/get_api_call_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/get_api_call_metrics.py` & `kittycad-0.4.2/kittycad/api/api_calls/get_api_call_metrics.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/get_async_operation.py` & `kittycad-0.4.2/kittycad/api/api_calls/get_async_operation.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/list_api_calls.py` & `kittycad-0.4.2/kittycad/api/api_calls/list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/list_api_calls_for_user.py` & `kittycad-0.4.2/kittycad/api/api_calls/list_api_calls_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/list_async_operations.py` & `kittycad-0.4.2/kittycad/api/api_calls/list_async_operations.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_calls/user_list_api_calls.py` & `kittycad-0.4.2/kittycad/api/api_calls/user_list_api_calls.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_tokens/create_api_token_for_user.py` & `kittycad-0.4.2/kittycad/api/api_tokens/create_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_tokens/delete_api_token_for_user.py` & `kittycad-0.4.2/kittycad/api/api_tokens/delete_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_tokens/get_api_token_for_user.py` & `kittycad-0.4.2/kittycad/api/api_tokens/get_api_token_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/api_tokens/list_api_tokens_for_user.py` & `kittycad-0.4.2/kittycad/api/api_tokens/list_api_tokens_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/apps/apps_github_callback.py` & `kittycad-0.4.2/kittycad/api/apps/apps_github_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/apps/apps_github_consent.py` & `kittycad-0.4.2/kittycad/api/apps/apps_github_consent.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/apps/apps_github_webhook.py` & `kittycad-0.4.2/kittycad/api/apps/apps_github_webhook.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/constant/get_physics_constant.py` & `kittycad-0.4.2/kittycad/api/constant/get_physics_constant.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/drawing/cmd.py` & `kittycad-0.4.2/kittycad/api/users/update_user_self.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,113 +1,114 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.drawing_cmd_req import DrawingCmdReq
 from ...models.error import Error
+from ...models.update_user import UpdateUser
+from ...models.user import User
 from ...types import Response
 
 
 def _get_kwargs(
-    body: DrawingCmdReq,
+    body: UpdateUser,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/drawing/cmd".format(client.base_url)  # noqa: E501
+    url = "{}/user".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
     if response.status_code == 200:
-        response_200 = response.json()
+        response_200 = User.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[dict, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: DrawingCmdReq,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Optional[Union[dict, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.put(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: DrawingCmdReq,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[dict, Error]]:
-    """Response depends on which command was submitted, so unfortunately the OpenAPI schema can't generate the right response type."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: DrawingCmdReq,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Response[Optional[Union[dict, Error]]]:
+) -> Response[Optional[Union[User, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.put(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: DrawingCmdReq,
+    body: UpdateUser,
     *,
     client: Client,
-) -> Optional[Union[dict, Error]]:
-    """Response depends on which command was submitted, so unfortunately the OpenAPI schema can't generate the right response type."""  # noqa: E501
+) -> Optional[Union[User, Error]]:
+    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.1/kittycad/api/drawing/cmd_batch.py` & `kittycad-0.4.2/kittycad/api/modeling/cmd_batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.drawing_cmd_req_batch import DrawingCmdReqBatch
-from ...models.drawing_outcomes import DrawingOutcomes
 from ...models.error import Error
+from ...models.modeling_cmd_req_batch import ModelingCmdReqBatch
+from ...models.modeling_outcomes import ModelingOutcomes
 from ...types import Response
 
 
 def _get_kwargs(
-    body: DrawingCmdReqBatch,
+    body: ModelingCmdReqBatch,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/drawing/cmd_batch".format(client.base_url)  # noqa: E501
+    url = "{}/modeling/cmd_batch".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
@@ -26,89 +26,89 @@
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[DrawingOutcomes, Error]]:
+) -> Optional[Union[ModelingOutcomes, Error]]:
     if response.status_code == 200:
-        response_200 = DrawingOutcomes.from_dict(response.json())
+        response_200 = ModelingOutcomes.from_dict(response.json())
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[DrawingOutcomes, Error]]]:
+) -> Response[Optional[Union[ModelingOutcomes, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: DrawingCmdReqBatch,
+    body: ModelingCmdReqBatch,
     *,
     client: Client,
-) -> Response[Optional[Union[DrawingOutcomes, Error]]]:
+) -> Response[Optional[Union[ModelingOutcomes, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: DrawingCmdReqBatch,
+    body: ModelingCmdReqBatch,
     *,
     client: Client,
-) -> Optional[Union[DrawingOutcomes, Error]]:
+) -> Optional[Union[ModelingOutcomes, Error]]:
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: DrawingCmdReqBatch,
+    body: ModelingCmdReqBatch,
     *,
     client: Client,
-) -> Response[Optional[Union[DrawingOutcomes, Error]]]:
+) -> Response[Optional[Union[ModelingOutcomes, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: DrawingCmdReqBatch,
+    body: ModelingCmdReqBatch,
     *,
     client: Client,
-) -> Optional[Union[DrawingOutcomes, Error]]:
+) -> Optional[Union[ModelingOutcomes, Error]]:
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.1/kittycad/api/executor/create_executor_term.py` & `kittycad-0.4.2/kittycad/api/executor/create_executor_term.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/executor/create_file_execution.py` & `kittycad-0.4.2/kittycad/api/executor/create_file_execution.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_center_of_mass.py` & `kittycad-0.4.2/kittycad/api/file/create_file_surface_area.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.file_center_of_mass import FileCenterOfMass
 from ...models.file_import_format import FileImportFormat
+from ...models.file_surface_area import FileSurfaceArea
 from ...types import Response
 
 
 def _get_kwargs(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/center-of-mass".format(client.base_url)  # noqa: E501
+    url = "{}/file/surface-area".format(client.base_url)  # noqa: E501
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -32,44 +32,44 @@
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
 def _parse_response(
     *, response: httpx.Response
-) -> Optional[Union[FileCenterOfMass, Error]]:
+) -> Optional[Union[FileSurfaceArea, Error]]:
     if response.status_code == 201:
-        response_201 = FileCenterOfMass.from_dict(response.json())
+        response_201 = FileSurfaceArea.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
+) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
+) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
@@ -81,31 +81,34 @@
 
 
 def sync(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[FileCenterOfMass, Error]]:
-    """Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileSurfaceArea, Error]]:
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint returns the square measure units.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Optional[Union[FileCenterOfMass, Error]]]:
+) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -115,16 +118,19 @@
 
 
 async def asyncio(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[FileCenterOfMass, Error]]:
-    """Get the center of mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileSurfaceArea, Error]]:
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint returns the square measure units.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             src_format=src_format,
             body=body,
             client=client,
```

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_conversion.py` & `kittycad-0.4.2/kittycad/api/file/create_file_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_conversion_with_base64_helper.py` & `kittycad-0.4.2/kittycad/api/file/create_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_density.py` & `kittycad-0.4.2/kittycad/api/file/create_file_density.py`

 * *Files 21% similar despite different names*

```diff
@@ -89,15 +89,18 @@
 def sync(
     material_mass: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileDensity, Error]]:
-    """Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint assumes if you are giving a material mass in a specific mass units, we return a density in mass unit per cubic measure unit.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         material_mass=material_mass,
         src_format=src_format,
         body=body,
         client=client,
@@ -127,15 +130,18 @@
 async def asyncio(
     material_mass: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileDensity, Error]]:
-    """Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint assumes if you are giving a material mass in a specific mass units, we return a density in mass unit per cubic measure unit.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the density of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             material_mass=material_mass,
             src_format=src_format,
             body=body,
```

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_mass.py` & `kittycad-0.4.2/kittycad/api/file/create_file_mass.py`

 * *Files 24% similar despite different names*

```diff
@@ -89,15 +89,18 @@
 def sync(
     material_density: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileMass, Error]]:
-    """Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint assumes if you are giving a material density in a specific mass unit per cubic measure unit, we return a mass in mass units. The same mass units as passed in the material density.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         material_density=material_density,
         src_format=src_format,
         body=body,
         client=client,
@@ -127,15 +130,18 @@
 async def asyncio(
     material_density: float,
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Optional[Union[FileMass, Error]]:
-    """Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint assumes if you are giving a material density in a specific mass unit per cubic measure unit, we return a mass in mass units. The same mass units as passed in the material density.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the mass of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             material_density=material_density,
             src_format=src_format,
             body=body,
```

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_surface_area.py` & `kittycad-0.4.2/kittycad/api/file/create_file_volume.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
 from ...models.file_import_format import FileImportFormat
-from ...models.file_surface_area import FileSurfaceArea
+from ...models.file_volume import FileVolume
 from ...types import Response
 
 
 def _get_kwargs(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/file/surface-area".format(client.base_url)  # noqa: E501
+    url = "{}/file/volume".format(client.base_url)  # noqa: E501
     if src_format is not None:
         if "?" in url:
             url = url + "&src_format=" + str(src_format)
         else:
             url = url + "?src_format=" + str(src_format)
 
     headers: Dict[str, Any] = client.get_headers()
@@ -30,46 +30,44 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(
-    *, response: httpx.Response
-) -> Optional[Union[FileSurfaceArea, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[FileVolume, Error]]:
     if response.status_code == 201:
-        response_201 = FileSurfaceArea.from_dict(response.json())
+        response_201 = FileVolume.from_dict(response.json())
         return response_201
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
+) -> Response[Optional[Union[FileVolume, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
+) -> Response[Optional[Union[FileVolume, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     response = httpx.post(
@@ -81,31 +79,34 @@
 
 
 def sync(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[FileSurfaceArea, Error]]:
-    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileVolume, Error]]:
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint returns the cubic measure units.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return sync_detailed(
         src_format=src_format,
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Response[Optional[Union[FileSurfaceArea, Error]]]:
+) -> Response[Optional[Union[FileVolume, Error]]]:
     kwargs = _get_kwargs(
         src_format=src_format,
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -115,16 +116,19 @@
 
 
 async def asyncio(
     src_format: FileImportFormat,
     body: bytes,
     *,
     client: Client,
-) -> Optional[Union[FileSurfaceArea, Error]]:
-    """Get the surface area of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
+) -> Optional[Union[FileVolume, Error]]:
+    """We assume any file given to us has one consistent unit throughout. We also assume the file is at the proper scale.
+    Currently, this endpoint returns the cubic measure units.
+    In the future, we will use the units inside the file if they are given and do any conversions if necessary for the calculation. But currently, that is not supported.
+    Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
     If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             src_format=src_format,
             body=body,
             client=client,
```

### Comparing `kittycad-0.4.1/kittycad/api/file/create_file_volume.py` & `kittycad-0.4.2/kittycad/api/users/list_users_extended.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,148 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.created_at_sort_mode import CreatedAtSortMode
 from ...models.error import Error
-from ...models.file_import_format import FileImportFormat
-from ...models.file_volume import FileVolume
+from ...models.extended_user_results_page import ExtendedUserResultsPage
 from ...types import Response
 
 
 def _get_kwargs(
-    src_format: FileImportFormat,
-    body: bytes,
+    sort_by: CreatedAtSortMode,
     *,
     client: Client,
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
 ) -> Dict[str, Any]:
-    url = "{}/file/volume".format(client.base_url)  # noqa: E501
-    if src_format is not None:
+    url = "{}/users-extended".format(client.base_url)  # noqa: E501
+    if limit is not None:
         if "?" in url:
-            url = url + "&src_format=" + str(src_format)
+            url = url + "&limit=" + str(limit)
         else:
-            url = url + "?src_format=" + str(src_format)
+            url = url + "?limit=" + str(limit)
+    if page_token is not None:
+        if "?" in url:
+            url = url + "&page_token=" + str(page_token)
+        else:
+            url = url + "?page_token=" + str(page_token)
+    if sort_by is not None:
+        if "?" in url:
+            url = url + "&sort_by=" + str(sort_by)
+        else:
+            url = url + "?sort_by=" + str(sort_by)
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[FileVolume, Error]]:
-    if response.status_code == 201:
-        response_201 = FileVolume.from_dict(response.json())
-        return response_201
+def _parse_response(
+    *, response: httpx.Response
+) -> Optional[Union[ExtendedUserResultsPage, Error]]:
+    if response.status_code == 200:
+        response_200 = ExtendedUserResultsPage.from_dict(response.json())
+        return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[FileVolume, Error]]]:
+) -> Response[Optional[Union[ExtendedUserResultsPage, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    src_format: FileImportFormat,
-    body: bytes,
+    sort_by: CreatedAtSortMode,
     *,
     client: Client,
-) -> Response[Optional[Union[FileVolume, Error]]]:
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Response[Optional[Union[ExtendedUserResultsPage, Error]]]:
     kwargs = _get_kwargs(
-        src_format=src_format,
-        body=body,
+        limit=limit,
+        page_token=page_token,
+        sort_by=sort_by,
         client=client,
     )
 
-    response = httpx.post(
+    response = httpx.get(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    src_format: FileImportFormat,
-    body: bytes,
+    sort_by: CreatedAtSortMode,
     *,
     client: Client,
-) -> Optional[Union[FileVolume, Error]]:
-    """Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Optional[Union[ExtendedUserResultsPage, Error]]:
+    """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
 
     return sync_detailed(
-        src_format=src_format,
-        body=body,
+        limit=limit,
+        page_token=page_token,
+        sort_by=sort_by,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    src_format: FileImportFormat,
-    body: bytes,
+    sort_by: CreatedAtSortMode,
     *,
     client: Client,
-) -> Response[Optional[Union[FileVolume, Error]]]:
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Response[Optional[Union[ExtendedUserResultsPage, Error]]]:
     kwargs = _get_kwargs(
-        src_format=src_format,
-        body=body,
+        limit=limit,
+        page_token=page_token,
+        sort_by=sort_by,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.post(**kwargs)
+        response = await _client.get(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    src_format: FileImportFormat,
-    body: bytes,
+    sort_by: CreatedAtSortMode,
     *,
     client: Client,
-) -> Optional[Union[FileVolume, Error]]:
-    """Get the volume of an object in a CAD file. If the file is larger than 25MB, it will be performed asynchronously.
-    If the operation is performed asynchronously, the `id` of the operation will be returned. You can use the `id` returned from the request to get status information about the async operation from the `/async/operations/{id}` endpoint."""  # noqa: E501
+    limit: Optional[int] = None,
+    page_token: Optional[str] = None,
+) -> Optional[Union[ExtendedUserResultsPage, Error]]:
+    """This endpoint required authentication by a KittyCAD employee. The users are returned in order of creation, with the most recently created users first."""  # noqa: E501
 
     return (
         await asyncio_detailed(
-            src_format=src_format,
-            body=body,
+            limit=limit,
+            page_token=page_token,
+            sort_by=sort_by,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.1/kittycad/api/file/get_file_conversion_with_base64_helper.py` & `kittycad-0.4.2/kittycad/api/file/get_file_conversion_with_base64_helper.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/hidden/auth_email.py` & `kittycad-0.4.2/kittycad/api/hidden/auth_email.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/hidden/auth_email_callback.py` & `kittycad-0.4.2/kittycad/api/hidden/auth_email_callback.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/hidden/logout.py` & `kittycad-0.4.2/kittycad/api/hidden/logout.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/meta/get_ai_plugin_manifest.py` & `kittycad-0.4.2/kittycad/api/meta/get_ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/meta/get_metadata.py` & `kittycad-0.4.2/kittycad/api/meta/get_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/meta/get_openai_schema.py` & `kittycad-0.4.2/kittycad/api/meta/get_openai_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/meta/get_schema.py` & `kittycad-0.4.2/kittycad/api/meta/get_schema.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/meta/ping.py` & `kittycad-0.4.2/kittycad/api/meta/ping.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/create_payment_information_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/create_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/create_payment_intent_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/create_payment_intent_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/delete_payment_information_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/delete_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/delete_payment_method_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/delete_payment_method_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/get_payment_balance_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/get_payment_balance_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/get_payment_information_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/get_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/list_invoices_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/list_invoices_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/list_payment_methods_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/list_payment_methods_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/update_payment_information_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/update_payment_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/payments/validate_customer_tax_information_for_user.py` & `kittycad-0.4.2/kittycad/api/payments/validate_customer_tax_information_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_acceleration_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_acceleration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_angle_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_angular_velocity_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_angular_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_area_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_area_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_charge_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_charge_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_concentration_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_concentration_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_data_transfer_rate_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_data_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_data_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_density_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_density_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_energy_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_energy_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_force_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_force_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_illuminance_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_illuminance_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_length_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_length_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_magnetic_field_strength_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_magnetic_flux_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_magnetic_flux_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_mass_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_mass_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_metric_power_cubed_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_metric_power_squared_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_metric_power_squared_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_metric_power_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_metric_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_power_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_power_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_pressure_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_pressure_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_radiation_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_radiation_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_radioactivity_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_radioactivity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_solid_angle_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_solid_angle_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_temperature_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_temperature_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_time_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_time_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_velocity_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_velocity_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_voltage_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_voltage_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/unit/get_volume_unit_conversion.py` & `kittycad-0.4.2/kittycad/api/unit/get_volume_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/delete_user_self.py` & `kittycad-0.4.2/kittycad/api/users/delete_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_session_for_user.py` & `kittycad-0.4.2/kittycad/api/users/get_session_for_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_user.py` & `kittycad-0.4.2/kittycad/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_user_extended.py` & `kittycad-0.4.2/kittycad/api/users/get_user_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_user_front_hash_self.py` & `kittycad-0.4.2/kittycad/api/users/get_user_front_hash_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_user_onboarding_self.py` & `kittycad-0.4.2/kittycad/api/users/get_user_onboarding_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_user_self.py` & `kittycad-0.4.2/kittycad/api/users/get_user_self.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/get_user_self_extended.py` & `kittycad-0.4.2/kittycad/api/users/get_user_self_extended.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/list_users.py` & `kittycad-0.4.2/kittycad/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/api/users/update_user_self.py` & `kittycad-0.4.2/kittycad/api/modeling/cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,113 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.error import Error
-from ...models.update_user import UpdateUser
-from ...models.user import User
+from ...models.modeling_cmd_req import ModelingCmdReq
 from ...types import Response
 
 
 def _get_kwargs(
-    body: UpdateUser,
+    body: ModelingCmdReq,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)  # noqa: E501
+    url = "{}/modeling/cmd".format(client.base_url)  # noqa: E501
 
     headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "content": body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[User, Error]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[dict, Error]]:
     if response.status_code == 200:
-        response_200 = User.from_dict(response.json())
+        response_200 = response.json()
         return response_200
     if response.status_code == 400:
         response_4XX = Error.from_dict(response.json())
         return response_4XX
     if response.status_code == 500:
         response_5XX = Error.from_dict(response.json())
         return response_5XX
     return Error.from_dict(response.json())
 
 
 def _build_response(
     *, response: httpx.Response
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Union[dict, Error]]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    body: UpdateUser,
+    body: ModelingCmdReq,
     *,
     client: Client,
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
-    response = httpx.put(
+    response = httpx.post(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    body: UpdateUser,
+    body: ModelingCmdReq,
     *,
     client: Client,
-) -> Optional[Union[User, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
+) -> Optional[Union[dict, Error]]:
+    """Response depends on which command was submitted, so unfortunately the OpenAPI schema can't generate the right response type."""  # noqa: E501
 
     return sync_detailed(
         body=body,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    body: UpdateUser,
+    body: ModelingCmdReq,
     *,
     client: Client,
-) -> Response[Optional[Union[User, Error]]]:
+) -> Response[Optional[Union[dict, Error]]]:
     kwargs = _get_kwargs(
         body=body,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.put(**kwargs)
+        response = await _client.post(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    body: UpdateUser,
+    body: ModelingCmdReq,
     *,
     client: Client,
-) -> Optional[Union[User, Error]]:
-    """This endpoint requires authentication by any KittyCAD user. It updates information about the authenticated user."""  # noqa: E501
+) -> Optional[Union[dict, Error]]:
+    """Response depends on which command was submitted, so unfortunately the OpenAPI schema can't generate the right response type."""  # noqa: E501
 
     return (
         await asyncio_detailed(
             body=body,
             client=client,
         )
     ).parsed
```

### Comparing `kittycad-0.4.1/kittycad/client.py` & `kittycad-0.4.2/kittycad/client.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/client_test.py` & `kittycad-0.4.2/kittycad/client_test.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/examples_test.py` & `kittycad-0.4.2/kittycad/examples_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 )
 from kittycad.api.apps import (
     apps_github_callback,
     apps_github_consent,
     apps_github_webhook,
 )
 from kittycad.api.constant import get_physics_constant
-from kittycad.api.drawing import cmd, cmd_batch
 from kittycad.api.executor import create_executor_term, create_file_execution
 from kittycad.api.file import (
     create_file_center_of_mass,
     create_file_conversion,
     create_file_conversion_with_base64_helper,
     create_file_density,
     create_file_mass,
@@ -40,14 +39,15 @@
 from kittycad.api.meta import (
     get_ai_plugin_manifest,
     get_metadata,
     get_openai_schema,
     get_schema,
     ping,
 )
+from kittycad.api.modeling import cmd, cmd_batch, modeling_commands_ws
 from kittycad.api.payments import (
     create_payment_information_for_user,
     create_payment_intent_for_user,
     delete_payment_information_for_user,
     delete_payment_method_for_user,
     get_payment_balance_for_user,
     get_payment_information_for_user,
@@ -109,27 +109,27 @@
     ApiToken,
     ApiTokenResultsPage,
     AppClientInfo,
     AsyncApiCallResultsPage,
     CodeOutput,
     Customer,
     CustomerBalance,
-    DrawingOutcomes,
     Error,
     ExtendedUser,
     ExtendedUserResultsPage,
     FileCenterOfMass,
     FileConversion,
     FileDensity,
     FileMass,
     FileSurfaceArea,
     FileVolume,
     Invoice,
     Mesh,
     Metadata,
+    ModelingOutcomes,
     Onboarding,
     PaymentIntent,
     PaymentMethod,
     PhysicsConstant,
     Pong,
     Session,
     UnitAccelerationConversion,
@@ -166,23 +166,24 @@
     VerificationToken,
 )
 from kittycad.models.api_call_query_group_by import ApiCallQueryGroupBy
 from kittycad.models.api_call_status import ApiCallStatus
 from kittycad.models.billing_info import BillingInfo
 from kittycad.models.code_language import CodeLanguage
 from kittycad.models.created_at_sort_mode import CreatedAtSortMode
-from kittycad.models.drawing_cmd import DrawCircle
-from kittycad.models.drawing_cmd_id import DrawingCmdId
-from kittycad.models.drawing_cmd_req import DrawingCmdReq
-from kittycad.models.drawing_cmd_req_batch import DrawingCmdReqBatch
 from kittycad.models.email_authentication_form import EmailAuthenticationForm
 from kittycad.models.file_export_format import FileExportFormat
 from kittycad.models.file_import_format import FileImportFormat
 from kittycad.models.image_type import ImageType
+from kittycad.models.line3d import Line3d
+from kittycad.models.modeling_cmd_id import ModelingCmdId
+from kittycad.models.modeling_cmd_req import ModelingCmdReq
+from kittycad.models.modeling_cmd_req_batch import ModelingCmdReqBatch
 from kittycad.models.physics_constant_name import PhysicsConstantName
+from kittycad.models.point3d import Point3d
 from kittycad.models.unit_acceleration_format import UnitAccelerationFormat
 from kittycad.models.unit_angle_format import UnitAngleFormat
 from kittycad.models.unit_angular_velocity_format import UnitAngularVelocityFormat
 from kittycad.models.unit_area_format import UnitAreaFormat
 from kittycad.models.unit_charge_format import UnitChargeFormat
 from kittycad.models.unit_concentration_format import UnitConcentrationFormat
 from kittycad.models.unit_data_format import UnitDataFormat
@@ -1019,197 +1020,14 @@
     ] = await get_physics_constant.asyncio_detailed(
         client=client,
         constant=PhysicsConstantName.PI,
     )
 
 
 @pytest.mark.skip
-def test_cmd():
-    # Create our client.
-    client = ClientFromEnv()
-
-    cmd.sync(
-        client=client,
-        body=DrawingCmdReq(
-            cmd=DrawCircle(
-                center=[
-                    3.14,
-                    3.14,
-                ],
-                radius=3.14,
-            ),
-            cmd_id=DrawingCmdId("<uuid>"),
-            file_id="<string>",
-        ),
-    )
-
-    # OR if you need more info (e.g. status_code)
-    cmd.sync_detailed(
-        client=client,
-        body=DrawingCmdReq(
-            cmd=DrawCircle(
-                center=[
-                    3.14,
-                    3.14,
-                ],
-                radius=3.14,
-            ),
-            cmd_id=DrawingCmdId("<uuid>"),
-            file_id="<string>",
-        ),
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_cmd_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    await cmd.asyncio(
-        client=client,
-        body=DrawingCmdReq(
-            cmd=DrawCircle(
-                center=[
-                    3.14,
-                    3.14,
-                ],
-                radius=3.14,
-            ),
-            cmd_id=DrawingCmdId("<uuid>"),
-            file_id="<string>",
-        ),
-    )
-
-    # OR run async with more info
-    await cmd.asyncio_detailed(
-        client=client,
-        body=DrawingCmdReq(
-            cmd=DrawCircle(
-                center=[
-                    3.14,
-                    3.14,
-                ],
-                radius=3.14,
-            ),
-            cmd_id=DrawingCmdId("<uuid>"),
-            file_id="<string>",
-        ),
-    )
-
-
-@pytest.mark.skip
-def test_cmd_batch():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[Union[DrawingOutcomes, Error]] = cmd_batch.sync(
-        client=client,
-        body=DrawingCmdReqBatch(
-            cmds={
-                "<string>": DrawingCmdReq(
-                    cmd=DrawCircle(
-                        center=[
-                            3.14,
-                            3.14,
-                        ],
-                        radius=3.14,
-                    ),
-                    cmd_id=DrawingCmdId("<uuid>"),
-                    file_id="<string>",
-                )
-            },
-            file_id="<string>",
-        ),
-    )
-
-    if isinstance(result, Error) or result is None:
-        print(result)
-        raise Exception("Error in response")
-
-    body: DrawingOutcomes = result
-    print(body)
-
-    # OR if you need more info (e.g. status_code)
-    response: Response[
-        Optional[Union[DrawingOutcomes, Error]]
-    ] = cmd_batch.sync_detailed(
-        client=client,
-        body=DrawingCmdReqBatch(
-            cmds={
-                "<string>": DrawingCmdReq(
-                    cmd=DrawCircle(
-                        center=[
-                            3.14,
-                            3.14,
-                        ],
-                        radius=3.14,
-                    ),
-                    cmd_id=DrawingCmdId("<uuid>"),
-                    file_id="<string>",
-                )
-            },
-            file_id="<string>",
-        ),
-    )
-
-
-# OR run async
-@pytest.mark.asyncio
-@pytest.mark.skip
-async def test_cmd_batch_async():
-    # Create our client.
-    client = ClientFromEnv()
-
-    result: Optional[Union[DrawingOutcomes, Error]] = await cmd_batch.asyncio(
-        client=client,
-        body=DrawingCmdReqBatch(
-            cmds={
-                "<string>": DrawingCmdReq(
-                    cmd=DrawCircle(
-                        center=[
-                            3.14,
-                            3.14,
-                        ],
-                        radius=3.14,
-                    ),
-                    cmd_id=DrawingCmdId("<uuid>"),
-                    file_id="<string>",
-                )
-            },
-            file_id="<string>",
-        ),
-    )
-
-    # OR run async with more info
-    response: Response[
-        Optional[Union[DrawingOutcomes, Error]]
-    ] = await cmd_batch.asyncio_detailed(
-        client=client,
-        body=DrawingCmdReqBatch(
-            cmds={
-                "<string>": DrawingCmdReq(
-                    cmd=DrawCircle(
-                        center=[
-                            3.14,
-                            3.14,
-                        ],
-                        radius=3.14,
-                    ),
-                    cmd_id=DrawingCmdId("<uuid>"),
-                    file_id="<string>",
-                )
-            },
-            file_id="<string>",
-        ),
-    )
-
-
-@pytest.mark.skip
 def test_create_file_center_of_mass():
     # Create our client.
     client = ClientFromEnv()
 
     result: Optional[Union[FileCenterOfMass, Error]] = create_file_center_of_mass.sync(
         client=client,
         src_format=FileImportFormat.DAE,
@@ -1622,14 +1440,237 @@
     # OR run async with more info
     response: Response[Optional[Error]] = await logout.asyncio_detailed(
         client=client,
     )
 
 
 @pytest.mark.skip
+def test_cmd():
+    # Create our client.
+    client = ClientFromEnv()
+
+    cmd.sync(
+        client=client,
+        body=ModelingCmdReq(
+            cmd=Line3d(
+                from_=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
+            cmd_id=ModelingCmdId("<uuid>"),
+            file_id="<string>",
+        ),
+    )
+
+    # OR if you need more info (e.g. status_code)
+    cmd.sync_detailed(
+        client=client,
+        body=ModelingCmdReq(
+            cmd=Line3d(
+                from_=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
+            cmd_id=ModelingCmdId("<uuid>"),
+            file_id="<string>",
+        ),
+    )
+
+
+# OR run async
+@pytest.mark.asyncio
+@pytest.mark.skip
+async def test_cmd_async():
+    # Create our client.
+    client = ClientFromEnv()
+
+    await cmd.asyncio(
+        client=client,
+        body=ModelingCmdReq(
+            cmd=Line3d(
+                from_=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
+            cmd_id=ModelingCmdId("<uuid>"),
+            file_id="<string>",
+        ),
+    )
+
+    # OR run async with more info
+    await cmd.asyncio_detailed(
+        client=client,
+        body=ModelingCmdReq(
+            cmd=Line3d(
+                from_=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+                to=Point3d(
+                    x=3.14,
+                    y=3.14,
+                    z=3.14,
+                ),
+            ),
+            cmd_id=ModelingCmdId("<uuid>"),
+            file_id="<string>",
+        ),
+    )
+
+
+@pytest.mark.skip
+def test_cmd_batch():
+    # Create our client.
+    client = ClientFromEnv()
+
+    result: Optional[Union[ModelingOutcomes, Error]] = cmd_batch.sync(
+        client=client,
+        body=ModelingCmdReqBatch(
+            cmds={
+                "<string>": ModelingCmdReq(
+                    cmd=Line3d(
+                        from_=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
+                    cmd_id=ModelingCmdId("<uuid>"),
+                    file_id="<string>",
+                )
+            },
+            file_id="<string>",
+        ),
+    )
+
+    if isinstance(result, Error) or result is None:
+        print(result)
+        raise Exception("Error in response")
+
+    body: ModelingOutcomes = result
+    print(body)
+
+    # OR if you need more info (e.g. status_code)
+    response: Response[
+        Optional[Union[ModelingOutcomes, Error]]
+    ] = cmd_batch.sync_detailed(
+        client=client,
+        body=ModelingCmdReqBatch(
+            cmds={
+                "<string>": ModelingCmdReq(
+                    cmd=Line3d(
+                        from_=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
+                    cmd_id=ModelingCmdId("<uuid>"),
+                    file_id="<string>",
+                )
+            },
+            file_id="<string>",
+        ),
+    )
+
+
+# OR run async
+@pytest.mark.asyncio
+@pytest.mark.skip
+async def test_cmd_batch_async():
+    # Create our client.
+    client = ClientFromEnv()
+
+    result: Optional[Union[ModelingOutcomes, Error]] = await cmd_batch.asyncio(
+        client=client,
+        body=ModelingCmdReqBatch(
+            cmds={
+                "<string>": ModelingCmdReq(
+                    cmd=Line3d(
+                        from_=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
+                    cmd_id=ModelingCmdId("<uuid>"),
+                    file_id="<string>",
+                )
+            },
+            file_id="<string>",
+        ),
+    )
+
+    # OR run async with more info
+    response: Response[
+        Optional[Union[ModelingOutcomes, Error]]
+    ] = await cmd_batch.asyncio_detailed(
+        client=client,
+        body=ModelingCmdReqBatch(
+            cmds={
+                "<string>": ModelingCmdReq(
+                    cmd=Line3d(
+                        from_=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                        to=Point3d(
+                            x=3.14,
+                            y=3.14,
+                            z=3.14,
+                        ),
+                    ),
+                    cmd_id=ModelingCmdId("<uuid>"),
+                    file_id="<string>",
+                )
+            },
+            file_id="<string>",
+        ),
+    )
+
+
+@pytest.mark.skip
 def test_get_openai_schema():
     # Create our client.
     client = ClientFromEnv()
 
     get_openai_schema.sync(
         client=client,
     )
@@ -4788,7 +4829,39 @@
         client=client,
     )
 
     # OR run async with more info
     await create_executor_term.asyncio_detailed(
         client=client,
     )
+
+
+@pytest.mark.skip
+def test_modeling_commands_ws():
+    # Create our client.
+    client = ClientFromEnv()
+
+    modeling_commands_ws.sync(
+        client=client,
+    )
+
+    # OR if you need more info (e.g. status_code)
+    modeling_commands_ws.sync_detailed(
+        client=client,
+    )
+
+
+# OR run async
+@pytest.mark.asyncio
+@pytest.mark.skip
+async def test_modeling_commands_ws_async():
+    # Create our client.
+    client = ClientFromEnv()
+
+    await modeling_commands_ws.asyncio(
+        client=client,
+    )
+
+    # OR run async with more info
+    await modeling_commands_ws.asyncio_detailed(
+        client=client,
+    )
```

### Comparing `kittycad-0.4.1/kittycad/models/__init__.py` & `kittycad-0.4.2/kittycad/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,28 +32,22 @@
 from .currency import Currency
 from .customer import Customer
 from .customer_balance import CustomerBalance
 from .device_access_token_request_form import DeviceAccessTokenRequestForm
 from .device_auth_request_form import DeviceAuthRequestForm
 from .device_auth_verify_params import DeviceAuthVerifyParams
 from .docker_system_info import DockerSystemInfo
-from .drawing_cmd import DrawingCmd
-from .drawing_cmd_id import DrawingCmdId
-from .drawing_cmd_req import DrawingCmdReq
-from .drawing_cmd_req_batch import DrawingCmdReqBatch
-from .drawing_error import DrawingError
-from .drawing_outcome import DrawingOutcome
-from .drawing_outcomes import DrawingOutcomes
 from .email_authentication_form import EmailAuthenticationForm
 from .engine_metadata import EngineMetadata
 from .environment import Environment
 from .error import Error
 from .executor_metadata import ExecutorMetadata
 from .extended_user import ExtendedUser
 from .extended_user_results_page import ExtendedUserResultsPage
+from .extrude import Extrude
 from .file_center_of_mass import FileCenterOfMass
 from .file_conversion import FileConversion
 from .file_density import FileDensity
 from .file_export_format import FileExportFormat
 from .file_import_format import FileImportFormat
 from .file_mass import FileMass
 from .file_surface_area import FileSurfaceArea
@@ -66,30 +60,40 @@
 from .invoice_line_item import InvoiceLineItem
 from .invoice_status import InvoiceStatus
 from .jetstream import Jetstream
 from .jetstream_api_stats import JetstreamApiStats
 from .jetstream_config import JetstreamConfig
 from .jetstream_stats import JetstreamStats
 from .leaf_node import LeafNode
+from .line3d import Line3d
 from .mesh import Mesh
 from .meta_cluster_info import MetaClusterInfo
 from .metadata import Metadata
 from .method import Method
+from .modeling_cmd import ModelingCmd
+from .modeling_cmd_id import ModelingCmdId
+from .modeling_cmd_req import ModelingCmdReq
+from .modeling_cmd_req_batch import ModelingCmdReqBatch
+from .modeling_error import ModelingError
+from .modeling_outcome import ModelingOutcome
+from .modeling_outcomes import ModelingOutcomes
 from .new_address import NewAddress
 from .o_auth2_client_info import OAuth2ClientInfo
 from .o_auth2_grant_type import OAuth2GrantType
 from .onboarding import Onboarding
 from .output_file import OutputFile
 from .payment_intent import PaymentIntent
 from .payment_method import PaymentMethod
 from .payment_method_card_checks import PaymentMethodCardChecks
 from .payment_method_type import PaymentMethodType
 from .physics_constant import PhysicsConstant
 from .physics_constant_name import PhysicsConstantName
 from .plugins_info import PluginsInfo
+from .point2d import Point2d
+from .point3d import Point3d
 from .point_e_metadata import PointEMetadata
 from .pong import Pong
 from .registry_service_config import RegistryServiceConfig
 from .runtime import Runtime
 from .session import Session
 from .system_info_cgroup_driver_enum import SystemInfoCgroupDriverEnum
 from .system_info_cgroup_version_enum import SystemInfoCgroupVersionEnum
```

### Comparing `kittycad-0.4.1/kittycad/models/ai_plugin_api.py` & `kittycad-0.4.2/kittycad/models/ai_plugin_api.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/ai_plugin_auth.py` & `kittycad-0.4.2/kittycad/models/ai_plugin_auth.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/ai_plugin_manifest.py` & `kittycad-0.4.2/kittycad/models/ai_plugin_manifest.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/api_call_query_group.py` & `kittycad-0.4.2/kittycad/models/api_call_query_group.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/api_call_query_group_by.py` & `kittycad-0.4.2/kittycad/models/api_call_query_group_by.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/api_call_status.py` & `kittycad-0.4.2/kittycad/models/api_call_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/api_call_with_price.py` & `kittycad-0.4.2/kittycad/models/api_call_with_price.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.method import Method
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 S = TypeVar("S", bound="ApiCallWithPrice")
 
 
 @attr.s(auto_attribs=True)
 class ApiCallWithPrice:
@@ -143,15 +144,20 @@
 
         duration = d.pop("duration", UNSET)
 
         email = d.pop("email", UNSET)
 
         endpoint = d.pop("endpoint", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         ip_address = d.pop("ip_address", UNSET)
 
         litterbox = d.pop("litterbox", UNSET)
 
         _method = d.pop("method", UNSET)
         method: Union[Unset, Method]
@@ -179,15 +185,20 @@
         else:
             started_at = isoparse(_started_at)
 
         status_code = d.pop("status_code", UNSET)
 
         stripe_invoice_item_id = d.pop("stripe_invoice_item_id", UNSET)
 
-        token = d.pop("token", UNSET)
+        _token = d.pop("token", UNSET)
+        token: Union[Unset, Uuid]
+        if isinstance(_token, Unset):
+            token = UNSET
+        else:
+            token = Uuid(_token)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.1/kittycad/models/api_call_with_price_results_page.py` & `kittycad-0.4.2/kittycad/models/api_call_with_price_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/api_token.py` & `kittycad-0.4.2/kittycad/models/api_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 G = TypeVar("G", bound="ApiToken")
 
 
 @attr.s(auto_attribs=True)
 class ApiToken:
@@ -64,15 +65,20 @@
         else:
             created_at = isoparse(_created_at)
 
         id = d.pop("id", UNSET)
 
         is_valid = d.pop("is_valid", UNSET)
 
-        token = d.pop("token", UNSET)
+        _token = d.pop("token", UNSET)
+        token: Union[Unset, Uuid]
+        if isinstance(_token, Unset):
+            token = UNSET
+        else:
+            token = Uuid(_token)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.1/kittycad/models/api_token_results_page.py` & `kittycad-0.4.2/kittycad/models/api_token_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/app_client_info.py` & `kittycad-0.4.2/kittycad/models/app_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/async_api_call.py` & `kittycad-0.4.2/kittycad/models/async_api_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.async_api_call_type import AsyncApiCallType
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 Z = TypeVar("Z", bound="AsyncApiCall")
 
 
 @attr.s(auto_attribs=True)
 class AsyncApiCall:
@@ -99,15 +100,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
         output = d.pop("output", UNSET)
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/async_api_call_output.py` & `kittycad-0.4.2/kittycad/models/async_api_call_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 F = TypeVar("F", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
 class FileConversion:
@@ -101,15 +102,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, FileExportFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
@@ -274,15 +280,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = FileImportFormat(_src_format)
@@ -437,15 +448,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         mass = d.pop("mass", UNSET)
 
         material_density = d.pop("material_density", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
@@ -601,15 +617,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = FileImportFormat(_src_format)
@@ -768,15 +789,20 @@
         else:
             created_at = isoparse(_created_at)
 
         density = d.pop("density", UNSET)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         material_mass = d.pop("material_mass", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
@@ -930,15 +956,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = FileImportFormat(_src_format)
```

### Comparing `kittycad-0.4.1/kittycad/models/async_api_call_results_page.py` & `kittycad-0.4.2/kittycad/models/async_api_call_results_page.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/async_api_call_type.py` & `kittycad-0.4.2/kittycad/models/async_api_call_type.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/billing_info.py` & `kittycad-0.4.2/kittycad/models/billing_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/cache_metadata.py` & `kittycad-0.4.2/kittycad/models/cache_metadata.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/card_details.py` & `kittycad-0.4.2/kittycad/models/card_details.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/cluster.py` & `kittycad-0.4.2/kittycad/models/cluster.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/code_output.py` & `kittycad-0.4.2/kittycad/models/code_output.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/commit.py` & `kittycad-0.4.2/kittycad/models/commit.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/connection.py` & `kittycad-0.4.2/kittycad/models/connection.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/country_code.py` & `kittycad-0.4.2/kittycad/models/country_code.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/currency.py` & `kittycad-0.4.2/kittycad/models/currency.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/customer.py` & `kittycad-0.4.2/kittycad/models/customer.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/customer_balance.py` & `kittycad-0.4.2/kittycad/models/customer_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 N = TypeVar("N", bound="CustomerBalance")
 
 
 @attr.s(auto_attribs=True)
 class CustomerBalance:
@@ -68,15 +69,20 @@
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         monthly_credits_remaining = d.pop("monthly_credits_remaining", UNSET)
 
         pre_pay_cash_remaining = d.pop("pre_pay_cash_remaining", UNSET)
 
         pre_pay_credits_remaining = d.pop("pre_pay_credits_remaining", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/device_access_token_request_form.py` & `kittycad-0.4.2/kittycad/models/device_access_token_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/device_auth_request_form.py` & `kittycad-0.4.2/kittycad/models/device_auth_request_form.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/device_auth_verify_params.py` & `kittycad-0.4.2/kittycad/models/device_auth_verify_params.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/docker_system_info.py` & `kittycad-0.4.2/kittycad/models/docker_system_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/drawing_cmd.py` & `kittycad-0.4.2/kittycad/models/extrude.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,56 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.drawing_cmd_id import DrawingCmdId
+from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="DrawCircle")
-
-
-@attr.s(auto_attribs=True)
-class DrawCircle:
-    center: Union[Unset, List[float]] = UNSET
-    radius: Union[Unset, float] = UNSET
-
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        center: Union[Unset, List[float]] = UNSET
-        if not isinstance(self.center, Unset):
-            center = self.center
-        radius = self.radius
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if center is not UNSET:
-            field_dict["center"] = center
-        if radius is not UNSET:
-            field_dict["radius"] = radius
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
-        d = src_dict.copy()
-        center = cast(List[float], d.pop("center", UNSET))
-
-        radius = d.pop("radius", UNSET)
-
-        draw_circle = cls(
-            center=center,
-            radius=radius,
-        )
-
-        draw_circle.additional_properties = d
-        return draw_circle
-
-    @property
-    def additional_keys(self) -> List[str]:
-        return list(self.additional_properties.keys())
-
-    def __getitem__(self, key: str) -> Any:
-        return self.additional_properties[key]
-
-    def __setitem__(self, key: str, value: Any) -> None:
-        self.additional_properties[key] = value
-
-    def __delitem__(self, key: str) -> None:
-        del self.additional_properties[key]
-
-    def __contains__(self, key: str) -> bool:
-        return key in self.additional_properties
-
-
-V = TypeVar("V", bound="Extrude")
+T = TypeVar("T", bound="Extrude")
 
 
 @attr.s(auto_attribs=True)
 class Extrude:
+    """Command for extruding a solid."""  # noqa: E501
+
     distance: Union[Unset, float] = UNSET
-    sketch: Union[Unset, DrawingCmdId] = UNSET
+    target: Union[Unset, ModelingCmdId] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         distance = self.distance
-        if not isinstance(self.sketch, Unset):
-            sketch = self.sketch
+        if not isinstance(self.target, Unset):
+            target = self.target
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if distance is not UNSET:
             field_dict["distance"] = distance
-        if sketch is not UNSET:
-            field_dict["sketch"] = sketch
+        if target is not UNSET:
+            field_dict["target"] = target
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         distance = d.pop("distance", UNSET)
 
-        _sketch = d.pop("sketch", UNSET)
-        sketch: Union[Unset, DrawingCmdId]
-        if isinstance(_sketch, Unset):
-            sketch = UNSET
+        _target = d.pop("target", UNSET)
+        target: Union[Unset, ModelingCmdId]
+        if isinstance(_target, Unset):
+            target = UNSET
         else:
-            sketch = DrawingCmdId(_sketch)
+            target = ModelingCmdId(_target)
 
         extrude = cls(
             distance=distance,
-            sketch=sketch,
+            target=target,
         )
 
         extrude.additional_properties = d
         return extrude
 
     @property
     def additional_keys(self) -> List[str]:
@@ -119,10 +63,7 @@
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
-
-
-DrawingCmd = Union[DrawCircle, Extrude]
```

### Comparing `kittycad-0.4.1/kittycad/models/drawing_cmd_req.py` & `kittycad-0.4.2/kittycad/models/modeling_cmd_req.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.drawing_cmd import DrawingCmd
-from ..models.drawing_cmd_id import DrawingCmdId
+from ..models.modeling_cmd import ModelingCmd
+from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="DrawingCmdReq")
+Q = TypeVar("Q", bound="ModelingCmdReq")
 
 
 @attr.s(auto_attribs=True)
-class DrawingCmdReq:
-    """A graphics command submitted to the KittyCAD engine via the Drawing API."""  # noqa: E501
+class ModelingCmdReq:
+    """A graphics command submitted to the KittyCAD engine via the Modeling API."""  # noqa: E501
 
-    cmd: Union[Unset, DrawingCmd] = UNSET
-    cmd_id: Union[Unset, DrawingCmdId] = UNSET
+    cmd: Union[Unset, ModelingCmd] = UNSET
+    cmd_id: Union[Unset, ModelingCmdId] = UNSET
     file_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         if not isinstance(self.cmd, Unset):
             cmd = self.cmd
@@ -35,40 +35,40 @@
             field_dict["cmd_id"] = cmd_id
         if file_id is not UNSET:
             field_dict["file_id"] = file_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         _cmd = d.pop("cmd", UNSET)
-        cmd: Union[Unset, DrawingCmd]
+        cmd: Union[Unset, ModelingCmd]
         if isinstance(_cmd, Unset):
             cmd = UNSET
         else:
             cmd = _cmd  # type: ignore[arg-type]
 
         _cmd_id = d.pop("cmd_id", UNSET)
-        cmd_id: Union[Unset, DrawingCmdId]
+        cmd_id: Union[Unset, ModelingCmdId]
         if isinstance(_cmd_id, Unset):
             cmd_id = UNSET
         else:
-            cmd_id = DrawingCmdId(_cmd_id)
+            cmd_id = ModelingCmdId(_cmd_id)
 
         file_id = d.pop("file_id", UNSET)
 
-        drawing_cmd_req = cls(
+        modeling_cmd_req = cls(
             cmd=cmd,
             cmd_id=cmd_id,
             file_id=file_id,
         )
 
-        drawing_cmd_req.additional_properties = d
-        return drawing_cmd_req
+        modeling_cmd_req.additional_properties = d
+        return modeling_cmd_req
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/drawing_cmd_req_batch.py` & `kittycad-0.4.2/kittycad/models/file_system_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="DrawingCmdReqBatch")
+E = TypeVar("E", bound="FileSystemMetadata")
 
 
 @attr.s(auto_attribs=True)
-class DrawingCmdReqBatch:
-    """A batch set of graphics commands submitted to the KittyCAD engine via the Drawing API."""  # noqa: E501
+class FileSystemMetadata:
+    """Metadata about our file system.
 
-    cmds: Union[Unset, Any] = UNSET
-    file_id: Union[Unset, str] = UNSET
+    This is mostly used for internal purposes and debugging."""  # noqa: E501
+
+    ok: Union[Unset, bool] = False
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        cmds = self.cmds
-        file_id = self.file_id
+        ok = self.ok
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if cmds is not UNSET:
-            field_dict["cmds"] = cmds
-        if file_id is not UNSET:
-            field_dict["file_id"] = file_id
+        if ok is not UNSET:
+            field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
-        cmds = d.pop("cmds", UNSET)
-        file_id = d.pop("file_id", UNSET)
+        ok = d.pop("ok", UNSET)
 
-        drawing_cmd_req_batch = cls(
-            cmds=cmds,
-            file_id=file_id,
+        file_system_metadata = cls(
+            ok=ok,
         )
 
-        drawing_cmd_req_batch.additional_properties = d
-        return drawing_cmd_req_batch
+        file_system_metadata.additional_properties = d
+        return file_system_metadata
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/drawing_error.py` & `kittycad-0.4.2/kittycad/models/modeling_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="DrawingError")
+H = TypeVar("H", bound="ModelingError")
 
 
 @attr.s(auto_attribs=True)
-class DrawingError:
-    """Why a command submitted to the Drawing API failed."""  # noqa: E501
+class ModelingError:
+    """Why a command submitted to the Modeling API failed."""  # noqa: E501
 
     error_code: Union[Unset, str] = UNSET
     external_message: Union[Unset, str] = UNSET
     internal_message: Union[Unset, str] = UNSET
     status_code: Union[Unset, int] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -35,33 +35,33 @@
             field_dict["internal_message"] = internal_message
         if status_code is not UNSET:
             field_dict["status_code"] = status_code
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         external_message = d.pop("external_message", UNSET)
 
         internal_message = d.pop("internal_message", UNSET)
 
         status_code = d.pop("status_code", UNSET)
 
-        drawing_error = cls(
+        modeling_error = cls(
             error_code=error_code,
             external_message=external_message,
             internal_message=internal_message,
             status_code=status_code,
         )
 
-        drawing_error.additional_properties = d
-        return drawing_error
+        modeling_error.additional_properties = d
+        return modeling_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/drawing_outcome.py` & `kittycad-0.4.2/kittycad/models/modeling_outcome.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.drawing_cmd_id import DrawingCmdId
+from ..models.modeling_cmd_id import ModelingCmdId
 from ..types import UNSET, Unset
-from .drawing_error import DrawingError
+from .modeling_error import ModelingError
 
 Success = Any
 
 
-Error = DrawingError
+Error = ModelingError
 
 
-H = TypeVar("H", bound="Cancelled")
+N = TypeVar("N", bound="Cancelled")
 
 
 @attr.s(auto_attribs=True)
 class Cancelled:
-    what_failed: Union[Unset, DrawingCmdId] = UNSET
+    what_failed: Union[Unset, ModelingCmdId] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         if not isinstance(self.what_failed, Unset):
             what_failed = self.what_failed
 
@@ -30,22 +30,22 @@
         field_dict.update({})
         if what_failed is not UNSET:
             field_dict["what_failed"] = what_failed
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _what_failed = d.pop("what_failed", UNSET)
-        what_failed: Union[Unset, DrawingCmdId]
+        what_failed: Union[Unset, ModelingCmdId]
         if isinstance(_what_failed, Unset):
             what_failed = UNSET
         else:
-            what_failed = DrawingCmdId(_what_failed)
+            what_failed = ModelingCmdId(_what_failed)
 
         cancelled = cls(
             what_failed=what_failed,
         )
 
         cancelled.additional_properties = d
         return cancelled
@@ -63,8 +63,8 @@
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
 
 
-DrawingOutcome = Union[Success, Error, Cancelled]
+ModelingOutcome = Union[Success, Error, Cancelled]
```

### Comparing `kittycad-0.4.1/kittycad/models/drawing_outcomes.py` & `kittycad-0.4.2/kittycad/models/modeling_outcomes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DrawingOutcomes")
+H = TypeVar("H", bound="ModelingOutcomes")
 
 
 @attr.s(auto_attribs=True)
-class DrawingOutcomes:
-    """The result from a batch of drawing commands."""  # noqa: E501
+class ModelingOutcomes:
+    """The result from a batch of modeling commands."""  # noqa: E501
 
     outcomes: Union[Unset, Any] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         outcomes = self.outcomes
@@ -23,24 +23,24 @@
         field_dict.update({})
         if outcomes is not UNSET:
             field_dict["outcomes"] = outcomes
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         outcomes = d.pop("outcomes", UNSET)
 
-        drawing_outcomes = cls(
+        modeling_outcomes = cls(
             outcomes=outcomes,
         )
 
-        drawing_outcomes.additional_properties = d
-        return drawing_outcomes
+        modeling_outcomes.additional_properties = d
+        return modeling_outcomes
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/email_authentication_form.py` & `kittycad-0.4.2/kittycad/models/email_authentication_form.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="EmailAuthenticationForm")
+J = TypeVar("J", bound="EmailAuthenticationForm")
 
 
 @attr.s(auto_attribs=True)
 class EmailAuthenticationForm:
     """The body of the form for email authentication."""  # noqa: E501
 
     callback_url: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["callback_url"] = callback_url
         if email is not UNSET:
             field_dict["email"] = email
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         callback_url = d.pop("callback_url", UNSET)
 
         email = d.pop("email", UNSET)
 
         email_authentication_form = cls(
             callback_url=callback_url,
```

### Comparing `kittycad-0.4.1/kittycad/models/engine_metadata.py` & `kittycad-0.4.2/kittycad/models/engine_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..models.cache_metadata import CacheMetadata
 from ..models.connection import Connection
 from ..models.environment import Environment
 from ..models.file_system_metadata import FileSystemMetadata
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="EngineMetadata")
+V = TypeVar("V", bound="EngineMetadata")
 
 
 @attr.s(auto_attribs=True)
 class EngineMetadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -53,15 +53,15 @@
             field_dict["git_hash"] = git_hash
         if pubsub is not UNSET:
             field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         async_jobs_running = d.pop("async_jobs_running", UNSET)
 
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/error.py` & `kittycad-0.4.2/kittycad/models/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="Error")
+L = TypeVar("L", bound="Error")
 
 
 @attr.s(auto_attribs=True)
 class Error:
     """Error information from a response."""  # noqa: E501
 
     error_code: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["message"] = message
         if request_id is not UNSET:
             field_dict["request_id"] = request_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         error_code = d.pop("error_code", UNSET)
 
         message = d.pop("message", UNSET)
 
         request_id = d.pop("request_id", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/executor_metadata.py` & `kittycad-0.4.2/kittycad/models/executor_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import attr
 
 from ..models.docker_system_info import DockerSystemInfo
 from ..models.environment import Environment
 from ..types import UNSET, Unset
 
-A = TypeVar("A", bound="ExecutorMetadata")
+E = TypeVar("E", bound="ExecutorMetadata")
 
 
 @attr.s(auto_attribs=True)
 class ExecutorMetadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -37,15 +37,15 @@
             field_dict["environment"] = environment
         if git_hash is not UNSET:
             field_dict["git_hash"] = git_hash
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _docker_info = d.pop("docker_info", UNSET)
         docker_info: Union[Unset, DockerSystemInfo]
         if isinstance(_docker_info, Unset):
             docker_info = UNSET
         else:
             docker_info = DockerSystemInfo(_docker_info)
```

### Comparing `kittycad-0.4.1/kittycad/models/extended_user.py` & `kittycad-0.4.2/kittycad/models/extended_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="ExtendedUser")
+Y = TypeVar("Y", bound="ExtendedUser")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUser:
     """Extended user information.
 
     This is mostly used for internal purposes. It returns a mapping of the user's information, including that of our third party services we use for users: MailChimp, Stripe, and Front"""  # noqa: E501
@@ -93,15 +93,15 @@
             field_dict["stripe_id"] = stripe_id
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/extended_user_results_page.py` & `kittycad-0.4.2/kittycad/models/extended_user_results_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="ExtendedUserResultsPage")
+H = TypeVar("H", bound="ExtendedUserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class ExtendedUserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.extended_user import ExtendedUser
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         from ..models.extended_user import ExtendedUser
 
         items = cast(List[ExtendedUser], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/file_center_of_mass.py` & `kittycad-0.4.2/kittycad/models/file_center_of_mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="FileCenterOfMass")
+M = TypeVar("M", bound="FileCenterOfMass")
 
 
 @attr.s(auto_attribs=True)
 class FileCenterOfMass:
     """A file center of mass result."""  # noqa: E501
 
     center_of_mass: Union[Unset, List[float]] = UNSET
@@ -75,15 +76,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
         d = src_dict.copy()
         center_of_mass = cast(List[float], d.pop("center_of_mass", UNSET))
 
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
@@ -95,15 +96,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = FileImportFormat(_src_format)
```

### Comparing `kittycad-0.4.1/kittycad/models/file_conversion.py` & `kittycad-0.4.2/kittycad/models/file_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_export_format import FileExportFormat
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="FileConversion")
+B = TypeVar("B", bound="FileConversion")
 
 
 @attr.s(auto_attribs=True)
 class FileConversion:
     """A file conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -79,15 +80,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -97,15 +98,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, FileExportFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/file_density.py` & `kittycad-0.4.2/kittycad/models/file_density.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="FileDensity")
+S = TypeVar("S", bound="FileDensity")
 
 
 @attr.s(auto_attribs=True)
 class FileDensity:
     """A file density result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -77,15 +78,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -97,15 +98,20 @@
         else:
             created_at = isoparse(_created_at)
 
         density = d.pop("density", UNSET)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         material_mass = d.pop("material_mass", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/file_export_format.py` & `kittycad-0.4.2/kittycad/models/file_export_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/file_import_format.py` & `kittycad-0.4.2/kittycad/models/file_import_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/file_mass.py` & `kittycad-0.4.2/kittycad/models/file_mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="FileMass")
+A = TypeVar("A", bound="FileMass")
 
 
 @attr.s(auto_attribs=True)
 class FileMass:
     """A file mass result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -77,15 +78,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -95,15 +96,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         mass = d.pop("mass", UNSET)
 
         material_density = d.pop("material_density", UNSET)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/file_surface_area.py` & `kittycad-0.4.2/kittycad/models/file_surface_area.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="FileSurfaceArea")
+H = TypeVar("H", bound="FileSurfaceArea")
 
 
 @attr.s(auto_attribs=True)
 class FileSurfaceArea:
     """A file surface area result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -73,15 +74,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -91,15 +92,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = FileImportFormat(_src_format)
```

### Comparing `kittycad-0.4.1/kittycad/models/file_system_metadata.py` & `kittycad-0.4.2/kittycad/models/point_e_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="FileSystemMetadata")
+S = TypeVar("S", bound="PointEMetadata")
 
 
 @attr.s(auto_attribs=True)
-class FileSystemMetadata:
-    """Metadata about our file system.
+class PointEMetadata:
+    """Metadata about our point-e instance.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
 
     ok: Union[Unset, bool] = False
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -25,24 +25,24 @@
         field_dict.update({})
         if ok is not UNSET:
             field_dict["ok"] = ok
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         ok = d.pop("ok", UNSET)
 
-        file_system_metadata = cls(
+        point_e_metadata = cls(
             ok=ok,
         )
 
-        file_system_metadata.additional_properties = d
-        return file_system_metadata
+        point_e_metadata.additional_properties = d
+        return point_e_metadata
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/file_volume.py` & `kittycad-0.4.2/kittycad/models/file_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.file_import_format import FileImportFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="FileVolume")
+G = TypeVar("G", bound="FileVolume")
 
 
 @attr.s(auto_attribs=True)
 class FileVolume:
     """A file volume result."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -73,15 +74,15 @@
             field_dict["user_id"] = user_id
         if volume is not UNSET:
             field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -91,15 +92,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _src_format = d.pop("src_format", UNSET)
         src_format: Union[Unset, FileImportFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
             src_format = FileImportFormat(_src_format)
```

### Comparing `kittycad-0.4.1/kittycad/models/gateway.py` & `kittycad-0.4.2/kittycad/models/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="Gateway")
+J = TypeVar("J", bound="Gateway")
 
 
 @attr.s(auto_attribs=True)
 class Gateway:
     """Gateway information."""  # noqa: E501
 
     auth_timeout: Union[Unset, int] = UNSET
@@ -39,15 +39,15 @@
             field_dict["port"] = port
         if tls_timeout is not UNSET:
             field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/index_info.py` & `kittycad-0.4.2/kittycad/models/index_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/invoice.py` & `kittycad-0.4.2/kittycad/models/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..models.currency import Currency
 from ..models.invoice_status import InvoiceStatus
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="Invoice")
+L = TypeVar("L", bound="Invoice")
 
 
 @attr.s(auto_attribs=True)
 class Invoice:
     """An invoice."""  # noqa: E501
 
     amount_due: Union[Unset, float] = UNSET
@@ -129,15 +129,15 @@
             field_dict["total"] = total
         if url is not UNSET:
             field_dict["url"] = url
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         amount_due = d.pop("amount_due", UNSET)
 
         amount_paid = d.pop("amount_paid", UNSET)
 
         amount_remaining = d.pop("amount_remaining", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/invoice_line_item.py` & `kittycad-0.4.2/kittycad/models/invoice_line_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.currency import Currency
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="InvoiceLineItem")
+Y = TypeVar("Y", bound="InvoiceLineItem")
 
 
 @attr.s(auto_attribs=True)
 class InvoiceLineItem:
     """An invoice line item."""  # noqa: E501
 
     amount: Union[Unset, float] = UNSET
@@ -45,15 +45,15 @@
             field_dict["invoice_item"] = invoice_item
         if metadata is not UNSET:
             field_dict["metadata"] = metadata
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         amount = d.pop("amount", UNSET)
 
         _currency = d.pop("currency", UNSET)
         currency: Union[Unset, Currency]
         if isinstance(_currency, Unset):
             currency = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/invoice_status.py` & `kittycad-0.4.2/kittycad/models/invoice_status.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/jetstream.py` & `kittycad-0.4.2/kittycad/models/jetstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import attr
 
 from ..models.jetstream_config import JetstreamConfig
 from ..models.jetstream_stats import JetstreamStats
 from ..models.meta_cluster_info import MetaClusterInfo
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="Jetstream")
+H = TypeVar("H", bound="Jetstream")
 
 
 @attr.s(auto_attribs=True)
 class Jetstream:
     """Jetstream information."""  # noqa: E501
 
     config: Union[Unset, JetstreamConfig] = UNSET
@@ -37,15 +37,15 @@
             field_dict["meta"] = meta
         if stats is not UNSET:
             field_dict["stats"] = stats
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _config = d.pop("config", UNSET)
         config: Union[Unset, JetstreamConfig]
         if isinstance(_config, Unset):
             config = UNSET
         else:
             config = JetstreamConfig(_config)
```

### Comparing `kittycad-0.4.1/kittycad/models/jetstream_api_stats.py` & `kittycad-0.4.2/kittycad/models/jetstream_api_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-U = TypeVar("U", bound="JetstreamApiStats")
+K = TypeVar("K", bound="JetstreamApiStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamApiStats:
     """Jetstream API statistics."""  # noqa: E501
 
     errors: Union[Unset, int] = UNSET
@@ -31,15 +31,15 @@
             field_dict["inflight"] = inflight
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         errors = d.pop("errors", UNSET)
 
         inflight = d.pop("inflight", UNSET)
 
         total = d.pop("total", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/jetstream_config.py` & `kittycad-0.4.2/kittycad/models/jetstream_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-S = TypeVar("S", bound="JetstreamConfig")
+V = TypeVar("V", bound="JetstreamConfig")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamConfig:
     """Jetstream configuration."""  # noqa: E501
 
     domain: Union[Unset, str] = UNSET
@@ -35,15 +35,15 @@
             field_dict["max_storage"] = max_storage
         if store_dir is not UNSET:
             field_dict["store_dir"] = store_dir
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         domain = d.pop("domain", UNSET)
 
         max_memory = d.pop("max_memory", UNSET)
 
         max_storage = d.pop("max_storage", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/jetstream_stats.py` & `kittycad-0.4.2/kittycad/models/jetstream_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.jetstream_api_stats import JetstreamApiStats
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="JetstreamStats")
+R = TypeVar("R", bound="JetstreamStats")
 
 
 @attr.s(auto_attribs=True)
 class JetstreamStats:
     """Jetstream statistics."""  # noqa: E501
 
     accounts: Union[Unset, int] = UNSET
@@ -49,15 +49,15 @@
             field_dict["reserved_store"] = reserved_store
         if store is not UNSET:
             field_dict["store"] = store
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         accounts = d.pop("accounts", UNSET)
 
         _api = d.pop("api", UNSET)
         api: Union[Unset, JetstreamApiStats]
         if isinstance(_api, Unset):
             api = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/leaf_node.py` & `kittycad-0.4.2/kittycad/models/leaf_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="LeafNode")
+N = TypeVar("N", bound="LeafNode")
 
 
 @attr.s(auto_attribs=True)
 class LeafNode:
     """Leaf node information."""  # noqa: E501
 
     auth_timeout: Union[Unset, int] = UNSET
@@ -35,15 +35,15 @@
             field_dict["port"] = port
         if tls_timeout is not UNSET:
             field_dict["tls_timeout"] = tls_timeout
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         auth_timeout = d.pop("auth_timeout", UNSET)
 
         host = d.pop("host", UNSET)
 
         port = d.pop("port", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/mesh.py` & `kittycad-0.4.2/kittycad/models/pong.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="Mesh")
+L = TypeVar("L", bound="Pong")
 
 
 @attr.s(auto_attribs=True)
-class Mesh:
-    mesh: Union[Unset, str] = UNSET
+class Pong:
+    """The response from the `/ping` endpoint."""  # noqa: E501
+
+    message: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        mesh = self.mesh
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if mesh is not UNSET:
-            field_dict["mesh"] = mesh
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
-        mesh = d.pop("mesh", UNSET)
+        message = d.pop("message", UNSET)
 
-        mesh = cls(
-            mesh=mesh,
+        pong = cls(
+            message=message,
         )
 
-        mesh.additional_properties = d
-        return mesh
+        pong.additional_properties = d
+        return pong
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/meta_cluster_info.py` & `kittycad-0.4.2/kittycad/models/meta_cluster_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="MetaClusterInfo")
+U = TypeVar("U", bound="MetaClusterInfo")
 
 
 @attr.s(auto_attribs=True)
 class MetaClusterInfo:
     """Jetstream statistics."""  # noqa: E501
 
     cluster_size: Union[Unset, int] = UNSET
@@ -31,15 +31,15 @@
             field_dict["leader"] = leader
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
         d = src_dict.copy()
         cluster_size = d.pop("cluster_size", UNSET)
 
         leader = d.pop("leader", UNSET)
 
         name = d.pop("name", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/metadata.py` & `kittycad-0.4.2/kittycad/models/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..models.engine_metadata import EngineMetadata
 from ..models.environment import Environment
 from ..models.executor_metadata import ExecutorMetadata
 from ..models.file_system_metadata import FileSystemMetadata
 from ..models.point_e_metadata import PointEMetadata
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="Metadata")
+S = TypeVar("S", bound="Metadata")
 
 
 @attr.s(auto_attribs=True)
 class Metadata:
     """Metadata about our currently running server.
 
     This is mostly used for internal purposes and debugging."""  # noqa: E501
@@ -67,15 +67,15 @@
             field_dict["point_e"] = point_e
         if pubsub is not UNSET:
             field_dict["pubsub"] = pubsub
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
         d = src_dict.copy()
         _cache = d.pop("cache", UNSET)
         cache: Union[Unset, CacheMetadata]
         if isinstance(_cache, Unset):
             cache = UNSET
         else:
             cache = CacheMetadata(_cache)
```

### Comparing `kittycad-0.4.1/kittycad/models/method.py` & `kittycad-0.4.2/kittycad/models/method.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/new_address.py` & `kittycad-0.4.2/kittycad/models/new_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..models.country_code import CountryCode
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="NewAddress")
+B = TypeVar("B", bound="NewAddress")
 
 
 @attr.s(auto_attribs=True)
 class NewAddress:
     """The struct that is used to create a new record. This is automatically generated and has all the same fields as the main struct only it is missing the `id`."""  # noqa: E501
 
     city: Union[Unset, str] = UNSET
@@ -49,15 +49,15 @@
             field_dict["user_id"] = user_id
         if zip is not UNSET:
             field_dict["zip"] = zip
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         city = d.pop("city", UNSET)
 
         _country = d.pop("country", UNSET)
         country: Union[Unset, CountryCode]
         if isinstance(_country, Unset):
             country = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/o_auth2_client_info.py` & `kittycad-0.4.2/kittycad/models/o_auth2_client_info.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/onboarding.py` & `kittycad-0.4.2/kittycad/models/onboarding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-B = TypeVar("B", bound="Onboarding")
+P = TypeVar("P", bound="Onboarding")
 
 
 @attr.s(auto_attribs=True)
 class Onboarding:
     """Onboarding details"""  # noqa: E501
 
-    first_call_from_their_machine_date: Union[Unset, str] = UNSET
+    first_call_from__their_machine_date: Union[Unset, str] = UNSET
     first_litterbox_execute_date: Union[Unset, str] = UNSET
     first_token_date: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        first_call_from_their_machine_date = self.first_call_from_their_machine_date
+        first_call_from__their_machine_date = self.first_call_from__their_machine_date
         first_litterbox_execute_date = self.first_litterbox_execute_date
         first_token_date = self.first_token_date
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if first_call_from_their_machine_date is not UNSET:
+        if first_call_from__their_machine_date is not UNSET:
             field_dict[
                 "first_call_from_their_machine_date"
-            ] = first_call_from_their_machine_date
+            ] = first_call_from__their_machine_date
         if first_litterbox_execute_date is not UNSET:
             field_dict["first_litterbox_execute_date"] = first_litterbox_execute_date
         if first_token_date is not UNSET:
             field_dict["first_token_date"] = first_token_date
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
-        first_call_from_their_machine_date = d.pop(
+        first_call_from__their_machine_date = d.pop(
             "first_call_from_their_machine_date", UNSET
         )
 
         first_litterbox_execute_date = d.pop("first_litterbox_execute_date", UNSET)
 
         first_token_date = d.pop("first_token_date", UNSET)
 
         onboarding = cls(
-            first_call_from_their_machine_date=first_call_from_their_machine_date,
+            first_call_from__their_machine_date=first_call_from__their_machine_date,
             first_litterbox_execute_date=first_litterbox_execute_date,
             first_token_date=first_token_date,
         )
 
         onboarding.additional_properties = d
         return onboarding
```

### Comparing `kittycad-0.4.1/kittycad/models/output_file.py` & `kittycad-0.4.2/kittycad/models/output_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="OutputFile")
+J = TypeVar("J", bound="OutputFile")
 
 
 @attr.s(auto_attribs=True)
 class OutputFile:
     """Output file contents."""  # noqa: E501
 
     contents: Union[Unset, str] = UNSET
@@ -27,15 +27,15 @@
             field_dict["contents"] = contents
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         contents = d.pop("contents", UNSET)
 
         name = d.pop("name", UNSET)
 
         output_file = cls(
             contents=contents,
```

### Comparing `kittycad-0.4.1/kittycad/models/payment_intent.py` & `kittycad-0.4.2/kittycad/models/payment_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="PaymentIntent")
+T = TypeVar("T", bound="PaymentIntent")
 
 
 @attr.s(auto_attribs=True)
 class PaymentIntent:
     """A payment intent response."""  # noqa: E501
 
     client_secret: Union[Unset, str] = UNSET
@@ -23,15 +23,15 @@
         field_dict.update({})
         if client_secret is not UNSET:
             field_dict["client_secret"] = client_secret
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         client_secret = d.pop("client_secret", UNSET)
 
         payment_intent = cls(
             client_secret=client_secret,
         )
```

### Comparing `kittycad-0.4.1/kittycad/models/payment_method.py` & `kittycad-0.4.2/kittycad/models/payment_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil.parser import isoparse
 
 from ..models.billing_info import BillingInfo
 from ..models.card_details import CardDetails
 from ..models.payment_method_type import PaymentMethodType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PaymentMethod")
+V = TypeVar("V", bound="PaymentMethod")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethod:
     """A payment method."""  # noqa: E501
 
     billing_info: Union[Unset, BillingInfo] = UNSET
@@ -53,15 +53,15 @@
             field_dict["metadata"] = metadata
         if type is not UNSET:
             field_dict["type"] = type
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _billing_info = d.pop("billing_info", UNSET)
         billing_info: Union[Unset, BillingInfo]
         if isinstance(_billing_info, Unset):
             billing_info = UNSET
         else:
             billing_info = BillingInfo(_billing_info)
```

### Comparing `kittycad-0.4.1/kittycad/models/payment_method_card_checks.py` & `kittycad-0.4.2/kittycad/models/payment_method_card_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="PaymentMethodCardChecks")
+C = TypeVar("C", bound="PaymentMethodCardChecks")
 
 
 @attr.s(auto_attribs=True)
 class PaymentMethodCardChecks:
     """Card checks."""  # noqa: E501
 
     address_line1_check: Union[Unset, str] = UNSET
@@ -31,15 +31,15 @@
             field_dict["address_postal_code_check"] = address_postal_code_check
         if cvc_check is not UNSET:
             field_dict["cvc_check"] = cvc_check
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         address_line1_check = d.pop("address_line1_check", UNSET)
 
         address_postal_code_check = d.pop("address_postal_code_check", UNSET)
 
         cvc_check = d.pop("cvc_check", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/physics_constant.py` & `kittycad-0.4.2/kittycad/models/physics_constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.physics_constant_name import PhysicsConstantName
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="PhysicsConstant")
+R = TypeVar("R", bound="PhysicsConstant")
 
 
 @attr.s(auto_attribs=True)
 class PhysicsConstant:
     """A physics constant."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -73,15 +74,15 @@
             field_dict["user_id"] = user_id
         if value is not UNSET:
             field_dict["value"] = value
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -98,15 +99,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
```

### Comparing `kittycad-0.4.1/kittycad/models/physics_constant_name.py` & `kittycad-0.4.2/kittycad/models/physics_constant_name.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/plugins_info.py` & `kittycad-0.4.2/kittycad/models/plugins_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="PluginsInfo")
+C = TypeVar("C", bound="PluginsInfo")
 
 
 @attr.s(auto_attribs=True)
 class PluginsInfo:
     """Available plugins per type.
 
     **Note**: Only unmanaged (V1) plugins are included in this list. V1 plugins are \"lazily\" loaded, and are not returned in this list if there is no resource using the plugin."""  # noqa: E501
@@ -45,15 +45,15 @@
             field_dict["network"] = network
         if volume is not UNSET:
             field_dict["volume"] = volume
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
         authorization = cast(List[str], d.pop("authorization", UNSET))
 
         log = cast(List[str], d.pop("log", UNSET))
 
         network = cast(List[str], d.pop("network", UNSET))
```

### Comparing `kittycad-0.4.1/kittycad/models/point_e_metadata.py` & `kittycad-0.4.2/kittycad/models/runtime.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-C = TypeVar("C", bound="PointEMetadata")
+E = TypeVar("E", bound="Runtime")
 
 
 @attr.s(auto_attribs=True)
-class PointEMetadata:
-    """Metadata about our point-e instance.
+class Runtime:
+    """Runtime describes an [OCI compliant](https://github.com/opencontainers/runtime-spec) runtime.  The runtime is invoked by the daemon via the `containerd` daemon. OCI runtimes act as an interface to the Linux kernel namespaces, cgroups, and SELinux."""  # noqa: E501
 
-    This is mostly used for internal purposes and debugging."""  # noqa: E501
-
-    ok: Union[Unset, bool] = False
+    path: Union[Unset, str] = UNSET
+    runtime_args: Union[Unset, List[str]] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        ok = self.ok
+        path = self.path
+        runtime_args: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.runtime_args, Unset):
+            runtime_args = self.runtime_args
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if ok is not UNSET:
-            field_dict["ok"] = ok
+        if path is not UNSET:
+            field_dict["path"] = path
+        if runtime_args is not UNSET:
+            field_dict["runtime_args"] = runtime_args
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
-        ok = d.pop("ok", UNSET)
+        path = d.pop("path", UNSET)
+
+        runtime_args = cast(List[str], d.pop("runtime_args", UNSET))
 
-        point_e_metadata = cls(
-            ok=ok,
+        runtime = cls(
+            path=path,
+            runtime_args=runtime_args,
         )
 
-        point_e_metadata.additional_properties = d
-        return point_e_metadata
+        runtime.additional_properties = d
+        return runtime
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/pong.py` & `kittycad-0.4.2/kittycad/models/mesh.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="Pong")
+C = TypeVar("C", bound="Mesh")
 
 
 @attr.s(auto_attribs=True)
-class Pong:
-    """The response from the `/ping` endpoint."""  # noqa: E501
-
-    message: Union[Unset, str] = UNSET
+class Mesh:
+    mesh: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        message = self.message
+        mesh = self.mesh
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if message is not UNSET:
-            field_dict["message"] = message
+        if mesh is not UNSET:
+            field_dict["mesh"] = mesh
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[C], src_dict: Dict[str, Any]) -> C:
         d = src_dict.copy()
-        message = d.pop("message", UNSET)
+        mesh = d.pop("mesh", UNSET)
 
-        pong = cls(
-            message=message,
+        mesh = cls(
+            mesh=mesh,
         )
 
-        pong.additional_properties = d
-        return pong
+        mesh.additional_properties = d
+        return mesh
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/registry_service_config.py` & `kittycad-0.4.2/kittycad/models/registry_service_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-M = TypeVar("M", bound="RegistryServiceConfig")
+T = TypeVar("T", bound="RegistryServiceConfig")
 
 
 @attr.s(auto_attribs=True)
 class RegistryServiceConfig:
     """RegistryServiceConfig stores daemon registry services configuration."""  # noqa: E501
 
     allow_nondistributable_artifacts_cid_rs: Union[Unset, List[str]] = UNSET
@@ -55,15 +55,15 @@
             field_dict["insecure_registry_cid_rs"] = insecure_registry_cid_rs
         if mirrors is not UNSET:
             field_dict["mirrors"] = mirrors
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[M], src_dict: Dict[str, Any]) -> M:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         allow_nondistributable_artifacts_cid_rs = cast(
             List[str], d.pop("allow_nondistributable_artifacts_cid_rs", UNSET)
         )
 
         allow_nondistributable_artifacts_hostnames = cast(
             List[str], d.pop("allow_nondistributable_artifacts_hostnames", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/runtime.py` & `kittycad-0.4.2/kittycad/models/modeling_cmd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.point2d import Point2d
 from ..types import UNSET, Unset
+from .extrude import Extrude
+from .line3d import Line3d
 
-S = TypeVar("S", bound="Runtime")
+AddLine = Line3d
 
 
-@attr.s(auto_attribs=True)
-class Runtime:
-    """Runtime describes an [OCI compliant](https://github.com/opencontainers/runtime-spec) runtime.  The runtime is invoked by the daemon via the `containerd` daemon. OCI runtimes act as an interface to the Linux kernel namespaces, cgroups, and SELinux."""  # noqa: E501
+K = TypeVar("K", bound="SelectionClick")
+
 
-    path: Union[Unset, str] = UNSET
-    runtime_args: Union[Unset, List[str]] = UNSET
+@attr.s(auto_attribs=True)
+class SelectionClick:
+    at: Union[Unset, Point2d] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        path = self.path
-        runtime_args: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.runtime_args, Unset):
-            runtime_args = self.runtime_args
+        if not isinstance(self.at, Unset):
+            at = self.at
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if path is not UNSET:
-            field_dict["path"] = path
-        if runtime_args is not UNSET:
-            field_dict["runtime_args"] = runtime_args
+        if at is not UNSET:
+            field_dict["at"] = at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[S], src_dict: Dict[str, Any]) -> S:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
-        path = d.pop("path", UNSET)
+        _at = d.pop("at", UNSET)
+        at: Union[Unset, Point2d]
+        if isinstance(_at, Unset):
+            at = UNSET
+        else:
+            at = Point2d(_at)
 
-        runtime_args = cast(List[str], d.pop("runtime_args", UNSET))
-
-        runtime = cls(
-            path=path,
-            runtime_args=runtime_args,
+        selection_click = cls(
+            at=at,
         )
 
-        runtime.additional_properties = d
-        return runtime
+        selection_click.additional_properties = d
+        return selection_click
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
@@ -58,7 +59,10 @@
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
+
+
+ModelingCmd = Union[AddLine, Extrude, SelectionClick]
```

### Comparing `kittycad-0.4.1/kittycad/models/session.py` & `kittycad-0.4.2/kittycad/models/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="Session")
+D = TypeVar("D", bound="Session")
 
 
 @attr.s(auto_attribs=True)
 class Session:
     """An authentication session.
 
     For our UIs, these are automatically created by Next.js."""  # noqa: E501
@@ -53,15 +54,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
@@ -71,15 +72,20 @@
         if isinstance(_expires, Unset):
             expires = UNSET
         else:
             expires = isoparse(_expires)
 
         id = d.pop("id", UNSET)
 
-        session_token = d.pop("session_token", UNSET)
+        _session_token = d.pop("session_token", UNSET)
+        session_token: Union[Unset, Uuid]
+        if isinstance(_session_token, Unset):
+            session_token = UNSET
+        else:
+            session_token = Uuid(_session_token)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
```

### Comparing `kittycad-0.4.1/kittycad/models/system_info_default_address_pools.py` & `kittycad-0.4.2/kittycad/models/system_info_default_address_pools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SystemInfoDefaultAddressPools")
+Y = TypeVar("Y", bound="SystemInfoDefaultAddressPools")
 
 
 @attr.s(auto_attribs=True)
 class SystemInfoDefaultAddressPools:
     base: Union[Unset, str] = UNSET
     size: Union[Unset, int] = UNSET
 
@@ -25,15 +25,15 @@
             field_dict["base"] = base
         if size is not UNSET:
             field_dict["size"] = size
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         base = d.pop("base", UNSET)
 
         size = d.pop("size", UNSET)
 
         system_info_default_address_pools = cls(
             base=base,
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_acceleration_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_acceleration_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_acceleration_format import UnitAccelerationFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="UnitAccelerationConversion")
+Y = TypeVar("Y", bound="UnitAccelerationConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAccelerationConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitAccelerationFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_acceleration_format.py` & `kittycad-0.4.2/kittycad/models/unit_acceleration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_angle_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_angle_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_angle_format import UnitAngleFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 D = TypeVar("D", bound="UnitAngleConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAngleConversion:
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitAngleFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_angle_format.py` & `kittycad-0.4.2/kittycad/models/unit_angle_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_angular_velocity_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_angular_velocity_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_angular_velocity_format import UnitAngularVelocityFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitAngularVelocityConversion")
+F = TypeVar("F", bound="UnitAngularVelocityConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAngularVelocityConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitAngularVelocityFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_angular_velocity_format.py` & `kittycad-0.4.2/kittycad/models/unit_angular_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_area_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_area_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_area_format import UnitAreaFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitAreaConversion")
+Z = TypeVar("Z", bound="UnitAreaConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitAreaConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitAreaFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_area_format.py` & `kittycad-0.4.2/kittycad/models/unit_area_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_charge_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_charge_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_charge_format import UnitChargeFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="UnitChargeConversion")
+G = TypeVar("G", bound="UnitChargeConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitChargeConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitChargeFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_concentration_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_concentration_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_concentration_format import UnitConcentrationFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitConcentrationConversion")
+L = TypeVar("L", bound="UnitConcentrationConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitConcentrationConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitConcentrationFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_concentration_format.py` & `kittycad-0.4.2/kittycad/models/unit_concentration_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_data_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_data_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_data_format import UnitDataFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Z = TypeVar("Z", bound="UnitDataConversion")
+N = TypeVar("N", bound="UnitDataConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitDataConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Z], src_dict: Dict[str, Any]) -> Z:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitDataFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_data_format.py` & `kittycad-0.4.2/kittycad/models/unit_data_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_data_transfer_rate_format import UnitDataTransferRateFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-G = TypeVar("G", bound="UnitDataTransferRateConversion")
+N = TypeVar("N", bound="UnitDataTransferRateConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitDataTransferRateConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[G], src_dict: Dict[str, Any]) -> G:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitDataTransferRateFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_data_transfer_rate_format.py` & `kittycad-0.4.2/kittycad/models/unit_data_transfer_rate_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_density_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_density_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_density_format import UnitDensityFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="UnitDensityConversion")
+H = TypeVar("H", bound="UnitDensityConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitDensityConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitDensityFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_density_format.py` & `kittycad-0.4.2/kittycad/models/unit_density_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_energy_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_energy_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_energy_format import UnitEnergyFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitEnergyConversion")
+V = TypeVar("V", bound="UnitEnergyConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitEnergyConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitEnergyFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_energy_format.py` & `kittycad-0.4.2/kittycad/models/unit_energy_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_force_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_illuminance_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_force_format import UnitForceFormat
+from ..models.unit_illuminance_format import UnitIlluminanceFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UnitForceConversion")
+T = TypeVar("T", bound="UnitIlluminanceConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitForceConversion:
+class UnitIlluminanceConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitForceFormat] = UNSET
-    src_format: Union[Unset, UnitForceFormat] = UNSET
+    output_format: Union[Unset, UnitIlluminanceFormat] = UNSET
+    src_format: Union[Unset, UnitIlluminanceFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitForceFormat]
+        output_format: Union[Unset, UnitIlluminanceFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitForceFormat(_output_format)
+            output_format = UnitIlluminanceFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitForceFormat]
+        src_format: Union[Unset, UnitIlluminanceFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitForceFormat(_src_format)
+            src_format = UnitIlluminanceFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_force_conversion = cls(
+        unit_illuminance_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_force_conversion.additional_properties = d
-        return unit_force_conversion
+        unit_illuminance_conversion.additional_properties = d
+        return unit_illuminance_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_force_format.py` & `kittycad-0.4.2/kittycad/models/unit_force_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_illuminance_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_time_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_illuminance_format import UnitIlluminanceFormat
+from ..models.unit_time_format import UnitTimeFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="UnitIlluminanceConversion")
+K = TypeVar("K", bound="UnitTimeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitIlluminanceConversion:
+class UnitTimeConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitIlluminanceFormat] = UNSET
-    src_format: Union[Unset, UnitIlluminanceFormat] = UNSET
+    output_format: Union[Unset, UnitTimeFormat] = UNSET
+    src_format: Union[Unset, UnitTimeFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitIlluminanceFormat]
+        output_format: Union[Unset, UnitTimeFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitIlluminanceFormat(_output_format)
+            output_format = UnitTimeFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitIlluminanceFormat]
+        src_format: Union[Unset, UnitTimeFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitIlluminanceFormat(_src_format)
+            src_format = UnitTimeFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_illuminance_conversion = cls(
+        unit_time_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_illuminance_conversion.additional_properties = d
-        return unit_illuminance_conversion
+        unit_time_conversion.additional_properties = d
+        return unit_time_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_illuminance_format.py` & `kittycad-0.4.2/kittycad/models/unit_illuminance_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_length_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_length_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_length_format import UnitLengthFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="UnitLengthConversion")
+Q = TypeVar("Q", bound="UnitLengthConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitLengthConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitLengthFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_length_format.py` & `kittycad-0.4.2/kittycad/models/unit_length_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_magnetic_field_strength_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_magnetic_field_strength_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_magnetic_field_strength_format import UnitMagneticFieldStrengthFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-E = TypeVar("E", bound="UnitMagneticFieldStrengthConversion")
+F = TypeVar("F", bound="UnitMagneticFieldStrengthConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitMagneticFieldStrengthConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitMagneticFieldStrengthFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_magnetic_flux_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_metric_power_cubed_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_magnetic_flux_format import UnitMagneticFluxFormat
+from ..models.unit_metric_power import UnitMetricPower
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UnitMagneticFluxConversion")
+V = TypeVar("V", bound="UnitMetricPowerCubedConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMagneticFluxConversion:
+class UnitMetricPowerCubedConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
-    src_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
+    output_format: Union[Unset, UnitMetricPower] = UNSET
+    src_format: Union[Unset, UnitMetricPower] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitMagneticFluxFormat]
+        output_format: Union[Unset, UnitMetricPower]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitMagneticFluxFormat(_output_format)
+            output_format = UnitMetricPower(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitMagneticFluxFormat]
+        src_format: Union[Unset, UnitMetricPower]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitMagneticFluxFormat(_src_format)
+            src_format = UnitMetricPower(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_magnetic_flux_conversion = cls(
+        unit_metric_power_cubed_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_magnetic_flux_conversion.additional_properties = d
-        return unit_magnetic_flux_conversion
+        unit_metric_power_cubed_conversion.additional_properties = d
+        return unit_metric_power_cubed_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_mass_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_mass_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_mass_format import UnitMassFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Q = TypeVar("Q", bound="UnitMassConversion")
+J = TypeVar("J", bound="UnitMassConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitMassConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Q], src_dict: Dict[str, Any]) -> Q:
+    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitMassFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_mass_format.py` & `kittycad-0.4.2/kittycad/models/unit_mass_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_metric_power.py` & `kittycad-0.4.2/kittycad/models/unit_metric_power.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_metric_power_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_metric_power_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_metric_power import UnitMetricPower
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 F = TypeVar("F", bound="UnitMetricPowerConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitMetricPowerConversion:
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitMetricPower]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_metric_power_cubed_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_metric_power_squared_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_metric_power import UnitMetricPower
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-D = TypeVar("D", bound="UnitMetricPowerCubedConversion")
+U = TypeVar("U", bound="UnitMetricPowerSquaredConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMetricPowerCubedConversion:
+class UnitMetricPowerSquaredConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
+    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitMetricPower]
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_metric_power_cubed_conversion = cls(
+        unit_metric_power_squared_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_metric_power_cubed_conversion.additional_properties = d
-        return unit_metric_power_cubed_conversion
+        unit_metric_power_squared_conversion.additional_properties = d
+        return unit_metric_power_squared_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_metric_power_squared_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_radioactivity_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_metric_power import UnitMetricPower
+from ..models.unit_radioactivity_format import UnitRadioactivityFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-J = TypeVar("J", bound="UnitMetricPowerSquaredConversion")
+P = TypeVar("P", bound="UnitRadioactivityConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitMetricPowerSquaredConversion:
+class UnitRadioactivityConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitMetricPower] = UNSET
-    src_format: Union[Unset, UnitMetricPower] = UNSET
+    output_format: Union[Unset, UnitRadioactivityFormat] = UNSET
+    src_format: Union[Unset, UnitRadioactivityFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[J], src_dict: Dict[str, Any]) -> J:
+    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitMetricPower]
+        output_format: Union[Unset, UnitRadioactivityFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitMetricPower(_output_format)
+            output_format = UnitRadioactivityFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitMetricPower]
+        src_format: Union[Unset, UnitRadioactivityFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitMetricPower(_src_format)
+            src_format = UnitRadioactivityFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_metric_power_squared_conversion = cls(
+        unit_radioactivity_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_metric_power_squared_conversion.additional_properties = d
-        return unit_metric_power_squared_conversion
+        unit_radioactivity_conversion.additional_properties = d
+        return unit_radioactivity_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_power_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_volume_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_power_format import UnitPowerFormat
+from ..models.unit_volume_format import UnitVolumeFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitPowerConversion")
+A = TypeVar("A", bound="UnitVolumeConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitPowerConversion:
+class UnitVolumeConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitPowerFormat] = UNSET
-    src_format: Union[Unset, UnitPowerFormat] = UNSET
+    output_format: Union[Unset, UnitVolumeFormat] = UNSET
+    src_format: Union[Unset, UnitVolumeFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitPowerFormat]
+        output_format: Union[Unset, UnitVolumeFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitPowerFormat(_output_format)
+            output_format = UnitVolumeFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitPowerFormat]
+        src_format: Union[Unset, UnitVolumeFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitPowerFormat(_src_format)
+            src_format = UnitVolumeFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_power_conversion = cls(
+        unit_volume_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_power_conversion.additional_properties = d
-        return unit_power_conversion
+        unit_volume_conversion.additional_properties = d
+        return unit_volume_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_pressure_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_pressure_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_pressure_format import UnitPressureFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-V = TypeVar("V", bound="UnitPressureConversion")
+Y = TypeVar("Y", bound="UnitPressureConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitPressureConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[V], src_dict: Dict[str, Any]) -> V:
+    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitPressureFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_pressure_format.py` & `kittycad-0.4.2/kittycad/models/unit_pressure_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_radiation_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_radiation_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_radiation_format import UnitRadiationFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-U = TypeVar("U", bound="UnitRadiationConversion")
+F = TypeVar("F", bound="UnitRadiationConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitRadiationConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[U], src_dict: Dict[str, Any]) -> U:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitRadiationFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_radiation_format.py` & `kittycad-0.4.2/kittycad/models/unit_radiation_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_radioactivity_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_temperature_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_radioactivity_format import UnitRadioactivityFormat
+from ..models.unit_temperature_format import UnitTemperatureFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitRadioactivityConversion")
+L = TypeVar("L", bound="UnitTemperatureConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitRadioactivityConversion:
+class UnitTemperatureConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitRadioactivityFormat] = UNSET
-    src_format: Union[Unset, UnitRadioactivityFormat] = UNSET
+    output_format: Union[Unset, UnitTemperatureFormat] = UNSET
+    src_format: Union[Unset, UnitTemperatureFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitRadioactivityFormat]
+        output_format: Union[Unset, UnitTemperatureFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitRadioactivityFormat(_output_format)
+            output_format = UnitTemperatureFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitRadioactivityFormat]
+        src_format: Union[Unset, UnitTemperatureFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitRadioactivityFormat(_src_format)
+            src_format = UnitTemperatureFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_radioactivity_conversion = cls(
+        unit_temperature_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_radioactivity_conversion.additional_properties = d
-        return unit_radioactivity_conversion
+        unit_temperature_conversion.additional_properties = d
+        return unit_temperature_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_radioactivity_format.py` & `kittycad-0.4.2/kittycad/models/unit_radioactivity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_solid_angle_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_solid_angle_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_solid_angle_format import UnitSolidAngleFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
 Y = TypeVar("Y", bound="UnitSolidAngleConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitSolidAngleConversion:
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitSolidAngleFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_temperature_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_force_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_temperature_format import UnitTemperatureFormat
+from ..models.unit_force_format import UnitForceFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-F = TypeVar("F", bound="UnitTemperatureConversion")
+E = TypeVar("E", bound="UnitForceConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitTemperatureConversion:
+class UnitForceConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitTemperatureFormat] = UNSET
-    src_format: Union[Unset, UnitTemperatureFormat] = UNSET
+    output_format: Union[Unset, UnitForceFormat] = UNSET
+    src_format: Union[Unset, UnitForceFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
+    def from_dict(cls: Type[E], src_dict: Dict[str, Any]) -> E:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitTemperatureFormat]
+        output_format: Union[Unset, UnitForceFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitTemperatureFormat(_output_format)
+            output_format = UnitForceFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitTemperatureFormat]
+        src_format: Union[Unset, UnitForceFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitTemperatureFormat(_src_format)
+            src_format = UnitForceFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_temperature_conversion = cls(
+        unit_force_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_temperature_conversion.additional_properties = d
-        return unit_temperature_conversion
+        unit_force_conversion.additional_properties = d
+        return unit_force_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_temperature_format.py` & `kittycad-0.4.2/kittycad/models/unit_temperature_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_time_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_velocity_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_time_format import UnitTimeFormat
+from ..models.unit_velocity_format import UnitVelocityFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-P = TypeVar("P", bound="UnitTimeConversion")
+N = TypeVar("N", bound="UnitVelocityConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitTimeConversion:
+class UnitVelocityConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitTimeFormat] = UNSET
-    src_format: Union[Unset, UnitTimeFormat] = UNSET
+    output_format: Union[Unset, UnitVelocityFormat] = UNSET
+    src_format: Union[Unset, UnitVelocityFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[P], src_dict: Dict[str, Any]) -> P:
+    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitTimeFormat]
+        output_format: Union[Unset, UnitVelocityFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitTimeFormat(_output_format)
+            output_format = UnitVelocityFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitTimeFormat]
+        src_format: Union[Unset, UnitVelocityFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitTimeFormat(_src_format)
+            src_format = UnitVelocityFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_time_conversion = cls(
+        unit_velocity_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_time_conversion.additional_properties = d
-        return unit_time_conversion
+        unit_velocity_conversion.additional_properties = d
+        return unit_velocity_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_time_format.py` & `kittycad-0.4.2/kittycad/models/unit_time_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_velocity_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_magnetic_flux_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_velocity_format import UnitVelocityFormat
+from ..models.unit_magnetic_flux_format import UnitMagneticFluxFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-Y = TypeVar("Y", bound="UnitVelocityConversion")
+D = TypeVar("D", bound="UnitMagneticFluxConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitVelocityConversion:
+class UnitMagneticFluxConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitVelocityFormat] = UNSET
-    src_format: Union[Unset, UnitVelocityFormat] = UNSET
+    output_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
+    src_format: Union[Unset, UnitMagneticFluxFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[Y], src_dict: Dict[str, Any]) -> Y:
+    def from_dict(cls: Type[D], src_dict: Dict[str, Any]) -> D:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitVelocityFormat]
+        output_format: Union[Unset, UnitMagneticFluxFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitVelocityFormat(_output_format)
+            output_format = UnitMagneticFluxFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitVelocityFormat]
+        src_format: Union[Unset, UnitMagneticFluxFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitVelocityFormat(_src_format)
+            src_format = UnitMagneticFluxFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_velocity_conversion = cls(
+        unit_magnetic_flux_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_velocity_conversion.additional_properties = d
-        return unit_velocity_conversion
+        unit_magnetic_flux_conversion.additional_properties = d
+        return unit_magnetic_flux_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_velocity_format.py` & `kittycad-0.4.2/kittycad/models/unit_velocity_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/unit_voltage_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_voltage_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
 from ..models.unit_voltage_format import UnitVoltageFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-L = TypeVar("L", bound="UnitVoltageConversion")
+H = TypeVar("H", bound="UnitVoltageConversion")
 
 
 @attr.s(auto_attribs=True)
 class UnitVoltageConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[L], src_dict: Dict[str, Any]) -> L:
+    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,15 +101,20 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
         output_format: Union[Unset, UnitVoltageFormat]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_volume_conversion.py` & `kittycad-0.4.2/kittycad/models/unit_power_conversion.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.api_call_status import ApiCallStatus
-from ..models.unit_volume_format import UnitVolumeFormat
+from ..models.unit_power_format import UnitPowerFormat
+from ..models.uuid import Uuid
 from ..types import UNSET, Unset
 
-K = TypeVar("K", bound="UnitVolumeConversion")
+F = TypeVar("F", bound="UnitPowerConversion")
 
 
 @attr.s(auto_attribs=True)
-class UnitVolumeConversion:
+class UnitPowerConversion:
     """A unit conversion."""  # noqa: E501
 
     completed_at: Union[Unset, datetime.datetime] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     error: Union[Unset, str] = UNSET
     id: Union[Unset, str] = UNSET
     input: Union[Unset, float] = UNSET
     output: Union[Unset, float] = UNSET
-    output_format: Union[Unset, UnitVolumeFormat] = UNSET
-    src_format: Union[Unset, UnitVolumeFormat] = UNSET
+    output_format: Union[Unset, UnitPowerFormat] = UNSET
+    src_format: Union[Unset, UnitPowerFormat] = UNSET
     started_at: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, ApiCallStatus] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
     user_id: Union[Unset, str] = UNSET
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -82,15 +83,15 @@
             field_dict["updated_at"] = updated_at
         if user_id is not UNSET:
             field_dict["user_id"] = user_id
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
+    def from_dict(cls: Type[F], src_dict: Dict[str, Any]) -> F:
         d = src_dict.copy()
         _completed_at = d.pop("completed_at", UNSET)
         completed_at: Union[Unset, datetime.datetime]
         if isinstance(_completed_at, Unset):
             completed_at = UNSET
         else:
             completed_at = isoparse(_completed_at)
@@ -100,33 +101,38 @@
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         error = d.pop("error", UNSET)
 
-        id = d.pop("id", UNSET)
+        _id = d.pop("id", UNSET)
+        id: Union[Unset, Uuid]
+        if isinstance(_id, Unset):
+            id = UNSET
+        else:
+            id = Uuid(_id)
 
         input = d.pop("input", UNSET)
 
         output = d.pop("output", UNSET)
 
         _output_format = d.pop("output_format", UNSET)
-        output_format: Union[Unset, UnitVolumeFormat]
+        output_format: Union[Unset, UnitPowerFormat]
         if isinstance(_output_format, Unset):
             output_format = UNSET
         else:
-            output_format = UnitVolumeFormat(_output_format)
+            output_format = UnitPowerFormat(_output_format)
 
         _src_format = d.pop("src_format", UNSET)
-        src_format: Union[Unset, UnitVolumeFormat]
+        src_format: Union[Unset, UnitPowerFormat]
         if isinstance(_src_format, Unset):
             src_format = UNSET
         else:
-            src_format = UnitVolumeFormat(_src_format)
+            src_format = UnitPowerFormat(_src_format)
 
         _started_at = d.pop("started_at", UNSET)
         started_at: Union[Unset, datetime.datetime]
         if isinstance(_started_at, Unset):
             started_at = UNSET
         else:
             started_at = isoparse(_started_at)
@@ -143,31 +149,31 @@
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user_id = d.pop("user_id", UNSET)
 
-        unit_volume_conversion = cls(
+        unit_power_conversion = cls(
             completed_at=completed_at,
             created_at=created_at,
             error=error,
             id=id,
             input=input,
             output=output,
             output_format=output_format,
             src_format=src_format,
             started_at=started_at,
             status=status,
             updated_at=updated_at,
             user_id=user_id,
         )
 
-        unit_volume_conversion.additional_properties = d
-        return unit_volume_conversion
+        unit_power_conversion.additional_properties = d
+        return unit_power_conversion
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `kittycad-0.4.1/kittycad/models/unit_volume_format.py` & `kittycad-0.4.2/kittycad/models/unit_volume_format.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/kittycad/models/update_user.py` & `kittycad-0.4.2/kittycad/models/update_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-N = TypeVar("N", bound="UpdateUser")
+R = TypeVar("R", bound="UpdateUser")
 
 
 @attr.s(auto_attribs=True)
 class UpdateUser:
     """The user-modifiable parts of a User."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -43,15 +43,15 @@
             field_dict["last_name"] = last_name
         if phone is not UNSET:
             field_dict["phone"] = phone
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[N], src_dict: Dict[str, Any]) -> N:
+    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         discord = d.pop("discord", UNSET)
 
         first_name = d.pop("first_name", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/user.py` & `kittycad-0.4.2/kittycad/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-H = TypeVar("H", bound="User")
+W = TypeVar("W", bound="User")
 
 
 @attr.s(auto_attribs=True)
 class User:
     """A user."""  # noqa: E501
 
     company: Union[Unset, str] = UNSET
@@ -79,15 +79,15 @@
             field_dict["phone"] = phone
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[H], src_dict: Dict[str, Any]) -> H:
+    def from_dict(cls: Type[W], src_dict: Dict[str, Any]) -> W:
         d = src_dict.copy()
         company = d.pop("company", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
```

### Comparing `kittycad-0.4.1/kittycad/models/user_results_page.py` & `kittycad-0.4.2/kittycad/models/user_results_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
-A = TypeVar("A", bound="UserResultsPage")
+B = TypeVar("B", bound="UserResultsPage")
 
 
 @attr.s(auto_attribs=True)
 class UserResultsPage:
     """A single page of results"""  # noqa: E501
 
     from ..models.user import User
@@ -33,15 +33,15 @@
             field_dict["items"] = items
         if next_page is not UNSET:
             field_dict["next_page"] = next_page
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[A], src_dict: Dict[str, Any]) -> A:
+    def from_dict(cls: Type[B], src_dict: Dict[str, Any]) -> B:
         d = src_dict.copy()
         from ..models.user import User
 
         items = cast(List[User], d.pop("items", UNSET))
 
         next_page = d.pop("next_page", UNSET)
```

### Comparing `kittycad-0.4.1/kittycad/models/verification_token.py` & `kittycad-0.4.2/kittycad/models/verification_token.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-R = TypeVar("R", bound="VerificationToken")
+K = TypeVar("K", bound="VerificationToken")
 
 
 @attr.s(auto_attribs=True)
 class VerificationToken:
     """A verification token for a user.
 
     This is typically used to verify a user's email address."""  # noqa: E501
@@ -49,15 +49,15 @@
             field_dict["identifier"] = identifier
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
-    def from_dict(cls: Type[R], src_dict: Dict[str, Any]) -> R:
+    def from_dict(cls: Type[K], src_dict: Dict[str, Any]) -> K:
         d = src_dict.copy()
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
```

### Comparing `kittycad-0.4.1/kittycad/types.py` & `kittycad-0.4.2/kittycad/types.py`

 * *Files identical despite different names*

### Comparing `kittycad-0.4.1/pyproject.toml` & `kittycad-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kittycad"
-version = "0.4.1"
+version = "0.4.2"
 description = "A client library for accessing KittyCAD"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "kittycad"},
@@ -26,15 +26,15 @@
 openapi-parser = "^0.2.6"
 openapi-spec-validator = "^0.5.6"
 prance = "^0.22.11"
 pyenchant = "^3.2.2"
 pytest = "^7.0.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.265"
+ruff = "^0.0.269"
 Sphinx = "^6.2.1"
 sphinx-autoapi = "^2.0.1"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-spelling = "^8.0.0"
 sphinx-copybutton = "^0.5.2"
 sphinxext-opengraph = "^0.8.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `kittycad-0.4.1/PKG-INFO` & `kittycad-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kittycad
-Version: 0.4.1
+Version: 0.4.2
 Summary: A client library for accessing KittyCAD
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

