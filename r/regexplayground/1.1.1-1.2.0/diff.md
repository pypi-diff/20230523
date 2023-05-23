# Comparing `tmp/regexplayground-1.1.1.tar.gz` & `tmp/regexplayground-1.2.0.tar.gz`

## Comparing `regexplayground-1.1.1.tar` & `regexplayground-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/__init__.py
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/app_guide.md
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/cheatsheet.md
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/examples.json
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/examples.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/ip.txt
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/pyregex_playground.css
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 regexplayground-1.1.1/src/regexplayground/pyregex_playground.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 regexplayground-1.1.1/LICENSE
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 regexplayground-1.1.1/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 regexplayground-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 regexplayground-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/__init__.py
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/app_guide.md
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/cheatsheet.md
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/examples.json
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/examples.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/ip.txt
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/pyregex_playground.css
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 regexplayground-1.2.0/src/regexplayground/pyregex_playground.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 regexplayground-1.2.0/LICENSE
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 regexplayground-1.2.0/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 regexplayground-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 regexplayground-1.2.0/PKG-INFO
```

### Comparing `regexplayground-1.1.1/src/regexplayground/app_guide.md` & `regexplayground-1.2.0/src/regexplayground/app_guide.md`

 * *Files identical despite different names*

### Comparing `regexplayground-1.1.1/src/regexplayground/cheatsheet.md` & `regexplayground-1.2.0/src/regexplayground/cheatsheet.md`

 * *Files identical despite different names*

### Comparing `regexplayground-1.1.1/src/regexplayground/examples.json` & `regexplayground-1.2.0/src/regexplayground/examples.json`

 * *Files identical despite different names*

### Comparing `regexplayground-1.1.1/src/regexplayground/examples.md` & `regexplayground-1.2.0/src/regexplayground/examples.md`

 * *Files identical despite different names*

### Comparing `regexplayground-1.1.1/src/regexplayground/pyregex_playground.css` & `regexplayground-1.2.0/src/regexplayground/pyregex_playground.css`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .container {
     height: auto;
     align: center middle;
 }
 
 .code_container {
     height: auto;
+    width: 100%;
     border: solid brown;
 }
 
 .examples_ip {
     padding: 0 1 0 1;
     margin: 0 1 0 1;
     border: none;
@@ -25,14 +26,15 @@
 
 .examples_op {
     padding: 0 1 1 1;
     margin: 0 1 0 1;
     border: none;
     background: lightgray;
     width: 100%;
+    color: black;
 }
 
 .examples_md {
     margin: 1 2 0 2;
     border: none;
 }
 
@@ -45,23 +47,28 @@
 }
 
 .playground_ip {
     padding: 0 1 0 1;
     border: none;
 }
 
-.playground_error {
+.error {
     min-height: 0;
     height: auto;
     width: 100%;
     color: red;
+    padding: 0 1 0 1;
+    border: round red;
 }
 
 .playground_ip_op {
     width: 100%;
+    padding: 0 1 0 1;
+    border: round gray;
+    border-title-align: center;
 }
 
 Button:focus {
     text-style: bold;
 }
 
 .buttons {
```

### Comparing `regexplayground-1.1.1/src/regexplayground/pyregex_playground.py` & `regexplayground-1.2.0/src/regexplayground/pyregex_playground.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from textual.app import App
 from textual.binding import Binding
 from textual.containers import Horizontal, Vertical
 from textual.widgets import Footer, Label, Input, MarkdownViewer, Button
 from textual.screen import Screen
-from rich.panel import Panel
 from rich.text import Text
 from rich.pretty import Pretty
 from rich.highlighter import Highlighter
 from rich.markdown import Markdown as RichMarkdown
 
 import json
 import re
@@ -71,18 +70,21 @@
         for unit in input_block:
             *i_setup, i_expr, l_op = unit
             try:
                 if i_setup:
                     exec(''.join(ip.value for ip in i_setup))
                 op = eval(i_expr.value)
                 l_op.update(Pretty(op))
+                l_op.styles.border = ('none', 'red')
+                l_op.styles.color = 'black'
             except ERROR_TYPES as e:
-                t = Panel(f'{e}', title=f'{type(e).__name__}', title_align='left')
-                l_op.update(t)
+                l_op.update(str(e))
+                l_op.styles.border = ('round', 'red')
                 l_op.styles.color = 'red'
+                l_op.border_title = str(type(e).__name__)
 
     def load_examples(self):
         self.v_examples = Vertical(classes='container')
         self.v_code_block = []
         self.input_collection = []
         comment_highlighter = CommentHighlighter()
         with open('examples.json', encoding='UTF-8') as f:
@@ -98,15 +100,15 @@
                 if setup:
                     exec(''.join(setup))
                 op = eval(expr)
 
                 t = [Input(value=line, classes='examples_ip',
                            highlighter=comment_highlighter, name=str(idx))
                      for line in lines]
-                l_op = Label(Pretty(op), classes='examples_op')
+                l_op = Label(Pretty(op), classes='examples_op', markup=False)
                 t.append(l_op)
                 self.input_collection[idx].append(t)
                 self.v_code_block[idx].mount(*t)
             self.v_examples.mount(Label(RichMarkdown(info), classes='examples_md'))
             self.v_examples.mount(self.v_code_block[idx])
             idx += 1
         self.v_container.mount(self.v_examples)
@@ -117,37 +119,36 @@
 
 
 class Playground(Screen):
     BINDINGS = [Binding('ctrl+p', 'update_ip', 'Update ip', show=True),
                 Binding('f1', 'guide', 'App Guide', show=False),
                 Binding('f2', 'cheatsheet', 'Cheatsheet', show=False),
                 Binding('f3', 'examples', 'Interactive Examples', show=False),
-                ('up', 'focus_previous', 'Focus previous'),
-                ('down', 'focus_next', 'Focus next'),
+                Binding('up', 'focus_previous', 'Focus previous', show=False),
+                Binding('down', 'focus_next', 'Focus next', show=False),
                ]
 
     def __init__(self):
         super().__init__()
 
         self.l_compile = Label('Compile', classes='playground_name')
         self.l_action = Label('Action', classes='playground_name')
 
-        self.l_compile_error = Label('')
-        self.l_action_error = Label('')
+        self.l_compile_error = Label()
+        self.l_action_error = Label()
 
         os.chdir(Path(__file__).parent.resolve())
         self.ip_file = 'ip.txt'
         self.read_data()
-        self.l_input = Label(classes='playground_ip_op')
-        self.ip_panel = partial(Panel, title='ip', title_align='center')
-        self.l_input.update(self.ip_panel(self.data))
-
-        self.l_output = Label(classes='playground_ip_op')
-        self.op_panel = partial(Panel, title='Output', title_align='center')
-        self.l_output.update(self.op_panel(''))
+        self.l_input = Label(classes='playground_ip_op', markup=False)
+        self.l_input.border_title = 'ip'
+        self.l_input.update(self.data)
+
+        self.l_output = Label(classes='playground_ip_op', markup=False)
+        self.l_output.border_title = 'Output'
 
         self.code_bg_color = 'silver'
         self.error_color = 'ansi_red'
 
         placeholder = 'Search pattern. Press Enter to compile.'
         self.i_compile = Input(placeholder=placeholder, value="re.compile(r'')",
                                classes='playground_ip')
@@ -182,40 +183,40 @@
     def on_input_submitted(self, event):
         self.l_compile_error.remove()
         ip = self.data
         try:
             self.i_compile.styles.background = self.code_bg_color
             pat = eval(self.i_compile.value)
         except ERROR_TYPES as e:
-            t = Panel(f'{e}', title=f'{type(e).__name__}', title_align='left')
-            self.l_compile_error = Label(t, classes='playground_error')
+            self.l_compile_error = Label(str(e), classes='error', markup=False)
+            self.l_compile_error.border_title = str(type(e).__name__)
             self.v_compile.mount(self.l_compile_error)
             self.i_compile.styles.background = self.error_color
         else:
             op = Text(ip)
             for m in pat.finditer(ip):
                 op.stylize('bold red', *m.span())
-            self.l_input.update(self.ip_panel(op))
+            self.l_input.update(op)
 
         self.l_action_error.remove()
         try:
             self.i_action.styles.background = self.code_bg_color
             if self.i_action.value:
                 op = eval(self.i_action.value)
             else:
                 op = ''
         except ERROR_TYPES as e:
-            t = Panel(f'{e}', title=f'{type(e).__name__}', title_align='left')
-            self.l_action_error = Label(t, classes='playground_error')
+            self.l_action_error = Label(str(e), classes='error', markup=False)
+            self.l_action_error.border_title = str(type(e).__name__)
             self.v_action.mount(self.l_action_error)
             self.i_action.styles.background = self.error_color
         else:
             if type(op) != str:
                 op = Pretty(op)
-            self.l_output.update(self.op_panel(op))
+            self.l_output.update(op)
 
     def on_button_pressed(self, event):
         button_label = str(event.button.label)
         if button_label == 'Cheatsheet':
             self.action_cheatsheet()
         elif button_label == 'Interactive Examples':
             self.action_examples()
@@ -233,15 +234,15 @@
         self.app.push_screen('cheatsheet')
 
     def action_examples(self):
         self.app.push_screen('examples')
 
     def action_update_ip(self):
         self.read_data()
-        self.l_input.update(self.ip_panel(self.data))
+        self.l_input.update(self.data)
 
 class PyRegexPlayground(App):
     SCREENS = {'playground': Playground(),
                'guide': ShowMarkdown('app_guide.md'),
                'cheatsheet': ShowMarkdown('cheatsheet.md'),
                'examples': Examples()}
     CSS_PATH = 'pyregex_playground.css'
```

### Comparing `regexplayground-1.1.1/LICENSE` & `regexplayground-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regexplayground-1.1.1/README.md` & `regexplayground-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `regexplayground-1.1.1/pyproject.toml` & `regexplayground-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "regexplayground"
-version = "1.1.1"
+version = "1.2.0"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "Playground for Python Regular Expressions. Also includes cheatsheet and interactive examples."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "textual>=0.16.0",
+  "textual>=0.24.1",
 ]
 
 [project.scripts]
 regexplayground = "regexplayground.pyregex_playground:main"
 
 [project.urls]
 "Source" = "https://github.com/learnbyexample/TUI-apps/tree/main/PyRegexPlayground"
```

### Comparing `regexplayground-1.1.1/PKG-INFO` & `regexplayground-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: regexplayground
-Version: 1.1.1
+Version: 1.2.0
 Summary: Playground for Python Regular Expressions. Also includes cheatsheet and interactive examples.
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/PyRegexPlayground
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: textual>=0.16.0
+Requires-Dist: textual>=0.24.1
 Description-Content-Type: text/markdown
 
 # Python re(gex)? playground
 
 This TUI application is intended as an interactive playground for Python Regular Expressions. The app also includes a comprehensive cheatsheet and several interactive examples.
 
 # Screenshot
```

