# Comparing `tmp/lean_dojo-1.7.1.tar.gz` & `tmp/lean_dojo-1.8.0.tar.gz`

## Comparing `lean_dojo-1.7.1.tar` & `lean_dojo-1.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/.readthedocs.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/mypy.ini
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/constants.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/container.py
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/utils.py
--rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/ExtractData.lean
--rw-r--r--   0        0        0    48599 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/ast.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/build_lean4_repo.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/cache.py
--rw-r--r--   0        0        0    20990 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/lean.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/trace.py
--rw-r--r--   0        0        0    43534 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/data_extraction/traced_data.py
--rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/interaction/Lean4Repl.lean
--rw-r--r--   0        0        0    17937 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/interaction/dojo.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/src/lean_dojo/interaction/parse_goals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/__init__.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/conftest.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/data_extraction/test_trace.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_commands.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_imports.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_init_errors.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_parse_goals.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_sorry.py
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_tactics.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/tests/interaction/test_timeout.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/LICENSE
--rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/README.md
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 lean_dojo-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/mypy.ini
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tmp.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/constants.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/container.py
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/utils.py
+-rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/ExtractData.lean
+-rw-r--r--   0        0        0    48595 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/ast.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/build_lean4_repo.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/cache.py
+-rw-r--r--   0        0        0    20689 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/lean.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/trace.py
+-rw-r--r--   0        0        0    43534 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/data_extraction/traced_data.py
+-rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/interaction/Lean4Repl.lean
+-rw-r--r--   0        0        0    18121 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/interaction/dojo.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/src/lean_dojo/interaction/parse_goals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/data_extraction/test_trace.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_commands.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_imports.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_init_errors.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_parse_goals.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_sorry.py
+-rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_tactics.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/tests/interaction/test_timeout.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/LICENSE
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/README.md
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 lean_dojo-1.8.0/PKG-INFO
```

### Comparing `lean_dojo-1.7.1/.readthedocs.yaml` & `lean_dojo-1.8.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/__init__.py` & `lean_dojo-1.8.0/src/lean_dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/constants.py` & `lean_dojo-1.8.0/src/lean_dojo/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 from typing import Tuple
 from loguru import logger
 from dotenv import load_dotenv
 
 load_dotenv()
 
-__version__ = "1.7.1"
+__version__ = "1.8.0"
 
 logger.remove()
 if "VERBOSE" in os.environ or "DEBUG" in os.environ:
     logger.add(sys.stderr, level="DEBUG")
 else:
     logger.add(sys.stderr, level="INFO")
```

### Comparing `lean_dojo-1.7.1/src/lean_dojo/container.py` & `lean_dojo-1.8.0/src/lean_dojo/container.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/utils.py` & `lean_dojo-1.8.0/src/lean_dojo/utils.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/ExtractData.lean` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/ExtractData.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/ast.py` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
             node_data = d["node"]
             if i == 0:
                 assert node_data["kind"] == "Lean.Parser.Module.header"
             node = Node.from_data(node_data, lean_file)
             node.traverse_postorder(_get_closure)
             children.append(node)
 
-        return cls(lean_file, lean_file.start_pos(), lean_file.end_pos(), children)
+        return cls(lean_file, lean_file.start_pos, lean_file.end_pos, children)
 
 
 def _parse_children(node_data: Dict[str, Any], lean_file: LeanFile) -> List[Node]:
     children = []
 
     for d in node_data["args"]:
         if (
```

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/build_lean4_repo.py` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/build_lean4_repo.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/cache.py` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/cache.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/lean.py` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/lean.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,43 +209,36 @@
         """Number of lines in a source file."""
         return len(self.code)
 
     def num_columns(self, line_nb: int) -> int:
         """Number of columns in a source file."""
         return len(self.get_line(line_nb))
 
-    def start_pos(self, zero_indexed: bool = False) -> Pos:
+    @property
+    def start_pos(self) -> Pos:
         """Return the start position of a source file.
 
-        Args:
-            zero_indexed (bool, optional): Whether to use 0-index instead of 1-index. Defaults to False.
-
         Returns:
             Pos: A :class:`Pos` object representing the start of this file.
         """
-        if zero_indexed:
-            return Pos(0, 0)
-        else:
-            return Pos(1, 1)
+        return Pos(1, 1)
 
-    def end_pos(self, zero_indexed: bool = False) -> Pos:
+    @property
+    def end_pos(self) -> Pos:
         """Return the end position of a source file.
 
         Args:
             zero_indexed (bool, optional): Whether to use 0-index instead of 1-index. Defaults to False.
 
         Returns:
             Pos: A :class:`Pos` object representing the end of this file.
         """
         # Line and column numbers are 1-indexed by default.
-        line_nb = self.num_lines - 1
-        column_nb = len(self.code[-1])
-        if not zero_indexed:
-            line_nb += 1
-            column_nb += 1
+        line_nb = self.num_lines
+        column_nb = 1 + len(self.code[-1])
         return Pos(line_nb, column_nb)
 
     def convert_pos(self, byte_idx: int) -> Pos:
         """Convert a byte index (:code:`String.Pos` in Lean 4) to a :class:`Pos` object."""
         n = 0
         for i, num_bytes in enumerate(self.num_bytes, start=1):
             n += num_bytes
```

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/trace.py` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/trace.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/data_extraction/traced_data.py` & `lean_dojo-1.8.0/src/lean_dojo/data_extraction/traced_data.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/interaction/Lean4Repl.lean` & `lean_dojo-1.8.0/src/lean_dojo/interaction/Lean4Repl.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/src/lean_dojo/interaction/dojo.py` & `lean_dojo-1.8.0/src/lean_dojo/interaction/dojo.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from ..constants import (
     TMP_DIR,
     TACTIC_CPU_LIMIT,
     TACTIC_MEMORY_LIMIT,
 )
 from ..utils import to_json_path
 from .parse_goals import parse_goals, Goal
-from ..data_extraction.traced_data import TracedFile
 from ..data_extraction.trace import get_traced_repo_path
 from ..data_extraction.lean import Theorem, LeanGitRepo, Pos
 from ..container import get_container, Mount, NativeContainer, DockerContainer
+from ..data_extraction.traced_data import TracedFile, get_code_without_comments
 
 
 _REPL_PROMPT = "REPL>"
 
 
 @dataclass(frozen=True)
 class CommandState:
@@ -364,17 +364,20 @@
         if self.uses_tactics:
             # Interaction through tactics.
             modified_code = self._modify_proof(traced_file)
         else:
             # Interaction through commands (supported only in Lean 4 via CommandElabM).
             lean_file = traced_file.lean_file
             pos = Pos(line_nb=self.entry[2], column_nb=1)
+            code_before = get_code_without_comments(
+                lean_file, lean_file.start_pos, pos, traced_file.comments
+            )
             modified_code = (
                 self._get_imports()
-                + lean_file[:pos]
+                + code_before
                 + "set_option maxHeartbeats 0 in\n#lean_dojo_repl\n\n"
                 + lean_file[pos:]
             )
 
         repl_file = "Lean4Repl.lean"
         repl_dst = Path(repl_file)
         with open("lakefile.lean", "a") as oup:
@@ -405,20 +408,22 @@
                 f"Failed to locate the theorem with `{self.entry.full_name}` as its fully qualified name"
             )
         proof_start, proof_end = traced_theorem.locate_proof()
         lean_file = traced_file.lean_file
 
         code_import = self._get_imports()
         code_proof = "\nby\n  lean_dojo_repl\n  sorry\n"
-        code_before_theorem = lean_file[: traced_theorem.start]
+        code_before_theorem = get_code_without_comments(
+            lean_file, lean_file.start_pos, traced_theorem.start, traced_file.comments
+        )
         code_thereom = lean_file[traced_theorem.start : proof_start]
         modified_code = (
             code_import
             + code_before_theorem
-            + "set_option maxHeartbeats 0 in\n"
+            + "\nset_option maxHeartbeats 0 in\n"
             + code_thereom
             + code_proof
             + lean_file[proof_end:]
         )
 
         return str(modified_code)
 
@@ -475,24 +480,22 @@
 
         Raises:
             DojoCrashError: _description_
 
         Returns:
             Dict[str, Any]: _description_
         """
-        logger.debug(f"Request: {req}")
         if self.proc.stdin is None:
             raise RuntimeError("self.proc.stdin is not initialized")
         self._check_alive()
         self.proc.stdin.write(req + "\n")
         try:
             res, msg = self._read_next_line()
         except EOFError:
-            raise DojoCrashError("EOF")
-        # logger.debug(f"Response: {res}")
+            raise DojoCrashError("Unexpected EOF")
         try:
             result: Dict[str, Any] = json.loads(res)
         except json.decoder.JSONDecodeError:
             raise DojoCrashError(f"Invalid JSON: {res}")
 
         result["message"] = msg
         return result
```

### Comparing `lean_dojo-1.7.1/src/lean_dojo/interaction/parse_goals.py` & `lean_dojo-1.8.0/src/lean_dojo/interaction/parse_goals.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/tests/conftest.py` & `lean_dojo-1.8.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def std4_repo():
     commit = get_latest_commit(STD4_URL)
     return LeanGitRepo(STD4_URL, commit)
 
 
 @pytest.fixture(scope="session")
 def mathlib4_repo():
-    commit = "3c307701fa7e9acbdc0680d7f3b9c9fed9081740"
+    commit = "fe4454af900584467d21f4fd4fe951d29d9332a7"
     return LeanGitRepo(MATHLIB4_URL, commit)
 
 
 @pytest.fixture(scope="session")
 def latest_mathlib4_repo():
     commit = get_latest_commit(MATHLIB4_URL)
     return LeanGitRepo(MATHLIB4_URL, commit)
```

### Comparing `lean_dojo-1.7.1/tests/interaction/test_commands.py` & `lean_dojo-1.8.0/tests/interaction/test_commands.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/tests/interaction/test_imports.py` & `lean_dojo-1.8.0/tests/interaction/test_imports.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/tests/interaction/test_init_errors.py` & `lean_dojo-1.8.0/tests/interaction/test_init_errors.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/tests/interaction/test_sorry.py` & `lean_dojo-1.8.0/tests/interaction/test_sorry.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/tests/interaction/test_tactics.py` & `lean_dojo-1.8.0/tests/interaction/test_tactics.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/.gitignore` & `lean_dojo-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/LICENSE` & `lean_dojo-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.7.1/README.md` & `lean_dojo-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## Requirements
 
 * Supported platforms: Linux, Windows WSL, and macOS
 * Git >= 2.25
 * 3.9 <= Python < 3.11
 * wget
 * [elan](https://github.com/leanprover/elan)
-* Recommended: Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
+* Strongly Rrecommended: Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
 
 
 ## Installation
 
 LeanDojo is available on [PyPI](https://pypi.org/project/lean-dojo/) and can be installed via pip:
 ```bash
 pip install lean-dojo
@@ -49,16 +49,16 @@
 * For general questions and discussions, please use [GitHub Discussions](https://github.com/lean-dojo/LeanDojo/discussions).  
 * To report a potential bug, please open an issue. In the issue, please include your OS information, the version of LeanDojo, the exact steps to reproduce the error, and complete logs in debug mode (setting the environment variable `VERBOSE` to 1). The more details you provide, the better we will be able to help you. 
 
 
 ## Related Links
 
 * [LeanDojo Website](https://leandojo.org/): The official website of LeanDojo.
-* [LeanDojo Benchmark](https://doi.org/10.5281/zenodo.8016385) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8016385.svg)](https://doi.org/10.5281/zenodo.8016385): The dataset used in our paper, consisting of 98,734 theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/19c869efa56bbb8b500f2724c0b77261edbfa28c) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb). 
-* [LeanDojo Benchmark 4](https://doi.org/10.5281/zenodo.8040109) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8040109.svg)](https://doi.org/10.5281/zenodo.8040109): The Lean 4 version of LeanDojo Benchmark, consisting of 106,446 theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/3c307701fa7e9acbdc0680d7f3b9c9fed9081740) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
+* [LeanDojo Benchmark](https://doi.org/10.5281/zenodo.8016385) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8016385.svg)](https://doi.org/10.5281/zenodo.8016385): The dataset used in our paper, consisting of theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/19c869efa56bbb8b500f2724c0b77261edbfa28c) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb). 
+* [LeanDojo Benchmark 4](https://doi.org/10.5281/zenodo.8040109) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8040109.svg)](https://doi.org/10.5281/zenodo.8040109): The Lean 4 version of LeanDojo Benchmark, consisting of theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/fe4454af900584467d21f4fd4fe951d29d9332a7) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
 * [ReProver](https://github.com/lean-dojo/ReProver): The ReProver (Retrieval-Augmented Prover) model in our paper.
 * [LeanDojo ChatGPT Plugin](https://github.com/lean-dojo/LeanDojoChatGPT)
 * [Lean Copilot: Running language models as copilots for theorem proving in Lean](https://github.com/lean-dojo/LeanCopilot)
 
 ## Citation
 
 [LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://leandojo.org/)
```

### Comparing `lean_dojo-1.7.1/pyproject.toml` & `lean_dojo-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
   "/docs",
   "/images",
   "/scripts",
 ]
 
 [project]
 name = "lean-dojo"
-version = "1.7.1"
+version = "1.8.0"
 authors = [
   { name="Kaiyu Yang", email="kaiyuy@caltech.edu" },
 ]
 description = "LeanDojo: Machine Learning for Theorem Proving in Lean"
 keywords = ["theorem proving", "machine learning", "Lean"]
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.9,<3.11"  # https://docs.ray.io/en/latest/ray-overview/installation.html#daily-releases-nightlies
+requires-python = ">=3.9,<3.12"  # https://docs.ray.io/en/latest/ray-overview/installation.html#daily-releases-nightlies
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
 ]
 dependencies = [
```

### Comparing `lean_dojo-1.7.1/PKG-INFO` & `lean_dojo-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lean-dojo
-Version: 1.7.1
+Version: 1.8.0
 Summary: LeanDojo: Machine Learning for Theorem Proving in Lean
 Project-URL: Homepage, https://leandojo.org/
 Project-URL: Bug Tracker, https://github.com/lean-dojo/LeanDojo/issues
 Author-email: Kaiyu Yang <kaiyuy@caltech.edu>
 License: MIT License
         
         Copyright (c) 2023 LeanDojo Team
@@ -28,15 +28,15 @@
         SOFTWARE.
 License-File: LICENSE
 Keywords: Lean,machine learning,theorem proving
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.11,>=3.9
+Requires-Python: <3.12,>=3.9
 Requires-Dist: filelock
 Requires-Dist: loguru
 Requires-Dist: lxml
 Requires-Dist: networkx
 Requires-Dist: pygithub
 Requires-Dist: python-dotenv
 Requires-Dist: ray[default]>=2.8
@@ -85,15 +85,15 @@
 ## Requirements
 
 * Supported platforms: Linux, Windows WSL, and macOS
 * Git >= 2.25
 * 3.9 <= Python < 3.11
 * wget
 * [elan](https://github.com/leanprover/elan)
-* Recommended: Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
+* Strongly Rrecommended: Generate a [GitHub personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#personal-access-tokens-classic) and set the environment variable `GITHUB_ACCESS_TOKEN` to it
 
 
 ## Installation
 
 LeanDojo is available on [PyPI](https://pypi.org/project/lean-dojo/) and can be installed via pip:
 ```bash
 pip install lean-dojo
@@ -117,16 +117,16 @@
 * For general questions and discussions, please use [GitHub Discussions](https://github.com/lean-dojo/LeanDojo/discussions).  
 * To report a potential bug, please open an issue. In the issue, please include your OS information, the version of LeanDojo, the exact steps to reproduce the error, and complete logs in debug mode (setting the environment variable `VERBOSE` to 1). The more details you provide, the better we will be able to help you. 
 
 
 ## Related Links
 
 * [LeanDojo Website](https://leandojo.org/): The official website of LeanDojo.
-* [LeanDojo Benchmark](https://doi.org/10.5281/zenodo.8016385) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8016385.svg)](https://doi.org/10.5281/zenodo.8016385): The dataset used in our paper, consisting of 98,734 theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/19c869efa56bbb8b500f2724c0b77261edbfa28c) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb). 
-* [LeanDojo Benchmark 4](https://doi.org/10.5281/zenodo.8040109) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8040109.svg)](https://doi.org/10.5281/zenodo.8040109): The Lean 4 version of LeanDojo Benchmark, consisting of 106,446 theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/3c307701fa7e9acbdc0680d7f3b9c9fed9081740) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
+* [LeanDojo Benchmark](https://doi.org/10.5281/zenodo.8016385) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8016385.svg)](https://doi.org/10.5281/zenodo.8016385): The dataset used in our paper, consisting of theorems and proofs extracted from [mathlib](https://github.com/leanprover-community/mathlib/commits/19c869efa56bbb8b500f2724c0b77261edbfa28c) by [generate-benchmark-lean3.ipynb](./scripts/generate-benchmark-lean3.ipynb). 
+* [LeanDojo Benchmark 4](https://doi.org/10.5281/zenodo.8040109) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8040109.svg)](https://doi.org/10.5281/zenodo.8040109): The Lean 4 version of LeanDojo Benchmark, consisting of theorems and proofs extracted from [mathlib4](https://github.com/leanprover-community/mathlib4/commit/fe4454af900584467d21f4fd4fe951d29d9332a7) by [generate-benchmark-lean4.ipynb](./scripts/generate-benchmark-lean4.ipynb).
 * [ReProver](https://github.com/lean-dojo/ReProver): The ReProver (Retrieval-Augmented Prover) model in our paper.
 * [LeanDojo ChatGPT Plugin](https://github.com/lean-dojo/LeanDojoChatGPT)
 * [Lean Copilot: Running language models as copilots for theorem proving in Lean](https://github.com/lean-dojo/LeanCopilot)
 
 ## Citation
 
 [LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://leandojo.org/)
```

