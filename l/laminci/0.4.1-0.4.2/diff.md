# Comparing `tmp/laminci-0.4.1.tar.gz` & `tmp/laminci-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laminci-0.4.1.tar", last modified: Mon Mar 27 05:41:59 2023, max compression
+gzip compressed data, was "laminci-0.4.2.tar", last modified: Wed Mar 29 20:03:51 2023, max compression
```

## Comparing `laminci-0.4.1.tar` & `laminci-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.4.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.4.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.4.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.4.1/.gitignore
--rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.4.1/README.md
--rw-r--r--   0        0        0     2076 2023-03-27 05:41:36.721182 laminci-0.4.1/docs/changelog.md
--rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.4.1/docs/guide/index.md
--rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.4.1/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.4.1/docs/index.md
--rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.4.1/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.4.1/docs/notes/index.md
--rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.4.1/lamin-project.yaml
--rw-r--r--   0        0        0      378 2023-03-27 05:41:27.337009 laminci-0.4.1/laminci/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-26 17:43:55.264065 laminci-0.4.1/laminci/_artifacts.py
--rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.4.1/laminci/_db.py
--rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.4.1/laminci/_docs.py
--rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.4.1/laminci/_env.py
--rw-r--r--   0        0        0     2255 2023-03-27 05:40:10.055613 laminci-0.4.1/laminci/_nox.py
--rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.4.1/laminci/db.py
--rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.4.1/laminci/nox.py
--rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.4.1/noxfile.py
--rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.4.1/tests/test_base.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1371 2023-02-23 21:08:15.192204 laminci-0.4.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-02-23 20:36:15.651723 laminci-0.4.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-02-23 20:36:15.652253 laminci-0.4.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1194 2023-02-23 20:36:15.627521 laminci-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1770 2023-02-23 20:36:15.623232 laminci-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2023-02-23 21:02:08.741159 laminci-0.4.2/README.md
+-rw-r--r--   0        0        0     2229 2023-03-29 20:03:32.064730 laminci-0.4.2/docs/changelog.md
+-rw-r--r--   0        0        0      339 2023-02-23 20:36:15.640096 laminci-0.4.2/docs/guide/index.md
+-rw-r--r--   0        0        0     1415 2023-02-23 20:46:33.157438 laminci-0.4.2/docs/guide/quickstart.ipynb
+-rw-r--r--   0        0        0        0 2023-02-23 21:02:08.741423 laminci-0.4.2/docs/index.md
+-rw-r--r--   0        0        0      805 2023-02-23 20:36:15.648759 laminci-0.4.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
+-rw-r--r--   0        0        0      223 2023-02-23 20:36:15.647572 laminci-0.4.2/docs/notes/index.md
+-rw-r--r--   0        0        0      122 2023-02-23 20:36:15.618482 laminci-0.4.2/lamin-project.yaml
+-rw-r--r--   0        0        0      378 2023-03-29 20:03:25.012545 laminci-0.4.2/laminci/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-26 17:43:55.264065 laminci-0.4.2/laminci/_artifacts.py
+-rw-r--r--   0        0        0     1794 2023-03-25 16:54:29.619400 laminci-0.4.2/laminci/_db.py
+-rw-r--r--   0        0        0      380 2023-02-23 22:56:58.478640 laminci-0.4.2/laminci/_docs.py
+-rw-r--r--   0        0        0      737 2023-02-23 22:56:58.478807 laminci-0.4.2/laminci/_env.py
+-rw-r--r--   0        0        0     2258 2023-03-29 20:02:50.066680 laminci-0.4.2/laminci/_nox.py
+-rw-r--r--   0        0        0      134 2023-02-23 21:55:02.625676 laminci-0.4.2/laminci/db.py
+-rw-r--r--   0        0        0      167 2023-02-23 21:55:02.625861 laminci-0.4.2/laminci/nox.py
+-rw-r--r--   0        0        0      497 2023-02-23 21:02:08.742361 laminci-0.4.2/noxfile.py
+-rw-r--r--   0        0        0      694 2023-03-09 14:11:55.514326 laminci-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-02-23 21:02:08.742721 laminci-0.4.2/tests/test_base.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 laminci-0.4.2/PKG-INFO
```

### Comparing `laminci-0.4.1/.github/workflows/build.yml` & `laminci-0.4.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/.github/workflows/latest-changes.yml` & `laminci-0.4.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/.gitignore` & `laminci-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/.pre-commit-config.yaml` & `laminci-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/docs/changelog.md` & `laminci-0.4.2/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+♻️ Replace `lndb` with `lamin` | [14](https://github.com/laminlabs/laminci/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-03-29 | 0.4.2
 🚸 Replace git checkout with git switch | [13](https://github.com/laminlabs/laminci/pull/13) | [falexwolf](https://github.com/falexwolf) | 2023-03-27 | 0.4.1
 ⬆️ Upgrade to LaminDB v0.35 | [12](https://github.com/laminlabs/laminci/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-03-26 | 0.4.0
 🚚 Rename `upload_docs_dir` to `upload_docs_artifact` |  | 2023-03-21 | 0.3.4
 🍱 Track images in docs | [11](https://github.com/laminlabs/laminci/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-03-12 | 0.3.2
 ➖ Remove dependency on lamindb in laminci | [10](https://github.com/laminlabs/laminci/pull/10) | [falexwolf](https://github.com/falexwolf) | 2023-03-09 | 0.3.0 / 0.3.1
 🍱 Track readme in docs upload | [9](https://github.com/laminlabs/laminci/pull/9) | [falexwolf](https://github.com/falexwolf) | 2023-03-06 | 0.2.5
 🐛 Implement overwrite | [8](https://github.com/laminlabs/laminci/pull/8) | [falexwolf](https://github.com/falexwolf) | 2023-02-28 | 0.2.4
```

### Comparing `laminci-0.4.1/docs/guide/quickstart.ipynb` & `laminci-0.4.2/docs/guide/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/docs/notes/YYYY-MM-DD-my-design-choice.ipynb` & `laminci-0.4.2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/laminci/_artifacts.py` & `laminci-0.4.2/laminci/_artifacts.py`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/laminci/_db.py` & `laminci-0.4.2/laminci/_db.py`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/laminci/_env.py` & `laminci-0.4.2/laminci/_env.py`

 * *Files identical despite different names*

### Comparing `laminci-0.4.1/laminci/_nox.py` & `laminci-0.4.2/laminci/_nox.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 from nox import Session
 
 from ._db import setup_local_test_postgres
 from ._env import get_package_name, get_schema_handle
 
 
 def login_testuser1(session: Session):
-    login_user_1 = "lndb login testuser1@lamin.ai --password cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS"  # noqa
+    login_user_1 = "lamin login testuser1@lamin.ai --password cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS"  # noqa
     session.run(*(login_user_1.split(" ")), external=True)
 
 
 def login_testuser2(session: Session):
-    login_user_1 = "lndb login testuser2@lamin.ai --password goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz"  # noqa
+    login_user_1 = "lamin login testuser2@lamin.ai --password goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz"  # noqa
     session.run(*(login_user_1.split(" ")), external=True)
 
 
 def setup_test_instances_from_main_branch(session: Session, schema: str = None):
     # spin up a postgres test instance
     pgurl = setup_local_test_postgres()
     # switch to the main branch
     if "GITHUB_BASE_REF" in os.environ and os.environ["GITHUB_BASE_REF"] != "":
         session.run("git", "switch", os.environ["GITHUB_BASE_REF"], external=True)
     session.install(".[test]")  # install current package from main branch
     # init a postgres instance
-    init_instance = f"lndb init --storage pgtest --db {pgurl}"
+    init_instance = f"lamin init --storage pgtest --db {pgurl}"
     schema_handle = get_schema_handle()
     if schema is None and schema_handle not in {None, "core"}:
         init_instance += f" --schema {schema_handle}"
     elif schema is not None:
         init_instance += f" --schema {schema}"
     session.run(*init_instance.split(" "), external=True)
     # go back to the PR branch
```

### Comparing `laminci-0.4.1/pyproject.toml` & `laminci-0.4.2/pyproject.toml`

 * *Files identical despite different names*

