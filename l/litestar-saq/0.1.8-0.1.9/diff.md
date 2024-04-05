# Comparing `tmp/litestar_saq-0.1.8.tar.gz` & `tmp/litestar_saq-0.1.9.tar.gz`

## Comparing `litestar_saq-0.1.8.tar` & `litestar_saq-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/Makefile
--rw-r--r--   0        0        0   190249 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/pdm.lock
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/workflows/docs-preview.yaml
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/workflows/pr-title.yaml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/examples/__init__.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/examples/basic.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/examples/tasks.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/__metadata__.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/_util.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/base.py
--rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/cli.py
--rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/config.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/controllers.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/exceptions.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/litestar_saq/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/tests/docker-compose.yml
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/LICENSE
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/README.md
--rw-r--r--   0        0        0     8383 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 litestar_saq-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/Makefile
+-rw-r--r--   0        0        0   190213 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/pdm.lock
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/workflows/docs-preview.yaml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/workflows/pr-title.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/examples/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/examples/basic.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/examples/tasks.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/__metadata__.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/_util.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/base.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/cli.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/config.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/controllers.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/exceptions.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/litestar_saq/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/tests/docker-compose.yml
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/README.md
+-rw-r--r--   0        0        0     8383 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 litestar_saq-0.1.9/PKG-INFO
```

### Comparing `litestar_saq-0.1.8/.pre-commit-config.yaml` & `litestar_saq-0.1.9/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       - id: check-case-conflict
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.292"
+    rev: "v0.1.0"
     hooks:
       - id: ruff
         args: ["--fix"]
         exclude: "docs"
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
@@ -49,10 +49,10 @@
             pytest-timeout,
             msgspec,
             types-click,
             types-redis,
             "litestar[cli]",
           ]
   - repo: https://github.com/sphinx-contrib/sphinx-lint
-    rev: "v0.6.8"
+    rev: "v0.8.1"
     hooks:
       - id: sphinx-lint
```

### Comparing `litestar_saq-0.1.8/CONTRIBUTING.rst` & `litestar_saq-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/Makefile` & `litestar_saq-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/pdm.lock` & `litestar_saq-0.1.9/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1373,27 +1373,27 @@
 files = [
     {file = "polyfactory-2.9.0-py3-none-any.whl", hash = "sha256:7513347be6327739174dbd4ca6ddd96981fb697437283acb5362a604cf6d7f58"},
     {file = "polyfactory-2.9.0.tar.gz", hash = "sha256:af61fc5b03d0c5bb343a2289bdce457f27bbf8aefba69c592dca0841f905e7a5"},
 ]
 
 [[package]]
 name = "pre-commit"
-version = "3.4.0"
+version = "3.5.0"
 requires_python = ">=3.8"
 summary = "A framework for managing and maintaining multi-language pre-commit hooks."
 dependencies = [
     "cfgv>=2.0.0",
     "identify>=1.0.0",
     "nodeenv>=0.11.1",
     "pyyaml>=5.1",
     "virtualenv>=20.10.0",
 ]
 files = [
-    {file = "pre_commit-3.4.0-py2.py3-none-any.whl", hash = "sha256:96d529a951f8b677f730a7212442027e8ba53f9b04d217c4c67dc56c393ad945"},
-    {file = "pre_commit-3.4.0.tar.gz", hash = "sha256:6bbd5129a64cad4c0dfaeeb12cd8f7ea7e15b77028d985341478c8af3c759522"},
+    {file = "pre_commit-3.5.0-py2.py3-none-any.whl", hash = "sha256:841dc9aef25daba9a0238cd27984041fa0467b4199fc4852e27950664919f660"},
+    {file = "pre_commit-3.5.0.tar.gz", hash = "sha256:5804465c675b659b0862f07907f96295d490822a450c4c40e747d0b1c6ebcb32"},
 ]
 
 [[package]]
 name = "pycparser"
 version = "2.21"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "C parser in Python"
@@ -1690,35 +1690,35 @@
     {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-win32.whl", hash = "sha256:84b554931e932c46f94ab306913ad7e11bba988104c5cff26d90d03f68258cd5"},
     {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-win_amd64.whl", hash = "sha256:25ac8c08322002b06fa1d49d1646181f0b2c72f5cbc15a85e80b4c30a544bb15"},
     {file = "ruamel.yaml.clib-0.2.8.tar.gz", hash = "sha256:beb2e0404003de9a4cab9753a8805a8fe9320ee6673136ed7f04255fe60bb512"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.292"
+version = "0.1.0"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 files = [
-    {file = "ruff-0.0.292-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:02f29db018c9d474270c704e6c6b13b18ed0ecac82761e4fcf0faa3728430c96"},
-    {file = "ruff-0.0.292-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:69654e564342f507edfa09ee6897883ca76e331d4bbc3676d8a8403838e9fade"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c3c91859a9b845c33778f11902e7b26440d64b9d5110edd4e4fa1726c41e0a4"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f4476f1243af2d8c29da5f235c13dca52177117935e1f9393f9d90f9833f69e4"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:be8eb50eaf8648070b8e58ece8e69c9322d34afe367eec4210fdee9a555e4ca7"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:9889bac18a0c07018aac75ef6c1e6511d8411724d67cb879103b01758e110a81"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6bdfabd4334684a4418b99b3118793f2c13bb67bf1540a769d7816410402a205"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:aa7c77c53bfcd75dbcd4d1f42d6cabf2485d2e1ee0678da850f08e1ab13081a8"},
-    {file = "ruff-0.0.292-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8e087b24d0d849c5c81516ec740bf4fd48bf363cfb104545464e0fca749b6af9"},
-    {file = "ruff-0.0.292-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:f160b5ec26be32362d0774964e218f3fcf0a7da299f7e220ef45ae9e3e67101a"},
-    {file = "ruff-0.0.292-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:ac153eee6dd4444501c4bb92bff866491d4bfb01ce26dd2fff7ca472c8df9ad0"},
-    {file = "ruff-0.0.292-py3-none-musllinux_1_2_i686.whl", hash = "sha256:87616771e72820800b8faea82edd858324b29bb99a920d6aa3d3949dd3f88fb0"},
-    {file = "ruff-0.0.292-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:b76deb3bdbea2ef97db286cf953488745dd6424c122d275f05836c53f62d4016"},
-    {file = "ruff-0.0.292-py3-none-win32.whl", hash = "sha256:e854b05408f7a8033a027e4b1c7f9889563dd2aca545d13d06711e5c39c3d003"},
-    {file = "ruff-0.0.292-py3-none-win_amd64.whl", hash = "sha256:f27282bedfd04d4c3492e5c3398360c9d86a295be00eccc63914438b4ac8a83c"},
-    {file = "ruff-0.0.292-py3-none-win_arm64.whl", hash = "sha256:7f67a69c8f12fbc8daf6ae6d36705037bde315abf8b82b6e1f4c9e74eb750f68"},
-    {file = "ruff-0.0.292.tar.gz", hash = "sha256:1093449e37dd1e9b813798f6ad70932b57cf614e5c2b5c51005bf67d55db33ac"},
+    {file = "ruff-0.1.0-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:87114e254dee35e069e1b922d85d4b21a5b61aec759849f393e1dbb308a00439"},
+    {file = "ruff-0.1.0-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:764f36d2982cc4a703e69fb73a280b7c539fd74b50c9ee531a4e3fe88152f521"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:65f4b7fb539e5cf0f71e9bd74f8ddab74cabdd673c6fb7f17a4dcfd29f126255"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:299fff467a0f163baa282266b310589b21400de0a42d8f68553422fa6bf7ee01"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0d412678bf205787263bb702c984012a4f97e460944c072fd7cfa2bd084857c4"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:a5391b49b1669b540924640587d8d24128e45be17d1a916b1801d6645e831581"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ee8cd57f454cdd77bbcf1e11ff4e0046fb6547cac1922cc6e3583ce4b9c326d1"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:fa7aeed7bc23861a2b38319b636737bf11cfa55d2109620b49cf995663d3e888"},
+    {file = "ruff-0.1.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b04cd4298b43b16824d9a37800e4c145ba75c29c43ce0d74cad1d66d7ae0a4c5"},
+    {file = "ruff-0.1.0-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:7186ccf54707801d91e6314a016d1c7895e21d2e4cd614500d55870ed983aa9f"},
+    {file = "ruff-0.1.0-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:d88adfd93849bc62449518228581d132e2023e30ebd2da097f73059900d8dce3"},
+    {file = "ruff-0.1.0-py3-none-musllinux_1_2_i686.whl", hash = "sha256:ad2ccdb3bad5a61013c76a9c1240fdfadf2c7103a2aeebd7bcbbed61f363138f"},
+    {file = "ruff-0.1.0-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:b77f6cfa72c6eb19b5cac967cc49762ae14d036db033f7d97a72912770fd8e1c"},
+    {file = "ruff-0.1.0-py3-none-win32.whl", hash = "sha256:480bd704e8af1afe3fd444cc52e3c900b936e6ca0baf4fb0281124330b6ceba2"},
+    {file = "ruff-0.1.0-py3-none-win_amd64.whl", hash = "sha256:a76ba81860f7ee1f2d5651983f87beb835def94425022dc5f0803108f1b8bfa2"},
+    {file = "ruff-0.1.0-py3-none-win_arm64.whl", hash = "sha256:45abdbdab22509a2c6052ecf7050b3f5c7d6b7898dc07e82869401b531d46da4"},
+    {file = "ruff-0.1.0.tar.gz", hash = "sha256:ad6b13824714b19c5f8225871cf532afb994470eecb74631cd3500fe817e6b3f"},
 ]
 
 [[package]]
 name = "saq"
 version = "0.12.0"
 summary = "Distributed Python job queue with asyncio and redis"
 dependencies = [
```

### Comparing `litestar_saq-0.1.8/.github/workflows/cd.yaml` & `litestar_saq-0.1.9/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/.github/workflows/ci.yaml` & `litestar_saq-0.1.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/.github/workflows/docs-preview.yaml` & `litestar_saq-0.1.9/.github/workflows/docs-preview.yaml`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/.github/workflows/docs.yaml` & `litestar_saq-0.1.9/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/.github/workflows/publish.yaml` & `litestar_saq-0.1.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/examples/basic.py` & `litestar_saq-0.1.9/examples/basic.py`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/examples/tasks.py` & `litestar_saq-0.1.9/examples/tasks.py`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/litestar_saq/_util.py` & `litestar_saq-0.1.9/litestar_saq/_util.py`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/litestar_saq/base.py` & `litestar_saq-0.1.9/litestar_saq/base.py`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/litestar_saq/cli.py` & `litestar_saq-0.1.9/litestar_saq/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     import asyncio
     import multiprocessing
     from typing import cast
 
     from click import IntRange, group, option
     from litestar.cli._utils import LitestarGroup, console
 
-    @group(cls=LitestarGroup, name="workers")
+    @group(cls=LitestarGroup, name="workers", no_args_is_help=True)
     def background_worker_group() -> None:
         """Manage background task workers."""
 
     @background_worker_group.command(
         name="run",
         help="Run background worker processes.",
     )
@@ -62,14 +62,34 @@
                 logging_config=cast("BaseLoggingConfig", app.logging_config),
             )
         except KeyboardInterrupt:
             loop = asyncio.get_event_loop()
             for worker_instance in plugin.get_workers():
                 loop.run_until_complete(worker_instance.stop())
 
+    @background_worker_group.command(
+        name="status",
+        help="Check the status of currently configured workers and queues.",
+    )
+    @option("-v", "--verbose", help="Enable verbose logging.", is_flag=True, default=None, type=bool, required=False)
+    @option("-d", "--debug", help="Enable debugging.", is_flag=True, default=None, type=bool, required=False)
+    def worker_status(
+        app: Litestar,
+        verbose: bool | None,
+        debug: bool | None,
+    ) -> None:
+        """Run the API server."""
+        console.rule("[yellow]Checking SAQ worker status[/]", align="left")
+        if app.logging_config is not None:
+            app.logging_config.configure()
+        if debug is not None or verbose is not None:
+            app.debug = True
+        plugin = get_saq_plugin(app)
+        show_saq_info(app, 1, plugin)
+
     return background_worker_group
 
 
 def get_saq_plugin(app: Litestar) -> SAQPlugin:
     """Retrieve a SAQ plugin from the Litestar application's plugins.
 
     This function attempts to find a SAQ plugin instance.
```

### Comparing `litestar_saq-0.1.8/litestar_saq/config.py` & `litestar_saq-0.1.9/litestar_saq/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,18 @@
 
     queue_configs: Collection[QueueConfig] = field(default_factory=lambda: [QueueConfig()])
     """Configuration for Queues"""
     redis: Redis | None = None
     """Pre-configured Redis instance to use."""
     redis_url: str | None = None
     """Redis URL to connect with."""
+    redis_kwargs: dict[str, Any] = field(
+        default_factory=lambda: {"socket_connect_timeout": 2, "socket_keepalive": 5, "health_check_interval": 5},
+    )
+    """Redis kwargs to pass into a redis instance."""
     namespace: str = "saq"
     """Namespace to use for Redis"""
     queue_instances: Mapping[str, Queue] | None = None
     """Current configured queue instances.  When None, queues will be auto-created on startup"""
     queues_dependency_key: str = field(default="task_queues")
     """Key to use for storing dependency information in litestar."""
     worker_processes: int = 1
@@ -135,20 +139,16 @@
         Returns:
             Dictionary of queues.
         """
         if self.redis is not None:
             return self.redis
         pool = ConnectionPool.from_url(
             url=cast("str", self.redis_url),
-            decode_responses=False,
-            socket_connect_timeout=2,
-            socket_keepalive=5,
-            health_check_interval=5,
         )
-        self.redis = Redis(connection_pool=pool)
+        self.redis = Redis(connection_pool=pool, **self.redis_kwargs)
         return self.redis
 
     def get_queues(self) -> TaskQueues:
         """Get the configured SAQ queues.
 
         Returns:
             Dictionary of queues.
```

### Comparing `litestar_saq-0.1.8/litestar_saq/controllers.py` & `litestar_saq-0.1.9/litestar_saq/controllers.py`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/litestar_saq/plugin.py` & `litestar_saq-0.1.9/litestar_saq/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/.gitignore` & `litestar_saq-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/LICENSE` & `litestar_saq-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar_saq-0.1.8/README.md` & `litestar_saq-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 
 
 ```
 
 You can start a background worker with the following command now:
 
 ```shell
-litestar --app-dir=examples/ --app basic:app tasks run-worker
+litestar --app-dir=examples/ --app basic:app workers run
 Using Litestar app from env: 'basic:app'
 Starting SAQ Workers ──────────────────────────────────────────────────────────────────
 INFO - 2023-10-04 17:39:03,255 - saq - worker - Worker starting: Queue<redis=Redis<ConnectionPool<Connection<host=localhost,port=6397,db=0>>>, name='samples'>
 INFO - 2023-10-04 17:39:06,545 - saq - worker - Worker shutting down
 ```
```

### Comparing `litestar_saq-0.1.8/pyproject.toml` & `litestar_saq-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   "litestar",
   "saq",
 ]
 license = {text = "MIT"}
 name = "litestar-saq"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.1.8"
+version = "0.1.9"
 
 [project.urls]
 Changelog = "https://cofin.github.io/litesatr-saq/latest/changelog"
 Discord = "https://discord.gg/X3FJqy8d2j"
 Documentation = "https://cofin.github.io/litesatr-saq/latest/"
 Homepage = "https://cofin.github.io/litesatr-saq/latest/"
 Issue = "https://github.com/cofin/litestar-saq/issues/"
```

### Comparing `litestar_saq-0.1.8/PKG-INFO` & `litestar_saq-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar-saq
-Version: 0.1.8
+Version: 0.1.9
 Summary: Litestar integration for SAQ
 Project-URL: Changelog, https://cofin.github.io/litesatr-saq/latest/changelog
 Project-URL: Discord, https://discord.gg/X3FJqy8d2j
 Project-URL: Documentation, https://cofin.github.io/litesatr-saq/latest/
 Project-URL: Homepage, https://cofin.github.io/litesatr-saq/latest/
 Project-URL: Issue, https://github.com/cofin/litestar-saq/issues/
 Project-URL: Source, https://github.com/cofin/litestar-saq
@@ -57,13 +57,13 @@
 
 
 ```
 
 You can start a background worker with the following command now:
 
 ```shell
-litestar --app-dir=examples/ --app basic:app tasks run-worker
+litestar --app-dir=examples/ --app basic:app workers run
 Using Litestar app from env: 'basic:app'
 Starting SAQ Workers ──────────────────────────────────────────────────────────────────
 INFO - 2023-10-04 17:39:03,255 - saq - worker - Worker starting: Queue<redis=Redis<ConnectionPool<Connection<host=localhost,port=6397,db=0>>>, name='samples'>
 INFO - 2023-10-04 17:39:06,545 - saq - worker - Worker shutting down
 ```
```

