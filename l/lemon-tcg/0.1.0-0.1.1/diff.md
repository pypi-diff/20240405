# Comparing `tmp/lemon_tcg-0.1.0.tar.gz` & `tmp/lemon_tcg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon_tcg-0.1.0.tar", last modified: Fri Apr  5 12:54:46 2024, max compression
+gzip compressed data, was "lemon_tcg-0.1.1.tar", last modified: Fri Apr  5 15:16:43 2024, max compression
```

## Comparing `lemon_tcg-0.1.0.tar` & `lemon_tcg-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.893369 lemon_tcg-0.1.0/
--rw-r--r--   0 blackbird   (501) staff       (20)    35149 2024-04-04 15:05:50.000000 lemon_tcg-0.1.0/LICENSE
--rw-r--r--   0 blackbird   (501) staff       (20)      587 2024-04-05 12:54:46.893242 lemon_tcg-0.1.0/PKG-INFO
--rw-r--r--   0 blackbird   (501) staff       (20)      217 2024-04-05 12:50:31.000000 lemon_tcg-0.1.0/README.md
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.886404 lemon_tcg-0.1.0/lemon_tcg/
--rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:05.000000 lemon_tcg-0.1.0/lemon_tcg/__init__.py
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.887810 lemon_tcg-0.1.0/lemon_tcg/constants/
--rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:10.000000 lemon_tcg-0.1.0/lemon_tcg/constants/__init__.py
--rw-r--r--   0 blackbird   (501) staff       (20)       73 2024-04-05 12:44:25.000000 lemon_tcg-0.1.0/lemon_tcg/constants/event_type.py
--rw-r--r--   0 blackbird   (501) staff       (20)       99 2024-04-04 18:21:23.000000 lemon_tcg-0.1.0/lemon_tcg/constants/language.py
--rw-r--r--   0 blackbird   (501) staff       (20)       85 2024-04-05 12:44:29.000000 lemon_tcg-0.1.0/lemon_tcg/constants/tile_state.py
--rw-r--r--   0 blackbird   (501) staff       (20)      773 2024-04-05 12:45:15.000000 lemon_tcg-0.1.0/lemon_tcg/context.py
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.890819 lemon_tcg-0.1.0/lemon_tcg/entities/
--rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:20.000000 lemon_tcg-0.1.0/lemon_tcg/entities/__init__.py
--rw-r--r--   0 blackbird   (501) staff       (20)      585 2024-04-05 12:44:43.000000 lemon_tcg-0.1.0/lemon_tcg/entities/base_save_state_entity.py
--rw-r--r--   0 blackbird   (501) staff       (20)      829 2024-04-05 12:46:26.000000 lemon_tcg-0.1.0/lemon_tcg/entities/base_save_state_entity_group.py
--rw-r--r--   0 blackbird   (501) staff       (20)      534 2024-04-05 12:44:48.000000 lemon_tcg-0.1.0/lemon_tcg/entities/board.py
--rw-r--r--   0 blackbird   (501) staff       (20)      743 2024-04-05 12:46:29.000000 lemon_tcg-0.1.0/lemon_tcg/entities/card.py
--rw-r--r--   0 blackbird   (501) staff       (20)      629 2024-04-05 12:46:31.000000 lemon_tcg-0.1.0/lemon_tcg/entities/config.py
--rw-r--r--   0 blackbird   (501) staff       (20)     1615 2024-04-05 12:44:54.000000 lemon_tcg-0.1.0/lemon_tcg/entities/coordinates.py
--rw-r--r--   0 blackbird   (501) staff       (20)      309 2024-04-05 12:46:33.000000 lemon_tcg-0.1.0/lemon_tcg/entities/deck.py
--rw-r--r--   0 blackbird   (501) staff       (20)      403 2024-04-05 12:46:36.000000 lemon_tcg-0.1.0/lemon_tcg/entities/game_state.py
--rw-r--r--   0 blackbird   (501) staff       (20)      605 2024-04-05 12:44:59.000000 lemon_tcg-0.1.0/lemon_tcg/entities/localized_value.py
--rw-r--r--   0 blackbird   (501) staff       (20)       93 2024-04-05 12:45:02.000000 lemon_tcg-0.1.0/lemon_tcg/entities/player.py
--rw-r--r--   0 blackbird   (501) staff       (20)      217 2024-04-05 12:45:00.000000 lemon_tcg-0.1.0/lemon_tcg/entities/player_card.py
--rw-r--r--   0 blackbird   (501) staff       (20)      145 2024-04-05 12:45:04.000000 lemon_tcg-0.1.0/lemon_tcg/entities/tile.py
--rw-r--r--   0 blackbird   (501) staff       (20)      600 2024-04-05 12:45:17.000000 lemon_tcg-0.1.0/lemon_tcg/game.py
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.891375 lemon_tcg-0.1.0/lemon_tcg/utils/
--rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:25.000000 lemon_tcg-0.1.0/lemon_tcg/utils/__init__.py
--rw-r--r--   0 blackbird   (501) staff       (20)     1082 2024-04-05 12:45:11.000000 lemon_tcg-0.1.0/lemon_tcg/utils/file_operations.py
--rw-r--r--   0 blackbird   (501) staff       (20)      146 2024-04-05 12:45:14.000000 lemon_tcg-0.1.0/lemon_tcg/utils/validator.py
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.887075 lemon_tcg-0.1.0/lemon_tcg.egg-info/
--rw-r--r--   0 blackbird   (501) staff       (20)      587 2024-04-05 12:54:46.000000 lemon_tcg-0.1.0/lemon_tcg.egg-info/PKG-INFO
--rw-r--r--   0 blackbird   (501) staff       (20)     1060 2024-04-05 12:54:46.000000 lemon_tcg-0.1.0/lemon_tcg.egg-info/SOURCES.txt
--rw-r--r--   0 blackbird   (501) staff       (20)        1 2024-04-05 12:54:46.000000 lemon_tcg-0.1.0/lemon_tcg.egg-info/dependency_links.txt
--rw-r--r--   0 blackbird   (501) staff       (20)       82 2024-04-05 12:54:46.000000 lemon_tcg-0.1.0/lemon_tcg.egg-info/requires.txt
--rw-r--r--   0 blackbird   (501) staff       (20)       16 2024-04-05 12:54:46.000000 lemon_tcg-0.1.0/lemon_tcg.egg-info/top_level.txt
--rw-r--r--   0 blackbird   (501) staff       (20)       38 2024-04-05 12:54:46.893413 lemon_tcg-0.1.0/setup.cfg
--rw-r--r--   0 blackbird   (501) staff       (20)      727 2024-04-05 12:51:05.000000 lemon_tcg-0.1.0/setup.py
-drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 12:54:46.892969 lemon_tcg-0.1.0/tests/
--rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:00.000000 lemon_tcg-0.1.0/tests/__init__.py
--rw-r--r--   0 blackbird   (501) staff       (20)      225 2024-04-05 12:45:27.000000 lemon_tcg-0.1.0/tests/conftest.py
--rw-r--r--   0 blackbird   (501) staff       (20)      168 2024-04-05 12:45:25.000000 lemon_tcg-0.1.0/tests/test_board.py
--rw-r--r--   0 blackbird   (501) staff       (20)      228 2024-04-05 12:45:28.000000 lemon_tcg-0.1.0/tests/test_card.py
--rw-r--r--   0 blackbird   (501) staff       (20)      644 2024-04-05 12:45:30.000000 lemon_tcg-0.1.0/tests/test_config.py
--rw-r--r--   0 blackbird   (501) staff       (20)     3191 2024-04-05 12:45:34.000000 lemon_tcg-0.1.0/tests/test_coordinates.py
--rw-r--r--   0 blackbird   (501) staff       (20)      551 2024-04-05 12:45:32.000000 lemon_tcg-0.1.0/tests/test_localized_value.py
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.342670 lemon_tcg-0.1.1/
+-rw-r--r--   0 blackbird   (501) staff       (20)    35149 2024-04-04 15:05:50.000000 lemon_tcg-0.1.1/LICENSE
+-rw-r--r--   0 blackbird   (501) staff       (20)      587 2024-04-05 15:16:43.342537 lemon_tcg-0.1.1/PKG-INFO
+-rw-r--r--   0 blackbird   (501) staff       (20)      217 2024-04-05 12:50:31.000000 lemon_tcg-0.1.1/README.md
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.338226 lemon_tcg-0.1.1/lemon_tcg/
+-rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:05.000000 lemon_tcg-0.1.1/lemon_tcg/__init__.py
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.339202 lemon_tcg-0.1.1/lemon_tcg/constants/
+-rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:10.000000 lemon_tcg-0.1.1/lemon_tcg/constants/__init__.py
+-rw-r--r--   0 blackbird   (501) staff       (20)       99 2024-04-04 18:21:23.000000 lemon_tcg-0.1.1/lemon_tcg/constants/language.py
+-rw-r--r--   0 blackbird   (501) staff       (20)       85 2024-04-05 12:44:29.000000 lemon_tcg-0.1.1/lemon_tcg/constants/tile_state.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      773 2024-04-05 12:45:15.000000 lemon_tcg-0.1.1/lemon_tcg/context.py
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.341013 lemon_tcg-0.1.1/lemon_tcg/entities/
+-rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:20.000000 lemon_tcg-0.1.1/lemon_tcg/entities/__init__.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      585 2024-04-05 12:44:43.000000 lemon_tcg-0.1.1/lemon_tcg/entities/base_save_state_entity.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      829 2024-04-05 12:46:26.000000 lemon_tcg-0.1.1/lemon_tcg/entities/base_save_state_entity_group.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      653 2024-04-05 14:36:41.000000 lemon_tcg-0.1.1/lemon_tcg/entities/board.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      743 2024-04-05 12:46:29.000000 lemon_tcg-0.1.1/lemon_tcg/entities/card.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      629 2024-04-05 12:46:31.000000 lemon_tcg-0.1.1/lemon_tcg/entities/config.py
+-rw-r--r--   0 blackbird   (501) staff       (20)     1615 2024-04-05 12:44:54.000000 lemon_tcg-0.1.1/lemon_tcg/entities/coordinates.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      309 2024-04-05 12:46:33.000000 lemon_tcg-0.1.1/lemon_tcg/entities/deck.py
+-rw-r--r--   0 blackbird   (501) staff       (20)     1422 2024-04-05 15:05:00.000000 lemon_tcg-0.1.1/lemon_tcg/entities/game_state.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      605 2024-04-05 12:44:59.000000 lemon_tcg-0.1.1/lemon_tcg/entities/localized_value.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      250 2024-04-05 13:39:45.000000 lemon_tcg-0.1.1/lemon_tcg/entities/player.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      217 2024-04-05 12:45:00.000000 lemon_tcg-0.1.1/lemon_tcg/entities/player_card.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      145 2024-04-05 12:45:04.000000 lemon_tcg-0.1.1/lemon_tcg/entities/tile.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      700 2024-04-05 14:49:56.000000 lemon_tcg-0.1.1/lemon_tcg/exceptions.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      828 2024-04-05 13:35:11.000000 lemon_tcg-0.1.1/lemon_tcg/game.py
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.341476 lemon_tcg-0.1.1/lemon_tcg/utils/
+-rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:25.000000 lemon_tcg-0.1.1/lemon_tcg/utils/__init__.py
+-rw-r--r--   0 blackbird   (501) staff       (20)     1082 2024-04-05 12:45:11.000000 lemon_tcg-0.1.1/lemon_tcg/utils/file_operations.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      102 2024-04-05 13:23:34.000000 lemon_tcg-0.1.1/lemon_tcg/utils/time_operations.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      146 2024-04-05 12:45:14.000000 lemon_tcg-0.1.1/lemon_tcg/utils/validator.py
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.338821 lemon_tcg-0.1.1/lemon_tcg.egg-info/
+-rw-r--r--   0 blackbird   (501) staff       (20)      587 2024-04-05 15:16:43.000000 lemon_tcg-0.1.1/lemon_tcg.egg-info/PKG-INFO
+-rw-r--r--   0 blackbird   (501) staff       (20)     1085 2024-04-05 15:16:43.000000 lemon_tcg-0.1.1/lemon_tcg.egg-info/SOURCES.txt
+-rw-r--r--   0 blackbird   (501) staff       (20)        1 2024-04-05 15:16:43.000000 lemon_tcg-0.1.1/lemon_tcg.egg-info/dependency_links.txt
+-rw-r--r--   0 blackbird   (501) staff       (20)       62 2024-04-05 15:16:43.000000 lemon_tcg-0.1.1/lemon_tcg.egg-info/requires.txt
+-rw-r--r--   0 blackbird   (501) staff       (20)       16 2024-04-05 15:16:43.000000 lemon_tcg-0.1.1/lemon_tcg.egg-info/top_level.txt
+-rw-r--r--   0 blackbird   (501) staff       (20)       38 2024-04-05 15:16:43.342721 lemon_tcg-0.1.1/setup.cfg
+-rw-r--r--   0 blackbird   (501) staff       (20)      696 2024-04-05 14:33:50.000000 lemon_tcg-0.1.1/setup.py
+drwxr-xr-x   0 blackbird   (501) staff       (20)        0 2024-04-05 15:16:43.342337 lemon_tcg-0.1.1/tests/
+-rw-r--r--   0 blackbird   (501) staff       (20)        0 2024-04-04 18:54:00.000000 lemon_tcg-0.1.1/tests/__init__.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      225 2024-04-05 12:45:27.000000 lemon_tcg-0.1.1/tests/conftest.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      168 2024-04-05 12:45:25.000000 lemon_tcg-0.1.1/tests/test_board.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      228 2024-04-05 12:45:28.000000 lemon_tcg-0.1.1/tests/test_card.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      644 2024-04-05 12:45:30.000000 lemon_tcg-0.1.1/tests/test_config.py
+-rw-r--r--   0 blackbird   (501) staff       (20)     3191 2024-04-05 12:45:34.000000 lemon_tcg-0.1.1/tests/test_coordinates.py
+-rw-r--r--   0 blackbird   (501) staff       (20)      551 2024-04-05 12:45:32.000000 lemon_tcg-0.1.1/tests/test_localized_value.py
```

### Comparing `lemon_tcg-0.1.0/LICENSE` & `lemon_tcg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/PKG-INFO` & `lemon_tcg-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemon_tcg
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library providing the game logic for the LemonTCG online multiplayer TCG game.
 Home-page: https://github.com/Zitronenjoghurt/LemonTCG
 Author: Zitronenjoghurt
 License: GNU General Public License v3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `lemon_tcg-0.1.0/lemon_tcg/context.py` & `lemon_tcg-0.1.1/lemon_tcg/context.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/base_save_state_entity.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/base_save_state_entity.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/base_save_state_entity_group.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/base_save_state_entity_group.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/board.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/board.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from pydantic import BaseModel, computed_field
-from lemon_tcg.constants.event_type import EventType
+from lemon_tcg.event.type import EventType
 from lemon_tcg.entities.coordinates import Coordinates
 from lemon_tcg.entities.tile import Tile
 from lemon_tcg.context import Context
 
 CONTEXT = Context.get_instance()
 
 class Board(BaseModel):
     height: int = CONTEXT.config.default_board_height
     width: int = CONTEXT.config.default_board_width
     tiles: list[Tile] = []
+    _dispatch_id: str = ""
 
     @computed_field 
     @property
     def tile_count(self) -> int:
-        return self.height * self.width
+        return self.height * self.width
+    
+    def register_events(self, dispatch_id: str) -> None:
+        self._dispatch_id = dispatch_id
```

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/card.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/card.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/config.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/config.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/coordinates.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/coordinates.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/entities/localized_value.py` & `lemon_tcg-0.1.1/lemon_tcg/entities/localized_value.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg/game.py` & `lemon_tcg-0.1.1/lemon_tcg/game.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from lemon_tcg.entities.game_state import GameState
+from lemon_tcg.entities.player import Player
 from lemon_tcg.libraries.game_state_library import GameStateLibrary
 
 GAME_STATES = GameStateLibrary.get_instance()
 
 class Game():
     def __init__(self, state: GameState) -> None:
         self.state = state
@@ -10,9 +11,15 @@
     @staticmethod
     def load_from_game_id(game_id: str) -> 'Game':
         game_state = GAME_STATES.get_by_id(id=game_id)
         if not isinstance(game_state, GameState):
             raise RuntimeError(f"Invalid game id '{game_id}'.")
         return Game(state=game_state)
     
+    @staticmethod
+    def new(players: list[Player]) -> 'Game':
+        state = GameState.create_new(players=players)
+        state.save_state()
+        return Game(state=state)
+    
     def save(self) -> None:
         self.state.save_state()
```

### Comparing `lemon_tcg-0.1.0/lemon_tcg/utils/file_operations.py` & `lemon_tcg-0.1.1/lemon_tcg/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/lemon_tcg.egg-info/PKG-INFO` & `lemon_tcg-0.1.1/lemon_tcg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemon-tcg
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library providing the game logic for the LemonTCG online multiplayer TCG game.
 Home-page: https://github.com/Zitronenjoghurt/LemonTCG
 Author: Zitronenjoghurt
 License: GNU General Public License v3.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `lemon_tcg-0.1.0/lemon_tcg.egg-info/SOURCES.txt` & `lemon_tcg-0.1.1/lemon_tcg.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.md
 setup.py
 lemon_tcg/__init__.py
 lemon_tcg/context.py
+lemon_tcg/exceptions.py
 lemon_tcg/game.py
 lemon_tcg.egg-info/PKG-INFO
 lemon_tcg.egg-info/SOURCES.txt
 lemon_tcg.egg-info/dependency_links.txt
 lemon_tcg.egg-info/requires.txt
 lemon_tcg.egg-info/top_level.txt
 lemon_tcg/constants/__init__.py
-lemon_tcg/constants/event_type.py
 lemon_tcg/constants/language.py
 lemon_tcg/constants/tile_state.py
 lemon_tcg/entities/__init__.py
 lemon_tcg/entities/base_save_state_entity.py
 lemon_tcg/entities/base_save_state_entity_group.py
 lemon_tcg/entities/board.py
 lemon_tcg/entities/card.py
@@ -24,14 +24,15 @@
 lemon_tcg/entities/game_state.py
 lemon_tcg/entities/localized_value.py
 lemon_tcg/entities/player.py
 lemon_tcg/entities/player_card.py
 lemon_tcg/entities/tile.py
 lemon_tcg/utils/__init__.py
 lemon_tcg/utils/file_operations.py
+lemon_tcg/utils/time_operations.py
 lemon_tcg/utils/validator.py
 tests/__init__.py
 tests/conftest.py
 tests/test_board.py
 tests/test_card.py
 tests/test_config.py
 tests/test_coordinates.py
```

### Comparing `lemon_tcg-0.1.0/setup.py` & `lemon_tcg-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="lemon_tcg",
     python_requires=">=3.9",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     description="A library providing the game logic for the LemonTCG online multiplayer TCG game.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Zitronenjoghurt",
     install_requires=[
-        'pydantic==2.6.4',
-        'PyDispatcher==2.0.7'
+        'pydantic==2.6.4'
     ],
     extras_require={'dev': ['pytest', 'coverage', 'pytest-cov', 'twine', 'wheel']},
     url="https://github.com/Zitronenjoghurt/LemonTCG"
 )
```

### Comparing `lemon_tcg-0.1.0/tests/test_config.py` & `lemon_tcg-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/tests/test_coordinates.py` & `lemon_tcg-0.1.1/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `lemon_tcg-0.1.0/tests/test_localized_value.py` & `lemon_tcg-0.1.1/tests/test_localized_value.py`

 * *Files identical despite different names*

