# Comparing `tmp/textual_fspicker-0.0.3-py3-none-any.whl.zip` & `tmp/textual_fspicker-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,16 @@
-Zip file size: 13341 bytes, number of entries: 12
--rw-r--r--  2.0 unx      740 b- defN 23-May-21 08:58 textual_fspicker/__init__.py
--rw-r--r--  2.0 unx     2305 b- defN 23-May-21 08:58 textual_fspicker/__main__.py
--rw-r--r--  2.0 unx     7980 b- defN 23-May-21 08:58 textual_fspicker/file_open.py
+Zip file size: 14773 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      813 b- defN 23-May-22 20:47 textual_fspicker/__init__.py
+-rw-r--r--  2.0 unx     2868 b- defN 23-May-22 20:47 textual_fspicker/__main__.py
+-rw-r--r--  2.0 unx     4225 b- defN 23-May-22 20:47 textual_fspicker/base_dialog.py
+-rw-r--r--  2.0 unx     5557 b- defN 23-May-22 20:47 textual_fspicker/file_open.py
 -rw-r--r--  2.0 unx     1822 b- defN 23-May-21 08:58 textual_fspicker/path_filters.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 20:02 textual_fspicker/py.typed
 -rw-r--r--  2.0 unx     2174 b- defN 23-May-19 09:53 textual_fspicker/safe_tests.py
+-rw-r--r--  2.0 unx     2457 b- defN 23-May-22 20:47 textual_fspicker/select_directory.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-17 19:18 textual_fspicker/parts/__init__.py
 -rw-r--r--  2.0 unx    15053 b- defN 23-May-21 08:58 textual_fspicker/parts/directory_navigation.py
--rw-r--r--  2.0 unx     6396 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1038 b- defN 23-May-21 09:00 textual_fspicker-0.0.3.dist-info/RECORD
-12 files, 38006 bytes uncompressed, 11575 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx     4168 b- defN 23-May-22 20:50 textual_fspicker-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 20:50 textual_fspicker-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-22 20:50 textual_fspicker-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1219 b- defN 23-May-22 20:50 textual_fspicker-0.0.4.dist-info/RECORD
+14 files, 40854 bytes uncompressed, 12721 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -1,37 +1,43 @@
 Filename: textual_fspicker/__init__.py
 Comment: 
 
 Filename: textual_fspicker/__main__.py
 Comment: 
 
+Filename: textual_fspicker/base_dialog.py
+Comment: 
+
 Filename: textual_fspicker/file_open.py
 Comment: 
 
 Filename: textual_fspicker/path_filters.py
 Comment: 
 
 Filename: textual_fspicker/py.typed
 Comment: 
 
 Filename: textual_fspicker/safe_tests.py
 Comment: 
 
+Filename: textual_fspicker/select_directory.py
+Comment: 
+
 Filename: textual_fspicker/parts/__init__.py
 Comment: 
 
 Filename: textual_fspicker/parts/directory_navigation.py
 Comment: 
 
-Filename: textual_fspicker-0.0.3.dist-info/METADATA
+Filename: textual_fspicker-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: textual_fspicker-0.0.3.dist-info/WHEEL
+Filename: textual_fspicker-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: textual_fspicker-0.0.3.dist-info/top_level.txt
+Filename: textual_fspicker-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_fspicker-0.0.3.dist-info/RECORD
+Filename: textual_fspicker-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_fspicker/__init__.py

```diff
@@ -3,20 +3,21 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.0.3"
+__version__    = "0.0.4"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
-from .file_open    import FileOpen
-from .path_filters import Filters
+from .file_open        import FileOpen
+from .select_directory import SelectDirectory
+from .path_filters     import Filters
 
 ##############################################################################
 # Export the imports.
-__all__ = [ "FileOpen", "Filters" ]
+__all__ = [ "FileOpen", "SelectDirectory", "Filters" ]
 
 ### __init__.py ends here
```

## textual_fspicker/__main__.py

```diff
@@ -2,52 +2,62 @@
 
 ##############################################################################
 # Python imports.
 from pathlib import Path
 
 ##############################################################################
 # Textual imports.
+from textual            import on
 from textual.app        import App, ComposeResult
-from textual.containers import Center
+from textual.containers import Center, Horizontal
 from textual.widgets    import Label, Button
 
 ##############################################################################
 # Local imports.
-from textual_fspicker import FileOpen, Filters
+from textual_fspicker import FileOpen, Filters, SelectDirectory
 
 ##############################################################################
 class TestApp( App[ None ] ):
     """A simple test application."""
 
     CSS = """
     Screen#_default {
         align: center middle;
     }
 
-    Screen#_default Button {
-        margin-bottom: 2;
+    Screen#_default Horizontal {
+        align: center middle;
+        height: auto;
+        margin-bottom: 1;
+    }
+
+    Screen#_default Horizontal Button {
+        margin-left: 1;
+        margin-right: 1;
     }
     """
 
     def compose( self ) -> ComposeResult:
         """Compose the layout of the test application."""
-        with Center():
-            yield Button( "Select a file" )
+        with Horizontal():
+            yield Button( "Select a file", id="file" )
+            yield Button( "Select a directory", id="directory" )
         with Center():
             yield Label( "Press the button to pick something" )
 
     def show_selected( self, to_show: Path ) -> None:
         """Show the file that was selected by the user.
 
         Args:
             to_show: The file to show.
         """
         self.query_one( Label ).update( str( to_show ) )
 
-    def on_button_pressed( self ):
+    @on( Button.Pressed, "#file" )
+    def open_file( self ) -> None:
         """Show the `FileOpen` dialog when the button is pushed."""
         self.push_screen(
             FileOpen( ".", filters=Filters(
                 ( "Any",     lambda _: True ),
                 ( "Emacs",   lambda p: p.suffix.lower() == ".el" ),
                 ( "Lisp",    lambda p: p.suffix.lower() in ( ".lisp", ".lsp", ".cl" ) ),
                 ( "Python",  lambda p: p.suffix.lower() == ".py" ),
@@ -55,12 +65,17 @@
                 ( "Clipper", lambda p: p.suffix.lower() in ( ".prg", ".ch" ) ),
                 ( "C",       lambda p: p.suffix.lower() in ( ".c", ".h" ) ),
                 ( "C++",     lambda p: p.suffix.lower() in ( ".cpp", ".cc", ".h" ) ),
             ) ),
             callback=self.show_selected
         )
 
+    @on( Button.Pressed, "#directory" )
+    def select_directory( self ) -> None:
+        """show the `SelectDirectory` dialog when the button is pushed."""
+        self.push_screen( SelectDirectory(), callback=self.show_selected )
+
 ##############################################################################
 if __name__ == "__main__":
     TestApp().run()
 
 ### __main__.py ends here
```

## textual_fspicker/file_open.py

```diff
@@ -3,156 +3,87 @@
 ##############################################################################
 # Python imports.
 from __future__ import annotations
 from pathlib    import Path
 
 ##############################################################################
 # Textual imports.
-from textual            import on
-from textual.app        import ComposeResult
-from textual.binding    import Binding
-from textual.containers import Horizontal, Vertical
-from textual.screen     import ModalScreen
-from textual.widgets    import Button, Input, Select
+from textual         import on
+from textual.app     import ComposeResult
+from textual.widgets import Button, Input, Select
 
 ##############################################################################
 # Local imports.
+from .base_dialog  import FileSystemPickerScreen
 from .parts        import DirectoryNavigation
 from .path_filters import Filters
 
 ##############################################################################
-class Dialog( Vertical ):
-    """Layout class for the main dialog area."""
-
-##############################################################################
-class InputBar( Horizontal ):
-    """The input bar area of the dialog."""
-
-##############################################################################
 class FileFilter( Select[ int ] ):
     """The file filter."""
 
 ##############################################################################
-class FileOpen( ModalScreen[ Path ] ):
+class FileOpen( FileSystemPickerScreen ):
     """A file opening dialog."""
 
     DEFAULT_CSS = """
-    FileOpen {
-        align: center middle;
-    }
-
-    FileOpen Dialog {
-        width: 80%;
-        height: 80%;
-        border: panel $panel-lighten-2;
-        background: $panel-lighten-1;
-        border-title-color: $text;
-        border-title-background: $panel-lighten-2;
-        border-subtitle-color: $text;
-        border-subtitle-background: $error;
-    }
-
-    FileOpen InputBar {
-        height: auto;
-        align: right middle;
-        padding-top: 1;
-        padding-right: 1;
-        padding-bottom: 1;
-    }
-
-    FileOpen InputBar Button {
-        margin-left: 1;
-    }
-
     FileOpen InputBar Input {
         width: 2fr;
     }
 
     FileOpen InputBar Select {
         width: 1fr;
     }
     """
 
-    BINDINGS = [
-        Binding( "escape", "dismiss" ),
-        Binding( "full_stop", "hidden" )
-    ]
-    """The bindings for the dialog."""
-
     def __init__(
             self,
             location: str | Path | None = None,
             title: str = "Open",
             must_exist: bool = True,
             filters: Filters | None = None
         ) -> None:
         """Initialise the `FileOpen` dialog.
 
         Args:
             location: Optional starting location.
             title: Optional title.
             must_exist: Flag to say if the file must exist.
+            filters: Optional filters to show in the dialog.
         """
-        super().__init__()
-        self._location = location
-        """The starting location."""
-        self._title = title
-        """The title for the dialog."""
+        super().__init__( location, title, select_button="Open" )
         self._must_exist = must_exist
         """Must the file exist?"""
         self._filters = filters
         """The filters for the dialog."""
 
-    def compose( self ) -> ComposeResult:
-        """Compose the child widgets.
-
-        Returns:
-            The widgets to compose.
-        """
-        with Dialog() as dialog:
-            dialog.border_title = self._title
-            yield DirectoryNavigation(self._location)
-            with InputBar():
-                yield Input()
-                if self._filters:
-                    yield FileFilter(
-                        self._filters.selections,
-                        prompt      = "File filter",
-                        value       = 0,
-                        allow_blank = False
-                    )
-                yield Button( "Open", id="open" )
-                yield Button( "Cancel", id="cancel" )
-
-    def _set_error( self, message: str="" ) -> None:
-        """Set or clear the error message.
-
-        Args:
-            message: Optional message to show as an error.
-        """
-        self.query_one( Dialog ).border_subtitle = message
+    def _input_bar( self ) -> ComposeResult:
+        """Provide any widgets for the input before, before the buttons."""
+        yield Input()
+        if self._filters:
+            yield FileFilter(
+                self._filters.selections,
+                prompt      = "File filter",
+                value       = 0,
+                allow_blank = False
+            )
 
     @on( DirectoryNavigation.Selected )
     def _select_file( self, event: DirectoryNavigation.Selected ) -> None:
         """Handle a file being selected in the picker.
 
         Args:
             event: The event to handle.
         """
         file_name       = self.query_one( Input )
         file_name.value = str( event.path.name )
         file_name.focus()
 
-    @on( DirectoryNavigation.PermissionError )
-    def _show_permission_error( self ) -> None:
-        """Show any permission error bubbled up from the directory navigator."""
-        self._set_error( "Permission error" )
-
     @on( Input.Submitted )
-    @on( Button.Pressed, "#open" )
+    @on( Button.Pressed, "#select" )
     def _confirm_file( self, event: Input.Submitted | Button.Pressed ) -> None:
         """Confirm the selection of the file in the input box.
 
         Args:
             event: The event to handle.
         """
         event.stop()
@@ -200,33 +131,18 @@
             # Finally, we've got some sort of pickable item and it's good to
             # be picked. Let's go with it.
             self.dismiss( result=chosen )
 
         else:
             self._set_error( "A file must be chosen" )
 
-    @on( Button.Pressed, "#cancel" )
-    def _cancel( self, event: Button.Pressed ) -> None:
-        """Cancel the dialog.
-
-        Args:
-            event: The even to handle.
-        """
-        event.stop()
-        self.dismiss()
-
     @on( Input.Changed )
-    @on( DirectoryNavigation.Changed )
     def _clear_error( self ) -> None:
         """Clear any error that might be showing."""
-        self._set_error()
-
-    def action_hidden( self ) -> None:
-        """Action for toggling the display of hidden files."""
-        self.query_one( DirectoryNavigation ).toggle_hidden()
+        super()._clear_error()
 
     @on( Select.Changed )
     def _change_filter( self, event: Select.Changed ) -> None:
         """Handle a change in the filter.
 
         Args:
             event: The event to handle.
```

## Comparing `textual_fspicker-0.0.3.dist-info/RECORD` & `textual_fspicker-0.0.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-textual_fspicker/__init__.py,sha256=FUz9CzbjP9eRy8ekM_TWOeS0aLrwWe3BfmgMaaRL2Dk,740
-textual_fspicker/__main__.py,sha256=P5L8aMAp_LloN1VpcxJTQBGb6iRTq-VuDYAXxWOq4ro,2305
-textual_fspicker/file_open.py,sha256=oAxxWgIBBSx1pNQIY9behjly7CWGsZBsi4nN0oAfhH0,7980
+textual_fspicker/__init__.py,sha256=v-NSeafCm8nwBSEhISMKIaDGUGFzZKX4xbTgh-bLfyA,813
+textual_fspicker/__main__.py,sha256=bau4JSyxfoDhih82NeM_Pg5KCwv4YXXYDnfEgSccvZc,2868
+textual_fspicker/base_dialog.py,sha256=WJGgIq--rMbsNGzNKw1hjhKQPmuRlatXvfyonn_R7DY,4225
+textual_fspicker/file_open.py,sha256=GAONfM-T4ytchjA7PH2B-HeZmejmW4-78g5QGHAAdcU,5557
 textual_fspicker/path_filters.py,sha256=XpPrynKVI_p8Tf6tUuhEmU5lxAaf3TQlsjKsRwXC5nk,1822
 textual_fspicker/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 textual_fspicker/safe_tests.py,sha256=U3gpqVRr7qcv7mqF-I_sFojtr9Pv5JyqFzAxGG7qofA,2174
+textual_fspicker/select_directory.py,sha256=vE1MYCL-_QqTyPiveJrxl90oEwjQB14lfSsHteUEBNM,2457
 textual_fspicker/parts/__init__.py,sha256=vjP1jzd5ty4IhwUZnVFkOjzctZn22EbwWDHh_16x-GM,389
 textual_fspicker/parts/directory_navigation.py,sha256=6jg6mBcBbVsH7DcimhsF2XKpwXqWBaVb4f2xx5G9mm0,15053
-textual_fspicker-0.0.3.dist-info/METADATA,sha256=CoAX4O10T8ZJX64-0AN4QYYBVSgw0PWyLI5lupuUmpo,6396
-textual_fspicker-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-textual_fspicker-0.0.3.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
-textual_fspicker-0.0.3.dist-info/RECORD,,
+textual_fspicker-0.0.4.dist-info/METADATA,sha256=6yJTI9rOEbi8znJMnJ_S7hqGGHgBeJiggCdI7bmimN0,4168
+textual_fspicker-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+textual_fspicker-0.0.4.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
+textual_fspicker-0.0.4.dist-info/RECORD,,
```

