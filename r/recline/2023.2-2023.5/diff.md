# Comparing `tmp/recline-2023.2.tar.gz` & `tmp/recline-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recline-2023.2.tar", max compression
+gzip compressed data, was "recline-2023.5.tar", max compression
```

## Comparing `recline-2023.2.tar` & `recline-2023.5.tar`

### file list

```diff
@@ -1,58 +1,57 @@
--rw-r--r--   0        0        0     1513 2023-02-08 13:57:07.334153 recline-2023.2/LICENSE
--rw-r--r--   0        0        0     5042 2023-02-08 13:57:07.334153 recline-2023.2/README.md
--rw-r--r--   0        0        0     1160 2023-02-08 13:57:07.334153 recline-2023.2/pyproject.toml
--rw-r--r--   0        0        0      371 2023-02-08 13:57:07.334153 recline-2023.2/recline/__init__.py
--rw-r--r--   0        0        0      565 2023-02-08 13:57:07.334153 recline-2023.2/recline/arg_types/__init__.py
--rw-r--r--   0        0        0     4148 2023-02-08 13:57:07.334153 recline-2023.2/recline/arg_types/choices.py
--rw-r--r--   0        0        0      668 2023-02-08 13:57:07.334153 recline-2023.2/recline/arg_types/flag.py
--rw-r--r--   0        0        0     1469 2023-02-08 13:57:07.334153 recline-2023.2/recline/arg_types/positional.py
--rw-r--r--   0        0        0     2905 2023-02-08 13:57:07.334153 recline-2023.2/recline/arg_types/ranged_int.py
--rw-r--r--   0        0        0     2642 2023-02-08 13:57:07.338153 recline-2023.2/recline/arg_types/recline_type.py
--rw-r--r--   0        0        0      941 2023-02-08 13:57:07.338153 recline-2023.2/recline/arg_types/recline_type_error.py
--rw-r--r--   0        0        0     1183 2023-02-08 13:57:07.338153 recline-2023.2/recline/arg_types/remainder.py
--rw-r--r--   0        0        0      454 2023-02-08 13:57:07.338153 recline-2023.2/recline/commands/__init__.py
--rw-r--r--   0        0        0     5230 2023-02-08 13:57:07.338153 recline-2023.2/recline/commands/async_command.py
--rw-r--r--   0        0        0     7874 2023-02-08 13:57:07.338153 recline-2023.2/recline/commands/builtin_commands.py
--rw-r--r--   0        0        0    16429 2023-02-08 13:57:07.338153 recline-2023.2/recline/commands/cli_command.py
--rw-r--r--   0        0        0     6044 2023-02-08 13:57:07.338153 recline-2023.2/recline/commands/man_utils.py
--rw-r--r--   0        0        0      315 2023-02-08 13:57:07.338153 recline-2023.2/recline/formatters/__init__.py
--rw-r--r--   0        0        0      559 2023-02-08 13:57:07.338153 recline-2023.2/recline/formatters/output_formatter.py
--rw-r--r--   0        0        0     3105 2023-02-08 13:57:07.338153 recline-2023.2/recline/formatters/table_formatter.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/recline/repl/__init__.py
--rw-r--r--   0        0        0     7969 2023-02-08 13:57:07.338153 recline-2023.2/recline/repl/completer.py
--rw-r--r--   0        0        0     9527 2023-02-08 13:57:07.338153 recline-2023.2/recline/repl/shell.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/__init__.py
--rw-r--r--   0        0        0    10174 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/LICENSE.rst
--rw-r--r--   0        0        0    29936 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/__init__.py
--rw-r--r--   0        0        0     1810 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/_check_module.py
--rw-r--r--   0        0        0     2987 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/bash_completion.d/python-argcomplete.sh
--rw-r--r--   0        0        0      524 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/compat.py
--rw-r--r--   0        0        0     3681 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/completers.py
--rw-r--r--   0        0        0    15351 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/my_argparse.py
--rw-r--r--   0        0        0    13218 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/my_shlex.py
--rw-r--r--   0        0        0     3072 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/argcomplete/shellintegration.py
--rw-r--r--   0        0        0     1084 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/docstring_parser/LICENSE
--rw-r--r--   0        0        0       86 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/docstring_parser/__init__.py
--rw-r--r--   0        0        0      808 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/docstring_parser/parser/__init__.py
--rw-r--r--   0        0        0     3942 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/docstring_parser/parser/common.py
--rw-r--r--   0        0        0     4164 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/docstring_parser/parser/google.py
--rw-r--r--   0        0        0     1571 2023-02-08 13:57:07.338153 recline-2023.2/recline/vendor/docstring_parser/parser/rest.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/tests/__init__.py
--rw-r--r--   0        0        0      287 2023-02-08 13:57:07.338153 recline-2023.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_arg_types/__init__.py
--rw-r--r--   0        0        0     2034 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_arg_types/test_choices.py
--rw-r--r--   0        0        0      989 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_arg_types/test_cliche_type.py
--rw-r--r--   0        0        0     1723 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_arg_types/test_positional.py
--rw-r--r--   0        0        0     1020 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_arg_types/test_ranged_int.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_commands/__init__.py
--rw-r--r--   0        0        0     3132 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_commands/test_async_command.py
--rw-r--r--   0        0        0     3541 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_commands/test_builtin_commands.py
--rw-r--r--   0        0        0     4811 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_commands/test_cli_command.py
--rw-r--r--   0        0        0     3553 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_commands/test_man_utils.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_formatters/__init__.py
--rw-r--r--   0        0        0     1223 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_formatters/test_table_formatter.py
--rw-r--r--   0        0        0        0 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_repl/__init__.py
--rw-r--r--   0        0        0     3560 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_repl/test_completer.py
--rw-r--r--   0        0        0     4288 2023-02-08 13:57:07.338153 recline-2023.2/tests/test_repl/test_shell.py
--rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 recline-2023.2/setup.py
--rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 recline-2023.2/PKG-INFO
+-rw-r--r--   0        0        0     1513 2023-05-23 11:23:51.760331 recline-2023.5/LICENSE
+-rw-r--r--   0        0        0     5042 2023-05-23 11:23:51.760331 recline-2023.5/README.md
+-rw-r--r--   0        0        0     1160 2023-05-23 11:23:51.760331 recline-2023.5/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-05-23 11:23:51.760331 recline-2023.5/recline/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/__init__.py
+-rw-r--r--   0        0        0     4148 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/choices.py
+-rw-r--r--   0        0        0      668 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/flag.py
+-rw-r--r--   0        0        0     1469 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/positional.py
+-rw-r--r--   0        0        0     2905 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/ranged_int.py
+-rw-r--r--   0        0        0     2642 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/recline_type.py
+-rw-r--r--   0        0        0      941 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/recline_type_error.py
+-rw-r--r--   0        0        0     1183 2023-05-23 11:23:51.760331 recline-2023.5/recline/arg_types/remainder.py
+-rw-r--r--   0        0        0      454 2023-05-23 11:23:51.760331 recline-2023.5/recline/commands/__init__.py
+-rw-r--r--   0        0        0     5230 2023-05-23 11:23:51.760331 recline-2023.5/recline/commands/async_command.py
+-rw-r--r--   0        0        0     7874 2023-05-23 11:23:51.760331 recline-2023.5/recline/commands/builtin_commands.py
+-rw-r--r--   0        0        0    16429 2023-05-23 11:23:51.760331 recline-2023.5/recline/commands/cli_command.py
+-rw-r--r--   0        0        0     6044 2023-05-23 11:23:51.760331 recline-2023.5/recline/commands/man_utils.py
+-rw-r--r--   0        0        0      315 2023-05-23 11:23:51.760331 recline-2023.5/recline/formatters/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-23 11:23:51.760331 recline-2023.5/recline/formatters/output_formatter.py
+-rw-r--r--   0        0        0     3105 2023-05-23 11:23:51.760331 recline-2023.5/recline/formatters/table_formatter.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.760331 recline-2023.5/recline/repl/__init__.py
+-rw-r--r--   0        0        0     7969 2023-05-23 11:23:51.760331 recline-2023.5/recline/repl/completer.py
+-rw-r--r--   0        0        0     9527 2023-05-23 11:23:51.760331 recline-2023.5/recline/repl/shell.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/__init__.py
+-rw-r--r--   0        0        0    10174 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/argcomplete/LICENSE.rst
+-rw-r--r--   0        0        0    29936 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/argcomplete/__init__.py
+-rw-r--r--   0        0        0     1810 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/argcomplete/_check_module.py
+-rw-r--r--   0        0        0     2987 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/argcomplete/bash_completion.d/python-argcomplete.sh
+-rw-r--r--   0        0        0      524 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/argcomplete/compat.py
+-rw-r--r--   0        0        0     3681 2023-05-23 11:23:51.760331 recline-2023.5/recline/vendor/argcomplete/completers.py
+-rw-r--r--   0        0        0    15351 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/argcomplete/my_argparse.py
+-rw-r--r--   0        0        0    13218 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/argcomplete/my_shlex.py
+-rw-r--r--   0        0        0     3072 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/argcomplete/shellintegration.py
+-rw-r--r--   0        0        0     1084 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/docstring_parser/LICENSE
+-rw-r--r--   0        0        0       86 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/docstring_parser/__init__.py
+-rw-r--r--   0        0        0      808 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/docstring_parser/parser/__init__.py
+-rw-r--r--   0        0        0     3942 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/docstring_parser/parser/common.py
+-rw-r--r--   0        0        0     4164 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/docstring_parser/parser/google.py
+-rw-r--r--   0        0        0     1571 2023-05-23 11:23:51.764331 recline-2023.5/recline/vendor/docstring_parser/parser/rest.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.764331 recline-2023.5/tests/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-23 11:23:51.764331 recline-2023.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_arg_types/__init__.py
+-rw-r--r--   0        0        0     2034 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_arg_types/test_choices.py
+-rw-r--r--   0        0        0      989 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_arg_types/test_cliche_type.py
+-rw-r--r--   0        0        0     1723 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_arg_types/test_positional.py
+-rw-r--r--   0        0        0     1020 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_arg_types/test_ranged_int.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_commands/test_async_command.py
+-rw-r--r--   0        0        0     3541 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_commands/test_builtin_commands.py
+-rw-r--r--   0        0        0     4811 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_commands/test_cli_command.py
+-rw-r--r--   0        0        0     3553 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_commands/test_man_utils.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_formatters/__init__.py
+-rw-r--r--   0        0        0     1223 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_formatters/test_table_formatter.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_repl/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_repl/test_completer.py
+-rw-r--r--   0        0        0     4288 2023-05-23 11:23:51.764331 recline-2023.5/tests/test_repl/test_shell.py
+-rw-r--r--   0        0        0     6180 1970-01-01 00:00:00.000000 recline-2023.5/PKG-INFO
```

### Comparing `recline-2023.2/LICENSE` & `recline-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `recline-2023.2/README.md` & `recline-2023.5/README.md`

 * *Files identical despite different names*

### Comparing `recline-2023.2/pyproject.toml` & `recline-2023.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "recline"
-version = "2023.2"
+version = "2023.5"
 description = "Writing argparse-based command line applications can become tedious, repetitive, and difficult to do right. Relax and let this library free you from that burden."
 license = "BSD-3-Clause"
 authors = ["NetApp <ng-netapp-oss@netapp.com>"]
 readme = "README.md"
 
 homepage = "https://github.com/NetApp/recline"
 repository = "https://github.com/NetApp/recline"
```

### Comparing `recline-2023.2/recline/arg_types/__init__.py` & `recline-2023.5/recline/arg_types/__init__.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/choices.py` & `recline-2023.5/recline/arg_types/choices.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/flag.py` & `recline-2023.5/recline/arg_types/flag.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/positional.py` & `recline-2023.5/recline/arg_types/positional.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/ranged_int.py` & `recline-2023.5/recline/arg_types/ranged_int.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/recline_type.py` & `recline-2023.5/recline/arg_types/recline_type.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/recline_type_error.py` & `recline-2023.5/recline/arg_types/recline_type_error.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/arg_types/remainder.py` & `recline-2023.5/recline/arg_types/remainder.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/commands/async_command.py` & `recline-2023.5/recline/commands/async_command.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/commands/builtin_commands.py` & `recline-2023.5/recline/commands/builtin_commands.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/commands/cli_command.py` & `recline-2023.5/recline/commands/cli_command.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/commands/man_utils.py` & `recline-2023.5/recline/commands/man_utils.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/formatters/output_formatter.py` & `recline-2023.5/recline/formatters/output_formatter.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/formatters/table_formatter.py` & `recline-2023.5/recline/formatters/table_formatter.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/repl/completer.py` & `recline-2023.5/recline/repl/completer.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/repl/shell.py` & `recline-2023.5/recline/repl/shell.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/LICENSE.rst` & `recline-2023.5/recline/vendor/argcomplete/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/__init__.py` & `recline-2023.5/recline/vendor/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/_check_module.py` & `recline-2023.5/recline/vendor/argcomplete/_check_module.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/bash_completion.d/python-argcomplete.sh` & `recline-2023.5/recline/vendor/argcomplete/bash_completion.d/python-argcomplete.sh`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/compat.py` & `recline-2023.5/recline/vendor/argcomplete/compat.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/completers.py` & `recline-2023.5/recline/vendor/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/my_argparse.py` & `recline-2023.5/recline/vendor/argcomplete/my_argparse.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/my_shlex.py` & `recline-2023.5/recline/vendor/argcomplete/my_shlex.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/argcomplete/shellintegration.py` & `recline-2023.5/recline/vendor/argcomplete/shellintegration.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/docstring_parser/LICENSE` & `recline-2023.5/recline/vendor/docstring_parser/LICENSE`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/docstring_parser/parser/__init__.py` & `recline-2023.5/recline/vendor/docstring_parser/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/docstring_parser/parser/common.py` & `recline-2023.5/recline/vendor/docstring_parser/parser/common.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/docstring_parser/parser/google.py` & `recline-2023.5/recline/vendor/docstring_parser/parser/google.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/recline/vendor/docstring_parser/parser/rest.py` & `recline-2023.5/recline/vendor/docstring_parser/parser/rest.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_arg_types/test_choices.py` & `recline-2023.5/tests/test_arg_types/test_choices.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_arg_types/test_cliche_type.py` & `recline-2023.5/tests/test_arg_types/test_cliche_type.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_arg_types/test_positional.py` & `recline-2023.5/tests/test_arg_types/test_positional.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_arg_types/test_ranged_int.py` & `recline-2023.5/tests/test_arg_types/test_ranged_int.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_commands/test_async_command.py` & `recline-2023.5/tests/test_commands/test_async_command.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_commands/test_builtin_commands.py` & `recline-2023.5/tests/test_commands/test_builtin_commands.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_commands/test_cli_command.py` & `recline-2023.5/tests/test_commands/test_cli_command.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_commands/test_man_utils.py` & `recline-2023.5/tests/test_commands/test_man_utils.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_formatters/test_table_formatter.py` & `recline-2023.5/tests/test_formatters/test_table_formatter.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_repl/test_completer.py` & `recline-2023.5/tests/test_repl/test_completer.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/tests/test_repl/test_shell.py` & `recline-2023.5/tests/test_repl/test_shell.py`

 * *Files identical despite different names*

### Comparing `recline-2023.2/setup.py` & `recline-2023.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,183 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: recline
+Version: 2023.5
+Summary: Writing argparse-based command line applications can become tedious, repetitive, and difficult to do right. Relax and let this library free you from that burden.
+Home-page: https://github.com/NetApp/recline
+License: BSD-3-Clause
+Keywords: cli,interactive,shell,argparse,recline
+Author: NetApp
+Author-email: ng-netapp-oss@netapp.com
+Requires-Python: >=3.7.2,<4
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Shells
+Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; sys_platform == "win32"
+Requires-Dist: windows-curses (>=2.3.0,<3.0.0) ; sys_platform == "win32"
+Project-URL: Documentation, https://netapp.github.io/recline
+Project-URL: Repository, https://github.com/NetApp/recline
+Description-Content-Type: text/markdown
+
+![](https://github.com/NetApp/recline/workflows/build/badge.svg?branch=main)
+[![Gitter](https://badges.gitter.im/netapp-recline/community.svg)](https://gitter.im/netapp-recline/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+
+# recline
+
+Writing argparse-based command line applications can become tedious, repetitive,
+and difficult to do right. Relax and let this library free you from that burden.
+
+This library helps you quickly implement an interactive command-based application in Python.
+
+## Documentation First
+We all know that writing documentation is very important and yet it can easily become
+and afterthought or a nice to have if we're not diligent. This is often because it
+means duplicating a piece of your implementation in words, effectively writing the
+same thing twice. Recline strives to deduplicate this work by taking a documentation
+first attitude where your documentation _becomes_ the implementation without additional
+work from you.
+
+## Interactive
+
+The default mode is to run a REPL interface where a prompt is given to the user, the
+user types one of the available commands, the application processes it, displays the
+result, and then control is returned to the user once more.
+
+But if your user isn't expected to or doesn't always want to run multiple commands,
+you also get a more traditional command-line interface for free.
+
+## Command-based
+
+The application will be command based. Each command will have one or more words
+that identify the command. It may also have one or more arguments that augment or
+vary the action that command will take.
+
+## Batteries included
+
+While the library is designed to be easy to implement for simple or small applications,
+it also comes with full power features for larger use cases including:
+
+* Tab completion
+* Input verification
+* Output formatting
+* Debugger integration
+
+# Before getting started
+
+Some things to consider and prepare before you can use this library.
+
+## Software requirements
+
+```
+1. Python 3.5 or later
+```
+
+## Installing and importing the library
+
+You can install the package [from pypi](https://pypi.org/project/recline) using the pip utility:
+
+```
+pip install recline
+```
+
+You can then import the library into your application:
+
+```python
+import recline
+```
+
+# Quick Start
+
+After installing the package, you can get started with a few lines in `hello.py`:
+
+```python
+import recline
+
+@recline.command
+def hello(name: str = None) -> None:
+    """A basic hello world
+
+    You can greet just about anybody with this command if they give you their name!
+
+    Args:
+        name: If a name is provided, the greeting will be more personal
+    """
+    response = "I'm at your command"
+    if name:
+        response += ", %s" % name
+    print(response)
+
+recline.relax()
+```
+
+## Interactive mode
+
+The default mode when a recline applciation is run is an interactive style. Running
+our above `hello.py` results in the following output:
+
+```
+$ python hello.py
+> help
+Available Commands:
+
+hello - A basic hello world You can greet just about anybody with this command if
+
+Built-in Commands
+-----------------
+exit - Exit the application
+help - Display a list of available commands and their short description
+man - Display the full man page for a given command
+> hello ?
+A basic hello world You can greet just about anybody with this command if
+
+Optional arguments:
+  -name <name> If a name is provided, the greeting will be more personal
+    Default: None
+> hello
+I'm at your command
+> hello -name Dave
+I'm at your command, Dave
+> exit
+$
+```
+
+## Non-interactive mode
+
+If you would like to use the application as part of a larger script, it is much
+easier to do in a non-interactive way. This is also possible using recline without
+needing to change the application. Here's an example:
+
+```
+$ python hello.py -c "hello -name Dave"
+I'm at your command, Dave
+$
+```
+
+See the [full documentation](https://netapp.github.io/recline) for more advanced usages and examples
+
+# Contributing [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/NetApp/recline/issues)
+
+You may read about the contribution process including how to build and test your changes [here](CONTRIBUTING.md).
+
+# Why recline?
+
+There are a large number of different command line libraries on PyPi and GitHub.
+And some of them have the same sort of decorator design. Most, however, are missing
+the interactive elements that recline focuses on (tab completion, command chaining,
+background jobs, man pages). If you're still looking for the right fit for your
+application and recline isn't it, you can check out these other fine projects (in no
+particular order):
+
+* https://github.com/kootenpv/cliche
+* https://github.com/gowithfloat/clippy
+* https://github.com/epsy/clize
+* https://github.com/pallets/click
+* https://github.com/micheles/plac
+* https://github.com/google/python-fire
+* https://github.com/kennethreitz-archive/clint
+* https://docs.openstack.org/cliff/latest
+* https://github.com/miguelgrinberg/climax
 
-packages = \
-['recline',
- 'recline.arg_types',
- 'recline.commands',
- 'recline.formatters',
- 'recline.repl',
- 'recline.vendor',
- 'recline.vendor.argcomplete',
- 'recline.vendor.docstring_parser',
- 'recline.vendor.docstring_parser.parser',
- 'tests',
- 'tests.test_arg_types',
- 'tests.test_commands',
- 'tests.test_formatters',
- 'tests.test_repl']
-
-package_data = \
-{'': ['*'], 'recline.vendor.argcomplete': ['bash_completion.d/*']}
-
-extras_require = \
-{':sys_platform == "win32"': ['windows-curses>=2.3.0,<3.0.0',
-                              'pyreadline3>=3.4.1,<4.0.0']}
-
-setup_kwargs = {
-    'name': 'recline',
-    'version': '2023.2',
-    'description': 'Writing argparse-based command line applications can become tedious, repetitive, and difficult to do right. Relax and let this library free you from that burden.',
-    'long_description': '![](https://github.com/NetApp/recline/workflows/build/badge.svg?branch=main)\n[![Gitter](https://badges.gitter.im/netapp-recline/community.svg)](https://gitter.im/netapp-recline/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)\n\n# recline\n\nWriting argparse-based command line applications can become tedious, repetitive,\nand difficult to do right. Relax and let this library free you from that burden.\n\nThis library helps you quickly implement an interactive command-based application in Python.\n\n## Documentation First\nWe all know that writing documentation is very important and yet it can easily become\nand afterthought or a nice to have if we\'re not diligent. This is often because it\nmeans duplicating a piece of your implementation in words, effectively writing the\nsame thing twice. Recline strives to deduplicate this work by taking a documentation\nfirst attitude where your documentation _becomes_ the implementation without additional\nwork from you.\n\n## Interactive\n\nThe default mode is to run a REPL interface where a prompt is given to the user, the\nuser types one of the available commands, the application processes it, displays the\nresult, and then control is returned to the user once more.\n\nBut if your user isn\'t expected to or doesn\'t always want to run multiple commands,\nyou also get a more traditional command-line interface for free.\n\n## Command-based\n\nThe application will be command based. Each command will have one or more words\nthat identify the command. It may also have one or more arguments that augment or\nvary the action that command will take.\n\n## Batteries included\n\nWhile the library is designed to be easy to implement for simple or small applications,\nit also comes with full power features for larger use cases including:\n\n* Tab completion\n* Input verification\n* Output formatting\n* Debugger integration\n\n# Before getting started\n\nSome things to consider and prepare before you can use this library.\n\n## Software requirements\n\n```\n1. Python 3.5 or later\n```\n\n## Installing and importing the library\n\nYou can install the package [from pypi](https://pypi.org/project/recline) using the pip utility:\n\n```\npip install recline\n```\n\nYou can then import the library into your application:\n\n```python\nimport recline\n```\n\n# Quick Start\n\nAfter installing the package, you can get started with a few lines in `hello.py`:\n\n```python\nimport recline\n\n@recline.command\ndef hello(name: str = None) -> None:\n    """A basic hello world\n\n    You can greet just about anybody with this command if they give you their name!\n\n    Args:\n        name: If a name is provided, the greeting will be more personal\n    """\n    response = "I\'m at your command"\n    if name:\n        response += ", %s" % name\n    print(response)\n\nrecline.relax()\n```\n\n## Interactive mode\n\nThe default mode when a recline applciation is run is an interactive style. Running\nour above `hello.py` results in the following output:\n\n```\n$ python hello.py\n> help\nAvailable Commands:\n\nhello - A basic hello world You can greet just about anybody with this command if\n\nBuilt-in Commands\n-----------------\nexit - Exit the application\nhelp - Display a list of available commands and their short description\nman - Display the full man page for a given command\n> hello ?\nA basic hello world You can greet just about anybody with this command if\n\nOptional arguments:\n  -name <name> If a name is provided, the greeting will be more personal\n    Default: None\n> hello\nI\'m at your command\n> hello -name Dave\nI\'m at your command, Dave\n> exit\n$\n```\n\n## Non-interactive mode\n\nIf you would like to use the application as part of a larger script, it is much\neasier to do in a non-interactive way. This is also possible using recline without\nneeding to change the application. Here\'s an example:\n\n```\n$ python hello.py -c "hello -name Dave"\nI\'m at your command, Dave\n$\n```\n\nSee the [full documentation](https://netapp.github.io/recline) for more advanced usages and examples\n\n# Contributing [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/NetApp/recline/issues)\n\nYou may read about the contribution process including how to build and test your changes [here](CONTRIBUTING.md).\n\n# Why recline?\n\nThere are a large number of different command line libraries on PyPi and GitHub.\nAnd some of them have the same sort of decorator design. Most, however, are missing\nthe interactive elements that recline focuses on (tab completion, command chaining,\nbackground jobs, man pages). If you\'re still looking for the right fit for your\napplication and recline isn\'t it, you can check out these other fine projects (in no\nparticular order):\n\n* https://github.com/kootenpv/cliche\n* https://github.com/gowithfloat/clippy\n* https://github.com/epsy/clize\n* https://github.com/pallets/click\n* https://github.com/micheles/plac\n* https://github.com/google/python-fire\n* https://github.com/kennethreitz-archive/clint\n* https://docs.openstack.org/cliff/latest\n* https://github.com/miguelgrinberg/climax\n',
-    'author': 'NetApp',
-    'author_email': 'ng-netapp-oss@netapp.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/NetApp/recline',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.2,<4',
-}
-
-
-setup(**setup_kwargs)
```

