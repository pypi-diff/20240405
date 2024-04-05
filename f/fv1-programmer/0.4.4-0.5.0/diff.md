# Comparing `tmp/fv1_programmer-0.4.4.tar.gz` & `tmp/fv1_programmer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.4.4.tar", max compression
+gzip compressed data, was "fv1_programmer-0.5.0.tar", max compression
```

## Comparing `fv1_programmer-0.4.4.tar` & `fv1_programmer-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1065 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/LICENSE
--rw-r--r--   0        0        0     4277 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/README.md
--rw-r--r--   0        0        0     1140 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2024-03-31 20:09:02.504319 fv1_programmer-0.4.4/asfv1/.git
--rw-r--r--   0        0        0     1157 2024-03-31 20:09:04.116324 fv1_programmer-0.4.4/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2024-03-31 20:09:04.116324 fv1_programmer-0.4.4/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2024-03-31 20:09:04.116324 fv1_programmer-0.4.4/asfv1/README.md
--rw-r--r--   0        0        0    54482 2024-03-31 20:09:04.116324 fv1_programmer-0.4.4/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2024-03-31 20:09:04.116324 fv1_programmer-0.4.4/asfv1/example.asm
--rw-r--r--   0        0        0      801 2024-03-31 20:09:04.116324 fv1_programmer-0.4.4/asfv1/setup.py
--rw-r--r--   0        0        0       31 2024-03-31 20:09:03.024320 fv1_programmer-0.4.4/disfv1/.git
--rw-r--r--   0        0        0     1157 2024-03-31 20:09:04.124324 fv1_programmer-0.4.4/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2024-03-31 20:09:04.124324 fv1_programmer-0.4.4/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2024-03-31 20:09:04.124324 fv1_programmer-0.4.4/disfv1/README.md
--rw-r--r--   0        0        0    17532 2024-03-31 20:09:04.124324 fv1_programmer-0.4.4/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2024-03-31 20:09:04.124324 fv1_programmer-0.4.4/disfv1/example.bin
--rw-r--r--   0        0        0      798 2024-03-31 20:09:04.124324 fv1_programmer-0.4.4/disfv1/setup.py
--rw-r--r--   0        0        0     6485 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/eeprom/eeprom.py
--rw-r--r--   0        0        0     1717 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3081 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/fv1_programmer/main.py
--rw-r--r--   0        0        0      802 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/fv1_programmer/pyinstaller.py
--rw-r--r--   0        0        0     3166 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/fv1_programmer/tui.css
--rw-r--r--   0        0        0    24895 2024-03-31 20:09:01.764316 fv1_programmer-0.4.4/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1404 2024-03-31 20:09:01.768316 fv1_programmer-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 fv1_programmer-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4277 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/README.md
+-rw-r--r--   0        0        0     1140 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2024-04-05 02:58:34.811276 fv1_programmer-0.5.0/asfv1/.git
+-rw-r--r--   0        0        0     1157 2024-04-05 02:58:35.595266 fv1_programmer-0.5.0/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2024-04-05 02:58:35.595266 fv1_programmer-0.5.0/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2024-04-05 02:58:35.595266 fv1_programmer-0.5.0/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2024-04-05 02:58:35.595266 fv1_programmer-0.5.0/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2024-04-05 02:58:35.595266 fv1_programmer-0.5.0/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2024-04-05 02:58:35.595266 fv1_programmer-0.5.0/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2024-04-05 02:58:35.079273 fv1_programmer-0.5.0/disfv1/.git
+-rw-r--r--   0        0        0     1157 2024-04-05 02:58:35.603266 fv1_programmer-0.5.0/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2024-04-05 02:58:35.603266 fv1_programmer-0.5.0/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2024-04-05 02:58:35.603266 fv1_programmer-0.5.0/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2024-04-05 02:58:35.603266 fv1_programmer-0.5.0/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2024-04-05 02:58:35.603266 fv1_programmer-0.5.0/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2024-04-05 02:58:35.603266 fv1_programmer-0.5.0/disfv1/setup.py
+-rw-r--r--   0        0        0     6485 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1587 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/dialogs.css
+-rw-r--r--   0        0        0     4809 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/dialogs.py
+-rw-r--r--   0        0        0     1729 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3081 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/main.py
+-rw-r--r--   0        0        0      802 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/pyinstaller.py
+-rw-r--r--   0        0        0     1785 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    26724 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1404 2024-04-05 02:58:34.487279 fv1_programmer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 fv1_programmer-0.5.0/PKG-INFO
```

### Comparing `fv1_programmer-0.4.4/LICENSE` & `fv1_programmer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/README.md` & `fv1_programmer-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/adaptor/adapter.py` & `fv1_programmer-0.5.0/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/adaptor/mcp2221.py` & `fv1_programmer-0.5.0/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/asfv1/.gitignore` & `fv1_programmer-0.5.0/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/asfv1/LICENSE` & `fv1_programmer-0.5.0/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/asfv1/README.md` & `fv1_programmer-0.5.0/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/asfv1/asfv1.py` & `fv1_programmer-0.5.0/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/asfv1/example.asm` & `fv1_programmer-0.5.0/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/asfv1/setup.py` & `fv1_programmer-0.5.0/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/disfv1/.gitignore` & `fv1_programmer-0.5.0/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/disfv1/LICENSE` & `fv1_programmer-0.5.0/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/disfv1/README.md` & `fv1_programmer-0.5.0/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/disfv1/disfv1.py` & `fv1_programmer-0.5.0/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/disfv1/setup.py` & `fv1_programmer-0.5.0/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/eeprom/eeprom.py` & `fv1_programmer-0.5.0/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/fv1_programmer/fv1.py` & `fv1_programmer-0.5.0/fv1_programmer/fv1.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,17 +29,17 @@
                       clamp=clamp, spinreals=spinreals,
                       wfunc=warning, efunc=error)
         try:
             fp.parse()
         except ASFV1Error:
             if len(errors) == 0:
                 errors = ["Failed to assemble program"]
-            return None, warnings, errors
+            return None, fp.icnt, warnings, errors
 
-        return fp.program, warnings, errors
+        return fp.program, fp.icnt, warnings, errors
 
     def from_bytearray(self, data : bytearray, relative=False, suppressraw=False) -> str:
         """
         Disassembles a binary FV1 program and sets the internal asm property to
         the disassembled output. Returns any warnings in a concatenated string.
         """
         warnings = []
@@ -52,11 +52,10 @@
                         relative=relative, nopraw=suppressraw,
                         wfunc=warning)
         fp.deparse()
         self.asm = fp.listing
 
         return warnings
 
-    def as_markdown(self,) -> str:
-        return f"""```
-{self.asm}
-```"""
+    @property
+    def assembly(self,) -> str:
+        return self.asm
```

### Comparing `fv1_programmer-0.4.4/fv1_programmer/main.py` & `fv1_programmer-0.5.0/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/fv1_programmer/pyinstaller.py` & `fv1_programmer-0.5.0/fv1_programmer/pyinstaller.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.4.4/fv1_programmer/tui.py` & `fv1_programmer-0.5.0/fv1_programmer/tui.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,150 +7,125 @@
 
 from rich.console import RenderableType
 
 from textual import events, on
 from textual import work
 from textual.reactive import reactive
 from textual.app import App, ComposeResult
+from textual.command import Hit, Hits, DiscoveryHit, Provider, CommandPalette
 from textual.binding import Binding
-from textual.containers import Container, Grid, Horizontal, VerticalScroll
-from textual.screen import Screen, ModalScreen
-from textual.worker import Worker, get_current_worker
+from textual.containers import Container, Horizontal, VerticalScroll
+from textual.screen import Screen
+from textual.worker import get_current_worker
 from textual.message import Message
 from textual.widget import Widget
 from textual.widgets import (
     Footer,
     Header,
     Static,
-    TextLog,
-    Button,
+    RichLog,
     TabbedContent,
     TabPane,
     Switch,
-    Markdown,
     DirectoryTree,
-    Label,
-    LoadingIndicator,
-    Input,
+    TextArea,
+    ContentSwitcher,
+    Markdown,
 )
 
+from functools import partial
 from typing import Iterable
 from pathlib import Path
-from fv1_programmer.fv1 import FV1Program, FV1_PROGRAM_MAX_BYTES
 import pyperclip
+from fv1_programmer.fv1 import FV1Program, FV1_PROGRAM_MAX_BYTES
+from fv1_programmer.dialogs import *
 
 
-__version__ = "0.4.4"
+__version__ = "0.5.0"
 
 _title = "FV1 Programmer"
+MIN_PROGRAM_NUM = 1
+MAX_PROGRAM_NUM = 8
 
-class BusyScreen(ModalScreen):
-    def __init__(self, message : str) -> None:
-        self.message = message
-        super().__init__()
+class FV1AppCommands(Provider):
+    """A command provider to open a Python file in the current working directory."""
 
-    def compose(self) -> ComposeResult:
-        yield Grid(
-            Label(self.message),
-            LoadingIndicator(),
-            id="busyscreen"
-        )
-
-
-class FilteredDirectoryTree(DirectoryTree):
-    def __init__(self, *args, **kwargs):
-        self.valid_suffixes = []
-        try:
-            self.valid_suffixes = kwargs.pop("valid_suffixes")
-        except KeyError:
-            pass
-        super().__init__(*args, **kwargs)
+    async def startup(self) -> None:
+        """Called once when the command palette is opened"""
+        self.discovery_commands = [
+            ("Rename current program", self.screen.action_rename_program_slot, "Provide your own name for this program slot"),
+            ("New program", self.screen.action_new, "Create a new, empty program in current slot (Ctr+N)"),
+            ("Delete current program", self.screen.action_delete,"Delete any program in current slot"),
+        ]
+
+    async def discover(self,) -> Hits:
+        for name, callback, help_msg in self.discovery_commands:
+            yield DiscoveryHit(name, callback, help=help_msg)
+
+    async def search(self, query: str) -> Hits:
+        """Search for Python files."""
+        matcher = self.matcher(query)  
+
+        app = self.app
+        assert isinstance(app, FV1App)
+
+        # Slot swapping commands
+        for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
+            command = f"Swap with slot {i}"
+            score = matcher.match(command)
+            if score > 0:
+                yield Hit(
+                    score,
+                    matcher.highlight(command),
+                    partial(self.screen.swap_with_slot, i),
+                    help=f"Swap this slot with slot {i}",
+                )
 
-    def filter_paths(self, paths: Iterable[Path]) -> Iterable[Path]:
-        return [path for path in paths if not path.name.startswith(".") and \
-                    # TODO: Support SpinCAD file types as well!
-                    path.is_dir() or (path.is_file() and path.suffix.lower() in self.valid_suffixes)]
 
-
-class LoadFileScreen(ModalScreen[Path]):
-    SUPPORTED_FILE_SUFFIXES = [".json", ".spn"]
-    selection : reactive[Path | None] = reactive(None)
+class FV1ProgramPane(Widget):
+    program : reactive[FV1Program | None] = reactive(None)
 
     def compose(self) -> ComposeResult:
-        yield Grid(
-            Static("Choose a file:", id="fileselectlabel"),
-            FilteredDirectoryTree("./", id="filetree", valid_suffixes=LoadFileScreen.SUPPORTED_FILE_SUFFIXES),
-            Button("Cancel", variant="error", id="filedialogcancel"),
-            Button("Select", variant="primary", id="filedialogselect"),
-            id="filedialog",
-        )
-
-    @on(DirectoryTree.FileSelected, "#filetree")
-    def do_file_selected(self, event : DirectoryTree.FileSelected):
-        self.selection = event.path
-
-    def watch_selection(self, new_path: Path):
-        self.selection = new_path
-        enabled = self.selection is not None
-        select_button = self.query_one("#filedialogselect", Button)
-        select_button.disabled = not enabled
-        if enabled:
-            select_button.focus()
-
-    @on(Button.Pressed, "#filedialogselect")
-    def do_select(self):
-        self.dismiss(self.selection)
-
-    @on(Button.Pressed, "#filedialogcancel")
-    def cancel(self):
-        self.dismiss(None)
+        with ContentSwitcher(initial="empty-slot"):  
+            yield Markdown(id="empty-slot")
+            yield TextArea.code_editor("", id="text-area-slot")
 
+    def watch_program(self, new_program: FV1Program):
+        if new_program is not None:
+            self.query_one(ContentSwitcher).current = "text-area-slot"
+            self.query_one(TextArea).text = new_program.assembly
+        else:
+            self.query_one(ContentSwitcher).current = "empty-slot"
 
-class SaveFileScreen(ModalScreen[Path]):
-    filename : reactive("")
+    def on_mount(self) -> None:
+        self.query_one(Markdown).update("""# Empty Program Slot
+This is an empty program slot that will be ignored when downloading to the Easy Spin pedal. <br>
 
-    def compose(self) -> ComposeResult:
-        yield Grid(
-            Static("Please specify a filename:", id="fileselectlabel"),
-            Input("my_programs", id="filesavefilename"),
-            Button("Cancel", variant="error", id="filedialogcancel"),
-            Button("Save", variant="primary", id="filedialogselect"),
-            id="filesavedialog",
-        )
-
-    @on(Input.Changed)
-    def check_filename(self, event: Input.Changed) -> None:
-        self.query_one("#filedialogselect", Button).disabled = \
-                    len(self.query_one("#filesavefilename", Input).value) < 1
-
-    @on(Button.Pressed, "#filedialogselect")
-    def do_save(self):
-        self.dismiss(self.query_one("#filesavefilename", Input).value)
-
-    @on(Button.Pressed, "#filedialogcancel")
-    def cancel(self):
-        self.dismiss(None)
+To add a program to this slot, you can do one of the following:
 
+- Click here or press Ctrl+N to [create a new program for editing](#new-program)
+- Drag and drop an appropriate file onto this window (.spn, .json)
 
-class FV1ProgramPane(Widget):
-    program : reactive[FV1Program | None] = reactive(None)
+Press *Ctrl+D* to delete a program and reset the program slot to be empty (ignored during download) <br>
 
-    def compose(self) -> ComposeResult:
-        yield Markdown()
+Also see these helpful links: <br>
 
-    def watch_program(self, new_program: FV1Program):
-        markdown = '# No program specified (leave this slot untouched)'
-        if new_program is not None:
-            markdown = new_program.as_markdown()
+Textual documentation for the editor keybindings: https://textual.textualize.io/widgets/text_area/#bindings <br>
+Easy Spin webpage: https://audiofab.com/products/easy-spin <br>
+""")
 
-        self.query_one(Markdown).update(markdown)
-
-    def on_mount(self) -> None:
-        self.query_one(Markdown).tooltip = """Ctrl+C - Copy to clipboard\nCtrl+V/Ctrl+T - Paste from clipboard\nCtrl+D - Delete this program"""
+    @on(Markdown.LinkClicked)
+    def on_click(self, event):
+        if event.href == "#new-program":
+            self.program = FV1Program("")
 
+    @on(TextArea.Changed)
+    def on_changed(self, event):
+        self.program.asm = self.query_one(TextArea).text
+        self.query_one(TextArea).focus()
 
 
 class ProgramTabs(Widget):
     def compose(self) -> ComposeResult:  
         with TabbedContent():
             with TabPane("Program 1", id="prog1"):
                 yield FV1ProgramPane(id="fv1prog1")
@@ -165,42 +140,18 @@
             with TabPane("Program 6", id="prog6"):
                 yield FV1ProgramPane(id="fv1prog6")
             with TabPane("Program 7", id="prog7"):
                 yield FV1ProgramPane(id="fv1prog7")
             with TabPane("Program 8", id="prog8"):
                 yield FV1ProgramPane(id="fv1prog8")
 
-
-class YesNoScreen(ModalScreen[bool]):
-    def __init__(self, message, no_text="No", yes_text="Yes",
-                 no_variant="primary", yes_variant="primary",
-                 *args, **kwargs):
-        self.message = message
-        self.no_text = no_text
-        self.yes_text = yes_text
-        self.no_variant = no_variant
-        self.yes_variant = yes_variant
-        super().__init__(*args, **kwargs)
-
-    def compose(self) -> ComposeResult:
-        yield Grid(
-            Static(self.message, id="yesnomessage"),
-            Button(self.no_text, variant=self.no_variant, id="yesnono"),
-            Button(self.yes_text, variant=self.yes_variant, id="yesnoyes"),
-            id="yesnodialog",
-        )
-
-    @on(Button.Pressed, "#yesnoyes")
-    def yes(self):
-        self.dismiss(True)
-
-    @on(Button.Pressed, "#yesnono")
-    def no(self):
-        self.dismiss(False)
-
+    # @on(TabbedContent.TabActivated)
+    # def on_tab_changed(self, event):
+    #     self.app.logger.info(event.pane.query_one(TextArea))
+    #     event.pane.query_one(TextArea).focus()
 
 class Title(Static):
     pass
 
 
 class OptionSwitch(Horizontal):
     def __init__(self, name, label) -> None:
@@ -242,25 +193,25 @@
     def write(self, s):
         self.log(str(s).rstrip())
 
 
 class MainScreen(Screen):
     TITLE = _title
     BINDINGS = [
-        ("ctrl+l", "load_file", "Load"),
-        ("ctrl+s", "save", "Save"),
-        ("ctrl+r", "read_eeprom", "Read"),
-        ("ctrl+w", "write_eeprom", "Write"),
-        ("f1", "app.toggle_class('TextLog', '-hidden')", "Log"),
+        Binding("ctrl+n", "new", "New Program", show=False, priority=True),
+        Binding("ctrl+p", "command_palette", show=False, priority=True),
+        Binding("ctrl+l", "load_file", "Load", priority=True),
+        Binding("ctrl+s", "save", "Save", priority=True),
+        Binding("ctrl+r", "read_eeprom", "Read", priority=True),
+        Binding("ctrl+w", "write_eeprom", "Write", priority=True),
+        ("f1", "app.toggle_class('RichLog', '-hidden')", "Log"),
         ("f2", "toggle_sidebar", "Settings"),
         ("ctrl+q", "request_quit", "Quit"),
-        Binding("ctrl+v", "paste", "Paste", show=False, priority=True),
-        Binding("ctrl+t", "paste", "Paste", show=False, priority=True),
-        Binding("ctrl+d", "delete", "Delete Program", show=False, priority=True),
     ]
+    COMMANDS = {FV1AppCommands}
 
     show_sidebar = reactive(False)
 
     class WriteEepromResult(Message):
         def __init__(self, programs : Iterable[dict], error=None) -> None:
             self.programs = programs
             self.error = error
@@ -272,30 +223,30 @@
             self.error = error
             super().__init__()
 
     def compose(self) -> ComposeResult:
         with Container():
             yield Sidebar(classes="-hidden")
             yield Header(show_clock=True)
-            yield TextLog(id="consolelog", classes="-hidden", wrap=False, highlight=True, markup=True)
+            yield RichLog(id="consolelog", classes="-hidden", wrap=False, highlight=True, markup=True)
             yield ProgramTabs()
             yield Footer()
 
     def action_toggle_sidebar(self) -> None:
         sidebar = self.query_one(Sidebar)
         self.set_focus(None)
         if sidebar.has_class("-hidden"):
             sidebar.remove_class("-hidden")
         else:
             if sidebar.query("*:focus"):
                 self.screen.set_focus(None)
             sidebar.add_class("-hidden")
 
     def console_log(self, renderable: RenderableType) -> None:
-        self.query_one(TextLog).write(renderable)
+        self.query_one(RichLog).write(renderable)
 
     def on_mount(self) -> None:
         sh = logging.StreamHandler(stream=ConsoleLogStream(self.console_log))
         sh.setLevel(logging.INFO)
         self.app.logger.addHandler(sh)
         self.app.logger.info(f"FV1 Programmer version {__version__}")
 
@@ -303,31 +254,70 @@
         def check_quit(should_quit : bool) -> None:
             if should_quit:
                 self.app.do_exit()
 
         self.app.push_screen(YesNoScreen("Are you sure you want to quit?",
                                          yes_variant="error"), check_quit)
 
+    def action_command_palette(self) -> None:
+        """Show the Textual command palette."""
+        if not CommandPalette.is_open(self):
+            self.app.push_screen(CommandPalette(), callback=self.app.call_next)
+
+    def swap_with_slot(self, dest_slot : int) -> None:
+        """Swaps the current program slot with `dest_slot`"""
+        active_tab_id = self.query_one(TabbedContent).active
+        active_slot = active_tab_id.split("prog")[1]
+        if active_slot == dest_slot:
+            return
+        active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
+        dest_program_pane = self.query_one(f"#fv1prog{dest_slot}", FV1ProgramPane)
+        tmp_prog = dest_program_pane.program
+        dest_program_pane.program = active_program_pane.program
+        active_program_pane.program = tmp_prog
+
+        active_name = self.query_one(TabbedContent).get_tab(f"{self.query_one(TabbedContent).active}").label
+        dest_name = self.query_one(TabbedContent).get_tab(f"prog{dest_slot}").label
+        self.rename_program_slot(active_slot, dest_name)
+        self.rename_program_slot(dest_slot, active_name)
+
+    def rename_program_slot(self, slot_num : int, name : str) -> None:
+        self.query_one(TabbedContent).get_tab(f"prog{slot_num}").label = name
+
+    def action_rename_program_slot(self,) -> None:
+        """Prompts the user for a name for the current program slot"""
+        def handle_program_rename(name : str) -> None:
+            if name and len(name):
+                self.rename_program_slot(self.query_one(TabbedContent).active.split("prog")[1], name)
+
+        self.app.push_screen(RenameSlotScreen(), handle_program_rename)
+
     def load_json_file(self, path : Path) -> None:
         with open(str(path), 'r') as f:
             d = json.load(f)
             programs = d.get("programs", [None]*8)
-            for i in range(1,9):
+            for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
                 program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
                 if programs[i - 1] is not None:
-                    program_pane.program = FV1Program(programs[i - 1])
+                    if isinstance(programs[i - 1], str):
+                        program_pane.program = FV1Program(programs[i - 1])
+                        self.rename_program_slot(i, f"Program {i}")
+                    else:
+                        self.rename_program_slot(i, programs[i - 1].get("name", f"Program {i}"))
+                        prog = programs[i - 1].get("asm", None)
+                        program_pane.program = FV1Program(prog) if prog is not None else prog
+
         self.app.show_toast(f"Loaded programs from {path}")
 
     def load_spn_file(self, path : Path, slot_number : int) -> None:
         with open(str(path), 'r') as f:
             program_pane = self.query_one(f"#fv1prog{slot_number}", FV1ProgramPane)
             program_pane.program = FV1Program("".join(f.readlines()))
+            self.rename_program_slot(slot_number, path.stem)
         self.app.show_toast(f"Loaded {path}")
-        if not self.app.setting_asfv1_spinreals:
-            self.app.show_toast(f"You may want to enable 'Spin Reals' in the settings!")
 
     def handle_load_file(self, path : Path) -> None:
         if path is not None and path.exists() and path.is_file():
             if path.suffix.lower() == ".json":
                 self.load_json_file(path)
             elif path.suffix.lower() == ".spn":
                 active_tab_id = self.query_one(TabbedContent).active
@@ -369,17 +359,20 @@
 
         except ValueError:
             pass
 
     def action_save(self) -> None:
         d = {"programs" : []}
 
-        for i in range(1,9):
+        for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
-            d["programs"].append(program_pane.program.asm if program_pane.program is not None else None)
+            prog_d = {}
+            prog_d["asm"] = program_pane.program.asm if program_pane.program is not None else None
+            prog_d["name"] = str(self.query_one(TabbedContent).get_tab(f"prog{i}").label)
+            d["programs"].append(prog_d)
 
         def handle_save_file(filename : str) -> None:
             def do_save_file(file_path):
                 with open(file_path, 'w') as f:
                     json.dump(d, f, indent=2)
                     self.app.show_toast(f"Programs saved to {file_path}")
 
@@ -396,20 +389,24 @@
                     do_save_file(save_path)
 
         self.app.push_screen(SaveFileScreen(), handle_save_file)
 
     def action_write_eeprom(self) -> None:
         programs = []
         errors = 0
-        for i in range(1,9):
+        for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             if program_pane.program is not None:
                 bin_array = self.assemble_and_validate_program(program_pane.program)
                 if bin_array is not None:
-                    programs.append({"program": i, "address" : (i - 1)*FV1_PROGRAM_MAX_BYTES, "data" : bin_array})
+                    if len(bin_array):
+                        programs.append({"program": i, "address" : (i - 1)*FV1_PROGRAM_MAX_BYTES, "data" : bin_array})
+                    else:
+                        # Program assembled but there are no instructions
+                        self.app.show_toast(f"Program {i} has no instructions.")
                 else:
                     self.app.show_toast(f"Program {i} failed to assemble. See log for details.")
                     errors += 1
 
         if errors > 0:
             self.app.show_toast("Errors while assembling. Download aborted.", severity="warning")
         else:
@@ -428,15 +425,15 @@
             from eeprom.eeprom import I2CEEPROM
             adaptor = MCP2221I2CAdaptor(self.app.cmdline_args.i2c_address,
                                         i2c_clock_speed=self.app.cmdline_args.i2c_clock_speed)
             adaptor.open()
             return I2CEEPROM(adaptor, self.app.cmdline_args.ee_size,
                              page_size_in_bytes=self.app.cmdline_args.ee_page_size)
 
-    @work(exclusive=True)
+    @work(exclusive=True, thread=True)
     def write_eeprom(self, programs : Iterable[dict], simulate : bool) -> None:
         worker = get_current_worker()
         eeprom = None
         error = None
         try:
             eeprom = self._get_eeprom()
 
@@ -478,30 +475,30 @@
         def do_read_eeprom():
             self.app.push_screen(BusyScreen("Reading from pedal..."))
             self.read_eeprom(self.app.setting_simulate,
                              self.app.setting_disfv1_relative,
                              self.app.setting_disfv1_suppressraw)
 
         num_programs = 0
-        for i in range(1,9):
+        for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             if program_pane.program is not None:
                 num_programs += 1
 
         if num_programs > 0:
             # Ask the user if they want to overwrite their current programs
             def check_overwrite(should_overwrite : bool) -> None:
                 if should_overwrite:
                     do_read_eeprom()
             self.app.push_screen(YesNoScreen("This will overwrite your current programs.\nAre you sure?"), check_overwrite)
 
         else:
             do_read_eeprom()
 
-    @work(exclusive=True)
+    @work(exclusive=True, thread=True)
     def read_eeprom(self, simulate : bool, relative : bool, suppressraw : bool) -> None:
         worker = get_current_worker()
         eeprom = None
         try:
             eeprom = self._get_eeprom()
 
             if eeprom is not None:
@@ -525,15 +522,15 @@
         self.app.pop_screen()
         if message.error is not None:
             self.app.logger.error(str(message.error))
             self.app.show_toast("EEPROM read failed! See log for details.", title="Error", severity="error")
             return
 
         were_warnings = False
-        for i in range(1,9):
+        for i in range(MIN_PROGRAM_NUM, MAX_PROGRAM_NUM + 1):
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             program_pane.program = message.programs[i - 1]["program"]
             warnings = message.programs[i - 1]["warnings"]
             if warnings is not None:
                 for warning in warnings:
                     self.app.logger.info(warning)
                     m = re.match(r"info: Read (\d+) instructions\.", warning)
@@ -542,34 +539,40 @@
                         were_warnings = True
 
         if were_warnings:
             self.app.show_toast("EEPROM read succeeded with warnings. See log for details.", title="Warning", severity="warning")
         else:
             self.app.show_toast("EEPROM read complete.")
 
-    def action_paste(self) -> None:
-        # Validate program
-        new_program = FV1Program(pyperclip.paste())
-        bin_array = self.assemble_and_validate_program(new_program)
-        if bin_array is not None:
-            active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
-            active_program_pane.program = FV1Program(pyperclip.paste())
-        else:
-            self.app.show_toast("Ignoring invalid clipboard contents. See log for details.")
-
     def action_delete(self) -> None:
-        active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
+        active_tab_id = self.query_one(TabbedContent).active
+        active_slot = active_tab_id.split("prog")[1]
+        active_program_pane = self.query_one(f"#fv1{active_tab_id}", FV1ProgramPane)
         active_program_pane.program = None
+        self.rename_program_slot(active_slot, f"Program {active_slot}")
+
+    def action_new(self) -> None:
+        active_tab_id = self.query_one(TabbedContent).active
+        active_slot = active_tab_id.split("prog")[1]
+        active_program_pane = self.query_one(f"#fv1{active_tab_id}", FV1ProgramPane)
+        active_program_pane.program = FV1Program("")
+        self.rename_program_slot(active_slot, f"Program {active_slot}")
+        active_program_pane.query_one(TextArea).focus()
 
     def assemble_and_validate_program(self, program) -> bytearray:
-        bin_array, warnings, errors = program.assemble(clamp=self.app.setting_asfv1_clamp,
-                                                       spinreals=self.app.setting_asfv1_spinreals)
+        bin_array, num_instructions, warnings, errors = program.assemble(clamp=self.app.setting_asfv1_clamp,
+                                                                         spinreals=self.app.setting_asfv1_spinreals)
         [self.app.logger.info(w) for w in warnings]
         [self.app.logger.info(e) for e in errors]
-        return bin_array if len(errors) == 0 else None
+        if len(errors) == 0:
+            if num_instructions > 0:
+                return bin_array
+            else:
+                return []
+        return None
 
 
 from dataclasses import dataclass
 @dataclass
 class Args:
     """Class emulating command line arguments to allow running via `textual run --dev`"""
     i2c_addr:int
@@ -579,16 +582,18 @@
     pad_value:int
     verify:bool
     debug:bool
     sim:Path
 
 
 class FV1App(App[None]):
-    CSS_PATH = "tui.css"
+    CSS_PATH = ["tui.css", "dialogs.css"]
     SCREENS = {"main" : MainScreen()}
+    ENABLE_COMMAND_PALETTE = False
+    COMMANDS = {}
 
     def __init__(self, cmdline_args=None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.cmdline_args = cmdline_args
 
         # See if we're being run by `textual run --dev`
         if 'devtools' in self.features:
@@ -624,16 +629,16 @@
             self.logger.addHandler(fh)
 
     # Intercept the app exit (the only thing connected to this should be Ctrl+C)
     # and make it behave like Copy
     def exit(self, result = None) -> None:
         active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
         if active_program_pane.program is not None:
-            pyperclip.copy(active_program_pane.program.asm)
-            self.show_toast("Current program copied to clipboard")
+            pyperclip.copy(active_program_pane.query_one(TextArea).selected_text)
+        #     self.show_toast("Current program copied to clipboard")
 
     def do_exit(self, result = None) -> None:
         super().exit(result)
 
     def on_mount(self) -> None:
         self.push_screen("main")
```

### Comparing `fv1_programmer-0.4.4/pyproject.toml` & `fv1_programmer-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.4.4"
+version = "0.5.0"
 homepage = "https://github.com/audiofab/fv1_programmer"
 description = "An FV-1 assembler/disassembler and EEPROM programming tool for the Spin Semiconductor FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -26,22 +26,22 @@
     {include = "adaptor"},
     {include = "asfv1"},
     {include = "disfv1"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-textual = "^0.30.0"
+textual = "^0.55.0"
 easymcp2221 = "^1.6.2"
 intelhex = "^2.3.0"
 pyperclip = "^1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
-textual-dev = "^1.0.1"
+textual-dev = "^1.5.1"
 pyinstaller = "^6.1.0"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
 ]
```

### Comparing `fv1_programmer-0.4.4/PKG-INFO` & `fv1_programmer-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fv1-programmer
-Version: 0.4.4
+Version: 0.5.0
 Summary: An FV-1 assembler/disassembler and EEPROM programming tool for the Spin Semiconductor FV-1 DSP
 Home-page: https://github.com/audiofab/fv1_programmer
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@audiofab.com
 Requires-Python: >=3.8,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: easymcp2221 (>=1.6.2,<2.0.0)
 Requires-Dist: intelhex (>=2.3.0,<3.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: textual (>=0.30.0,<0.31.0)
+Requires-Dist: textual (>=0.55.0,<0.56.0)
 Description-Content-Type: text/markdown
 
 # FV-1 Programmer
 
 An FV-1 assembler/disassembler and EEPROM programming tool for the [Audiofab](https://audiofab.com/) [Easy Spin](https://audiofab.com/products/easy-spin) effects pedal.
 
 This utility was made possible by the amazing [Textual](https://textual.textualize.io/) project. Check it out!
```

