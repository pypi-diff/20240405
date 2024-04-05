# Comparing `tmp/nonebot-plugin-fishing-0.2.2a2.tar.gz` & `tmp/nonebot-plugin-fishing-0.2.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fishing-0.2.2a2.tar", last modified: Sun Mar 24 04:31:11 2024, max compression
+gzip compressed data, was "nonebot-plugin-fishing-0.2.2a3.tar", last modified: Fri Apr  5 11:18:29 2024, max compression
```

## Comparing `nonebot-plugin-fishing-0.2.2a2.tar` & `nonebot-plugin-fishing-0.2.2a3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:31:11.581557 nonebot-plugin-fishing-0.2.2a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-24 04:31:11.581557 nonebot-plugin-fishing-0.2.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:31:11.577557 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:31:11.581557 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/migrations/701dd8215883_init_db.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:31:11.581557 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-24 04:31:11.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-24 04:31:11.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:31:11.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-24 04:31:11.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-24 04:31:11.000000 nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-24 04:31:05.000000 nonebot-plugin-fishing-0.2.2a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:31:11.581557 nonebot-plugin-fishing-0.2.2a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 11:18:29.000000 nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-05 11:18:25.000000 nonebot-plugin-fishing-0.2.2a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 11:18:29.614387 nonebot-plugin-fishing-0.2.2a3/setup.cfg
```

### Comparing `nonebot-plugin-fishing-0.2.2a2/LICENSE` & `nonebot-plugin-fishing-0.2.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.2a2/PKG-INFO` & `nonebot-plugin-fishing-0.2.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.2a2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.2a3 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
```

### Comparing `nonebot-plugin-fishing-0.2.2a2/README.md` & `nonebot-plugin-fishing-0.2.2a3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/__init__.py` & `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/config.py` & `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/data_source.py` & `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing/migrations/701dd8215883_init_db.py` & `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """init db
 
-迁移 ID: 701dd8215883
+迁移 ID: 7609e6d106dd
 父迁移: 
-创建时间: 2024-03-24 11:32:01.614944
+创建时间: 2024-04-05 19:08:58.835014
 
 """
 from __future__ import annotations
 
 from collections.abc import Sequence
 
 from alembic import op
 import sqlalchemy as sa
 
 
-revision: str = '701dd8215883'
+revision: str = '7609e6d106dd'
 down_revision: str | Sequence[str] | None = None
 branch_labels: str | Sequence[str] | None = ('nonebot_plugin_fishing',)
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = "") -> None:
     if name:
         return
     # ### commands auto generated by Alembic - please adjust! ###
     op.create_table('nonebot_plugin_fishing_fishingrecord',
     sa.Column('id', sa.Integer(), nullable=False),
-    sa.Column('user_id', sa.String(), nullable=False),
+    sa.Column('user_id', sa.String(length=32), nullable=False),
     sa.Column('time', sa.Integer(), nullable=False),
     sa.Column('frequency', sa.Integer(), nullable=False),
-    sa.Column('fishes', sa.String(), nullable=False),
+    sa.Column('fishes', sa.TEXT(), nullable=False),
     sa.Column('coin', sa.Integer(), nullable=False),
     sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_fishing_fishingrecord')),
     info={'bind_key': 'nonebot_plugin_fishing'}
     )
     # ### end Alembic commands ###
```

### Comparing `nonebot-plugin-fishing-0.2.2a2/nonebot_plugin_fishing.egg-info/PKG-INFO` & `nonebot-plugin-fishing-0.2.2a3/nonebot_plugin_fishing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.2a2
+Version: 0.2.2a3
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.2a2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.2a3 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
```

