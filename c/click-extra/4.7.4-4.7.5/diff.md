# Comparing `tmp/click_extra-4.7.4.tar.gz` & `tmp/click_extra-4.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.7.4.tar", max compression
+gzip compressed data, was "click_extra-4.7.5.tar", max compression
```

## Comparing `click_extra-4.7.4.tar` & `click_extra-4.7.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6372 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/__init__.py
--rw-r--r--   0        0        0    30983 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/colorize.py
--rw-r--r--   0        0        0    15732 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/commands.py
--rw-r--r--   0        0        0    16297 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/config.py
--rw-r--r--   0        0        0     4069 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/decorators.py
--rw-r--r--   0        0        0     6205 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/docs_update.py
--rw-r--r--   0        0        0    11858 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/logging.py
--rw-r--r--   0        0        0    26623 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/parameters.py
--rw-r--r--   0        0        0    17237 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/py.typed
--rw-r--r--   0        0        0     7676 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/pygments.py
--rw-r--r--   0        0        0     4969 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/sphinx.py
--rw-r--r--   0        0        0     6340 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/tabulate.py
--rw-r--r--   0        0        0     2716 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/telemetry.py
--rw-r--r--   0        0        0    23592 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/testing.py
--rw-r--r--   0        0        0      770 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    13021 2024-02-23 17:20:59.967946 click_extra-4.7.4/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    26207 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    15221 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    17030 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7216 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    21037 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0    10884 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8406 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14491 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3165 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8259 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3551 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     8925 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2637 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/timer.py
--rw-r--r--   0        0        0    17896 2024-02-23 17:20:59.971946 click_extra-4.7.4/click_extra/version.py
--rw-r--r--   0        0        0     9187 2024-02-23 17:20:59.975946 click_extra-4.7.4/pyproject.toml
--rw-r--r--   0        0        0     6735 2024-02-23 17:20:59.975946 click_extra-4.7.4/readme.md
--rw-r--r--   0        0        0     9827 1970-01-01 00:00:00.000000 click_extra-4.7.4/PKG-INFO
+-rw-r--r--   0        0        0     7446 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/__init__.py
+-rw-r--r--   0        0        0    31127 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/colorize.py
+-rw-r--r--   0        0        0    15756 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/commands.py
+-rw-r--r--   0        0        0    16508 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/config.py
+-rw-r--r--   0        0        0     4069 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/decorators.py
+-rw-r--r--   0        0        0     6205 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11866 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/logging.py
+-rw-r--r--   0        0        0    27132 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/parameters.py
+-rw-r--r--   0        0        0    17269 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/py.typed
+-rw-r--r--   0        0        0     7843 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/pygments.py
+-rw-r--r--   0        0        0     5057 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/sphinx.py
+-rw-r--r--   0        0        0     6340 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2716 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2024-04-05 10:52:24.651415 click_extra-4.7.5/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    13021 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    26216 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    14677 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    17030 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7216 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    21037 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10884 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8404 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14482 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     8925 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2637 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/timer.py
+-rw-r--r--   0        0        0    17760 2024-04-05 10:52:24.655415 click_extra-4.7.5/click_extra/version.py
+-rw-r--r--   0        0        0     8981 2024-04-05 10:52:24.659415 click_extra-4.7.5/pyproject.toml
+-rw-r--r--   0        0        0     6735 2024-04-05 10:52:24.659415 click_extra-4.7.5/readme.md
+-rw-r--r--   0        0        0     9827 1970-01-01 00:00:00.000000 click_extra-4.7.5/PKG-INFO
```

### Comparing `click_extra-4.7.4/click_extra/colorize.py` & `click_extra-4.7.5/click_extra/colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 """Helpers and utilities to apply ANSI coloring to terminal content."""
 
 from __future__ import annotations
 
 import dataclasses
 import os
 import re
+from collections.abc import Iterable
 from configparser import RawConfigParser
 from dataclasses import dataclass
 from gettext import gettext as _
 from operator import getitem
-from typing import Sequence, cast
+from typing import Callable, Sequence, cast
 
 import click
 import cloup
 import regex as re3
 from boltons.strutils import complement_int_list, int_ranges_from_int_list
 from cloup._util import identity
 from cloup.styling import Color, IStyle
@@ -619,15 +620,15 @@
                 "The matching result contains named groups that were not processed. "
                 "There is an edge-case in the design of regular expressions."
             )
             raise ValueError(msg)
 
         return txt
 
-    def highlight_extra_keywords(self, help_text):
+    def highlight_extra_keywords(self, help_text: str) -> str:
         """Highlight extra keywords in help screens based on the theme.
 
         It is based on regular expressions. While this is not a bullet-proof method, it
         is good enough. After all, help screens are not consumed by machine but are
         designed for humans.
 
         .. danger::
@@ -792,22 +793,27 @@
                     self.colorize,
                     help_text,
                     flags=re.VERBOSE,
                 )
 
         return help_text
 
-    def getvalue(self):
+    def getvalue(self) -> str:
         """Wrap original `Click.HelpFormatter.getvalue()` to force extra-colorization on
         rendering."""
         help_text = super().getvalue()
         return self.highlight_extra_keywords(help_text)
 
 
-def highlight(string, substrings, styling_method, ignore_case=False):
+def highlight(
+    string: str,
+    substrings: Iterable[str],
+    styling_method: Callable,
+    ignore_case: bool = False,
+) -> str:
     """Highlights parts of the ``string`` that matches ``substrings``.
 
     Takes care of overlapping parts within the ``string``.
     """
     # Ranges of character indices flagged for highlighting.
     ranges = set()
 
@@ -816,22 +822,22 @@
         flags = re3.IGNORECASE if ignore_case else 0
         ranges |= {
             f"{match.start()}-{match.end() - 1}"
             for match in re3.finditer(part, string, flags=flags, overlapped=True)
         }
 
     # Reduce ranges, compute complement ranges, transform them to list of integers.
-    ranges = ",".join(ranges)
-    highlight_ranges = int_ranges_from_int_list(ranges)
+    range_arg = ",".join(ranges)
+    highlight_ranges = int_ranges_from_int_list(range_arg)
     untouched_ranges = int_ranges_from_int_list(
-        complement_int_list(ranges, range_end=len(string)),
+        complement_int_list(range_arg, range_end=len(string)),
     )
 
     # Apply style to range of characters flagged as matching.
     styled_str = ""
     for i, j in sorted(highlight_ranges + untouched_ranges):
         segment = getitem(string, slice(i, j + 1))
         if (i, j) in highlight_ranges:
             segment = styling_method(segment)
-        styled_str += segment
+        styled_str += str(segment)
 
     return styled_str
```

### Comparing `click_extra-4.7.4/click_extra/commands.py` & `click_extra-4.7.5/click_extra/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 import click
 import cloup
 
-from . import Command, Group
+from . import Command, Group, Option
 from .colorize import ColorOption, ExtraHelpColorsMixin, HelpExtraFormatter, HelpOption
 from .config import ConfigOption
 from .logging import VerbosityOption
 from .parameters import (
     ExtraOption,
     ShowParamsOption,
     all_envvars,
@@ -120,15 +120,15 @@
 
     @color.deleter
     def color(self) -> None:
         """Reset the color value so it defaults to inheritance from parent's."""
         self._color = None
 
 
-def default_extra_params():
+def default_extra_params() -> list[Option]:
     """Default additional options added to ``extra_command`` and ``extra_group``.
 
     .. caution::
         The order of options has been carefully crafted to handle subtle edge-cases and
         avoid leaky states in unittests.
 
         You can still override this hard-coded order for easthetic reasons and it
```

### Comparing `click_extra-4.7.4/click_extra/config.py` & `click_extra-4.7.5/click_extra/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,19 +188,19 @@
         if len(extensions) == 1:
             ext_pattern = extensions[0]
         else:
             # Use brace notation for multiple extension matching.
             ext_pattern = f"{{{','.join(extensions)}}}"
         return f"{app_dir}{os.path.sep}*.{ext_pattern}"
 
-    def get_help_record(self, ctx):
+    def get_help_record(self, ctx: Context) -> tuple[str, str] | None:
         """Replaces the default value by the pretty version of the configuration
         matching pattern."""
         # Pre-compute pretty_path to bypass infinite recursive loop on get_default.
-        pretty_path = shrinkuser(Path(self.get_default(ctx)))
+        pretty_path = shrinkuser(Path(self.get_default(ctx)))  # type: ignore[arg-type]
         with patch.object(ConfigOption, "get_default") as mock_method:
             mock_method.return_value = pretty_path
             return super().get_help_record(ctx)
 
     def search_and_read_conf(self, pattern: str) -> Iterable[tuple[Path | URL, str]]:
         """Search on local file system or remote URL files matching the provided
         pattern.
@@ -235,15 +235,15 @@
             pattern,
             flags=NODIR | GLOBSTAR | DOTGLOB | GLOBTILDE | BRACE | FOLLOW | IGNORECASE,
         ):
             file_path = Path(file).resolve()
             logger.debug(f"Configuration file found at {file_path}")
             yield file_path, file_path.read_text()
 
-    def parse_conf(self, conf_text: str) -> dict | None:
+    def parse_conf(self, conf_text: str) -> dict[str, Any] | None:
         """Try to parse the provided content with each format in the order provided by
         the user.
 
         A successful parsing in any format is supposed to return a ``dict``. Any other
         result, including any raised exception, is considered a failure and the next
         format is tried.
         """
@@ -291,37 +291,39 @@
         """
         for conf_path, conf_text in self.search_and_read_conf(pattern):
             user_conf = self.parse_conf(conf_text)
             if user_conf is not None:
                 return conf_path, user_conf
         return None, None
 
-    def load_ini_config(self, content):
+    def load_ini_config(self, content: str) -> dict[str, Any]:
         """Utility method to parse INI configuration file.
 
         Internal convention is to use a dot (``.``, as set by ``self.SEP``) in
         section IDs as a separator between levels. This is a workaround
         the limitation of ``INI`` format which doesn't allow for sub-sections.
 
         Returns a ready-to-use data structure.
         """
         ini_config = ConfigParser(interpolation=ExtendedInterpolation())
         ini_config.read_string(content)
 
-        conf = {}
+        conf: dict[str, Any] = {}
         for section_id in ini_config.sections():
             # Extract all options of the section.
             sub_conf = {}
             for option_id in ini_config.options(section_id):
                 target_type = self.get_tree_value(
                     self.params_types,
                     section_id,
                     option_id,
                 )
 
+                value: Any
+
                 if target_type in (None, str):
                     value = ini_config.get(section_id, option_id)
 
                 elif target_type is int:
                     value = ini_config.getint(section_id, option_id)
 
                 elif target_type is float:
@@ -345,15 +347,15 @@
                 sub_conf[option_id] = value
 
             # Place collected options at the right level of the dict tree.
             merge(conf, self.init_tree_dict(*section_id.split(self.SEP), leaf=sub_conf))
 
         return conf
 
-    def recursive_update(self, a, b):
+    def recursive_update(self, a: dict[str, Any], b: dict[str, Any]) -> dict[str, Any]:
         """Like standard ``dict.update()``, but recursive so sub-dict gets updated.
 
         Ignore elements present in ``b`` but not in ``a``.
         """
         for k, v in b.items():
             if isinstance(v, dict) and isinstance(a.get(k), dict):
                 a[k] = self.recursive_update(a[k], v)
@@ -361,15 +363,15 @@
             elif k in a:
                 a[k] = b[k]
             elif self.strict:
                 msg = f"Parameter {k!r} is not allowed in configuration file."
                 raise ValueError(msg)
         return a
 
-    def merge_default_map(self, ctx, user_conf):
+    def merge_default_map(self, ctx: Context, user_conf: dict) -> None:
         """Save the user configuration into the context's ``default_map``.
 
         Merge the user configuration into the pre-computed template structure, which
         will filter out all unrecognized options not supported by the command. Then
         cleans up blank values and update the context's ``default_map``.
         """
         filtered_conf = self.recursive_update(self.params_template, user_conf)
```

### Comparing `click_extra-4.7.4/click_extra/decorators.py` & `click_extra-4.7.5/click_extra/decorators.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/docs_update.py` & `click_extra-4.7.5/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/logging.py` & `click_extra-4.7.5/click_extra/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
         Will returns Click Extra's internal logger first, then the option's custom
         logger.
         """
         for name in ("click_extra", self.logger_name):
             yield logging.getLogger(name)
 
-    def reset_loggers(self):
+    def reset_loggers(self) -> None:
         """Forces all loggers managed by the option to be reset to the default level.
 
         Reset loggers in reverse order to ensure the internal logger is reset last.
 
         .. danger::
             Resseting loggers is extremely important for unittests. Because they're
             global, loggers have tendency to leak and pollute their state between
```

### Comparing `click_extra-4.7.4/click_extra/parameters.py` & `click_extra-4.7.5/click_extra/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,25 +28,28 @@
 from functools import cached_property, reduce
 from gettext import gettext as _
 from operator import getitem, methodcaller
 from typing import (
     Any,
     Callable,
     ContextManager,
+    Iterator,
     cast,
 )
 from unittest.mock import patch
 
 import click
 from boltons.iterutils import unique
 from mergedeep import merge
 from tabulate import tabulate
 
 from . import (
+    Command,
     Option,
+    Parameter,
     ParamType,
     Style,
     echo,
     get_current_context,
 )
 
 
@@ -299,15 +302,15 @@
         """
         if excluded_params is not None:
             self.excluded_params = excluded_params
 
         super().__init__(*args, **kwargs)
 
     @staticmethod
-    def init_tree_dict(*path: str, leaf: Any = None):
+    def init_tree_dict(*path: str, leaf: Any = None) -> Any:
         """Utility method to recursively create a nested dict structure whose keys are
         provided by ``path`` list and at the end is populated by a copy of ``leaf``."""
 
         def dive(levels):
             if levels:
                 return {levels[0]: dive(levels[1:])}
             return leaf
@@ -318,15 +321,17 @@
     def get_tree_value(tree_dict: dict[str, Any], *path: str) -> Any | None:
         """Get in the ``tree_dict`` the value located at the ``path``."""
         try:
             return reduce(getitem, path, tree_dict)
         except KeyError:
             return None
 
-    def _flatten_tree_dict_gen(self, tree_dict, parent_key):
+    def _flatten_tree_dict_gen(
+        self, tree_dict: MutableMapping, parent_key: str | None = None
+    ) -> Iterable[tuple[str, Any]]:
         """`Source of this snippet
         <https://www.freecodecamp.org/news/how-to-flatten-a-dictionary-in-python-in-4-different-ways/>`_.
         """
         for k, v in tree_dict.items():
             new_key = f"{parent_key}{self.SEP}{k}" if parent_key else k
             if isinstance(v, MutableMapping):
                 yield from self.flatten_tree_dict(v, new_key).items()
@@ -338,15 +343,20 @@
         tree_dict: MutableMapping,
         parent_key: str | None = None,
     ) -> dict[str, Any]:
         """Recursively traverse the tree-like ``dict`` and produce a flat ``dict`` whose
         keys are path and values are the leaf's content."""
         return dict(self._flatten_tree_dict_gen(tree_dict, parent_key))
 
-    def _recurse_cmd(self, cmd, top_level_params, parent_keys):
+    def _recurse_cmd(
+        self,
+        cmd: Command,
+        top_level_params: Iterable[str],
+        parent_keys: tuple[str, ...],
+    ) -> Iterator[tuple[tuple[str, ...], Parameter]]:
         """Recursive generator to walk through all subcommands and their parameters."""
         if hasattr(cmd, "commands"):
             for subcmd_id, subcmd in cmd.commands.items():
                 if subcmd_id in top_level_params:
                     msg = (
                         f"{cmd.name}{self.SEP}{subcmd_id} subcommand conflicts with "
                         f"{top_level_params} top-level parameters"
@@ -358,33 +368,35 @@
 
                 yield from self._recurse_cmd(
                     subcmd,
                     top_level_params,
                     ((*parent_keys, subcmd.name)),
                 )
 
-    def walk_params(self):
+    def walk_params(self) -> Iterator[tuple[tuple[str, ...], Parameter]]:
         """Generates an unfiltered list of all CLI parameters.
 
         Everything is included, from top-level groups to subcommands, and from options
         to arguments.
 
         Returns a 2-elements tuple:
             - the first being a tuple of keys leading to the parameter
             - the second being the parameter object itself
         """
         ctx = get_current_context()
         cli = ctx.find_root().command
+        assert cli.name is not None
 
         # Keep track of top-level CLI parameter IDs to check conflict with command
         # IDs later.
         top_level_params = set()
 
         # Global, top-level options shared by all subcommands.
         for p in cli.params:
+            assert p.name is not None
             top_level_params.add(p.name)
             yield (cli.name, p.name), p
 
         # Subcommand-specific options.
         yield from self._recurse_cmd(cli, top_level_params, (cli.name,))
 
     TYPE_MAP: dict[type[ParamType], type[str | int | float | bool | list]] = {
@@ -406,15 +418,15 @@
 
     Keys are subclasses of ``click.types.ParamType``. Values are expected to be simple
     builtins Python types.
 
     This mapping can be seen as a reverse of the ``click.types.convert_type()`` method.
     """
 
-    def get_param_type(self, param):
+    def get_param_type(self, param: Parameter) -> type[str | int | float | bool | list]:
         """Get the Python type of a Click parameter.
 
         See the list of
         `custom types provided by Click <https://click.palletsprojects.com/en/8.1.x/api/#types>`_.
         """
         if param.multiple or param.nargs != 1:
             return list
@@ -443,15 +455,15 @@
 
         # Custom parameters are expected to convert from strings, as that's the default
         # type of command lines.
         # See: https://click.palletsprojects.com/en/8.1.x/api/#click.ParamType
         if isinstance(param.type, ParamType):
             return str
 
-        msg = f"Can't guess the appropriate Python type of {param!r} parameter."
+        msg = f"Can't guess the appropriate Python type of {param!r} parameter."  # type:ignore[unreachable]
         raise ValueError(msg)
 
     @cached_property
     def excluded_params(self) -> Iterable[str]:
         """List of parameter IDs to exclude from the parameter structure.
 
         Elements of this list are expected to be the fully-qualified ID of the
@@ -487,35 +499,35 @@
             merge(objects, self.init_tree_dict(*keys, leaf=param))
 
         self.params_template = template
         self.params_types = types
         self.params_objects = objects
 
     @cached_property
-    def params_template(self):
+    def params_template(self) -> dict[str, Any]:
         """Returns a tree-like dictionary whose keys shadows the CLI options and
         subcommands and values are ``None``.
 
         Perfect to serve as a template for configuration files.
         """
         self.build_param_trees()
         return self.params_template
 
     @cached_property
-    def params_types(self):
+    def params_types(self) -> dict[str, Any]:
         """Returns a tree-like dictionary whose keys shadows the CLI options and
         subcommands and values are their expected Python type.
 
         Perfect to parse configuration files and user-provided parameters.
         """
         self.build_param_trees()
         return self.params_types
 
     @cached_property
-    def params_objects(self):
+    def params_objects(self) -> dict[str, Any]:
         """Returns a tree-like dictionary whose keys shadows the CLI options and
         subcommands and values are parameter objects.
 
         Perfect to parse configuration files and user-provided parameters.
         """
         self.build_param_trees()
         return self.params_objects
```

### Comparing `click_extra-4.7.4/click_extra/platforms.py` & `click_extra-4.7.5/click_extra/platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from __future__ import annotations
 
 import platform
 import sys
 from dataclasses import dataclass, field
 from itertools import combinations
-from typing import Iterable
+from typing import Iterable, Iterator
 
 from . import cache
 
 """ Below is the collection of heuristics used to identify each platform.
 
 All these heuristics can be hard-cached as the underlying system is not suppose to
 change between code execution.
@@ -244,15 +244,15 @@
             self,
             "platform_ids",
             frozenset({p.id for p in self.platforms}),
         )
         # Double-check there is no duplicate platforms.
         assert len(self.platforms) == len(self.platform_ids)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Platform]:
         """Iterate over the platforms of the group."""
         yield from self.platforms
 
     def __len__(self) -> int:
         """Return the number of platforms in the group."""
         return len(self.platforms)
```

### Comparing `click_extra-4.7.4/click_extra/pygments.py` & `click_extra-4.7.5/click_extra/pygments.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Helpers and utilities to allow Pygments to parse and render ANSI codes."""
 
 from __future__ import annotations
 
+from typing import Iterable, Iterator
+
 from pygments import lexers
 from pygments.filter import Filter
 from pygments.filters import TokenMergeFilter
 from pygments.formatter import _lookup_style  # type: ignore[attr-defined]
 from pygments.formatters import HtmlFormatter
 from pygments.lexer import Lexer, LexerMeta
 from pygments.lexers.algebra import GAPConsoleLexer
@@ -32,15 +34,15 @@
 from pygments.lexers.python import PythonConsoleLexer
 from pygments.lexers.r import RConsoleLexer
 from pygments.lexers.ruby import RubyConsoleLexer
 from pygments.lexers.shell import ShellSessionBaseLexer
 from pygments.lexers.special import OutputLexer
 from pygments.lexers.sql import PostgresConsoleLexer, SqliteConsoleLexer
 from pygments.style import StyleMeta
-from pygments.token import Generic, string_to_tokentype
+from pygments.token import Generic, _TokenType, string_to_tokentype
 from pygments_ansi_color import (
     AnsiColorLexer,
     ExtendedColorHtmlFormatterMixin,
     color_tokens,
 )
 
 DEFAULT_TOKEN_TYPE = Generic.Output
@@ -66,15 +68,17 @@
         """
         super().__init__(**options)
         self.ansi_lexer = AnsiColorLexer()
         self.token_type = string_to_tokentype(
             options.get("token_type", DEFAULT_TOKEN_TYPE),
         )
 
-    def filter(self, lexer, stream):
+    def filter(
+        self, lexer: Lexer, stream: Iterable[tuple[_TokenType, str]]
+    ) -> Iterator[tuple[_TokenType, str]]:
         """Transform each token of ``token_type`` type into a stream of ANSI tokens."""
         for ttype, value in stream:
             if ttype == self.token_type:
                 # TODO: Should we re-wrap the resulting list of token into their
                 # original Generic.Output?
                 yield from self.ansi_lexer.get_tokens(value)
             else:
@@ -112,15 +116,15 @@
         ``Generic.Output`` monoblocks into ANSI tokens.
         """
         super().__init__(*args, **kwargs)
         self.filters.append(TokenMergeFilter())
         self.filters.append(AnsiFilter())
 
 
-def collect_session_lexers():
+def collect_session_lexers() -> Iterator[type[Lexer]]:
     """Retrieve all lexers producing shell-like sessions in Pygments.
 
     This function contain a manually-maintained list of lexers, to which we dynamiccaly
     adds lexers inheriting from ``ShellSessionBaseLexer``.
 
     .. hint::
```

### Comparing `click_extra-4.7.4/click_extra/sphinx.py` & `click_extra-4.7.5/click_extra/sphinx.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     Fix the need to have both ``.. click:example::`` and ``.. click:run::`` directives
     in the same ``{eval-rst}`` block in MyST. This is required to have both directives
     shares states and context.
 """
 
 from __future__ import annotations
 
+from typing import Any
+
 from docutils.statemachine import ViewList
 from sphinx.highlighting import PygmentsBridge
 
 from .pygments import AnsiHtmlFormatter
 from .tests.conftest import ExtraCliRunner
 
 
@@ -71,28 +73,29 @@
     ``.. click:run::`` directive with an ANSI Shell Session:
     ``.. code-block:: ansi-shell-session``.
 
     ``.. sourcecode:: shell-session`` has been `released in Pallets-Sphinx-Themes 2.1.0
     <https://github.com/pallets/pallets-sphinx-themes/pull/62>`_.
     """
 
-    def append(self, *args, **kwargs):
+    def append(self, *args, **kwargs) -> None:
         """Search the default code block and replace it with our own version."""
         default_code_block = ".. sourcecode:: shell-session"
         new_code_block = ".. code-block:: ansi-shell-session"
 
         if default_code_block in args:
-            args = list(args)
+            new_args = list(args)
             index = args.index(default_code_block)
-            args[index] = new_code_block
+            new_args[index] = new_code_block
+            args = tuple(new_args)
 
         return super().append(*args, **kwargs)
 
 
-def setup(app):
+def setup(app: Any) -> None:
     """Register new directives, augmented with ANSI coloring.
 
     New directives:
         - ``.. click:example::``
         - ``.. click:run::``
 
     .. danger::
```

### Comparing `click_extra-4.7.4/click_extra/tabulate.py` & `click_extra-4.7.5/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/telemetry.py` & `click_extra-4.7.5/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/testing.py` & `click_extra-4.7.5/click_extra/testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/__init__.py` & `click_extra-4.7.5/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/conftest.py` & `click_extra-4.7.5/click_extra/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_colorize.py` & `click_extra-4.7.5/click_extra/tests/test_colorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,21 @@
     skip_windows_colors,
 )
 
 
 def test_theme_definition():
     """Ensure we do not leave any property we would have inherited from cloup and
     logging primitives."""
-    assert set(HelpTheme.__dataclass_fields__).issubset(
-        HelpExtraTheme.__dataclass_fields__,
+    assert (
+        set(HelpTheme.__dataclass_fields__)
+        <= HelpExtraTheme.__dataclass_fields__.keys()
     )
 
     log_levels = {level.lower() for level in LOG_LEVELS}
-    assert log_levels.issubset(HelpExtraTheme.__dataclass_fields__)
+    assert log_levels <= HelpExtraTheme.__dataclass_fields__.keys()
     assert log_levels.isdisjoint(HelpTheme.__dataclass_fields__)
 
 
 def test_extra_theme():
     theme = HelpExtraTheme()
 
     # Check the same instance is returned when no attribute is set.
```

### Comparing `click_extra-4.7.4/click_extra/tests/test_commands.py` & `click_extra-4.7.5/click_extra/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,35 +56,26 @@
                 continue
             members.add(name)
         return members
 
     click_members = fetch_root_members(click)
 
     cloup_members = {m for m in cloup.__all__ if not m.startswith("_")}
-    # XXX Color cannot be imported from cloup. It leads to an issue in the way autodoc
-    # is trying to render it:
-    #   Exception occurred:
-    #     File ".../python3.11/site-packages/cloup/_util.py", line 128, in __setattr__
-    #       raise Exception("you can't set attributes on this class")
-    #   Exception: you can't set attributes on this class
-    # This has been reported upstream at: https://github.com/janluke/cloup/issues/177
-    # and https://github.com/sphinx-doc/sphinx/issues/11986
-    cloup_members.remove("Color")
 
     tree = ast.parse(Path(__file__).parent.joinpath("../__init__.py").read_bytes())
     click_extra_members = []
     for node in tree.body:
         if isinstance(node, ast.Assign):
             for target in node.targets:
                 if target.id == "__all__":
                     for element in node.value.elts:
                         click_extra_members.append(element.s)
 
-    assert click_members.issubset(click_extra_members)
-    assert cloup_members.issubset(click_extra_members)
+    assert click_members <= set(click_extra_members)
+    assert cloup_members <= set(click_extra_members)
 
     expected_members = sorted(
         click_members.union(cloup_members).union(click_extra_members),
         key=lambda m: (m.lower(), m),
     )
     assert expected_members == click_extra_members
```

### Comparing `click_extra-4.7.4/click_extra/tests/test_config.py` & `click_extra-4.7.5/click_extra/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_logging.py` & `click_extra-4.7.5/click_extra/tests/test_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def test_level_default_order():
     assert tuple(LOG_LEVELS) == ("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG")
 
 
 def test_root_logger_defaults():
     """Check our internal default is aligned to Python's root logger."""
-    # Check the root logger is the default logger, ans that getLogger is
+    # Check the root logger is the default logger, and that getLogger is
     # properly patched on Python 3.8.
     assert logging.getLogger() is logging.getLogger("root")
     assert logging.getLogger() is logging.root
 
     # Check root logger's level.
     assert logging.root.getEffectiveLevel() == logging.WARNING
     assert logging._levelToName[logging.root.level] == "WARNING"
```

### Comparing `click_extra-4.7.4/click_extra/tests/test_parameters.py` & `click_extra-4.7.5/click_extra/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_platforms.py` & `click_extra-4.7.5/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_pygments.py` & `click_extra-4.7.5/click_extra/tests/test_pygments.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             # Extarct lexer alias from the test file path.
             lexer_candidates.add(filename.parent.name)
 
     assert lexer_candidates
     lexer_classes = {find_lexer_class_by_name(alias) for alias in lexer_candidates}
     # We cannot test for strict equality yet, as some ANSI-ready lexers do not
     # have any test artifacts producing ``Generic.Output`` tokens.
-    assert lexer_classes.issubset(collect_session_lexers())
+    assert lexer_classes <= set(collect_session_lexers())
 
 
 def collect_classes(klass, prefix="Ansi"):
     """Returns all classes defined in ``click_extra.pygments`` that are a subclass of
     ``klass``, and whose name starts with the provided ``prefix``."""
     klasses = {}
     for name, var in extra_pygments.__dict__.items():
```

### Comparing `click_extra-4.7.4/click_extra/tests/test_tabulate.py` & `click_extra-4.7.5/click_extra/tests/test_tabulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,16 +506,16 @@
     "vertical": vertical_table,
 }
 
 
 def test_recognized_modes():
     """Check all rendering modes proposed by the table module are accounted for and
     there is no duplicates."""
-    assert set(tabulate._table_formats).issubset(expected_renderings.keys())
-    assert set(tabulate._table_formats).issubset(output_formats)
+    assert set(tabulate._table_formats) <= expected_renderings.keys()
+    assert set(tabulate._table_formats) <= set(output_formats)
 
     assert len(output_formats) == len(expected_renderings.keys())
     assert set(output_formats) == set(expected_renderings.keys())
 
 
 @fixture
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
```

### Comparing `click_extra-4.7.4/click_extra/tests/test_telemetry.py` & `click_extra-4.7.5/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_testing.py` & `click_extra-4.7.5/click_extra/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_timer.py` & `click_extra-4.7.5/click_extra/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/tests/test_version.py` & `click_extra-4.7.5/click_extra/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/timer.py` & `click_extra-4.7.5/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/click_extra/version.py` & `click_extra-4.7.5/click_extra/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,26 +91,22 @@
         exec_name: str | None = None,
         version: str | None = None,
         prog_name: str | None = None,
         env_info: dict[str, str] | None = None,
         # Field style overrides.
         message_style: IStyle | None = None,
         module_style: IStyle | None = None,
-        module_name_style: IStyle
-        | None = default_theme.invoked_command,  # type: ignore[has-type]
+        module_name_style: IStyle | None = default_theme.invoked_command,
         module_file_style: IStyle | None = None,
         module_version_style: IStyle | None = Style(fg="green"),
-        package_name_style: IStyle
-        | None = default_theme.invoked_command,  # type: ignore[has-type]
+        package_name_style: IStyle | None = default_theme.invoked_command,
         package_version_style: IStyle | None = Style(fg="green"),
-        exec_name_style: IStyle
-        | None = default_theme.invoked_command,  # type: ignore[has-type]
+        exec_name_style: IStyle | None = default_theme.invoked_command,
         version_style: IStyle | None = Style(fg="green"),
-        prog_name_style: IStyle
-        | None = default_theme.invoked_command,  # type: ignore[has-type]
+        prog_name_style: IStyle | None = default_theme.invoked_command,
         env_info_style: IStyle | None = Style(fg="bright_black"),
         is_flag=True,
         expose_value=False,
         is_eager=True,
         help=_("Show the version and exit."),
         **kwargs,
     ) -> None:
```

### Comparing `click_extra-4.7.4/pyproject.toml` & `click_extra-4.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.7.4"
+version = "4.7.5"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -66,22 +66,21 @@
 
 [tool.poetry.dependencies]
 # Python versions and their status: https://devguide.python.org/versions/
 python = "^3.8"
 # XXX boltons.ecoutils 23.0.0 breaks PDB interactive sessions in pytest.
 # Investigation of the root cause is being discussed upstream at:
 # https://github.com/mahmoud/boltons/issues/334
-boltons = "^23.0.0"
+boltons = "^24.0.0"
 # Click 8.1.4 fix @group.command calls with a custom command_class. See:
 # https://github.com/pallets/click/issues/2416
 # https://github.com/pallets/click/pull/2417
 click = "^8.1.4"
-# Cloup 3.0.0 changed HelpTheme to a dataclass: https://github.com/janluke/cloup/pull/163
-# Cloup 3.0.1 fixed copying of Constraint: https://github.com/janluke/cloup/issues/166
-cloup = "^3.0.1"
+# Cloup 3.0.5 fix incompatibility with autodoc: https://github.com/janluke/cloup/issues/177
+cloup = "^3.0.5"
 commentjson = "^0.9.0"
 mergedeep = "^1.3.4"
 # Pallets-Sphinx-Themes 2.1.1 is the first version removing old and conflicting Python 2 code.
 Pallets-Sphinx-Themes = "^2.1.1"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
 pygments = "^2.14"
 # pygments-ansi-color 0.3.0 is the first version to set the default theme of ANSI colors.
@@ -101,20 +100,18 @@
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = { extras = ["toml"], version = "^7.2.3" }
 furo = "^2024.1.29"
 mypy = "^1.2.0"
 myst-parser = "^2.0.0"
-# XXX Cap pytest to 7.x series while we wait for https://github.com/smarie/python-pytest-cases/issues/330
-# to be fixed.
-pytest = "<8.0.0"
+pytest = "^8.0.0"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
-pytest-cases = "^3.7.0"
-pytest-cov = "^4.0.0"
+pytest-cases = "^3.8.3"
+pytest-cov = "^5.0.0"
 pytest-github-actions-annotate-failures = "^0.2.0"
 pytest-httpserver = "^1.0.6"
 pytest-randomly = "^3.12.0"
 sphinx-autodoc-typehints = "^2.0.0"
 sphinx-copybutton = "^0.5.2"
 # sphinx-design 0.5.0 is the first to allow Sphinx 7.
 sphinx-design = "^0.5.0"
@@ -185,15 +182,15 @@
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
 [tool.bumpversion]
-current_version = "4.7.4"
+current_version = "4.7.5"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 # Update Python package version in any __init__.py file.
 glob = "./**/__init__.py"
 ignore_missing_version = true
```

### Comparing `click_extra-4.7.4/readme.md` & `click_extra-4.7.5/readme.md`

 * *Files identical despite different names*

### Comparing `click_extra-4.7.4/PKG-INFO` & `click_extra-4.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.7.4
+Version: 4.7.5
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -37,17 +37,17 @@
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0)
-Requires-Dist: boltons (>=23.0.0,<24.0.0)
+Requires-Dist: boltons (>=24.0.0,<25.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
-Requires-Dist: cloup (>=3.0.1,<4.0.0)
+Requires-Dist: cloup (>=3.0.5,<4.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0)
 Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: regex (>=2023.3.22,<2024.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.7.4 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.7.5 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -21,16 +21,16 @@
 Interfaces Classifier: Topic :: System :: Logging Classifier: Topic :: System
 :: Shells Classifier: Topic :: Terminals Classifier: Topic :: Text Processing
 :: Filters Classifier: Topic :: Text Processing :: Markup :: HTML Classifier:
 Topic :: Text Processing :: Markup :: Markdown Classifier: Topic :: Text
 Processing :: Markup :: XML Classifier: Topic :: Text Processing :: Markup ::
 reStructuredText Classifier: Topic :: Utilities Classifier: Typing :: Typed
 Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0) Requires-Dist: boltons
-(>=23.0.0,<24.0.0) Requires-Dist: click (>=8.1.4,<9.0.0) Requires-Dist: cloup
-(>=3.0.1,<4.0.0) Requires-Dist: commentjson (>=0.9.0,<0.10.0) Requires-Dist:
+(>=24.0.0,<25.0.0) Requires-Dist: click (>=8.1.4,<9.0.0) Requires-Dist: cloup
+(>=3.0.5,<4.0.0) Requires-Dist: commentjson (>=0.9.0,<0.10.0) Requires-Dist:
 mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pygments (>=2.14,<3.0) Requires-Dist:
 pygments-ansi-color (>=0.3.0,<0.4.0) Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: regex (>=2023.3.22,<2024.0.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: sphinx (>=6) Requires-Dist: tabulate
 [widechars] (>=0.9,<0.10) Requires-Dist: tomli (>=2.0.1,<3.0.0) ;
 python_version < "3.11" Requires-Dist: wcmatch (>=8.5,<9.0) Requires-Dist:
 xmltodict (>=0.13.0,<0.14.0) Project-URL: Changelog, https://
```

