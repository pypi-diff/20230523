# Comparing `tmp/oregpt-0.1.3.tar.gz` & `tmp/oregpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oregpt-0.1.3.tar", max compression
+gzip compressed data, was "oregpt-0.2.0.tar", max compression
```

## Comparing `oregpt-0.1.3.tar` & `oregpt-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1076 2023-05-07 04:09:40.942289 oregpt-0.1.3/LICENSE
--rw-r--r--   0        0        0     2612 2023-05-15 11:00:22.153239 oregpt-0.1.3/README.md
--rw-r--r--   0        0        0     2116 2023-05-15 00:57:48.021998 oregpt-0.1.3/oregpt/chat_bot.py
--rw-r--r--   0        0        0     3647 2023-05-15 11:00:22.153431 oregpt-0.1.3/oregpt/command.py
--rw-r--r--   0        0        0     2077 2023-05-15 11:00:22.153598 oregpt-0.1.3/oregpt/main.py
--rw-r--r--   0        0        0      304 2023-05-07 08:41:56.348724 oregpt-0.1.3/oregpt/resources/config.yml
--rw-r--r--   0        0        0     2352 2023-05-15 00:57:48.022534 oregpt-0.1.3/oregpt/stdinout.py
--rw-r--r--   0        0        0     2117 2023-05-15 11:00:30.334307 oregpt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 04:09:40.943569 oregpt-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1290 2023-05-15 11:00:22.153925 oregpt-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     1765 2023-05-15 11:00:22.154075 oregpt-0.1.3/tests/test_chat_bot.py
--rw-r--r--   0        0        0     1425 2023-05-15 11:00:22.154223 oregpt-0.1.3/tests/test_command.py
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 oregpt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 04:09:40.942289 oregpt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2931 2023-05-22 23:45:15.320328 oregpt-0.2.0/README.md
+-rw-r--r--   0        0        0     2258 2023-05-22 23:42:21.940062 oregpt-0.2.0/oregpt/chat_bot.py
+-rw-r--r--   0        0        0     3647 2023-05-22 23:42:21.940259 oregpt-0.2.0/oregpt/command.py
+-rw-r--r--   0        0        0     3163 2023-05-22 23:42:21.940425 oregpt-0.2.0/oregpt/main.py
+-rw-r--r--   0        0        0      339 2023-05-22 23:42:21.940590 oregpt-0.2.0/oregpt/resources/config.yml
+-rw-r--r--   0        0        0     2352 2023-05-22 13:07:43.877240 oregpt-0.2.0/oregpt/stdinout.py
+-rw-r--r--   0        0        0     2134 2023-05-22 23:45:26.313793 oregpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 04:09:40.943569 oregpt-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1338 2023-05-22 23:42:21.941494 oregpt-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1796 2023-05-22 23:42:21.941642 oregpt-0.2.0/tests/test_chat_bot.py
+-rw-r--r--   0        0        0     1430 2023-05-22 23:42:21.941784 oregpt-0.2.0/tests/test_command.py
+-rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 oregpt-0.2.0/PKG-INFO
```

### Comparing `oregpt-0.1.3/LICENSE` & `oregpt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oregpt-0.1.3/README.md` & `oregpt-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,26 +29,37 @@
 
 ## Usage
 Once you have installed oregpt, you can run it by typing:
 ```bash
 $ oregpt
 ```
 
+There are a few options:
+```bash
+$ oregpt --help
+Usage: oregpt [OPTIONS]
+
+Options:
+  -m, --model_name TEXT      Model name in OpenAI (e.g, gpt-3.5-turbo, gpt-4)
+  -a, --assistant_role TEXT  Role setting for Assistant (AI)
+  --help                     Show this message and exit.
+```
+
 ## Supported commands on chat
 Commands such as saving and loading conversations are available as the following:
 
 |  Command  |  Description  |
 | ---- | ---- |
 | `/exit`    | Exit from this chat tool |
 | `/quit`    | Exit from this chat tool |
 | `/q`       | Exit from this chat tool |
 | `/clear`   | Clear chat history all |
 | `/history` | Show chat history in json format |
-| `/save`    | Save chat hisotry in json format |
-| `/load`    | Load chat hisotry from a json file |
+| `/save`    | Save chat history in json format |
+| `/load`    | Load chat history from a json file |
 | `/help`    | Show all commands which you can use in this chat tool |
 
 ## Configuration
 You can specify the place of conversation `log`,
 [style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
 and
 [the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
@@ -60,14 +71,15 @@
     model: gpt-3.5-turbo
 # You can also specify OpenAI's API key here
 #     api_key: <your-api-key>
 character:
     user:
         name: Me
         style: "#00BEFE"
+        role: "You are a chat bot"
     assistant:
         name: AI
         style: "#87CEEB"
     system:
         name: System
         style: "#cc0000"
 ```
```

### Comparing `oregpt-0.1.3/oregpt/chat_bot.py` & `oregpt-0.2.0/oregpt/chat_bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 
 import openai
 
 from oregpt.stdinout import StdInOut
 
 
 class ChatBot:
-    SYSTEM_ROLE = [{"role": "system", "content": "You are a chat bot"}]
-
-    def __init__(self, model: str, std_in_out: StdInOut):
+    def __init__(self, model: str, assistant_role: str, std_in_out: StdInOut):
         self._std_in_out = std_in_out
         # Model list: gpt-4, gpt-4-0314, gpt-4-32k, gpt-4-32k-0314, gpt-3.5-turbo, gpt-3.5-turbo-0301
         # https://platform.openai.com/docs/models/overview
         self._model = model
-
+        self._assistant_role = [{"role": "system", "content": assistant_role}]
         self._initialize_log()
 
     def _initialize_log(self) -> None:
-        self._log: list[dict[str, str]] = deepcopy(ChatBot.SYSTEM_ROLE)
+        self._log: list[dict[str, str]] = deepcopy(self._assistant_role)
 
     @property
     def model(self) -> str:
         return self._model
 
     @property
+    def assistant_role(self) -> list[dict[str, str]]:
+        return deepcopy(self._assistant_role)
+
+    @property
     def log(self) -> list[dict[str, str]]:
         return self._log
 
     @property
     def std_in_out(self) -> StdInOut:
         return self._std_in_out
```

### Comparing `oregpt-0.1.3/oregpt/command.py` & `oregpt-0.2.0/oregpt/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 def _abspath(x: str) -> str:
     return os.path.abspath(os.path.expanduser(x))
 
 
 @register
 class SaveCommand(Command):
-    """Save chat hisotry in json format"""
+    """Save chat history in json format"""
 
     representations: list[str] = ["save"]
 
     def execute(self) -> None:
         file_name = ""
         if len(self._args) == 1:
             file_name = _abspath(self._args[0].strip())
@@ -103,15 +103,15 @@
         directory.mkdir(parents=True, exist_ok=True)
         self._bot.save(file_name)
         self._bot.std_in_out.print_system(f"Save all conversation history in {file_name}")
 
 
 @register
 class LoadCommand(Command):
-    """Load chat hisotry from a json file"""
+    """Load chat history from a json file"""
 
     representations: list[str] = ["load"]
 
     def execute(self) -> None:
         print(self._args)
         if len(self._args) != 1:
             self._bot.std_in_out.print_system("Loaded file was not specified as an argument")
```

### Comparing `oregpt-0.1.3/oregpt/main.py` & `oregpt-0.2.0/oregpt/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pathlib
 import shutil
-from typing import Any
+from enum import Enum
+from typing import Any, Optional
 
+import click
 import openai
 import yaml
 
 from oregpt.chat_bot import ChatBot
 from oregpt.command import CommandBuilder
 from oregpt.stdinout import StdInOut
 
@@ -30,35 +32,60 @@
     if value := os.getenv("OPENAI_API_KEY"):
         openai.api_key = value
         return
 
     raise LookupError("OpenAI's API key was not found in config.yml and environment variables")
 
 
-def main() -> int:
+class Status(Enum):
+    USER = 1
+    BOT = 2
+
+
+def prefer_left(lhs: str, rhs: Optional[str]) -> str:
+    if lhs != "":
+        return lhs
+    if rhs is not None:
+        return rhs
+    raise Exception("Set as an argument or in ~/.config/oregpt/config.yml")
+
+
+# Add "type: ignore" to avoid this https://github.com/python/typeshed/issues/6156
+@click.command()  # type: ignore
+@click.option("--model_name", "-m", type=str, help="Model name in OpenAI (e.g, gpt-3.5-turbo, gpt-4)", default="")  # type: ignore
+@click.option("--assistant_role", "-a", type=str, help="Role setting for Assistant (AI)", default="")  # type: ignore
+def main(model_name: str, assistant_role: str) -> int:
     config = load_config()
     initialize_open_ai_key(config["openai"])
+    model_name = prefer_left(model_name, config["openai"].get("model"))
+    assistant_role = prefer_left(assistant_role, config["character"]["assistant"].get("role"))
     std_in_out = StdInOut(config["character"], lambda: "To exit, type /q, /quit, /exit, or Ctrl + C")
-    bot = ChatBot(config["openai"]["model"], std_in_out)
+    bot = ChatBot(model_name, assistant_role, std_in_out)
     command_builder = CommandBuilder(config, bot)
 
-    try:
-        while True:
+    while True:
+        try:
+            status = Status.USER
             message = std_in_out.input().lower()
             if command := command_builder.build(message):
                 command.execute()
             else:
+                status = Status.BOT
                 if command_builder.looks_like_command(message):
                     std_in_out.print_system("Invalid command. Valid commands are as the following:")
                     command_builder.build("/help").execute()  # type: ignore
                 else:
                     bot.respond(message)
-    except KeyboardInterrupt:
-        return 0
-    except Exception as e:
-        raise Exception(f"Something happened: {str(e)}") from e
+        except KeyboardInterrupt:
+            if status == Status.BOT:
+                std_in_out.print_assistant("\n")
+            else:
+                return 0
+        except Exception as e:
+            raise Exception(f"Something happened: {str(e)}") from e
+            return 1
 
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `oregpt-0.1.3/oregpt/stdinout.py` & `oregpt-0.2.0/oregpt/stdinout.py`

 * *Files identical despite different names*

### Comparing `oregpt-0.1.3/pyproject.toml` & `oregpt-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oregpt"
-version = "0.1.3"
+version = "0.2.0"
 description = "A tiny GPT CLI tool"
 authors = ["Shinichi Takayanagi <shinichi.takayanagi@gmail.com>"]
 homepage = "https://github.com/shinichi-takayanagi/oregpt"
 repository = "https://github.com/shinichi-takayanagi/oregpt"
 license = "MIT"
 readme = "README.md"
 keywords = ["gpt-chatbot", "gpt-cli", "openai-cli"]
@@ -25,14 +25,15 @@
 oregpt = "oregpt.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.6"
 pyyaml = "^6.0"
 prompt-toolkit = "^3.0.38"
+click = "^8.1.3"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `oregpt-0.1.3/tests/conftest.py` & `oregpt-0.2.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # https://stackoverflow.com/a/42156088/3926333
 class Helpers:
     @staticmethod
     def make_std_in_out():
         return StdInOut({}, lambda: "Dummy")
 
     @staticmethod
-    def make_chat_bot(name: str):
-        return ChatBot(name, Helpers.make_std_in_out())
+    def make_chat_bot(name: str, role: str):
+        return ChatBot(name, role, Helpers.make_std_in_out())
 
 
 @pytest.fixture
 def helpers():
     return Helpers
 
 
@@ -41,8 +41,8 @@
     @contextlib.contextmanager
     def _print_as_contextmanager(*args, **kwargs):
         yield
 
     monkeypatch.setattr(ChatCompletion, "create", _create)
     monkeypatch.setattr(StdInOut, "_print", _print)
     monkeypatch.setattr(StdInOut, "print_assistant_thinking", _print_as_contextmanager)
-    return helpers.make_chat_bot("Yes")
+    return helpers.make_chat_bot("THE AI", "You are a great chat bot")
```

### Comparing `oregpt-0.1.3/tests/test_chat_bot.py` & `oregpt-0.2.0/tests/test_chat_bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,58 @@
 import json
 
 import pytest
 
-from oregpt.chat_bot import ChatBot
-
 
 @pytest.fixture
 def tmp_file(tmpdir_factory):
     return tmpdir_factory.mktemp("data").join("test.json")
 
 
 def test_initialized_property(helpers):
-    bot = helpers.make_chat_bot("THE AI")
+    bot = helpers.make_chat_bot("THE AI", "You are a bot")
     assert bot.model == "THE AI"
-    assert bot.log == ChatBot.SYSTEM_ROLE
+    assert bot.log == bot.assistant_role
 
 
 def test_respond_and_log(patched_bot):
     what_user_said = "Hello, world"
-    assert patched_bot.log == ChatBot.SYSTEM_ROLE
+    assert patched_bot.log == patched_bot.assistant_role
     assert pytest.DUMMY_CONTENT == patched_bot.respond(what_user_said)
-    assert patched_bot.log == ChatBot.SYSTEM_ROLE + [
+    assert patched_bot.log == patched_bot.assistant_role + [
         {"role": "user", "content": what_user_said},
         {"role": "assistant", "content": pytest.DUMMY_CONTENT},
     ]
 
 
 def test_save(tmp_file, patched_bot):
     what_user_said = "Hello, world???"
     patched_bot.respond(what_user_said)
     patched_bot.save(str(tmp_file))
 
     with tmp_file.open("r") as file:
         assert patched_bot.log == json.load(file)
-        assert patched_bot.log == ChatBot.SYSTEM_ROLE + [
+        assert patched_bot.log == patched_bot.assistant_role + [
             {"role": "user", "content": what_user_said},
             {"role": "assistant", "content": pytest.DUMMY_CONTENT},
         ]
 
 
 def test_load(tmp_file, patched_bot, helpers):
     what_user_said = "Hello, world"
     patched_bot.respond(what_user_said)
     patched_bot.save(str(tmp_file))
 
-    bot = helpers.make_chat_bot("THE AI")
+    bot = helpers.make_chat_bot("THE AI", "You are a bot")
     bot.load(tmp_file)
     assert bot.log == patched_bot.log
 
 
 def test_clear(patched_bot):
     what_user_said = "Hello, world"
     patched_bot.respond(what_user_said)
-    assert patched_bot.log == ChatBot.SYSTEM_ROLE + [
+    assert patched_bot.log == patched_bot.assistant_role + [
         {"role": "user", "content": what_user_said},
         {"role": "assistant", "content": pytest.DUMMY_CONTENT},
     ]
     patched_bot.clear()
-    assert patched_bot._log == ChatBot.SYSTEM_ROLE
+    assert patched_bot._log == patched_bot.assistant_role
```

### Comparing `oregpt-0.1.3/tests/test_command.py` & `oregpt-0.2.0/tests/test_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import pytest
 
-from oregpt.chat_bot import ChatBot
 from oregpt.command import (
     ClearCommand,
     CommandBuilder,
     ExitCommand,
     HelpCommand,
     HistoryCommand,
     LoadCommand,
     SaveCommand,
 )
 
 
 def test_command_builder_build(helpers):
-    command_builder = CommandBuilder({}, helpers.make_chat_bot("Yahoo"))
+    command_builder = CommandBuilder({}, helpers.make_chat_bot("Yahoo", "You are a bot"))
     for command_type in [ExitCommand, ClearCommand, HistoryCommand, SaveCommand, LoadCommand, HelpCommand]:
         for representation in command_type.representations:
             assert isinstance(command_builder.build(f"/{representation}"), command_type)
 
 
 def test_command_builder_looks_like_command(helpers):
-    command_builder = CommandBuilder({}, helpers.make_chat_bot("Yahoo"))
+    command_builder = CommandBuilder({}, helpers.make_chat_bot("Yahoo", "You are a bot"))
     assert command_builder.looks_like_command("/hoge hoge") == True
     assert command_builder.looks_like_command("/hoge") == True
     assert command_builder.looks_like_command("/") == True
     assert command_builder.looks_like_command("hoge hoge") == False
     assert command_builder.looks_like_command("hoge") == False
     assert command_builder.looks_like_command("") == False
 
@@ -35,8 +34,8 @@
         command.execute()
 
 
 def test_clear_command(patched_bot):
     cl = ClearCommand({}, patched_bot, [])
     patched_bot.respond("Hi, bot-san")
     cl.execute()
-    assert patched_bot.log == ChatBot.SYSTEM_ROLE
+    assert patched_bot.log == patched_bot.assistant_role
```

### Comparing `oregpt-0.1.3/PKG-INFO` & `oregpt-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: oregpt
-Version: 0.1.3
+Version: 0.2.0
 Summary: A tiny GPT CLI tool
 Home-page: https://github.com/shinichi-takayanagi/oregpt
 License: MIT
 Keywords: gpt-chatbot,gpt-cli,openai-cli
 Author: Shinichi Takayanagi
 Author-email: shinichi.takayanagi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: openai (>=0.27.6,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/shinichi-takayanagi/oregpt
 Description-Content-Type: text/markdown
 
 # oregpt
@@ -52,26 +53,37 @@
 
 ## Usage
 Once you have installed oregpt, you can run it by typing:
 ```bash
 $ oregpt
 ```
 
+There are a few options:
+```bash
+$ oregpt --help
+Usage: oregpt [OPTIONS]
+
+Options:
+  -m, --model_name TEXT      Model name in OpenAI (e.g, gpt-3.5-turbo, gpt-4)
+  -a, --assistant_role TEXT  Role setting for Assistant (AI)
+  --help                     Show this message and exit.
+```
+
 ## Supported commands on chat
 Commands such as saving and loading conversations are available as the following:
 
 |  Command  |  Description  |
 | ---- | ---- |
 | `/exit`    | Exit from this chat tool |
 | `/quit`    | Exit from this chat tool |
 | `/q`       | Exit from this chat tool |
 | `/clear`   | Clear chat history all |
 | `/history` | Show chat history in json format |
-| `/save`    | Save chat hisotry in json format |
-| `/load`    | Load chat hisotry from a json file |
+| `/save`    | Save chat history in json format |
+| `/load`    | Load chat history from a json file |
 | `/help`    | Show all commands which you can use in this chat tool |
 
 ## Configuration
 You can specify the place of conversation `log`,
 [style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
 and
 [the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
@@ -83,14 +95,15 @@
     model: gpt-3.5-turbo
 # You can also specify OpenAI's API key here
 #     api_key: <your-api-key>
 character:
     user:
         name: Me
         style: "#00BEFE"
+        role: "You are a chat bot"
     assistant:
         name: AI
         style: "#87CEEB"
     system:
         name: System
         style: "#cc0000"
 ```
```

