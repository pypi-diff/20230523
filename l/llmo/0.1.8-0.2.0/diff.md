# Comparing `tmp/llmo-0.1.8.tar.gz` & `tmp/llmo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.1.8.tar", last modified: Mon May 22 22:30:09 2023, max compression
+gzip compressed data, was "llmo-0.2.0.tar", last modified: Tue May 23 03:58:25 2023, max compression
```

## Comparing `llmo-0.1.8.tar` & `llmo-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.1.8/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.1.8/llmo/__init__.py
--rw-r--r--   0        0        0     2898 2023-05-22 22:11:47.649149 llmo-0.1.8/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.1.8/llmo/constants.py
--rw-r--r--   0        0        0     9299 2023-05-22 22:11:47.653617 llmo-0.1.8/llmo/gui.py
--rw-r--r--   0        0        0      353 2023-05-21 18:43:49.180818 llmo-0.1.8/llmo/layout.css
--rw-r--r--   0        0        0     5878 2023-05-22 21:51:03.478418 llmo-0.1.8/llmo/llms.py
--rw-r--r--   0        0        0     1045 2023-05-22 22:03:50.352845 llmo-0.1.8/llmo/shell_mode.py
--rw-r--r--   0        0        0      699 2023-05-22 22:30:09.099067 llmo-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.1.8/tests/test_openai.py
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.2.0/llmo/__init__.py
+-rw-r--r--   0        0        0     2898 2023-05-22 22:11:47.649149 llmo-0.2.0/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.2.0/llmo/constants.py
+-rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.2.0/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.2.0/llmo/layout.css
+-rw-r--r--   0        0        0     5982 2023-05-23 03:45:21.644631 llmo-0.2.0/llmo/llms.py
+-rw-r--r--   0        0        0     1045 2023-05-22 22:03:50.352845 llmo-0.2.0/llmo/shell_mode.py
+-rw-r--r--   0        0        0      699 2023-05-23 03:58:25.722045 llmo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.2.0/tests/test_openai.py
+-rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 llmo-0.2.0/PKG-INFO
```

### Comparing `llmo-0.1.8/LICENSE` & `llmo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.1.8/README.md` & `llmo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `llmo-0.1.8/llmo/cli.py` & `llmo-0.2.0/llmo/cli.py`

 * *Files identical despite different names*

### Comparing `llmo-0.1.8/llmo/gui.py` & `llmo-0.2.0/llmo/gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,36 @@
     Button,
     Header,
     TextLog,
     ContentSwitcher,
     Footer,
     LoadingIndicator,
     Markdown,
-    Select,
+    Select, Switch,
 )
 
 from llmo.constants import MODELS
 from llmo.llms import OpenAI
 
 
 class LLMInterface(Protocol):
+    has_personality: bool
+
     def submit(self, prompt: str, files: Iterable[Path] = None) -> str:
         ...
 
     async def asubmit(self, prompt: str, files: Iterable[Path] = None):
         ...
 
+    def add_personality(self) -> None:
+        ...
+
+    def remove_personality(self) -> None:
+        ...
+
 
 class LLMO(App):
     CSS_PATH = "layout.css"
     BINDINGS = [
         ("ctrl+z", "switch_tab", "Switch Tab"),
         ("ctrl+x", "reset_chat", "Reset Chat"),
         ("s", "stage_file", "Stage File"),
@@ -53,15 +61,15 @@
         rich_text_mode: bool = False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.staged_files = set(staged_files) if staged_files else set()
         self.prompt = prompt
         self.current_tab = current_tab
-        self.openai_client = llm_client or OpenAI()
+        self.llm_client = llm_client or OpenAI()
         self.selected_file = None
         self.rich_text_mode = rich_text_mode
         self.markdown = ""
 
     def on_mount(self):
         input_widget = self.query_one("#prompt", Input)
         input_widget.focus()
@@ -81,15 +89,15 @@
                 self.markdown,
                 id="response",
             )
 
         with Container(id="app"):
             yield Header()
 
-            with Horizontal(id="tabs"):
+            with Horizontal(id="tabs", classes="container"):
                 yield Button(
                     "Context",
                     id="context-choice-button",
                     variant="warning",
                 )
                 yield Button(
                     "Chat",
@@ -121,36 +129,42 @@
                                 *(ListItem(Label(str(k))) for k in self.staged_files),
                                 id="staged-files",
                             )
                             yield Markdown("## Model Settings")
                             yield Select(
                                 ((m, m) for m in MODELS),
                                 id="model-select",
-                                value=self.openai_client.model,
+                                value=self.llm_client.model,
                             )
                             yield Input(
-                                value=self.openai_client.api_key,
+                                value=self.llm_client.api_key,
                                 placeholder="API Key",
                                 password=True,
                                 id="api-key-input",
                             )
+                            yield Label("Personality: ")
+                            yield Switch(value=self.llm_client.has_personality, id="personality-switch")
 
                 with Vertical(id="chat"):
                     with VerticalScroll(id="scroll-area"):
                         yield response_view
                     yield Input(
                         placeholder="Type here",
                         id="prompt",
                     )
 
         yield Footer()
 
+    @on(Switch.Changed)
+    def toggle_personality(self, event: Switch.Changed) -> None:
+        self.llm_client.add_personality() if event.switch.value else self.llm_client.remove_personality()
+
     @on(Select.Changed)
     def select_changed(self, event: Select.Changed) -> None:
-        self.openai_client.model = str(event.value)
+        self.llm_client.model = str(event.value)
 
     def update_stage_file_button_variant(self):
         selected_file = self.selected_file
         stage_file_button = self.query_one("#stage-file-button", Button)
         if selected_file and selected_file not in self.staged_files:
             stage_file_button.variant = "success"
         else:
@@ -204,54 +218,54 @@
         response_view = self.query_one("#response")  # noqa
         if self.rich_text_mode:
             response_view: Markdown
             self.markdown = ""
             response_view.update(self.markdown)
         else:
             response_view: TextLog
-            self.openai_client.reset()
+            self.llm_client.reset()
             response_view.clear()
         # clear prompt
         self.query_one("#prompt", Input).value = ""
 
     def on_input_changed(self, event: Input.Changed):
         if event.input.id == "prompt":
             self.prompt = event.input.value
         elif event.input.id == "api-key-input":
-            self.openai_client.api_key = event.input.value
-            openai.api_key = self.openai_client.api_key
+            self.llm_client.api_key = event.input.value
+            openai.api_key = self.llm_client.api_key
         else:
             raise ValueError(f"Unknown input: {event.input.id}")
 
     async def on_input_submitted(self, _: Input.Submitted):
         await self.handle_submission()
 
     async def handle_submission(self):
         prompt_area = self.query_one("#prompt")
         loading_indicator = LoadingIndicator()
         await prompt_area.mount(loading_indicator)
 
         if not self.rich_text_mode:
             response = await asyncio.get_event_loop().run_in_executor(
                 None,
-                self.openai_client.submit,
+                self.llm_client.submit,
                 self.prompt,
                 self.staged_files,
             )
             log = self.query_one("#response", TextLog)
             log.write(f">> {self.prompt}\n")
             log.write(response)
             log.write("\n\n")
         else:
             scroll_area = self.query_one("#scroll-area")
             output = self.query_one("#response", Markdown)
             self.markdown += f"{self.prompt}"
             output.update(self.markdown)
             self.markdown += "\n---\n"
-            async for content in self.openai_client.asubmit(
+            async for content in self.llm_client.asubmit(
                 prompt=self.prompt,
                 files=self.staged_files,
             ):
                 self.markdown += content
                 output.update(self.markdown)
                 output.scroll_page_down()
                 scroll_area.scroll_page_down()
```

### Comparing `llmo-0.1.8/llmo/llms.py` & `llmo-0.2.0/llmo/llms.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,30 +25,34 @@
     model: str = "gpt-3.5-turbo"
     temperature: float = 0.7
     messages: deque[Message] = field(default_factory=deque)
     api_key: str = None
     system_prompt: str = (
         "You are an AI programming assistant named Elmo. "
         "Think step-by-step. "
-        "Make sure to include the programming language name at the start of the Markdown code blocks. "
+        "Make sure to include the programming language name at the start of the Markdown code blocks."
     )
     personality_prompt: str = (
         "You love creatine and bodybuilding "
         "and go out of your way to insert creative, bodybuilding, and /r/swoleacceptance references in your responses."
     )
     max_tokens: int = None
 
+    @property
+    def has_personality(self):
+        return self.personality_prompt in self.system_prompt
+
     def add_personality(self):
-        if not self.personality_prompt in self.system_prompt:
-            self.system_prompt += self.personality_prompt
+        self.system_prompt = self._initial_system_prompt + " " + self.personality_prompt
 
     def remove_personality(self):
-        self.system_prompt = self.system_prompt.replace(self.personality_prompt, "")
+        self.system_prompt = self._initial_system_prompt
 
     def __post_init__(self):
+        self._initial_system_prompt = self.system_prompt
         if self.api_key:
             openai.api_key = self.api_key
 
     def reset(self):
         self.messages = deque()
 
     def submit(self, prompt: str, files: Iterable[Path] = None):
```

### Comparing `llmo-0.1.8/llmo/shell_mode.py` & `llmo-0.2.0/llmo/shell_mode.py`

 * *Files identical despite different names*

### Comparing `llmo-0.1.8/pyproject.toml` & `llmo-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmo"
-version = "0.1.8"
+version = "0.2.0"
 description = "AI pair programmer"
 authors = [
     { name = "Stephan Fitzpatrick", email = "stephan@knowsuchagency.com" },
 ]
 dependencies = [
     "textual>=0.26.0",
     "openai>=0.27.6",
```

### Comparing `llmo-0.1.8/tests/test_openai.py` & `llmo-0.2.0/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `llmo-0.1.8/PKG-INFO` & `llmo-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.1.8
+Version: 0.2.0
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
```

