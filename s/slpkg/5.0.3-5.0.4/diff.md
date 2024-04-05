# Comparing `tmp/slpkg-5.0.3.tar.gz` & `tmp/slpkg-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slpkg-5.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "slpkg-5.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `slpkg-5.0.3.tar` & `slpkg-5.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1945 2024-04-01 14:26:33.000000 slpkg-5.0.3/README.md
--rw-r--r--   0        0        0     1716 2024-04-01 14:26:33.000000 slpkg-5.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/binaries/__init__.py
--rw-r--r--   0        0        0     8384 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/binaries/install.py
--rw-r--r--   0        0        0     2306 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/binaries/required.py
--rw-r--r--   0        0        0      985 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/blacklist.py
--rw-r--r--   0        0        0     6379 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/check_updates.py
--rw-r--r--   0        0        0     1374 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/checks.py
--rw-r--r--   0        0        0     1404 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/checksum.py
--rw-r--r--   0        0        0     4061 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/choose_packages.py
--rw-r--r--   0        0        0      844 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/cleanings.py
--rw-r--r--   0        0        0     5455 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/configs.py
--rw-r--r--   0        0        0     3725 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/dependees.py
--rw-r--r--   0        0        0     1906 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/dialog_box.py
--rw-r--r--   0        0        0     4967 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/dialog_configs.py
--rw-r--r--   0        0        0     4351 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/download_only.py
--rw-r--r--   0        0        0     3852 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/downloader.py
--rw-r--r--   0        0        0      430 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/error_messages.py
--rw-r--r--   0        0        0     1538 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/find_installed.py
--rw-r--r--   0        0        0     1328 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/gpg_verify.py
--rw-r--r--   0        0        0    81814 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/install_data.py
--rw-r--r--   0        0        0     3662 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/load_data.py
--rw-r--r--   0        0        0    27101 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/main.py
--rw-r--r--   0        0        0     6126 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/multi_process.py
--rw-r--r--   0        0        0    11270 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/new_configs.py
--rw-r--r--   0        0        0     2403 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/progress_bar.py
--rw-r--r--   0        0        0     5679 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/remove_packages.py
--rw-r--r--   0        0        0     4341 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/repo_info.py
--rw-r--r--   0        0        0    34786 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/repositories.py
--rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/__init__.py
--rw-r--r--   0        0        0     1075 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/dependencies.py
--rw-r--r--   0        0        0     4561 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/sbo_generate.py
--rw-r--r--   0        0        0    11449 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/sbos/slackbuild.py
--rw-r--r--   0        0        0     2569 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/search.py
--rw-r--r--   0        0        0      587 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/toml_errors.py
--rw-r--r--   0        0        0     4391 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/tracking.py
--rw-r--r--   0        0        0    30454 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/update_repositories.py
--rw-r--r--   0        0        0     8587 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/upgrade.py
--rw-r--r--   0        0        0     7486 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/utilities.py
--rw-r--r--   0        0        0        0 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/__init__.py
--rw-r--r--   0        0        0     5768 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/asciibox.py
--rw-r--r--   0        0        0     6265 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/cli_menu.py
--rw-r--r--   0        0        0      740 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/version.py
--rw-r--r--   0        0        0     6926 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/view_package.py
--rw-r--r--   0        0        0     9945 2024-04-01 14:26:33.000000 slpkg-5.0.3/slpkg/views/views.py
--rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 slpkg-5.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1945 2024-04-05 09:21:31.000000 slpkg-5.0.4/README.md
+-rw-r--r--   0        0        0     1694 2024-04-05 09:21:31.000000 slpkg-5.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/binaries/__init__.py
+-rw-r--r--   0        0        0     8384 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/binaries/install.py
+-rw-r--r--   0        0        0     2306 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/binaries/required.py
+-rw-r--r--   0        0        0      985 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/blacklist.py
+-rw-r--r--   0        0        0     6382 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/check_updates.py
+-rw-r--r--   0        0        0     1273 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/checks.py
+-rw-r--r--   0        0        0     1404 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/checksum.py
+-rw-r--r--   0        0        0     4249 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/choose_packages.py
+-rw-r--r--   0        0        0      844 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/cleanings.py
+-rw-r--r--   0        0        0     5566 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/configs.py
+-rw-r--r--   0        0        0     3725 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/dependees.py
+-rw-r--r--   0        0        0     1944 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/dialog_box.py
+-rw-r--r--   0        0        0     5007 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/dialog_configs.py
+-rw-r--r--   0        0        0     4351 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/download_only.py
+-rw-r--r--   0        0        0     3852 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/downloader.py
+-rw-r--r--   0        0        0      430 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/error_messages.py
+-rw-r--r--   0        0        0     1538 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/find_installed.py
+-rw-r--r--   0        0        0     1328 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/gpg_verify.py
+-rw-r--r--   0        0        0    81814 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/install_data.py
+-rw-r--r--   0        0        0     3657 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/load_data.py
+-rw-r--r--   0        0        0    27101 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/main.py
+-rw-r--r--   0        0        0     6253 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/multi_process.py
+-rw-r--r--   0        0        0    11270 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/new_configs.py
+-rw-r--r--   0        0        0     2661 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/progress_bar.py
+-rw-r--r--   0        0        0     5679 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/remove_packages.py
+-rw-r--r--   0        0        0     4341 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/repo_info.py
+-rw-r--r--   0        0        0    34786 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/repositories.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/sbos/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/sbos/dependencies.py
+-rw-r--r--   0        0        0     4561 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0        0        0    11449 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/sbos/slackbuild.py
+-rw-r--r--   0        0        0     2569 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/search.py
+-rw-r--r--   0        0        0      587 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/toml_errors.py
+-rw-r--r--   0        0        0     4391 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/tracking.py
+-rw-r--r--   0        0        0    31304 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/update_repositories.py
+-rw-r--r--   0        0        0     9177 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/upgrade.py
+-rw-r--r--   0        0        0     7755 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/views/__init__.py
+-rw-r--r--   0        0        0     5768 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/views/asciibox.py
+-rw-r--r--   0        0        0     6265 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/views/cli_menu.py
+-rw-r--r--   0        0        0      740 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/views/version.py
+-rw-r--r--   0        0        0     6926 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/views/view_package.py
+-rw-r--r--   0        0        0     9945 2024-04-05 09:21:31.000000 slpkg-5.0.4/slpkg/views/views.py
+-rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 slpkg-5.0.4/PKG-INFO
```

### Comparing `slpkg-5.0.3/README.md` & `slpkg-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/pyproject.toml` & `slpkg-5.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "slpkg"
-version = "5.0.3"
+version = "5.0.4"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 maintainers = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
@@ -32,16 +32,15 @@
     "Topic :: System :: Installation/Setup",
     "Topic :: System :: Systems Administration",
     "Topic :: System :: Software Distribution",
     "Development Status :: 5 - Production/Stable"
 ]
 
 dependencies = [
-    "pythondialog>=3.5.3",
-    "progress>=1.6",
+    "pythondialog>=3.5.3"
 ]
 
 [tool.flit_core]
 name = "slpkg"
 
 [project.urls]
 Homepage = "https://dslackw.gitlab.io/slpkg/"
```

### Comparing `slpkg-5.0.3/slpkg/binaries/install.py` & `slpkg-5.0.4/slpkg/binaries/install.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/binaries/required.py` & `slpkg-5.0.4/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/blacklist.py` & `slpkg-5.0.4/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/check_updates.py` & `slpkg-5.0.4/slpkg/check_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 self.repositories(repo)
 
     def repositories(self, repo: str) -> None:
         local_chg_txt: Path = Path(self.repos.repositories[repo]['path'],
                                    self.repos.repositories[repo]['changelog_txt'])
         repo_chg_txt: str = (f"{self.repos.repositories[repo]['mirror'][0]}"
                              f"{self.repos.repositories[repo]['changelog_txt']}")
-        repo_data_file: Path = Path(self.repos.repositories_path, repo, self.repos.data_json)
+        repo_data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
 
         if not repo_data_file.is_file():
             self.compare[repo]: dict = True
         else:
             self.compare[repo] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
 
     def compare_the_changelogs(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
@@ -137,15 +137,15 @@
         else:
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
         if self.option_for_check:
             print()
 
     def updates(self) -> dict:
-        message: str = 'Checking for news, please wait...'
+        message: str = 'Checking for news, please wait'
         if self.progress_bar or self.option_for_progress_bar:
             queue = Queue()
 
             # Starting multiprocessing
             process_1 = Process(target=self.check_the_repositories, args=(queue,))
             process_2 = Process(target=self.progress.progress_bar, args=(message,))
 
@@ -160,14 +160,14 @@
                 process_2.terminate()
 
             self.compare: dict = queue.get()
             self.error_connected: list = queue.get()
 
             print('\x1b[?25h')
         else:
-            print(f'\r{message} ', end='')
+            print(f'\r{message}... ', end='')
             self.check_the_repositories()
             print()
 
         self.error_connected_repositories()
         self.view_messages()
         return self.compare
```

### Comparing `slpkg-5.0.3/slpkg/checks.py` & `slpkg-5.0.4/slpkg/checks.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         if not_packages:
             self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
                                             exit_status=1)
 
     def is_package_installed(self, packages: list) -> None:
         """ Checking for installed packages. """
         not_found: list = []
-        blacklist_packages: list = self.utils.ignore_packages(packages)
 
         for pkg in packages:
-            if not self.utils.is_package_installed(pkg) or pkg in blacklist_packages:
+            if not self.utils.is_package_installed(pkg):
                 not_found.append(pkg)
 
         if not_found:
             self.errors.raise_error_message(f"Not found '{', '.join(not_found)}' installed packages",
                                             exit_status=1)
```

### Comparing `slpkg-5.0.3/slpkg/checksum.py` & `slpkg-5.0.4/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/choose_packages.py` & `slpkg-5.0.4/slpkg/choose_packages.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     def packages(self, data: dict, packages: list, method: str) -> list:
         if self.dialog:
             title: str = f' Choose packages you want to {method} '
 
             if method in ('remove', 'find'):
                 self.choose_from_installed(packages)
             elif method == 'upgrade':
+                title: str = f' Choose packages you want to {method} or add '
                 self.choose_for_upgraded(data, packages)
             else:
                 self.choose_for_others(data, packages)
 
             if not self.choices:
                 return packages
 
@@ -44,53 +45,55 @@
                 os.system('clear')
                 raise SystemExit(0)
 
             os.system('clear')
 
         return packages
 
-    def choose_from_installed(self, packages: list):
+    def choose_from_installed(self, packages: list) -> None:
         """ Choose installed packages for remove or find. """
-        installed_packages: list = list(self.utils.all_installed().values())
-
-        for package in installed_packages:
-            package_name: str = self.utils.split_package(package)['name']
-            package_version: str = self.utils.split_package(package)['version']
+        for name, package in self.utils.all_installed().items():
+            version: str = self.utils.split_package(package)['version']
 
             for pkg in packages:
-                if pkg in package or pkg == '*':
-                    self.choices.extend([(package_name, package_version, False, f'Package: {package}')])
+                if pkg in name or pkg == '*':
+                    self.choices.extend([(name, version, False, f'Package: {package}')])
 
-    def choose_for_upgraded(self, data: dict, packages: list):
+    def choose_for_upgraded(self, data: dict, packages: list) -> None:
         """ Choose packages that they will going to upgrade. """
-        for pkg in packages:
-            for package in data.keys():
+        for package in packages:
+
+            if package in data.keys():
+                inst_package: str = self.utils.is_package_installed(package)
+                inst_package_version: str = self.utils.split_package(inst_package)['version']
+                inst_package_build: str = self.utils.split_package(inst_package)['build']
 
-                if pkg == package:
-                    inst_package: str = self.utils.is_package_installed(package)
-                    inst_package_version: str = self.utils.split_package(inst_package)['version']
-                    inst_package_build: str = self.utils.split_package(inst_package)['build']
-                    repo_ver: str = data[package]['version']
-                    repo_build_tag: str = data[package]['build']
+                repo_ver: str = data[package]['version']
+                repo_build_tag: str = data[package]['build']
 
+                if not inst_package_version:
+                    self.choices.extend(
+                        [(package, f'None -> {repo_ver}', True,
+                          f'Installed: None -> Available: {repo_ver} Build: {repo_build_tag}')])
+                else:
                     self.choices.extend(
                         [(package, f'{inst_package_version} -> {repo_ver}', True,
                           f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
                           f'Available: {repo_ver} Build: {repo_build_tag}')])
 
-    def choose_for_others(self, data: dict, packages: list):
+    def choose_for_others(self, data: dict, packages: list) -> None:
         """ Choose packages for others methods like install, tracking etc. """
         if self.repository == '*':
             for pkg in packages:
-                for name, repo in data.items():
-                    for package in repo.keys():
+                for repo_name, repo_data in data.items():
+                    for package in repo_data.keys():
                         if pkg in package or pkg == '*':
-                            version: str = repo[package]['version']
+                            version: str = repo_data[package]['version']
                             self.choices.extend([(package, version, False, f'Package: {package}-{version} '
-                                                                           f'> {name}')])
+                                                                           f'> {repo_name}')])
 
         else:
             for pkg in packages:
                 for package in data.keys():
                     if pkg in package or pkg == '*':
                         version: str = data[package]['version']
                         self.choices.extend([(package, version, False, f'Package: {package}-{version} '
```

### Comparing `slpkg-5.0.3/slpkg/cleanings.py` & `slpkg-5.0.4/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/configs.py` & `slpkg-5.0.4/slpkg/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     new_packages: bool = False
     removed_packages: bool = False
     downloader: str = 'wget'
     wget_options: str = '--c -q --progress=bar:force:noscroll --show-progress'
     curl_options: str = ''
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer --delete'
+    lftp_mirror_extra_options = {}
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     progress_bar: bool = False
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
     border_color: str = 'bold_green'
@@ -91,14 +92,15 @@
             new_packages: bool = config['NEW_PACKAGES']
             removed_packages: bool = config['REMOVED_PACKAGES']
             downloader: str = config['DOWNLOADER']
             wget_options: str = config['WGET_OPTIONS']
             curl_options: str = config['CURL_OPTIONS']
             lftp_get_options: str = config['LFTP_GET_OPTIONS']
             lftp_mirror_options: str = config['LFTP_MIRROR_OPTIONS']
+            lftp_mirror_extra_options = config['LFTP_MIRROR_EXTRA_OPTIONS']
             ascii_characters: bool = config['ASCII_CHARACTERS']
             file_list_suffix: str = config['FILE_LIST_SUFFIX']
             parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
             progress_bar: str = config['PROGRESS_BAR']
             progress_spinner: str = config['PROGRESS_SPINNER']
             spinner_color: str = config['SPINNER_COLOR']
             border_color: str = config['BORDER_COLOR']
```

### Comparing `slpkg-5.0.3/slpkg/dependees.py` & `slpkg-5.0.4/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/dialog_box.py` & `slpkg-5.0.4/slpkg/dialog_box.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,22 +30,22 @@
         )
 
         code, tags = self.d.checklist(text=text, choices=choices, title=title, height=height,  width=width,
                                       list_height=list_height, help_status=True, **self.more_kwargs)
 
         return code, tags
 
-    def mixedform(self, text: str, title: str, elements: list, height: int, width: int) -> Tuple[bool, list]:
+    def mixedform(self, text: str, title: str, elements: list, height: int, width: int, form_height) -> Tuple[bool, list]:
         """ Display a mixedform box. """
         self.more_kwargs.update(
             {"item_help": True,
              "help_tags": True}
         )
         code, tags = self.d.mixedform(text=text, title=title, elements=elements,  # type: ignore
-                                      height=height, width=width, help_button=True,
+                                      height=height, width=width, form_height=form_height, help_button=True,
                                       help_status=True, **self.more_kwargs)
 
         return code, tags
 
     def msgbox(self, text: str, height: int, width: int) -> None:
         """ Display a message box. """
         self.d.msgbox(text, height, width)
```

### Comparing `slpkg-5.0.3/slpkg/dialog_configs.py` & `slpkg-5.0.4/slpkg/dialog_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,30 +27,31 @@
             self.errors.raise_error_message(f"You should enable the dialog in the "
                                             f"'{self.etc_path}/{self.prog_name}.toml' file", exit_status=1)
 
     def edit(self) -> None:
         """ Read and write the configuration file. """
         self.is_dialog_enabled()
         elements: list = []
-        height: int = 35
-        width: int = 74
+        height: int = 9
+        width: int = 0
+        form_height: int = 0
         text: str = f'Edit the configuration file: {self.config_file}'
         title: str = ' Configuration File '
 
         # Creating the elements for the dialog form.
         for i, (key, value) in enumerate(self.configs['CONFIGS'].items(), start=1):
             if value is True:
                 value: str = 'true'
             elif value is False:
                 value: str = 'false'
             elements.extend(
                 [(key, i, 1, str(value), i, 21, 47, 200, '0x0', f'Config: {key} = {value}')]
             )
 
-        code, tags = self.dialogbox.mixedform(text, title, elements, height, width)
+        code, tags = self.dialogbox.mixedform(text, title, elements, height, width, form_height)
 
         os.system('clear')
 
         if code == 'help':
             tags = self.configs.values()
             self.help()
```

### Comparing `slpkg-5.0.3/slpkg/download_only.py` & `slpkg-5.0.4/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/downloader.py` & `slpkg-5.0.4/slpkg/downloader.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/find_installed.py` & `slpkg-5.0.4/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/gpg_verify.py` & `slpkg-5.0.4/slpkg/gpg_verify.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/install_data.py` & `slpkg-5.0.4/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/load_data.py` & `slpkg-5.0.4/slpkg/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
     def load(self, repository: str) -> dict:
         print('\rDatabase loading... ', end='')
         data: dict = {}
         if repository == '*':
             for repo, item in self.repos.repositories.items():
                 if item['enable']:  # Check if the repository is enabled
-                    json_data_file: Path = Path(f'{self.repos.repositories_path}/{repo}', self.repos.data_json)
+                    json_data_file: Path = Path(self.repos.repositories[repo]['path'], self.repos.data_json)
                     data[repo] = self.read_data_file(json_data_file)
         else:
-            json_data_file: Path = Path(f'{self.repos.repositories_path}/{repository}', self.repos.data_json)
+            json_data_file: Path = Path(self.repos.repositories[repository]['path'], self.repos.data_json)
+
             data: dict = self.read_data_file(json_data_file)
 
         blacklist: tuple = self.black.packages()
         if blacklist:
             if repository == '*':
                 self._remove_blacklist_from_all_repos(data)
             else:
```

### Comparing `slpkg-5.0.3/slpkg/main.py` & `slpkg-5.0.4/slpkg/main.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/multi_process.py` & `slpkg-5.0.4/slpkg/multi_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+import shutil
 import subprocess
 from datetime import datetime
 from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
+from slpkg.error_messages import Errors
 from slpkg.views.asciibox import AsciiBox
 from slpkg.progress_bar import ProgressBar
-from slpkg.error_messages import Errors
 
 
 class MultiProcess(Configs):
 
     def __init__(self, flags=None):
         super(Configs, self).__init__()
 
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.ascii = AsciiBox()
         self.errors = Errors()
 
+        self.columns, self.rows = shutil.get_terminal_size()
         self.timestamp: str = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.head_message: str = f'Timestamp: {self.timestamp}'
         self.bottom_message: str = 'EOF - End of log file'
 
         if flags is not None:
             self.option_for_progress_bar: bool = self.utils.is_option(
                 ('-B', '--progress-bar'), flags)
@@ -63,20 +65,21 @@
 
             # Wait until process 1 finish
             process_1.join()
 
             # Terminate process 2 if process 1 finished
             if not process_1.is_alive():
                 process_2.terminate()
+                print(f"\r{' ' * (self.columns - 1)}", end='')  # Delete previous line.
                 if process_1.exitcode != 0:
-                    print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} {filename} {failed}{' ' * 17}", end='\r')
+                    print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} {filename} {failed}", end='')
                 elif installed:
-                    print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} {filename} {skip}{' ' * 17}", end='\r')
+                    print(f"\r{'':>2}{self.bred}{self.ascii.bullet}{self.endc} {filename} {skip}", end='')
                 else:
-                    print(f"\r{'':>2}{self.bgreen}{self.ascii.bullet}{self.endc} {filename} {done}{' ' * 17}", end='\r')
+                    print(f"\r{'':>2}{self.bgreen}{self.ascii.bullet}{self.endc} {filename} {done}", end='')
 
             # Restore the terminal cursor
             print('\x1b[?25h', self.endc)
         else:
             self._run(command)
 
     def _run(self, command: str, stdout=subprocess.PIPE, stderr=subprocess.STDOUT) -> None:
```

### Comparing `slpkg-5.0.3/slpkg/new_configs.py` & `slpkg-5.0.4/slpkg/new_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/remove_packages.py` & `slpkg-5.0.4/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/repo_info.py` & `slpkg-5.0.4/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/repositories.py` & `slpkg-5.0.4/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/sbos/dependencies.py` & `slpkg-5.0.4/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/sbos/sbo_generate.py` & `slpkg-5.0.4/slpkg/sbos/sbo_generate.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/sbos/slackbuild.py` & `slpkg-5.0.4/slpkg/sbos/slackbuild.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/search.py` & `slpkg-5.0.4/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/toml_errors.py` & `slpkg-5.0.4/slpkg/toml_errors.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/tracking.py` & `slpkg-5.0.4/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/update_repositories.py` & `slpkg-5.0.4/slpkg/update_repositories.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         self.utils = Utilities()
         self.data = InstallData()
         self.generate = SBoGenerate()
         self.check_updates = CheckUpdates(flags, repository)
         self.download = Downloader(flags)
 
         self.repos_for_update: dict = {}
+        self.lftp_extra_options: str = ' '
 
         self.option_for_repository: bool = self.utils.is_option(
             ('-o', '--repository='), flags)
 
     def repositories(self) -> None:
         self.repos_for_update: dict = self.check_updates.updates()
         self.update_the_repositories()
@@ -70,35 +71,41 @@
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository,
             self.repos.pprkut_repo_name: self.pprkut_repository
         }
 
         if self.option_for_repository:
             self.view_downloading_message(self.repository)
+            self.set_lftp_extra_options(self.repository)
             repositories[self.repository]()
         else:
             for repo, update in self.repos_for_update.items():
                 if update:
                     self.view_downloading_message(repo)
+                    self.set_lftp_extra_options(repo)
                     repositories[repo]()
 
     def view_downloading_message(self, repo: str) -> None:
         print(f"Syncing with the repository '{self.green}{repo}{self.endc}', please wait...\n")
 
+    def set_lftp_extra_options(self, repository: str) -> None:
+        if self.lftp_mirror_extra_options.get(repository):
+            self.lftp_extra_options: str = f' {self.lftp_mirror_extra_options[repository]} '
+
     def slack_repository(self) -> None:
         urls: dict = {}
         self.utils.create_directory(self.repos.slack_repo_path)
 
         self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
         self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
 
         if self.repos.slack_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.slack_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.slack_repo_mirror[0]} '
                 f'{self.repos.slack_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}'
             packages: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}'
             checksums: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}'
@@ -118,16 +125,16 @@
         self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_checksums)
 
         changelog: str = f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}'
 
         if self.repos.slack_extra_repo_local[0].startswith('file'):
             urls[self.repos.slack_extra_repo_name] = ((changelog,), self.repos.slack_extra_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_extra_repo_mirror)} '
-                f'{self.repos.slack_extra_repo_path}'
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
+                f'{"".join(self.repos.slack_extra_repo_mirror)} {self.repos.slack_extra_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}'
             checksums: str = f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_checksums}'
             urls[self.repos.slack_extra_repo_name] = ((changelog, packages, checksums),
                                                       self.repos.slack_extra_repo_path)
@@ -148,16 +155,16 @@
                                          self.repos.slack_patches_repo_checksums)
 
         changelog: str = f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}'
 
         if self.repos.slack_patches_repo_local[0].startswith('file'):
             urls[self.repos.slack_patches_repo_name] = ((changelog,), self.repos.slack_patches_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_patches_repo_mirror)} '
-                f'{self.repos.slack_patches_repo_path}'
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
+                f'{"".join(self.repos.slack_patches_repo_mirror)} {self.repos.slack_patches_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = (f'{"".join(self.repos.slack_patches_repo_mirror)}'
                              f'{self.repos.slack_patches_repo_packages}')
             checksums: str = (f'{"".join(self.repos.slack_patches_repo_mirror)}'
                               f'{self.repos.slack_patches_repo_checksums}')
@@ -178,15 +185,15 @@
         self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
 
         changelog: str = f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}'
 
         if self.repos.alien_repo_local[0].startswith('file'):
             urls[self.repos.alien_repo_name] = ((changelog,), self.repos.alien_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.alien_repo_mirror)} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{"".join(self.repos.alien_repo_mirror)} '
                 f'{self.repos.alien_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}'
             checksums: str = f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}'
 
@@ -206,15 +213,15 @@
         self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
 
         changelog: str = f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}'
 
         if self.repos.multilib_repo_local[0].startswith('file'):
             urls[self.repos.multilib_repo_name] = ((changelog,), self.repos.multilib_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.multilib_repo_mirror)} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{"".join(self.repos.multilib_repo_mirror)} '
                 f'{self.repos.multilib_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}'
             checksums: str = f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_checksums}'
 
@@ -234,16 +241,16 @@
         self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
 
         changelog: str = f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}'
 
         if self.repos.restricted_repo_local[0].startswith('file'):
             urls[self.repos.restricted_repo_name] = ((changelog,), self.repos.restricted_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.restricted_repo_mirror)} '
-                f'{self.repos.restricted_repo_path}'
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
+                f'{"".join(self.repos.restricted_repo_mirror)} {self.repos.restricted_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}'
             checksums: str = f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}'
 
             urls[self.repos.restricted_repo_name] = ((changelog, packages, checksums),
@@ -259,15 +266,15 @@
 
         self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
         self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
 
         if self.repos.gnome_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.gnome_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.gnome_repo_mirror[0]} '
                 f'{self.repos.gnome_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}'
             packages: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}'
             checksums: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}'
@@ -287,15 +294,15 @@
         self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_checksums)
 
         changelog: str = f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}'
 
         if self.repos.msb_repo_local[0].startswith('file'):
             urls[self.repos.msb_repo_name] = ((changelog,), self.repos.msb_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.msb_repo_mirror)} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{"".join(self.repos.msb_repo_mirror)} '
                 f'{self.repos.msb_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}'
             checksums: str = f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_checksums}'
 
@@ -311,15 +318,15 @@
 
         self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_packages)
         self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_checksums)
 
         if self.repos.csb_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.csb_repo_mirror)} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{"".join(self.repos.csb_repo_mirror)} '
                 f'{self.repos.csb_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_changelog}'
             packages: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}'
             checksums: str = f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_checksums}'
@@ -336,15 +343,15 @@
 
         self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
         self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
 
         if self.repos.conraid_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.conraid_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.conraid_repo_mirror[0]} '
                 f'{self.repos.conraid_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}'
             packages: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}'
             checksums: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}'
@@ -361,15 +368,15 @@
 
         self.utils.remove_file_if_exists(self.repos.slackdce_repo_path, self.repos.slackdce_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.slackdce_repo_path, self.repos.slackdce_repo_packages)
         self.utils.remove_file_if_exists(self.repos.slackdce_repo_path, self.repos.slackdce_repo_checksums)
 
         if self.repos.slackdce_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.slackdce_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.slackdce_repo_mirror[0]} '
                 f'{self.repos.slackdce_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.slackdce_repo_mirror[0]}{self.repos.slackdce_repo_changelog}'
             packages: str = f'{self.repos.slackdce_repo_mirror[0]}{self.repos.slackdce_repo_packages}'
             checksums: str = f'{self.repos.slackdce_repo_mirror[0]}{self.repos.slackdce_repo_checksums}'
@@ -386,15 +393,15 @@
 
         self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
         self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
 
         if self.repos.slackonly_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.slackonly_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.slackonly_repo_mirror[0]} '
                 f'{self.repos.slackonly_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}'
             packages: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}'
             checksums: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}'
@@ -412,15 +419,15 @@
 
         self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
         self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
 
         if self.repos.salixos_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.salixos_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.salixos_repo_mirror[0]} '
                 f'{self.repos.salixos_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}'
             packages: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}'
             checksums: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}'
@@ -443,16 +450,16 @@
                                          self.repos.salixos_extra_repo_checksums)
 
         changelog: str = f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}'
 
         if self.repos.salixos_extra_repo_local[0].startswith('file'):
             urls[self.repos.salixos_extra_repo_name] = ((changelog,), self.repos.salixos_extra_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_extra_repo_mirror)} '
-                f'{self.repos.salixos_extra_repo_path}'
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
+                f'{"".join(self.repos.salixos_extra_repo_mirror)} {self.repos.salixos_extra_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = f'{"".join(self.repos.salixos_extra_repo_mirror)}' \
                             f'{self.repos.salixos_extra_repo_packages}'
             checksums: str = (f'{"".join(self.repos.salixos_extra_repo_mirror)}'
                               f'{self.repos.salixos_extra_repo_checksums}')
@@ -476,16 +483,16 @@
                                          self.repos.salixos_patches_repo_checksums)
 
         changelog: str = f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}'
 
         if self.repos.salixos_patches_repo_local[0].startswith('file'):
             urls[self.repos.salixos_patches_repo_name] = ((changelog,), self.repos.salixos_patches_repo_path)
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_patches_repo_mirror)} '
-                f'{self.repos.salixos_patches_repo_path}'
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
+                f'{"".join(self.repos.salixos_patches_repo_mirror)} {self.repos.salixos_patches_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             packages: str = (f'{"".join(self.repos.salixos_patches_repo_mirror)}'
                              f'{self.repos.salixos_patches_repo_packages}')
             checksums: str = (f'{"".join(self.repos.salixos_patches_repo_mirror)}'
                               f'{self.repos.salixos_patches_repo_checksums}')
@@ -503,15 +510,15 @@
 
         self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
         self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
 
         if self.repos.slackel_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.slackel_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.slackel_repo_mirror[0]} '
                 f'{self.repos.slackel_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}'
             packages: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}'
             checksums: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}'
@@ -528,15 +535,15 @@
 
         self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
         self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
 
         if self.repos.slint_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.slint_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.slint_repo_mirror[0]} '
                 f'{self.repos.slint_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}'
             packages: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}'
             checksums: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}'
@@ -553,15 +560,15 @@
 
         self.utils.remove_file_if_exists(self.repos.pprkut_repo_path, self.repos.pprkut_repo_changelog)
         self.utils.remove_file_if_exists(self.repos.pprkut_repo_path, self.repos.pprkut_repo_packages)
         self.utils.remove_file_if_exists(self.repos.pprkut_repo_path, self.repos.pprkut_repo_checksums)
 
         if self.repos.pprkut_repo_local[0].startswith('file'):
             lftp_command: str = (
-                f'lftp {self.lftp_mirror_options} {self.repos.pprkut_repo_mirror[0]} '
+                f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}{self.repos.pprkut_repo_mirror[0]} '
                 f'{self.repos.pprkut_repo_path}'
             )
             self.multi_process.process(lftp_command)
         else:
             changelog: str = f'{self.repos.pprkut_repo_mirror[0]}{self.repos.pprkut_repo_changelog}'
             packages: str = f'{self.repos.pprkut_repo_mirror[0]}{self.repos.pprkut_repo_packages}'
             checksums: str = f'{self.repos.pprkut_repo_mirror[0]}{self.repos.pprkut_repo_checksums}'
@@ -574,15 +581,15 @@
 
     def ponce_repository(self) -> None:
         """ Update the slackbuild repositories. """
         self.utils.create_directory(self.repos.ponce_repo_path)
         self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
         self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
 
-        lftp_command: str = (f'lftp {self.lftp_mirror_options} '
+        lftp_command: str = (f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
                              f'{self.repos.ponce_repo_mirror[0]} {self.repos.ponce_repo_path}')
 
         self.multi_process.process(lftp_command)
 
         # It checks if there is the SLACKBUILDS.TXT file, otherwise going to create it.
         if not Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds).is_file():
             self.generate.slackbuild_file(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
@@ -590,15 +597,15 @@
         self.data.install_ponce_data()
 
     def sbo_repository(self) -> None:
         self.utils.create_directory(self.repos.sbo_repo_path)
         self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
         self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
 
-        lftp_command: str = (f'lftp {self.lftp_mirror_options} '
+        lftp_command: str = (f'lftp {self.lftp_mirror_options}{self.lftp_extra_options}'
                              f'{self.repos.sbo_repo_mirror[0]} {self.repos.sbo_repo_path}')
 
         self.multi_process.process(lftp_command)
 
         # It checks if there is the SLACKBUILDS.TXT file, otherwise going to create it.
         if not Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds).is_file():
             self.generate.slackbuild_file(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
```

### Comparing `slpkg-5.0.3/slpkg/upgrade.py` & `slpkg-5.0.4/slpkg/upgrade.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,16 +74,26 @@
             try:
                 if parse(repo_version) > parse(inst_version):
                     return True
 
                 if parse(repo_version) == parse(inst_version) and int(repo_build) > int(inst_build):
                     return True
             except InvalidVersion as err:
+                # Different options to compare packages.
+                repo_package: str = self.data[inst_name]['package']
+                if repo_version > inst_version:  # Try to compare the strings.
+                    return True
+                elif repo_version == inst_version and int(repo_build) > int(inst_build):
+                    return True
+                elif installed != repo_package[:-4]:  # Add the package if a new one on the repository.
+                    return True
+                elif installed == repo_package[:-4]:  # Not new packages in the repository.
+                    return False
                 self._write_log_file(installed, inst_name, err)
-                return False
+
         return False
 
     def _write_log_file(self, installed: str, name: str, err: InvalidVersion) -> None:
         """ Writes a log file for invalid versions. """
         if self.log_path.is_dir():
             with self.upgrade_log_file.open('a') as log:
                 log.write(f"Installed: {installed}, "
```

### Comparing `slpkg-5.0.3/slpkg/utilities.py` & `slpkg-5.0.4/slpkg/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,29 +21,36 @@
         super(Configs, self).__init__()
         self.black = Blacklist()
         self.errors = Errors()
 
     def is_package_installed(self, name: str) -> str:
         """ Returns the installed package binary. """
         installed_package: Generator = self.log_packages.glob(f'{name}*')
+
         for installed in installed_package:
             inst_name: str = self.split_package(installed.name)['name']
-            if inst_name == name:
+            if inst_name == name and inst_name not in self.ignore_packages([inst_name]):
                 return installed.name
         return ''
 
     def all_installed(self) -> dict:
         """ Return all installed packages from /val/log/packages folder. """
         installed_packages: dict = {}
+
         for file in self.log_packages.glob('*'):
             name: str = self.split_package(file.name)['name']
 
             if not name.startswith('.'):
                 installed_packages[name] = file.name
 
+        blacklist_packages: list = self.ignore_packages(list(installed_packages.keys()))
+        if blacklist_packages:
+            for black in blacklist_packages:
+                del installed_packages[black]
+
         return installed_packages
 
     @staticmethod
     def remove_file_if_exists(path: Path, file: str) -> None:
         """ Remove the old files. """
         archive: Path = Path(path, file)
         if archive.is_file():
```

### Comparing `slpkg-5.0.3/slpkg/views/asciibox.py` & `slpkg-5.0.4/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/views/cli_menu.py` & `slpkg-5.0.4/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/views/version.py` & `slpkg-5.0.4/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (5, 0, 3)
+        self.version_info: tuple = (5, 0, 4)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'GNU General Public License v3 (GPLv3)'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
         self.email: str = 'dslackw@gmail.com'
 
     def view(self) -> None:
```

### Comparing `slpkg-5.0.3/slpkg/views/view_package.py` & `slpkg-5.0.4/slpkg/views/view_package.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/slpkg/views/views.py` & `slpkg-5.0.4/slpkg/views/views.py`

 * *Files identical despite different names*

### Comparing `slpkg-5.0.3/PKG-INFO` & `slpkg-5.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 5.0.3
+Version: 5.0.4
 Summary: Package manager utility for Slackware Linux
 Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Maintainer-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,15 +20,14 @@
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Software Distribution
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Dist: pythondialog>=3.5.3
-Requires-Dist: progress>=1.6
 Requires-Dist: PySocks>=1.7.1 ; extra == "socks"
 Project-URL: Changelog, https://gitlab.com/dslackw/slpkg/-/blob/master/ChangeLog.txt
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
 Project-URL: Homepage, https://dslackw.gitlab.io/slpkg/
 Project-URL: Repository, https://gitlab.com/dslackw/slpkg.git
 Provides-Extra: socks
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: slpkg Version: 5.0.3 Summary: Package manager
+Metadata-Version: 2.1 Name: slpkg Version: 5.0.4 Summary: Package manager
 utility for Slackware Linux Keywords: slackware,linux,package,manager,tool
 Author-email: Dimitris Zlatanidis
 gmail.com> Maintainer-email: Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English Classifier: Environment :: Console
 Classifier: Operating System :: POSIX Classifier: Operating System :: POSIX ::
@@ -10,28 +10,28 @@
 Language :: Python :: 3 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Utilities Classifier: Topic :: Software Development ::
 Build Tools Classifier: Topic :: System :: Archiving :: Packaging Classifier:
 Topic :: System :: Software Distribution Classifier: Topic :: System ::
 Installation/Setup Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Software Distribution Classifier: Development
 Status :: 5 - Production/Stable Requires-Dist: pythondialog>=3.5.3 Requires-
-Dist: progress>=1.6 Requires-Dist: PySocks>=1.7.1 ; extra == "socks" Project-
-URL: Changelog, https://gitlab.com/dslackw/slpkg/-/blob/master/ChangeLog.txt
-Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/ Project-URL:
-Homepage, https://dslackw.gitlab.io/slpkg/ Project-URL: Repository, https://
-gitlab.com/dslackw/slpkg.git Provides-Extra: socks [[https://gitlab.com/
-dslackw/slpkg/-/raw/site/docs/images/logo.png]](https://dslackw.gitlab.io/
-slpkg) ## About Slpkg is a software package manager that installs, updates and
-removes packages on _S_l_a_c_k_w_a_r_e-based systems. It automatically calculates
-dependencies and figures out what things need to happen to install packages.
-Slpkg makes it easier to manage groups of machines without the need for manual
-updates. Slpkg works in accordance with the standards of the _s_l_a_c_k_b_u_i_l_d_s_._o_r_g
-organization to build packages. It also uses the Slackware Linux instructions
-for installing, upgrading or removing packages. ## Homepage Visit the project
-website [here](https://dslackw.gitlab.io/slpkg/). ## Source * _G_i_t_L_a_b
-repository. * _S_l_a_c_k_B_u_i_l_d_s_._o_r_g repository. * _S_o_u_r_c_e_F_o_r_g_e repository. * _P_y_P_i
-repository. ## License [MIT License](https://dslackw.gitlab.io/slpkg/license/
-) ## Donate Did you know that we developers love coffee? [[paypal]](https://
-www.paypal.me/dslackw) ## Support Please support: * _S_l_a_c_k_w_a_r_e project. *
-_S_l_a_c_k_B_u_i_l_d_s project. * _A_l_i_e_n_B_o_b project. Thank you all for your support! ##
-Copyrights SlackwareÂ® is a Registered Trademark of Patrick Volkerding. Linux
-is a Registered Trademark of Linus Torvalds.
+Dist: PySocks>=1.7.1 ; extra == "socks" Project-URL: Changelog, https://
+gitlab.com/dslackw/slpkg/-/blob/master/ChangeLog.txt Project-URL:
+Documentation, https://dslackw.gitlab.io/slpkg/ Project-URL: Homepage, https://
+dslackw.gitlab.io/slpkg/ Project-URL: Repository, https://gitlab.com/dslackw/
+slpkg.git Provides-Extra: socks [[https://gitlab.com/dslackw/slpkg/-/raw/site/
+docs/images/logo.png]](https://dslackw.gitlab.io/slpkg) ## About Slpkg is a
+software package manager that installs, updates and removes packages on
+_S_l_a_c_k_w_a_r_e-based systems. It automatically calculates dependencies and figures
+out what things need to happen to install packages. Slpkg makes it easier to
+manage groups of machines without the need for manual updates. Slpkg works in
+accordance with the standards of the _s_l_a_c_k_b_u_i_l_d_s_._o_r_g organization to build
+packages. It also uses the Slackware Linux instructions for installing,
+upgrading or removing packages. ## Homepage Visit the project website [here]
+(https://dslackw.gitlab.io/slpkg/). ## Source * _G_i_t_L_a_b repository. *
+_S_l_a_c_k_B_u_i_l_d_s_._o_r_g repository. * _S_o_u_r_c_e_F_o_r_g_e repository. * _P_y_P_i repository. ##
+License [MIT License](https://dslackw.gitlab.io/slpkg/license/) ## Donate Did
+you know that we developers love coffee? [[paypal]](https://www.paypal.me/
+dslackw) ## Support Please support: * _S_l_a_c_k_w_a_r_e project. * _S_l_a_c_k_B_u_i_l_d_s project.
+* _A_l_i_e_n_B_o_b project. Thank you all for your support! ## Copyrights SlackwareÂ®
+is a Registered Trademark of Patrick Volkerding. Linux is a Registered
+Trademark of Linus Torvalds.
```

