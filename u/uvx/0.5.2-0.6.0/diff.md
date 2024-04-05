# Comparing `tmp/uvx-0.5.2.tar.gz` & `tmp/uvx-0.6.0.tar.gz`

## Comparing `uvx-0.5.2.tar` & `uvx-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 uvx-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/_constants.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/_maybe.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/_python.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/_symlinks.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/cli.py
--rw-r--r--   0        0        0    12957 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/core.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.5.2/src/uvx/py.typed
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.5.2/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.5.2/README.md
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 uvx-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_constants.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_maybe.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_python.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/_symlinks.py
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/cli.py
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/core.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uvx-0.6.0/src/uvx/py.typed
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 uvx-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 uvx-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 uvx-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 uvx-0.6.0/README.md
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 uvx-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 uvx-0.6.0/PKG-INFO
```

### Comparing `uvx-0.5.2/CHANGELOG.md` & `uvx-0.6.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.6.0 (2024-04-05)
+
+### Feature
+
+* Implemented  first version of `uvx upgrade` ([`ffcb73a`](https://github.com/robinvandernoord/uvx/commit/ffcb73ad928f089ef3c0c3705b00fc04c840c9ff))
+* Work in progress on uvx upgrade ([`d48524a`](https://github.com/robinvandernoord/uvx/commit/d48524adf5a9a08ae4d4b8485789ff33e937f278))
+
 ## v0.5.2 (2024-03-19)
 
 ### Fix
 
 * Exclude these files from pip build ([`0899653`](https://github.com/robinvandernoord/uvx/commit/08996536a64b78680d2cf8e452ee3e871a610464))
 
 ## v0.5.1 (2024-03-19)
```

### Comparing `uvx-0.5.2/src/uvx/_python.py` & `uvx-0.6.0/src/uvx/_python.py`

 * *Files identical despite different names*

### Comparing `uvx-0.5.2/src/uvx/_symlinks.py` & `uvx-0.6.0/src/uvx/_symlinks.py`

 * *Files identical despite different names*

### Comparing `uvx-0.5.2/src/uvx/cli.py` & `uvx-0.6.0/src/uvx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 
 @app.command()
 def inject(into: str, package_specs: list[str]):
     output(
         inject_packages(
             into,
-            package_specs,
+            set(package_specs),
         )
     )
 
 
 # list
 def _list_short(name: str, metadata: Maybe[Metadata]):
     rich.print("-", name, metadata.map_or("[red]?[/red]", lambda md: md.installed_version))
@@ -174,17 +174,17 @@
 def runpython(venv: str, ctx: Context):
     """Run 'python' in the right venv."""
     with as_virtualenv(venv) as venv_path:
         python = venv_path / "bin" / "python"
         subprocess.run([python, *ctx.args])  # nosec
 
 
+# todo:
 # self-upgrade (uv and uvx)
-
-# ...
+# upgrade-all
 
 
 def add_to_bashrc(text: str, with_comment: bool = True):
     """Add text to ~/.bashrc, usually with a comment (uvx + timestamp)."""
     with (Path.home() / ".bashrc").resolve().open("a") as f:
         now = str(datetime.now()).split(".")[0]
         final_text = "\n"
```

### Comparing `uvx-0.5.2/src/uvx/core.py` & `uvx-0.6.0/src/uvx/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     python = python or existing_metadata.map_or(None, lambda metadata: metadata.python_raw)
 
     uninstall_package(new_metadata.name, force=force)
     extras = metadata.injected if (with_injected and metadata and metadata.injected) else []
     return install_package(install_spec, python=python, force=force, extras=extras, no_cache=no_cache)
 
 
-def inject_packages(into: str, package_specs: list[str]) -> Result[str, Exception]:
+def inject_packages(into: str, package_specs: set[str]) -> Result[str, Exception]:
     match collect_metadata(into):
         case Err(e):
             return Err(e)
         case Ok(meta):
             # just bind meta
             ...
 
@@ -253,15 +253,15 @@
 
     with virtualenv(venv), exit_on_pb_error():
         try:
             animate(uv("pip", "install", *package_specs), text=f"injecting {package_specs}")
         except plumbum.ProcessExecutionError as e:
             return Err(e)
 
-    meta.injected = (meta.injected or []) + package_specs
+    meta.injected = (meta.injected or set()) | package_specs
     store_metadata(meta, venv)
 
     return Ok(f"💉 Injected {package_specs} into {meta.name}.")  # :needle:
 
 
 def remove_dir(path: Path):
     """
@@ -275,34 +275,66 @@
 
 
 def upgrade_package(
     package_name: str, force: bool = False, skip_injected: bool = False, no_cache: bool = False
 ) -> Result[str, Exception]:
     # run `uv pip install --upgrade package` with requested install spec (version, extras, injected)
     # if --force is used, the previous version is ignored.
-    print("upgrade", package_name)
-
     match collect_metadata(package_name):
         case Err(e):
             return Err(e)
         case Ok(spec_metadata):
             # bind spec_metadata
             ...
 
     workdir = ensure_local_folder()
     venv = workdir / "venvs" / spec_metadata.name
 
     if not venv.exists():
-        return Err(
-            NotADirectoryError(
-                f"No virtualenv for '{package_name}', stopping. Use '--force' to remove an executable with that name anyway."
-            )
-        )
+        return Err(NotADirectoryError(f"No virtualenv for '{package_name}', stopping. Use 'uvx install' instead."))
+
+    meta = read_metadata(venv).unwrap_or(spec_metadata)
+
+    old_version = meta.installed_version
+
+    with virtualenv(venv), exit_on_pb_error():
+        # pip upgrade package[extras]==version *injected
+        # if version spec in spec_metadata use that instead
+        # if --force, drop version spec
+        base_pkg = meta.name
+        extras = meta.extras
+        injected = [] if skip_injected else (meta.injected or [])
+        version = spec_metadata.requested_version or ("" if force else meta.requested_version)
+        options = []
+        if force:
+            options.append("--no-cache")
+
+        upgrade_spec = base_pkg + version
+        if extras:
+            upgrade_spec += "[" + ",".join(extras) + "]"
+
+        try:
+            animate(uv("pip", "install", "--upgrade", upgrade_spec, *injected, *options), text=f"upgrading {base_pkg}")
+        except plumbum.ProcessExecutionError as e:
+            return Err(e)
+
+        meta.requested_version = version
+        new_version = meta.installed_version = get_package_version(meta.name, venv)
+        store_metadata(meta, venv)
+
+    if old_version == new_version:
+        # todo: if meta.requested_version - warn
+        msg = f"🌟 '{package_name}' is already up to date at version {new_version}!"
+        if meta.requested_version:
+            msg += f"\n💡 This package was installed with a version constraint ({meta.requested_version}). If you want to ignore this constraint, use `uvx upgrade --force {package_name}`."
+
+    else:
+        msg = f"🚀 Successfully updated '{package_name}' from version {old_version} to version {new_version}!"
 
-    return Ok("todo")
+    return Ok(msg)
 
 
 def uninstall_package(package_name: str, force: bool = False) -> Result[str, Exception]:
     """
     Uninstalls a package.
 
     Args:
```

### Comparing `uvx-0.5.2/src/uvx/metadata.py` & `uvx-0.6.0/src/uvx/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     scripts: dict[str, bool]  # {script: is_installed}
     install_spec: str  # e.g. '2fas' or '2fas[gui]>=0.1.0'
     extras: set[str]  # .e.g. {'gui'}
     requested_version: Optional[str]  # e.g. ">=0.1.0"
     installed_version: str
     python: str = ""
     python_raw: str = ""
-    injected: Optional[list[str]] = None
+    injected: Optional[set[str]] = None
 
     @typing.overload
     def _convert_type(self, value: set[V]) -> list[V]:  # type: ignore
         """Convert set of V to list of V."""
 
     @typing.overload
     def _convert_type(self, value: T) -> T:
```

### Comparing `uvx-0.5.2/LICENSE.txt` & `uvx-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uvx-0.5.2/README.md` & `uvx-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `uvx-0.5.2/pyproject.toml` & `uvx-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-0.5.2/PKG-INFO` & `uvx-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 0.5.2
+Version: 0.6.0
 Summary: uvx: pipx for uv
 Project-URL: Documentation, https://github.com/robinvandernoord/uvx#readme
 Project-URL: Issues, https://github.com/robinvandernoord/uvx/issues
 Project-URL: Source, https://github.com/robinvandernoord/uvx
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

