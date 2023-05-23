# Comparing `tmp/woke-3.4.1.tar.gz` & `tmp/woke-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woke-3.4.1.tar", max compression
+gzip compressed data, was "woke-3.4.2.tar", max compression
```

## Comparing `woke-3.4.1.tar` & `woke-3.4.2.tar`

### file list

```diff
@@ -1,240 +1,240 @@
--rw-r--r--   0        0        0      751 2023-05-12 17:51:48.462949 woke-3.4.1/LICENSE
--rw-r--r--   0        0        0     3415 2023-05-12 17:51:48.462949 woke-3.4.1/README.md
--rw-r--r--   0        0        0     2720 2023-05-12 19:49:40.584205 woke-3.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.492949 woke-3.4.1/woke/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/__init__.py
--rw-r--r--   0        0        0    20473 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/cfg.py
--rw-r--r--   0        0        0     1013 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/__init__.py
--rw-r--r--   0        0        0    21743 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/api.py
--rw-r--r--   0        0        0       61 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/axelar/__init__.py
--rw-r--r--   0        0        0    15183 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/axelar/proxy_contract_id.py
--rw-r--r--   0        0        0     6389 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/balance_state_var.py
--rw-r--r--   0        0        0     4759 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/bug_empty_byte_array_copy.py
--rw-r--r--   0        0        0     1777 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/call_options_not_called.py
--rw-r--r--   0        0        0     4162 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/missing_return.py
--rw-r--r--   0        0        0     3013 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/msg_value_nonpayable_function.py
--rw-r--r--   0        0        0     8723 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
--rw-r--r--   0        0        0    17299 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/ownable.py
--rw-r--r--   0        0        0    23312 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/proxy_contract_selector_clashes.py
--rw-r--r--   0        0        0    13982 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/reentrancy.py
--rw-r--r--   0        0        0     2766 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/unchecked_return_value.py
--rw-r--r--   0        0        0     6242 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/unsafe_delegatecall.py
--rw-r--r--   0        0        0     1344 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/unsafe_selfdestruct.py
--rw-r--r--   0        0        0     5982 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/unsafe_tx_origin.py
--rw-r--r--   0        0        0     1397 2023-05-12 18:46:14.658233 woke-3.4.1/woke/analysis/detectors/unused_contract.py
--rw-r--r--   0        0        0    12233 2023-05-12 17:51:48.496283 woke-3.4.1/woke/analysis/detectors/utils.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/__init__.py
--rw-r--r--   0        0        0    10947 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/enums.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/__init__.py
--rw-r--r--   0        0        0     5941 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/abc.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/__init__.py
--rw-r--r--   0        0        0     5854 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/abc.py
--rw-r--r--   0        0        0    16974 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/contract_definition.py
--rw-r--r--   0        0        0     3079 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/enum_definition.py
--rw-r--r--   0        0        0     1361 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/enum_value.py
--rw-r--r--   0        0        0     4408 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/error_definition.py
--rw-r--r--   0        0        0     5162 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/event_definition.py
--rw-r--r--   0        0        0    18683 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/function_definition.py
--rw-r--r--   0        0        0    12891 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/modifier_definition.py
--rw-r--r--   0        0        0     3414 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/struct_definition.py
--rw-r--r--   0        0        0     2654 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/user_defined_value_type_definition.py
--rw-r--r--   0        0        0    19473 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/declaration/variable_declaration.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/__init__.py
--rw-r--r--   0        0        0     6583 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/abc.py
--rw-r--r--   0        0        0     4063 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/assignment.py
--rw-r--r--   0        0        0     2959 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/binary_operation.py
--rw-r--r--   0        0        0     2087 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/conditional.py
--rw-r--r--   0        0        0     1361 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/elementary_type_name_expression.py
--rw-r--r--   0        0        0     8933 2023-05-12 17:51:48.496283 woke-3.4.1/woke/ast/ir/expression/function_call.py
--rw-r--r--   0        0        0     2142 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/function_call_options.py
--rw-r--r--   0        0        0     5709 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/identifier.py
--rw-r--r--   0        0        0     1996 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/index_access.py
--rw-r--r--   0        0        0     2661 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/index_range_access.py
--rw-r--r--   0        0        0     1437 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/literal.py
--rw-r--r--   0        0        0    19431 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/member_access.py
--rw-r--r--   0        0        0     1376 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/new_expression.py
--rw-r--r--   0        0        0     2191 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/tuple_expression.py
--rw-r--r--   0        0        0     3071 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/expression/unary_operation.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/__init__.py
--rw-r--r--   0        0        0    10965 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/identifier_path.py
--rw-r--r--   0        0        0     8998 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/import_directive.py
--rw-r--r--   0        0        0     3752 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/inheritance_specifier.py
--rw-r--r--   0        0        0     5700 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/modifier_invocation.py
--rw-r--r--   0        0        0     3462 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/override_specifier.py
--rw-r--r--   0        0        0     4311 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/parameter_list.py
--rw-r--r--   0        0        0     1534 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/pragma_directive.py
--rw-r--r--   0        0        0     9307 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/source_unit.py
--rw-r--r--   0        0        0     2315 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/structured_documentation.py
--rw-r--r--   0        0        0     4541 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/try_catch_clause.py
--rw-r--r--   0        0        0     5698 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/meta/using_for_directive.py
--rw-r--r--   0        0        0     4812 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/reference_resolver.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/__init__.py
--rw-r--r--   0        0        0     5608 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/abc.py
--rw-r--r--   0        0        0     3135 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/block.py
--rw-r--r--   0        0        0     1611 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/break_statement.py
--rw-r--r--   0        0        0     1635 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/continue_statement.py
--rw-r--r--   0        0        0     2563 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/do_while_statement.py
--rw-r--r--   0        0        0     2452 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/emit_statement.py
--rw-r--r--   0        0        0     6016 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/expression_statement.py
--rw-r--r--   0        0        0     5735 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/for_statement.py
--rw-r--r--   0        0        0     3423 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/if_statement.py
--rw-r--r--   0        0        0    10276 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/inline_assembly.py
--rw-r--r--   0        0        0     1583 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/placeholder_statement.py
--rw-r--r--   0        0        0     3336 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/return_statement.py
--rw-r--r--   0        0        0     2608 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/revert_statement.py
--rw-r--r--   0        0        0     3134 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/try_statement.py
--rw-r--r--   0        0        0     2454 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/unchecked_block.py
--rw-r--r--   0        0        0     4330 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/variable_declaration_statement.py
--rw-r--r--   0        0        0     2596 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/statement/while_statement.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/__init__.py
--rw-r--r--   0        0        0     4932 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/abc.py
--rw-r--r--   0        0        0     4092 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/array_type_name.py
--rw-r--r--   0        0        0     5967 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/elementary_type_name.py
--rw-r--r--   0        0        0     3987 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/function_type_name.py
--rw-r--r--   0        0        0     3938 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/mapping.py
--rw-r--r--   0        0        0    11314 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/type_name/user_defined_type_name.py
--rw-r--r--   0        0        0       36 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/utils/__init__.py
--rw-r--r--   0        0        0      589 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/utils/init_tuple.py
--rw-r--r--   0        0        0      578 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/yul/__init__.py
--rw-r--r--   0        0        0      705 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/yul/abc.py
--rw-r--r--   0        0        0     1817 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/yul/assignment.py
--rw-r--r--   0        0        0     4317 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/yul/block.py
--rw-r--r--   0        0        0      301 2023-05-12 17:51:48.499616 woke-3.4.1/woke/ast/ir/yul/break_statement.py
--rw-r--r--   0        0        0     1200 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/case_statement.py
--rw-r--r--   0        0        0      304 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/continue_statement.py
--rw-r--r--   0        0        0     1659 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/expression_statement.py
--rw-r--r--   0        0        0     1893 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/for_loop.py
--rw-r--r--   0        0        0     2323 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/function_call.py
--rw-r--r--   0        0        0     2298 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/function_definition.py
--rw-r--r--   0        0        0     1492 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/identifier.py
--rw-r--r--   0        0        0     1582 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/if_statement.py
--rw-r--r--   0        0        0      301 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/leave.py
--rw-r--r--   0        0        0     1781 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/literal.py
--rw-r--r--   0        0        0     1802 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/switch.py
--rw-r--r--   0        0        0      921 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/typed_name.py
--rw-r--r--   0        0        0     2097 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/ir/yul/variable_declaration.py
--rw-r--r--   0        0        0    37866 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/nodes.py
--rw-r--r--   0        0        0    47087 2023-05-12 17:51:48.502949 woke-3.4.1/woke/ast/types.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/__init__.py
--rw-r--r--   0        0        0     3501 2023-05-12 19:05:20.623625 woke-3.4.1/woke/cli/__main__.py
--rw-r--r--   0        0        0     7942 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/accounts.py
--rw-r--r--   0        0        0     4650 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/compile.py
--rw-r--r--   0        0        0       54 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/console.py
--rw-r--r--   0        0        0     3838 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/detect.py
--rw-r--r--   0        0        0     3791 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/fuzz.py
--rw-r--r--   0        0        0    11813 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/init.py
--rw-r--r--   0        0        0     1081 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/lsp.py
--rw-r--r--   0        0        0     3154 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/run.py
--rw-r--r--   0        0        0     4922 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/svm.py
--rw-r--r--   0        0        0     2258 2023-05-12 17:51:48.502949 woke-3.4.1/woke/cli/test.py
--rw-r--r--   0        0        0      187 2023-05-12 17:51:48.502949 woke-3.4.1/woke/compiler/__init__.py
--rw-r--r--   0        0        0     1814 2023-05-12 17:51:48.502949 woke-3.4.1/woke/compiler/build_data_model.py
--rw-r--r--   0        0        0     3120 2023-05-12 17:51:48.502949 woke-3.4.1/woke/compiler/compilation_unit.py
--rw-r--r--   0        0        0    41479 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/compiler.py
--rw-r--r--   0        0        0       97 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/exceptions.py
--rw-r--r--   0        0        0      103 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/solc_frontend/__init__.py
--rw-r--r--   0        0        0       48 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/solc_frontend/exceptions.py
--rw-r--r--   0        0        0     8554 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/solc_frontend/input_data_model.py
--rw-r--r--   0        0        0     8728 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/solc_frontend/output_data_model.py
--rw-r--r--   0        0        0     3571 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/solc_frontend/solc_runner.py
--rw-r--r--   0        0        0     2455 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/source_path_resolver.py
--rw-r--r--   0        0        0     4813 2023-05-12 17:51:48.506283 woke-3.4.1/woke/compiler/source_unit_name_resolver.py
--rw-r--r--   0        0        0     1118 2023-05-12 17:51:48.506283 woke-3.4.1/woke/config/__init__.py
--rw-r--r--   0        0        0     6912 2023-05-12 17:51:48.506283 woke-3.4.1/woke/config/data_model.py
--rw-r--r--   0        0        0    12682 2023-05-12 17:51:48.506283 woke-3.4.1/woke/config/woke_config.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.506283 woke-3.4.1/woke/contracts/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.506283 woke-3.4.1/woke/contracts/woke/__init__.py
--rw-r--r--   0        0        0    64087 2023-05-12 17:51:48.506283 woke-3.4.1/woke/contracts/woke/console.sol
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.506283 woke-3.4.1/woke/core/__init__.py
--rw-r--r--   0        0        0      386 2023-05-12 17:51:48.506283 woke-3.4.1/woke/core/enums.py
--rw-r--r--   0        0        0    24829 2023-05-12 17:51:48.506283 woke-3.4.1/woke/core/solidity_version.py
--rw-r--r--   0        0        0      678 2023-05-12 17:51:48.506283 woke-3.4.1/woke/deployment/__init__.py
--rw-r--r--   0        0        0    14848 2023-05-12 17:51:48.506283 woke-3.4.1/woke/deployment/core.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/__init__.py
--rw-r--r--   0        0        0     4552 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/blocks.py
--rw-r--r--   0        0        0    28963 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/call_trace.py
--rw-r--r--   0        0        0    25863 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/chain_interfaces.py
--rw-r--r--   0        0        0     1132 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/constants.py
--rw-r--r--   0        0        0    96257 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/core.py
--rw-r--r--   0        0        0     7270 2023-05-12 17:51:48.506283 woke-3.4.1/woke/development/globals.py
--rw-r--r--   0        0        0   161115 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/hardhat_console.py
--rw-r--r--   0        0        0     1093 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/internal.py
--rw-r--r--   0        0        0       39 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/json_rpc/__init__.py
--rw-r--r--   0        0        0      302 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/json_rpc/abc.py
--rw-r--r--   0        0        0     2070 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/json_rpc/communicator.py
--rw-r--r--   0        0        0      821 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/json_rpc/http.py
--rw-r--r--   0        0        0     2912 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/json_rpc/ipc.py
--rw-r--r--   0        0        0      625 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/json_rpc/websocket.py
--rw-r--r--   0        0        0     6572 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/primitive_types.py
--rw-r--r--   0        0        0    90006 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/pytypes_generator.py
--rw-r--r--   0        0        0    28061 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/transactions.py
--rw-r--r--   0        0        0     7389 2023-05-12 17:51:48.509616 woke-3.4.1/woke/development/utils.py
--rw-r--r--   0        0        0       47 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/__init__.py
--rw-r--r--   0        0        0      310 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/commands/__init__.py
--rw-r--r--   0        0        0     4033 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/commands/generate_control_flow_graph.py
--rw-r--r--   0        0        0     1097 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/commands/generate_imports_graph.py
--rw-r--r--   0        0        0     4247 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/commands/generate_inheritance_graph.py
--rw-r--r--   0        0        0     2163 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/commands/generate_linearized_inheritance_graph.py
--rw-r--r--   0        0        0    31491 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/common_structures.py
--rw-r--r--   0        0        0     1900 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/context.py
--rw-r--r--   0        0        0     2574 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/document_sync.py
--rw-r--r--   0        0        0      130 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/enums.py
--rw-r--r--   0        0        0      471 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/features/__init__.py
--rw-r--r--   0        0        0     6969 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/features/code_action.py
--rw-r--r--   0        0        0    10904 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/features/code_lens.py
--rw-r--r--   0        0        0    19824 2023-05-12 17:51:48.509616 woke-3.4.1/woke/lsp/features/completion.py
--rw-r--r--   0        0        0     9948 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/definition.py
--rw-r--r--   0        0        0     1446 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/diagnostic.py
--rw-r--r--   0        0        0     4305 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/document_link.py
--rw-r--r--   0        0        0     8407 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/document_symbol.py
--rw-r--r--   0        0        0    17901 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/hover.py
--rw-r--r--   0        0        0     3850 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/implementation.py
--rw-r--r--   0        0        0     5092 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/references.py
--rw-r--r--   0        0        0     8935 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/rename.py
--rw-r--r--   0        0        0     9505 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/type_definition.py
--rw-r--r--   0        0        0    11043 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/features/type_hierarchy.py
--rw-r--r--   0        0        0    39957 2023-05-12 19:49:18.774669 woke-3.4.1/woke/lsp/lsp_compiler.py
--rw-r--r--   0        0        0      328 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/lsp_data_model.py
--rw-r--r--   0        0        0     8941 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/lsp_parser.py
--rw-r--r--   0        0        0     5551 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/methods.py
--rw-r--r--   0        0        0     1897 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/protocol_structures.py
--rw-r--r--   0        0        0     2229 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/rpc_protocol.py
--rw-r--r--   0        0        0    37738 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/server.py
--rw-r--r--   0        0        0     6597 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/server_capabilities.py
--rw-r--r--   0        0        0       86 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/utils/__init__.py
--rw-r--r--   0        0        0     1021 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/utils/position.py
--rw-r--r--   0        0        0      459 2023-05-12 17:51:48.512949 woke-3.4.1/woke/lsp/utils/uri.py
--rw-r--r--   0        0        0       50 2023-05-12 17:51:48.512949 woke-3.4.1/woke/regex_parser/__init__.py
--rw-r--r--   0        0        0     1690 2023-05-12 17:51:48.512949 woke-3.4.1/woke/regex_parser/solidity_import.py
--rw-r--r--   0        0        0     6653 2023-05-12 17:51:48.512949 woke-3.4.1/woke/regex_parser/solidity_parser.py
--rw-r--r--   0        0        0       36 2023-05-12 17:51:48.512949 woke-3.4.1/woke/svm/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-12 17:51:48.512949 woke-3.4.1/woke/svm/abc.py
--rw-r--r--   0        0        0      270 2023-05-12 17:51:48.512949 woke-3.4.1/woke/svm/exceptions.py
--rw-r--r--   0        0        0    11721 2023-05-12 17:51:48.512949 woke-3.4.1/woke/svm/svm.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.512949 woke-3.4.1/woke/templates/scripts/__init__.py
--rw-r--r--   0        0        0      184 2023-05-12 17:51:48.512949 woke-3.4.1/woke/templates/scripts/deploy.py
--rw-r--r--   0        0        0        0 2023-05-12 17:51:48.512949 woke-3.4.1/woke/templates/tests/__init__.py
--rw-r--r--   0        0        0      140 2023-05-12 17:51:48.512949 woke-3.4.1/woke/templates/tests/test_default.py
--rw-r--r--   0        0        0      678 2023-05-12 17:51:48.512949 woke-3.4.1/woke/testing/__init__.py
--rw-r--r--   0        0        0    10878 2023-05-12 17:51:48.512949 woke-3.4.1/woke/testing/core.py
--rw-r--r--   0        0        0    24381 2023-05-12 17:51:48.512949 woke-3.4.1/woke/testing/coverage.py
--rw-r--r--   0        0        0      187 2023-05-12 17:51:48.512949 woke-3.4.1/woke/testing/fuzzing/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-12 17:51:48.512949 woke-3.4.1/woke/testing/fuzzing/fuzz_test.py
--rw-r--r--   0        0        0    10795 2023-05-12 17:51:48.516283 woke-3.4.1/woke/testing/fuzzing/fuzzer.py
--rw-r--r--   0        0        0     5780 2023-05-12 17:51:48.516283 woke-3.4.1/woke/testing/fuzzing/generators.py
--rw-r--r--   0        0        0      298 2023-05-12 17:51:48.516283 woke-3.4.1/woke/testing/pytest_plugin.py
--rw-r--r--   0        0        0      170 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/__init__.py
--rw-r--r--   0        0        0      560 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/context_managers.py
--rw-r--r--   0        0        0      515 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/decorators.py
--rw-r--r--   0        0        0      158 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/enums.py
--rw-r--r--   0        0        0     1699 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/file_utils.py
--rw-r--r--   0        0        0      384 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/keyed_default_dict.py
--rw-r--r--   0        0        0      194 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/networking.py
--rw-r--r--   0        0        0     1017 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/openzeppelin.py
--rw-r--r--   0        0        0      630 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/string.py
--rw-r--r--   0        0        0     1747 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/tee.py
--rw-r--r--   0        0        0     3765 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/threaded_child_watcher.py
--rw-r--r--   0        0        0      424 2023-05-12 17:51:48.516283 woke-3.4.1/woke/utils/version.py
--rw-r--r--   0        0        0     6129 1970-01-01 00:00:00.000000 woke-3.4.1/setup.py
--rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 woke-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0      751 2023-05-13 06:28:54.162344 woke-3.4.2/LICENSE
+-rw-r--r--   0        0        0     3415 2023-05-13 06:29:36.852316 woke-3.4.2/README.md
+-rw-r--r--   0        0        0     2720 2023-05-23 13:18:21.574662 woke-3.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.189011 woke-3.4.2/woke/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.189011 woke-3.4.2/woke/analysis/__init__.py
+-rw-r--r--   0        0        0    20473 2023-05-23 12:59:50.604420 woke-3.4.2/woke/analysis/cfg.py
+-rw-r--r--   0        0        0     1013 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/__init__.py
+-rw-r--r--   0        0        0    21743 2023-05-23 12:59:50.607753 woke-3.4.2/woke/analysis/detectors/api.py
+-rw-r--r--   0        0        0       61 2023-05-13 06:28:54.189011 woke-3.4.2/woke/analysis/detectors/axelar/__init__.py
+-rw-r--r--   0        0        0    15183 2023-05-13 06:29:36.852316 woke-3.4.2/woke/analysis/detectors/axelar/proxy_contract_id.py
+-rw-r--r--   0        0        0     6389 2023-05-13 06:29:36.852316 woke-3.4.2/woke/analysis/detectors/balance_state_var.py
+-rw-r--r--   0        0        0     4759 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/bug_empty_byte_array_copy.py
+-rw-r--r--   0        0        0     1777 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/call_options_not_called.py
+-rw-r--r--   0        0        0     4162 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/missing_return.py
+-rw-r--r--   0        0        0     3013 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/msg_value_nonpayable_function.py
+-rw-r--r--   0        0        0     8723 2023-05-13 06:29:36.852316 woke-3.4.2/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py
+-rw-r--r--   0        0        0    17299 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/ownable.py
+-rw-r--r--   0        0        0    23312 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/proxy_contract_selector_clashes.py
+-rw-r--r--   0        0        0    13982 2023-05-23 12:59:50.607753 woke-3.4.2/woke/analysis/detectors/reentrancy.py
+-rw-r--r--   0        0        0     2766 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/unchecked_return_value.py
+-rw-r--r--   0        0        0     6242 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/unsafe_delegatecall.py
+-rw-r--r--   0        0        0     1344 2023-05-22 07:04:56.893614 woke-3.4.2/woke/analysis/detectors/unsafe_selfdestruct.py
+-rw-r--r--   0        0        0     5982 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/unsafe_tx_origin.py
+-rw-r--r--   0        0        0     1397 2023-05-13 06:28:54.192344 woke-3.4.2/woke/analysis/detectors/unused_contract.py
+-rw-r--r--   0        0        0    12233 2023-05-23 12:59:50.607753 woke-3.4.2/woke/analysis/detectors/utils.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/__init__.py
+-rw-r--r--   0        0        0    10947 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/enums.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/__init__.py
+-rw-r--r--   0        0        0     5941 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/abc.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/__init__.py
+-rw-r--r--   0        0        0     5854 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/abc.py
+-rw-r--r--   0        0        0    16974 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/contract_definition.py
+-rw-r--r--   0        0        0     3079 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/enum_definition.py
+-rw-r--r--   0        0        0     1361 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/enum_value.py
+-rw-r--r--   0        0        0     4408 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/error_definition.py
+-rw-r--r--   0        0        0     5162 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/event_definition.py
+-rw-r--r--   0        0        0    18683 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/function_definition.py
+-rw-r--r--   0        0        0    12891 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/modifier_definition.py
+-rw-r--r--   0        0        0     3414 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/struct_definition.py
+-rw-r--r--   0        0        0     2654 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/declaration/user_defined_value_type_definition.py
+-rw-r--r--   0        0        0    19473 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/declaration/variable_declaration.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/__init__.py
+-rw-r--r--   0        0        0     6583 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/abc.py
+-rw-r--r--   0        0        0     4063 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/expression/assignment.py
+-rw-r--r--   0        0        0     2959 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/binary_operation.py
+-rw-r--r--   0        0        0     2087 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/conditional.py
+-rw-r--r--   0        0        0     1361 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/elementary_type_name_expression.py
+-rw-r--r--   0        0        0     8933 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/expression/function_call.py
+-rw-r--r--   0        0        0     2142 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/expression/function_call_options.py
+-rw-r--r--   0        0        0     5709 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/expression/identifier.py
+-rw-r--r--   0        0        0     1996 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/index_access.py
+-rw-r--r--   0        0        0     2661 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/index_range_access.py
+-rw-r--r--   0        0        0     1437 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/literal.py
+-rw-r--r--   0        0        0    19431 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/expression/member_access.py
+-rw-r--r--   0        0        0     1376 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/new_expression.py
+-rw-r--r--   0        0        0     2191 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/expression/tuple_expression.py
+-rw-r--r--   0        0        0     3071 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/expression/unary_operation.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.192344 woke-3.4.2/woke/ast/ir/meta/__init__.py
+-rw-r--r--   0        0        0    10965 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/identifier_path.py
+-rw-r--r--   0        0        0     8998 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/import_directive.py
+-rw-r--r--   0        0        0     3752 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/inheritance_specifier.py
+-rw-r--r--   0        0        0     5700 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/modifier_invocation.py
+-rw-r--r--   0        0        0     3462 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/override_specifier.py
+-rw-r--r--   0        0        0     4311 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/parameter_list.py
+-rw-r--r--   0        0        0     1534 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/pragma_directive.py
+-rw-r--r--   0        0        0     9307 2023-05-23 12:59:50.607753 woke-3.4.2/woke/ast/ir/meta/source_unit.py
+-rw-r--r--   0        0        0     2315 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/meta/structured_documentation.py
+-rw-r--r--   0        0        0     4541 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/meta/try_catch_clause.py
+-rw-r--r--   0        0        0     5698 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/meta/using_for_directive.py
+-rw-r--r--   0        0        0     4812 2023-05-22 07:04:56.893614 woke-3.4.2/woke/ast/ir/reference_resolver.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/__init__.py
+-rw-r--r--   0        0        0     5608 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/abc.py
+-rw-r--r--   0        0        0     3135 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/block.py
+-rw-r--r--   0        0        0     1611 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/break_statement.py
+-rw-r--r--   0        0        0     1635 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/continue_statement.py
+-rw-r--r--   0        0        0     2563 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/do_while_statement.py
+-rw-r--r--   0        0        0     2452 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/emit_statement.py
+-rw-r--r--   0        0        0     6016 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/expression_statement.py
+-rw-r--r--   0        0        0     5735 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/for_statement.py
+-rw-r--r--   0        0        0     3423 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/if_statement.py
+-rw-r--r--   0        0        0    10276 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/inline_assembly.py
+-rw-r--r--   0        0        0     1583 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/placeholder_statement.py
+-rw-r--r--   0        0        0     3336 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/return_statement.py
+-rw-r--r--   0        0        0     2608 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/revert_statement.py
+-rw-r--r--   0        0        0     3134 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/try_statement.py
+-rw-r--r--   0        0        0     2454 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/unchecked_block.py
+-rw-r--r--   0        0        0     4330 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/statement/variable_declaration_statement.py
+-rw-r--r--   0        0        0     2596 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/statement/while_statement.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/type_name/__init__.py
+-rw-r--r--   0        0        0     4932 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/type_name/abc.py
+-rw-r--r--   0        0        0     4092 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/array_type_name.py
+-rw-r--r--   0        0        0     5967 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/elementary_type_name.py
+-rw-r--r--   0        0        0     3987 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/function_type_name.py
+-rw-r--r--   0        0        0     3938 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/mapping.py
+-rw-r--r--   0        0        0    11314 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/type_name/user_defined_type_name.py
+-rw-r--r--   0        0        0       36 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/utils/__init__.py
+-rw-r--r--   0        0        0      589 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/utils/init_tuple.py
+-rw-r--r--   0        0        0      578 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/abc.py
+-rw-r--r--   0        0        0     1817 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/assignment.py
+-rw-r--r--   0        0        0     4317 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/block.py
+-rw-r--r--   0        0        0      301 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/break_statement.py
+-rw-r--r--   0        0        0     1200 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/case_statement.py
+-rw-r--r--   0        0        0      304 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/continue_statement.py
+-rw-r--r--   0        0        0     1659 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/expression_statement.py
+-rw-r--r--   0        0        0     1893 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/for_loop.py
+-rw-r--r--   0        0        0     2323 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/function_call.py
+-rw-r--r--   0        0        0     2298 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/function_definition.py
+-rw-r--r--   0        0        0     1492 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/identifier.py
+-rw-r--r--   0        0        0     1582 2023-05-13 06:28:54.195678 woke-3.4.2/woke/ast/ir/yul/if_statement.py
+-rw-r--r--   0        0        0      301 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/leave.py
+-rw-r--r--   0        0        0     1781 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/literal.py
+-rw-r--r--   0        0        0     1802 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/switch.py
+-rw-r--r--   0        0        0      921 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/typed_name.py
+-rw-r--r--   0        0        0     2097 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/ir/yul/variable_declaration.py
+-rw-r--r--   0        0        0    37866 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/nodes.py
+-rw-r--r--   0        0        0    47087 2023-05-13 06:29:36.855649 woke-3.4.2/woke/ast/types.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/__init__.py
+-rw-r--r--   0        0        0     3501 2023-05-13 06:29:36.855649 woke-3.4.2/woke/cli/__main__.py
+-rw-r--r--   0        0        0     7942 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/accounts.py
+-rw-r--r--   0        0        0     4650 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/compile.py
+-rw-r--r--   0        0        0       54 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/console.py
+-rw-r--r--   0        0        0     3838 2023-05-23 12:59:50.611086 woke-3.4.2/woke/cli/detect.py
+-rw-r--r--   0        0        0     3791 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/fuzz.py
+-rw-r--r--   0        0        0    11813 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/init.py
+-rw-r--r--   0        0        0     1081 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/lsp.py
+-rw-r--r--   0        0        0     3154 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/run.py
+-rw-r--r--   0        0        0     4922 2023-05-13 06:28:54.199011 woke-3.4.2/woke/cli/svm.py
+-rw-r--r--   0        0        0     2258 2023-05-22 07:04:56.893614 woke-3.4.2/woke/cli/test.py
+-rw-r--r--   0        0        0      187 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/__init__.py
+-rw-r--r--   0        0        0     1814 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/build_data_model.py
+-rw-r--r--   0        0        0     3120 2023-05-13 06:29:36.855649 woke-3.4.2/woke/compiler/compilation_unit.py
+-rw-r--r--   0        0        0    41479 2023-05-23 12:59:50.614420 woke-3.4.2/woke/compiler/compiler.py
+-rw-r--r--   0        0        0       97 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/exceptions.py
+-rw-r--r--   0        0        0      103 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/exceptions.py
+-rw-r--r--   0        0        0     8554 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/input_data_model.py
+-rw-r--r--   0        0        0     8728 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/output_data_model.py
+-rw-r--r--   0        0        0     3571 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/solc_frontend/solc_runner.py
+-rw-r--r--   0        0        0     2455 2023-05-13 06:28:54.199011 woke-3.4.2/woke/compiler/source_path_resolver.py
+-rw-r--r--   0        0        0     4813 2023-05-13 06:29:36.855649 woke-3.4.2/woke/compiler/source_unit_name_resolver.py
+-rw-r--r--   0        0        0     1118 2023-05-13 06:28:54.199011 woke-3.4.2/woke/config/__init__.py
+-rw-r--r--   0        0        0     6912 2023-05-23 12:59:50.614420 woke-3.4.2/woke/config/data_model.py
+-rw-r--r--   0        0        0    12682 2023-05-13 06:29:36.855649 woke-3.4.2/woke/config/woke_config.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/contracts/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/contracts/woke/__init__.py
+-rw-r--r--   0        0        0    64087 2023-05-13 06:28:54.199011 woke-3.4.2/woke/contracts/woke/console.sol
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/core/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-13 06:29:36.855649 woke-3.4.2/woke/core/enums.py
+-rw-r--r--   0        0        0    24829 2023-05-13 06:29:36.855649 woke-3.4.2/woke/core/solidity_version.py
+-rw-r--r--   0        0        0      678 2023-05-13 06:29:36.855649 woke-3.4.2/woke/deployment/__init__.py
+-rw-r--r--   0        0        0    14848 2023-05-13 06:29:36.858982 woke-3.4.2/woke/deployment/core.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.199011 woke-3.4.2/woke/development/__init__.py
+-rw-r--r--   0        0        0     4552 2023-05-13 06:28:54.199011 woke-3.4.2/woke/development/blocks.py
+-rw-r--r--   0        0        0    28963 2023-05-13 06:29:36.858982 woke-3.4.2/woke/development/call_trace.py
+-rw-r--r--   0        0        0    25863 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/chain_interfaces.py
+-rw-r--r--   0        0        0     1132 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/constants.py
+-rw-r--r--   0        0        0    96441 2023-05-23 13:17:34.084931 woke-3.4.2/woke/development/core.py
+-rw-r--r--   0        0        0     7270 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/globals.py
+-rw-r--r--   0        0        0   161115 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/hardhat_console.py
+-rw-r--r--   0        0        0     1093 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/internal.py
+-rw-r--r--   0        0        0       39 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/__init__.py
+-rw-r--r--   0        0        0      302 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/abc.py
+-rw-r--r--   0        0        0     2070 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/communicator.py
+-rw-r--r--   0        0        0      821 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/http.py
+-rw-r--r--   0        0        0     2912 2023-05-13 06:29:36.858982 woke-3.4.2/woke/development/json_rpc/ipc.py
+-rw-r--r--   0        0        0      625 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/json_rpc/websocket.py
+-rw-r--r--   0        0        0     6572 2023-05-13 06:28:54.202344 woke-3.4.2/woke/development/primitive_types.py
+-rw-r--r--   0        0        0    89995 2023-05-23 13:17:34.084931 woke-3.4.2/woke/development/pytypes_generator.py
+-rw-r--r--   0        0        0    28061 2023-05-22 07:04:56.893614 woke-3.4.2/woke/development/transactions.py
+-rw-r--r--   0        0        0     7389 2023-05-13 06:28:54.205678 woke-3.4.2/woke/development/utils.py
+-rw-r--r--   0        0        0       47 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/__init__.py
+-rw-r--r--   0        0        0      310 2023-05-22 07:04:56.893614 woke-3.4.2/woke/lsp/commands/__init__.py
+-rw-r--r--   0        0        0     4033 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/commands/generate_control_flow_graph.py
+-rw-r--r--   0        0        0     1097 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/commands/generate_imports_graph.py
+-rw-r--r--   0        0        0     4247 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/commands/generate_inheritance_graph.py
+-rw-r--r--   0        0        0     2163 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/commands/generate_linearized_inheritance_graph.py
+-rw-r--r--   0        0        0    31491 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/common_structures.py
+-rw-r--r--   0        0        0     1900 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/context.py
+-rw-r--r--   0        0        0     2574 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/document_sync.py
+-rw-r--r--   0        0        0      130 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/enums.py
+-rw-r--r--   0        0        0      471 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/__init__.py
+-rw-r--r--   0        0        0     6969 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/code_action.py
+-rw-r--r--   0        0        0    10904 2023-05-22 07:04:56.893614 woke-3.4.2/woke/lsp/features/code_lens.py
+-rw-r--r--   0        0        0    19824 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/completion.py
+-rw-r--r--   0        0        0     9948 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/definition.py
+-rw-r--r--   0        0        0     1446 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/diagnostic.py
+-rw-r--r--   0        0        0     4305 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/document_link.py
+-rw-r--r--   0        0        0     8407 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/document_symbol.py
+-rw-r--r--   0        0        0    17901 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/features/hover.py
+-rw-r--r--   0        0        0     3850 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/implementation.py
+-rw-r--r--   0        0        0     5092 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/references.py
+-rw-r--r--   0        0        0     8935 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/rename.py
+-rw-r--r--   0        0        0     9505 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/type_definition.py
+-rw-r--r--   0        0        0    11043 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/features/type_hierarchy.py
+-rw-r--r--   0        0        0    39957 2023-05-23 12:59:50.614420 woke-3.4.2/woke/lsp/lsp_compiler.py
+-rw-r--r--   0        0        0      328 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/lsp_data_model.py
+-rw-r--r--   0        0        0     8941 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/lsp_parser.py
+-rw-r--r--   0        0        0     5551 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/methods.py
+-rw-r--r--   0        0        0     1897 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/protocol_structures.py
+-rw-r--r--   0        0        0     2229 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/rpc_protocol.py
+-rw-r--r--   0        0        0    37738 2023-05-22 07:04:56.893614 woke-3.4.2/woke/lsp/server.py
+-rw-r--r--   0        0        0     6597 2023-05-13 06:29:36.858982 woke-3.4.2/woke/lsp/server_capabilities.py
+-rw-r--r--   0        0        0       86 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/utils/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/utils/position.py
+-rw-r--r--   0        0        0      459 2023-05-13 06:28:54.205678 woke-3.4.2/woke/lsp/utils/uri.py
+-rw-r--r--   0        0        0       50 2023-05-13 06:28:54.205678 woke-3.4.2/woke/regex_parser/__init__.py
+-rw-r--r--   0        0        0     1690 2023-05-13 06:28:54.205678 woke-3.4.2/woke/regex_parser/solidity_import.py
+-rw-r--r--   0        0        0     6653 2023-05-23 12:59:50.617753 woke-3.4.2/woke/regex_parser/solidity_parser.py
+-rw-r--r--   0        0        0       36 2023-05-13 06:28:54.205678 woke-3.4.2/woke/svm/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-13 06:29:36.858982 woke-3.4.2/woke/svm/abc.py
+-rw-r--r--   0        0        0      270 2023-05-13 06:28:54.205678 woke-3.4.2/woke/svm/exceptions.py
+-rw-r--r--   0        0        0    11721 2023-05-13 06:29:36.858982 woke-3.4.2/woke/svm/svm.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/scripts/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/scripts/deploy.py
+-rw-r--r--   0        0        0        0 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/tests/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-13 06:28:54.205678 woke-3.4.2/woke/templates/tests/test_default.py
+-rw-r--r--   0        0        0      678 2023-05-13 06:29:36.858982 woke-3.4.2/woke/testing/__init__.py
+-rw-r--r--   0        0        0    10878 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/core.py
+-rw-r--r--   0        0        0    24381 2023-05-13 06:29:36.858982 woke-3.4.2/woke/testing/coverage.py
+-rw-r--r--   0        0        0      187 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/__init__.py
+-rw-r--r--   0        0        0     4999 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/fuzz_test.py
+-rw-r--r--   0        0        0    10795 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/fuzzer.py
+-rw-r--r--   0        0        0     5780 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/fuzzing/generators.py
+-rw-r--r--   0        0        0      298 2023-05-13 06:28:54.209011 woke-3.4.2/woke/testing/pytest_plugin.py
+-rw-r--r--   0        0        0      170 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-23 12:59:50.617753 woke-3.4.2/woke/utils/context_managers.py
+-rw-r--r--   0        0        0      515 2023-05-23 12:59:50.617753 woke-3.4.2/woke/utils/decorators.py
+-rw-r--r--   0        0        0      158 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/enums.py
+-rw-r--r--   0        0        0     1699 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/file_utils.py
+-rw-r--r--   0        0        0      384 2023-05-13 06:29:36.858982 woke-3.4.2/woke/utils/keyed_default_dict.py
+-rw-r--r--   0        0        0      194 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/networking.py
+-rw-r--r--   0        0        0     1017 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/openzeppelin.py
+-rw-r--r--   0        0        0      630 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/string.py
+-rw-r--r--   0        0        0     1747 2023-05-13 06:29:36.858982 woke-3.4.2/woke/utils/tee.py
+-rw-r--r--   0        0        0     3765 2023-05-13 06:28:54.209011 woke-3.4.2/woke/utils/threaded_child_watcher.py
+-rw-r--r--   0        0        0      424 2023-05-13 06:29:36.858982 woke-3.4.2/woke/utils/version.py
+-rw-r--r--   0        0        0     6129 1970-01-01 00:00:00.000000 woke-3.4.2/setup.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 woke-3.4.2/PKG-INFO
```

### Comparing `woke-3.4.1/LICENSE` & `woke-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/README.md` & `woke-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/pyproject.toml` & `woke-3.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "woke"
-version = "3.4.1"
+version = "3.4.2"
 description = "Woke is a Python-based development and testing framework for Solidity."
 license = "ISC"
 authors = ["Ackee Blockchain"]
 readme = "README.md"
 homepage = "https://ackeeblockchain.com"
 repository = "https://github.com/Ackee-Blockchain/woke"
 documentation = "https://ackeeblockchain.com/woke/docs/latest"
```

### Comparing `woke-3.4.1/woke/analysis/cfg.py` & `woke-3.4.2/woke/analysis/cfg.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/__init__.py` & `woke-3.4.2/woke/analysis/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/api.py` & `woke-3.4.2/woke/analysis/detectors/api.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/axelar/proxy_contract_id.py` & `woke-3.4.2/woke/analysis/detectors/axelar/proxy_contract_id.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/balance_state_var.py` & `woke-3.4.2/woke/analysis/detectors/balance_state_var.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/bug_empty_byte_array_copy.py` & `woke-3.4.2/woke/analysis/detectors/bug_empty_byte_array_copy.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/call_options_not_called.py` & `woke-3.4.2/woke/analysis/detectors/call_options_not_called.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/missing_return.py` & `woke-3.4.2/woke/analysis/detectors/missing_return.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/msg_value_nonpayable_function.py` & `woke-3.4.2/woke/analysis/detectors/msg_value_nonpayable_function.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py` & `woke-3.4.2/woke/analysis/detectors/overflow_calldata_tuple_reencoding_bug.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/ownable.py` & `woke-3.4.2/woke/analysis/detectors/ownable.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/proxy_contract_selector_clashes.py` & `woke-3.4.2/woke/analysis/detectors/proxy_contract_selector_clashes.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/reentrancy.py` & `woke-3.4.2/woke/analysis/detectors/reentrancy.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/unchecked_return_value.py` & `woke-3.4.2/woke/analysis/detectors/unchecked_return_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/unsafe_delegatecall.py` & `woke-3.4.2/woke/analysis/detectors/unsafe_delegatecall.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/unsafe_selfdestruct.py` & `woke-3.4.2/woke/analysis/detectors/unsafe_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/unsafe_tx_origin.py` & `woke-3.4.2/woke/analysis/detectors/unsafe_tx_origin.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/unused_contract.py` & `woke-3.4.2/woke/analysis/detectors/unused_contract.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/analysis/detectors/utils.py` & `woke-3.4.2/woke/analysis/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/enums.py` & `woke-3.4.2/woke/ast/enums.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/abc.py` & `woke-3.4.2/woke/ast/ir/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/abc.py` & `woke-3.4.2/woke/ast/ir/declaration/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/contract_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/contract_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/enum_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/enum_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/enum_value.py` & `woke-3.4.2/woke/ast/ir/declaration/enum_value.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/error_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/error_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/event_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/event_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/function_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/modifier_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/modifier_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/struct_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/struct_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/user_defined_value_type_definition.py` & `woke-3.4.2/woke/ast/ir/declaration/user_defined_value_type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/declaration/variable_declaration.py` & `woke-3.4.2/woke/ast/ir/declaration/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/abc.py` & `woke-3.4.2/woke/ast/ir/expression/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/assignment.py` & `woke-3.4.2/woke/ast/ir/expression/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/binary_operation.py` & `woke-3.4.2/woke/ast/ir/expression/binary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/conditional.py` & `woke-3.4.2/woke/ast/ir/expression/conditional.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/elementary_type_name_expression.py` & `woke-3.4.2/woke/ast/ir/expression/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/function_call.py` & `woke-3.4.2/woke/ast/ir/expression/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/function_call_options.py` & `woke-3.4.2/woke/ast/ir/expression/function_call_options.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/identifier.py` & `woke-3.4.2/woke/ast/ir/expression/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/index_access.py` & `woke-3.4.2/woke/ast/ir/expression/index_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/index_range_access.py` & `woke-3.4.2/woke/ast/ir/expression/index_range_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/literal.py` & `woke-3.4.2/woke/ast/ir/expression/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/member_access.py` & `woke-3.4.2/woke/ast/ir/expression/member_access.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/new_expression.py` & `woke-3.4.2/woke/ast/ir/expression/new_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/tuple_expression.py` & `woke-3.4.2/woke/ast/ir/expression/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/expression/unary_operation.py` & `woke-3.4.2/woke/ast/ir/expression/unary_operation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/identifier_path.py` & `woke-3.4.2/woke/ast/ir/meta/identifier_path.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/import_directive.py` & `woke-3.4.2/woke/ast/ir/meta/import_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/inheritance_specifier.py` & `woke-3.4.2/woke/ast/ir/meta/inheritance_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/modifier_invocation.py` & `woke-3.4.2/woke/ast/ir/meta/modifier_invocation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/override_specifier.py` & `woke-3.4.2/woke/ast/ir/meta/override_specifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/parameter_list.py` & `woke-3.4.2/woke/ast/ir/meta/parameter_list.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/pragma_directive.py` & `woke-3.4.2/woke/ast/ir/meta/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/source_unit.py` & `woke-3.4.2/woke/ast/ir/meta/source_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/structured_documentation.py` & `woke-3.4.2/woke/ast/ir/meta/structured_documentation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/try_catch_clause.py` & `woke-3.4.2/woke/ast/ir/meta/try_catch_clause.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/meta/using_for_directive.py` & `woke-3.4.2/woke/ast/ir/meta/using_for_directive.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/reference_resolver.py` & `woke-3.4.2/woke/ast/ir/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/abc.py` & `woke-3.4.2/woke/ast/ir/statement/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/block.py` & `woke-3.4.2/woke/ast/ir/statement/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/break_statement.py` & `woke-3.4.2/woke/ast/ir/statement/break_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/continue_statement.py` & `woke-3.4.2/woke/ast/ir/statement/continue_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/do_while_statement.py` & `woke-3.4.2/woke/ast/ir/statement/do_while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/emit_statement.py` & `woke-3.4.2/woke/ast/ir/statement/emit_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/expression_statement.py` & `woke-3.4.2/woke/ast/ir/statement/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/for_statement.py` & `woke-3.4.2/woke/ast/ir/statement/for_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/if_statement.py` & `woke-3.4.2/woke/ast/ir/statement/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/inline_assembly.py` & `woke-3.4.2/woke/ast/ir/statement/inline_assembly.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/placeholder_statement.py` & `woke-3.4.2/woke/ast/ir/statement/placeholder_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/return_statement.py` & `woke-3.4.2/woke/ast/ir/statement/return_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/revert_statement.py` & `woke-3.4.2/woke/ast/ir/statement/revert_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/try_statement.py` & `woke-3.4.2/woke/ast/ir/statement/try_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/unchecked_block.py` & `woke-3.4.2/woke/ast/ir/statement/unchecked_block.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/variable_declaration_statement.py` & `woke-3.4.2/woke/ast/ir/statement/variable_declaration_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/statement/while_statement.py` & `woke-3.4.2/woke/ast/ir/statement/while_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/type_name/abc.py` & `woke-3.4.2/woke/ast/ir/type_name/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/type_name/array_type_name.py` & `woke-3.4.2/woke/ast/ir/type_name/array_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/type_name/elementary_type_name.py` & `woke-3.4.2/woke/ast/ir/type_name/elementary_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/type_name/function_type_name.py` & `woke-3.4.2/woke/ast/ir/type_name/function_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/type_name/mapping.py` & `woke-3.4.2/woke/ast/ir/type_name/mapping.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/type_name/user_defined_type_name.py` & `woke-3.4.2/woke/ast/ir/type_name/user_defined_type_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/utils/init_tuple.py` & `woke-3.4.2/woke/ast/ir/utils/init_tuple.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/__init__.py` & `woke-3.4.2/woke/ast/ir/yul/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/abc.py` & `woke-3.4.2/woke/ast/ir/yul/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/assignment.py` & `woke-3.4.2/woke/ast/ir/yul/assignment.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/block.py` & `woke-3.4.2/woke/ast/ir/yul/block.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/case_statement.py` & `woke-3.4.2/woke/ast/ir/yul/case_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/expression_statement.py` & `woke-3.4.2/woke/ast/ir/yul/expression_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/for_loop.py` & `woke-3.4.2/woke/ast/ir/yul/for_loop.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/function_call.py` & `woke-3.4.2/woke/ast/ir/yul/function_call.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/function_definition.py` & `woke-3.4.2/woke/ast/ir/yul/function_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/identifier.py` & `woke-3.4.2/woke/ast/ir/yul/identifier.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/if_statement.py` & `woke-3.4.2/woke/ast/ir/yul/if_statement.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/literal.py` & `woke-3.4.2/woke/ast/ir/yul/literal.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/switch.py` & `woke-3.4.2/woke/ast/ir/yul/switch.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/typed_name.py` & `woke-3.4.2/woke/ast/ir/yul/typed_name.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/ir/yul/variable_declaration.py` & `woke-3.4.2/woke/ast/ir/yul/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/nodes.py` & `woke-3.4.2/woke/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/ast/types.py` & `woke-3.4.2/woke/ast/types.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/__main__.py` & `woke-3.4.2/woke/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/accounts.py` & `woke-3.4.2/woke/cli/accounts.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/compile.py` & `woke-3.4.2/woke/cli/compile.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/detect.py` & `woke-3.4.2/woke/cli/detect.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/fuzz.py` & `woke-3.4.2/woke/cli/fuzz.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/init.py` & `woke-3.4.2/woke/cli/init.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/lsp.py` & `woke-3.4.2/woke/cli/lsp.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/run.py` & `woke-3.4.2/woke/cli/run.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/svm.py` & `woke-3.4.2/woke/cli/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/cli/test.py` & `woke-3.4.2/woke/cli/test.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/build_data_model.py` & `woke-3.4.2/woke/compiler/build_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/compilation_unit.py` & `woke-3.4.2/woke/compiler/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/compiler.py` & `woke-3.4.2/woke/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/solc_frontend/input_data_model.py` & `woke-3.4.2/woke/compiler/solc_frontend/input_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/solc_frontend/output_data_model.py` & `woke-3.4.2/woke/compiler/solc_frontend/output_data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/solc_frontend/solc_runner.py` & `woke-3.4.2/woke/compiler/solc_frontend/solc_runner.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/source_path_resolver.py` & `woke-3.4.2/woke/compiler/source_path_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/compiler/source_unit_name_resolver.py` & `woke-3.4.2/woke/compiler/source_unit_name_resolver.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/config/__init__.py` & `woke-3.4.2/woke/config/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/config/data_model.py` & `woke-3.4.2/woke/config/data_model.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/config/woke_config.py` & `woke-3.4.2/woke/config/woke_config.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/contracts/woke/console.sol` & `woke-3.4.2/woke/contracts/woke/console.sol`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/core/solidity_version.py` & `woke-3.4.2/woke/core/solidity_version.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/deployment/__init__.py` & `woke-3.4.2/woke/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/deployment/core.py` & `woke-3.4.2/woke/deployment/core.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/blocks.py` & `woke-3.4.2/woke/development/blocks.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/call_trace.py` & `woke-3.4.2/woke/development/call_trace.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/chain_interfaces.py` & `woke-3.4.2/woke/development/chain_interfaces.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/constants.py` & `woke-3.4.2/woke/development/constants.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/core.py` & `woke-3.4.2/woke/development/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1626,14 +1626,19 @@
                 f"Unable to find function with selector {selector.hex()} in contract {fqn}"
             )
         elif get_origin(expected_type) is list:
             return [
                 self._convert_from_web3_type(tx, v, get_args(expected_type)[0])
                 for v in value
             ]
+        elif get_origin(expected_type) is tuple:
+            return tuple(
+                self._convert_from_web3_type(tx, v, t)
+                for v, t in zip(value, get_args(expected_type))
+            )
         elif dataclasses.is_dataclass(expected_type):
             assert isinstance(value, tuple)
             resolved_types = get_type_hints(expected_type)
             field_types = [
                 resolved_types[field.name]
                 for field in dataclasses.fields(expected_type)
                 if field.init
@@ -1920,17 +1925,17 @@
     def _send_transaction(
         self, tx_params: TxParams, from_: Optional[Union[Account, Address, str]]
     ) -> str:
         assert "from" in tx_params
         assert "nonce" in tx_params
 
         if self._chain_id in {56, 97}:
-            # BSC doesn't support access lists and tx type            
+            # BSC doesn't support access lists and tx type
             tx_params.pop("type", None)
-            tx_params.pop("accessList", None)            
+            tx_params.pop("accessList", None)
 
         self._confirm_transaction(tx_params)
 
         if self.require_signed_txs:
             if isinstance(from_, (Account, Address)):
                 key = from_.private_key
             elif from_ is None and self._default_tx_account is not None:
```

### Comparing `woke-3.4.1/woke/development/globals.py` & `woke-3.4.2/woke/development/globals.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/hardhat_console.py` & `woke-3.4.2/woke/development/hardhat_console.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/internal.py` & `woke-3.4.2/woke/development/internal.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/json_rpc/communicator.py` & `woke-3.4.2/woke/development/json_rpc/communicator.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/json_rpc/http.py` & `woke-3.4.2/woke/development/json_rpc/http.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/json_rpc/ipc.py` & `woke-3.4.2/woke/development/json_rpc/ipc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/json_rpc/websocket.py` & `woke-3.4.2/woke/development/json_rpc/websocket.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/primitive_types.py` & `woke-3.4.2/woke/development/primitive_types.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/pytypes_generator.py` & `woke-3.4.2/woke/development/pytypes_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,17 +594,16 @@
                 for c in contract.linearized_base_contracts:
                     for event in c.events:
                         if event.event_selector == selector:
                             event_decl = event
                             break
                     if event_decl is not None:
                         break
-                assert (
-                    event_decl is not None
-                ), f"Could not find event {item['name']} in contract {fqn} or its bases"
+                if event_decl is None:
+                    continue
 
                 if selector not in self.__events_index:
                     self.__events_index[selector] = {}
                 event_module_name = "pytypes." + _make_path_alphanum(
                     event_decl.parent.parent.source_unit_name[:-3]
                 ).replace("/", ".")
                 self.__events_index[selector][fqn] = (
@@ -2090,12 +2089,15 @@
                 f"Cannot sanitize name for declaration {declaration} with parent {parent}"
             )
 
         if declaration in renames:
             return renames[declaration]
 
         new_name = declaration.name
+        while new_name.startswith("__"):
+            new_name = new_name[1:]
+
         while check(new_name):
             new_name = new_name + "_"
 
         renames[declaration] = new_name
         return new_name
```

### Comparing `woke-3.4.1/woke/development/transactions.py` & `woke-3.4.2/woke/development/transactions.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/development/utils.py` & `woke-3.4.2/woke/development/utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/commands/generate_control_flow_graph.py` & `woke-3.4.2/woke/lsp/commands/generate_control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/commands/generate_imports_graph.py` & `woke-3.4.2/woke/lsp/commands/generate_imports_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/commands/generate_inheritance_graph.py` & `woke-3.4.2/woke/lsp/commands/generate_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/commands/generate_linearized_inheritance_graph.py` & `woke-3.4.2/woke/lsp/commands/generate_linearized_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/common_structures.py` & `woke-3.4.2/woke/lsp/common_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/context.py` & `woke-3.4.2/woke/lsp/context.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/document_sync.py` & `woke-3.4.2/woke/lsp/document_sync.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/code_action.py` & `woke-3.4.2/woke/lsp/features/code_action.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/code_lens.py` & `woke-3.4.2/woke/lsp/features/code_lens.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/completion.py` & `woke-3.4.2/woke/lsp/features/completion.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/definition.py` & `woke-3.4.2/woke/lsp/features/definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/diagnostic.py` & `woke-3.4.2/woke/lsp/features/diagnostic.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/document_link.py` & `woke-3.4.2/woke/lsp/features/document_link.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/document_symbol.py` & `woke-3.4.2/woke/lsp/features/document_symbol.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/hover.py` & `woke-3.4.2/woke/lsp/features/hover.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/implementation.py` & `woke-3.4.2/woke/lsp/features/implementation.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/references.py` & `woke-3.4.2/woke/lsp/features/references.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/rename.py` & `woke-3.4.2/woke/lsp/features/rename.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/type_definition.py` & `woke-3.4.2/woke/lsp/features/type_definition.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/features/type_hierarchy.py` & `woke-3.4.2/woke/lsp/features/type_hierarchy.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/lsp_compiler.py` & `woke-3.4.2/woke/lsp/lsp_compiler.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/lsp_parser.py` & `woke-3.4.2/woke/lsp/lsp_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/methods.py` & `woke-3.4.2/woke/lsp/methods.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/protocol_structures.py` & `woke-3.4.2/woke/lsp/protocol_structures.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/rpc_protocol.py` & `woke-3.4.2/woke/lsp/rpc_protocol.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/server.py` & `woke-3.4.2/woke/lsp/server.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/server_capabilities.py` & `woke-3.4.2/woke/lsp/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/lsp/utils/position.py` & `woke-3.4.2/woke/lsp/utils/position.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/regex_parser/solidity_import.py` & `woke-3.4.2/woke/regex_parser/solidity_import.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/regex_parser/solidity_parser.py` & `woke-3.4.2/woke/regex_parser/solidity_parser.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/svm/abc.py` & `woke-3.4.2/woke/svm/abc.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/svm/svm.py` & `woke-3.4.2/woke/svm/svm.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/testing/__init__.py` & `woke-3.4.2/woke/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/testing/core.py` & `woke-3.4.2/woke/testing/core.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/testing/coverage.py` & `woke-3.4.2/woke/testing/coverage.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/testing/fuzzing/fuzz_test.py` & `woke-3.4.2/woke/testing/fuzzing/fuzz_test.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/testing/fuzzing/fuzzer.py` & `woke-3.4.2/woke/testing/fuzzing/fuzzer.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/testing/fuzzing/generators.py` & `woke-3.4.2/woke/testing/fuzzing/generators.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/context_managers.py` & `woke-3.4.2/woke/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/decorators.py` & `woke-3.4.2/woke/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/file_utils.py` & `woke-3.4.2/woke/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/openzeppelin.py` & `woke-3.4.2/woke/utils/openzeppelin.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/string.py` & `woke-3.4.2/woke/utils/string.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/tee.py` & `woke-3.4.2/woke/utils/tee.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/woke/utils/threaded_child_watcher.py` & `woke-3.4.2/woke/utils/threaded_child_watcher.py`

 * *Files identical despite different names*

### Comparing `woke-3.4.1/setup.py` & `woke-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 entry_points = \
 {'console_scripts': ['woke = woke.cli.__main__:main',
                      'woke-solc = woke.cli.__main__:woke_solc']}
 
 setup_kwargs = {
     'name': 'woke',
-    'version': '3.4.1',
+    'version': '3.4.2',
     'description': 'Woke is a Python-based development and testing framework for Solidity.',
     'long_description': '# Woke\n\nWoke is a Python-based development and testing framework for Solidity.\n\nFeatures:\n\n- **Testing framework** - a testing framework for Solidity smart contracts with Python-native equivalents of Solidity types and blazing fast execution.\n\n- **Fuzzer** - a property-based fuzzer for Solidity smart contracts that allows testers to write their fuzz tests in Python.\n\n- **Vulnerability detectors**\n\n- **LSP server**\n\n## Dependencies\n\n- [Python](https://www.python.org/downloads/release/python-3910/) (version 3.7 or higher)\n\n> :warning: Python 3.11 is experimentally supported.\n\n## Installation\n\nvia `pip`\n\n```shell\npip3 install woke\n```\n\n## Documentation & Contribution\n\nWoke documentation can be found [here](https://ackeeblockchain.com/woke/docs/latest).\n\nThere you can also find a section on [contributing](https://ackeeblockchain.com/woke/docs/latest/contributing/).\n\n## Features\n\n### Testing framework\n\nSee [examples](examples) and [documentation](https://ackeeblockchain.com/woke/docs/latest/testing-framework/overview) for more information.\n\nWriting tests is as simple as:\n\n```python\nfrom woke.testing import *\nfrom pytypes.contracts.Counter import Counter\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n\n    counter = Counter.deploy()\n    assert counter.count() == 0\n\n    counter.increment()\n    assert counter.count() == 1\n```\n\n### Fuzzer\n\nFuzzer builds on top of the testing framework and allows efficient fuzz testing of Solidity smart contracts.\n\n```python\nfrom woke.testing import *\nfrom woke.testing.fuzzing import *\nfrom pytypes.contracts.Counter import Counter\n\nclass CounterTest(FuzzTest):\n    def pre_sequence(self) -> None:\n        self.counter = Counter.deploy()\n        self.count = 0\n\n    @flow()\n    def increment(self) -> None:\n        self.counter.increment()\n        self.count += 1\n\n    @flow()\n    def decrement(self) -> None:\n        with may_revert(Panic(PanicCodeEnum.UNDERFLOW_OVERFLOW)) as e:\n            self.counter.decrement()\n\n        if e.value is not None:\n            assert self.count == 0\n        else:\n            self.count -= 1\n\n    @invariant(period=10)\n    def count(self) -> None:\n        assert self.counter.count() == self.count\n\n@default_chain.connect()\ndef test_counter():\n    default_chain.set_default_accounts(default_chain.accounts[0])\n    CounterTest().run(sequences_count=30, flows_count=100)\n```\n\n### Vulnerability detectors\n\nVulnerability detectors can be run using:\n```shell\nwoke detect\n```\n\n### LSP server\n\nWoke implements an [LSP](https://microsoft.github.io/language-server-protocol/) server for Solidity. The only currently supported communication channel is TCP.\n\nWoke LSP server can be run using:\n\n```shell\nwoke lsp\n```\n\nOr with an optional --port argument:\n\n```shell\nwoke lsp --port 1234\n```\n\nAll LSP server features can be found in the [documentation](https://ackeeblockchain.com/woke/docs/latest/language-server/).\n\n## License\n\nThis project is licensed under the [ISC license](https://github.com/Ackee-Blockchain/woke/blob/main/LICENSE).\n\n## Partners\n\nRockawayX             |  Coinbase\n:-------------------------:|:-------------------------:\n[![](https://github.com/Ackee-Blockchain/woke/blob/main/images/rockawayx.jpg?raw=true)](https://rockawayx.com/)  |  [![](https://github.com/Ackee-Blockchain/woke/blob/main/images/coinbase.png?raw=true)](https://www.coinbase.com/)\n\n\n\n\n\n\n',
     'author': 'Ackee Blockchain',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ackeeblockchain.com',
```

### Comparing `woke-3.4.1/PKG-INFO` & `woke-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woke
-Version: 3.4.1
+Version: 3.4.2
 Summary: Woke is a Python-based development and testing framework for Solidity.
 Home-page: https://ackeeblockchain.com
 License: ISC
 Keywords: ethereum,solidity,security,testing,development,framework,audit
 Author: Ackee Blockchain
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: License :: OSI Approved
```

