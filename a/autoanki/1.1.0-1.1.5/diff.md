# Comparing `tmp/autoanki-1.1.0.tar.gz` & `tmp/autoanki-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.1.0.tar", last modified: Thu Apr  4 21:59:39 2024, max compression
+gzip compressed data, was "autoanki-1.1.5.tar", last modified: Fri Apr  5 18:04:51 2024, max compression
```

## Comparing `autoanki-1.1.0.tar` & `autoanki-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.914944 autoanki-1.1.0/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.0/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.0/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     4165 2024-04-04 21:59:39.914877 autoanki-1.1.0/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     3632 2024-04-04 21:52:38.000000 autoanki-1.1.0/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.0/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-04 21:59:39.915222 autoanki-1.1.0/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.907486 autoanki-1.1.0/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.909363 autoanki-1.1.0/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     5514 2024-04-01 00:05:03.000000 autoanki-1.1.0/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.910960 autoanki-1.1.0/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7312 2024-03-31 20:22:09.000000 autoanki-1.1.0/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.912651 autoanki-1.1.0/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13541 2024-04-01 14:40:06.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.912893 autoanki-1.1.0/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     5924 2024-04-04 21:35:35.000000 autoanki-1.1.0/src/autoanki/DeckManager/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.914193 autoanki-1.1.0/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     2178 2024-04-01 00:02:43.000000 autoanki-1.1.0/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      270 2024-03-31 23:26:31.000000 autoanki-1.1.0/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5561 2024-03-31 20:00:33.000000 autoanki-1.1.0/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.0/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.0/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.914615 autoanki-1.1.0/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     4165 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      795 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.0/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.209319 autoanki-1.1.5/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.5/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.5/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     4826 2024-04-05 18:04:51.209228 autoanki-1.1.5/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     4293 2024-04-05 17:17:58.000000 autoanki-1.1.5/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.5/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-05 18:04:51.209635 autoanki-1.1.5/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.201833 autoanki-1.1.5/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.203347 autoanki-1.1.5/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     5484 2024-04-05 17:52:25.000000 autoanki-1.1.5/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.204825 autoanki-1.1.5/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     7294 2024-04-05 15:59:59.000000 autoanki-1.1.5/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.5/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.206174 autoanki-1.1.5/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13046 2024-04-05 16:28:43.000000 autoanki-1.1.5/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.5/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.5/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.5/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.5/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.206602 autoanki-1.1.5/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     3372 2024-04-05 16:01:12.000000 autoanki-1.1.5/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.5/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     2676 2024-04-05 16:28:54.000000 autoanki-1.1.5/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.208614 autoanki-1.1.5/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     3158 2024-04-05 17:59:23.000000 autoanki-1.1.5/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-05 16:04:00.000000 autoanki-1.1.5/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5561 2024-03-31 20:00:33.000000 autoanki-1.1.5/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.5/src/autoanki/Dictionary/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.5/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-05 18:04:51.208971 autoanki-1.1.5/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     4826 2024-04-05 18:04:51.000000 autoanki-1.1.5/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      878 2024-04-05 18:04:51.000000 autoanki-1.1.5/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-05 18:04:51.000000 autoanki-1.1.5/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.5/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-05 18:04:51.000000 autoanki-1.1.5/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.1.0/LICENSE.txt` & `autoanki-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.0/PKG-INFO` & `autoanki-1.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.0
+Version: 1.1.5
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,25 +15,27 @@
 
 > **❗️** <br>
 Pull requests welcome! If you think you can improve AA in any way, open a PR!
 
 # autoanki
 Tool for generating Anki flashcards to learn Chinese.
 
-<img src="media/images/example.jpg" alt="Text to Anki" width="80%"/>
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
 
 ## Motivation
 
-When learning Chinese, usually the advice given is to learn the top X most common words.
-This is good advice, as you can get pretty far with this, however it's not perfect.
+When learning Chinese, advice is to learn the top X most common words.
+This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
-For example, Harry Potter. This book will have normal distrobution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
+For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
+With autoanki, you selectivley add words to an Anki file to continue progressing with your lanuage learning skills.
+
 ## Usage
 
 autoanki is both a library and a command-line tool.
 
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
@@ -47,24 +49,29 @@
 Then create an instance of autoanki using the database
 ```
 aa = AutoAnki(db_path)
 ```
 Add whatever books you want in your deck. These can be a single file, or a folder
 ```
 bookpath = 'short-story.txt'
-aa.add_book(bookpath, 'My first book😆')
+aa.add_book(bookpath, 'My first book🍎')
 ```
 Once all of your books are added, the definitions need to be found, and then you can create a deck!
 ```
 aa.complete_unfinished_definitions()
 aa.create_deck("AutoAnki Deck", "output")
 ```
 This will automatically have the .apkg extension, which Anki uses. 
 Import this file into Anki, and you're all set.
 
+#### Other commands
+If you want to see the status of the database, use:
+```
+aa.print_database_info()
+```
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
@@ -87,33 +94,31 @@
 - frequency
 - hsk_level
 - top_level
 - audio_path
 - image_path
 - definition
 
-![Dictionary table](media/images/dictionary-table.jpg "Dictionary table") 
-*Dictionary table*  
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="80%"/>
 
 #### book_list:
 - book_name
 - book_table_name
 - language
 
-![Book list table](media/images/book_list_table.jpg "Book list table")
-*Book list table*
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_list_table.jpg?raw=true" alt="Book list table" width="50%"/>
 
 ### book
  - book_table_word_id
  - dictionary_word_id
  - number_of_appearances 
 
-![Book table](media/images/book_table.jpg "Book table")
-*Book table*
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="80%"/>
 
 ## Planned features
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
+To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence.
```

### Comparing `autoanki-1.1.0/setup.cfg` & `autoanki-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.1.0
+version = 1.1.5
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls =
```

### Comparing `autoanki-1.1.0/src/autoanki/AutoAnki.py` & `autoanki-1.1.5/src/autoanki/AutoAnki.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,134 +10,127 @@
 GREEN = "\u001b[32m"
 YELLOW = "\u001b[33m"
 BLUE = "\u001b[34m"
 MAGENTA = "\u001b[35m"
 CYAN = "\u001b[36m"
 WHITE = "\u001b[37m"
 RESET = "\u001b[0m"
-# Add this to see the function name:
-#%(funcName)s
 logging.basicConfig(
-    # filename='HISTORYlistener.log',
-    level=logging.DEBUG,
+    # filename='HISTORY.log',
+    level=logging.WARNING,
     format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)18s{RESET}: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 
-logger = logging.getLogger('autoanki')
-logger.setLevel(logging.INFO)
-logger.debug(f"logger active")
-
-logging.basicConfig(
-    # filename='HISTORYlistener.log',
-    level=logging.CRITICAL,
-    format=f'--{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)18s{RESET}: %(message)s',
-    datefmt='%Y-%m-%d %H:%M:%S',
-)
-
-
 class AutoAnki:
 
-    def __init__(self, database_filepath='autoanki.db', logging_level=20):
+    def __init__(self, database_filepath='autoanki.db', debug_level=20):
         """
         Creates an instance of autoanki.
         This creates a book cleaner, database connection, and deck maker
         :param database_filepath: The filepath for the database
         :param logging_level: between 0 (DEBUG) and 50(CRITICAL)
         """
-        logger.setLevel(logging_level)
-        logger.info("Connecting to database...")
+        self.logger = logging.getLogger('autoanki')
+        self.logger.setLevel(debug_level)
+        self.logger.debug(f"logger active")
+        self.logger.info("Connecting to database...")
 
-        self.database_filepath = database_filepath
+        self.book_cleaner = BookCleaner(debug_level)
 
-        self.book_cleaner = BookCleaner()
+        self.database_filepath = database_filepath
         if not DatabaseManager.is_database(database_filepath):
-            logger.info("Creating database...")
+            self.logger.info("Creating database...")
             DatabaseManager.create_autoanki_db(database_filepath)
-            logger.info("Done creating database.")
-        self.database_manager = DatabaseManager(database_filepath)
-        self.dictionary = CEDictionary()
-        self.deck_manager = DeckManager()
+            self.logger.info("Done creating database.")
+        self.database_manager = DatabaseManager(database_filepath, debug_level)
 
-        logger.info("Connected!")
+        self.dictionary = CEDictionary(debug_level)
+        self.deck_manager = DeckManager(debug_level)
+
+        self.logger.info("Connected!")
 
     def add_book(self, book_path: str, book_name: str = 'New Book'):
         """
         Add a directory full of files to the database
         :param book_path: The filepath to the directory that contains the files to add. e.g. lost_prince.txt
         :param book_name: The name of the book being added e.g. "Lost Prince"
         :return:
         """
 
-        logger.debug(f"autoanki: Adding book from [{book_path}]")
+        self.logger.debug(f"autoanki: Adding book from [{book_path}]")
 
         # Clean the book
         if not self.book_cleaner.clean(book_path):
-            #logger.warning("autoanki: Unable to clean book [" + book_name + "].")
+            # logger.warning("autoanki: Unable to clean book [" + book_name + "].")
             return
 
         # Add the book to the database
         if not self.database_manager.add_book(book_path, book_name):
-            #logger.warning("Unable to add [" + book_name + "] to database.")
+            self.logger.warning("Unable to add [" + book_name + "] to database.")
             return
 
-        logger.info("autoanki: Added [" + book_path + "].")
+        self.logger.info("autoanki: Added [" + book_path + "].")
 
     def complete_unfinished_definitions(self):
         """
         autoanki contains an internal definitions table that is scraped from the internet. As words are added to
         autoanki, their definitions must be found. This function passively finds definitions and adds them to the table
         :return: None
         """
 
         # TODO Make progress bar for unfinished records
-        logger.info("Checking for records...")
+        self.logger.info("Checking for records...")
         self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         response_rows = self.database_manager.cursor.fetchall()
         #while len(response_rows) > 0:
         self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         response_rows = self.database_manager.cursor.fetchall()
         if len(response_rows) > 0:
-            logger.info("Adding " + str(len(response_rows)) + " rows to dictionary table")
+            self.logger.info("Adding " + str(len(response_rows)) + " rows to dictionary table")
             for row in response_rows:
                 word = row[0]
 
-                logger.debug(f"Finding: [{word}]...")
+                self.logger.debug(f"Finding: [{word}]...")
                 params = self.dictionary.find_word(word)
                 if not params:
-                    logger.info(f"Could not find: [{word}]")
+                    self.logger.info(f"❌Could not find: [{word}]")
                 else:
+                    self.logger.info(f"✅Found: [{word}]")
                     self.database_manager.update_definition(params)
 
         else:
-            logger.info("No new rows to complete in dictionary table")
+            self.logger.info("No new rows to complete in dictionary table")
             # time.sleep(2)
 
+    def print_database_info(self):
+        self.database_manager.print_info()
+
     @staticmethod
     def is_database(db_path):
         return DatabaseManager.is_database(db_path)
 
     @staticmethod
     def create_autoanki_db(db_path: str):
         DatabaseManager.create_autoanki_db(db_path)
 
     def create_deck(self, deck_name: str, filepath: str):
         """
         Creates a deck file in the directory of the main file.
         :return:
         """
 
-        logger.info("Generating deck file [" + deck_name + ".apk]")
+        self.logger.info("Generating deck file [" + deck_name + ".apk]")
         words = self.database_manager.get_all_completed_definitions()
 
         deck_path = self.deck_manager.generate_deck_file(words, deck_name, filepath)
         if deck_path is None:
-            logger.warning("Was not able to create deck file for [", deck_name, "]")
+            self.logger.warning("Was not able to create deck file for [", deck_name, "]")
         else:
-            logger.info("Generated deck file [" + deck_path + "]")
+            self.logger.info("Generated deck file [" + deck_path + "]")
 
     @property
     def book_list(self):
         """
         Get a list of the books in the database
         :return: List of book names
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `autoanki-1.1.0/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.1.5/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 CLEANED_FILES_SUFFIX = '_cleaned'
 # Sentences That should not be added to the completed file.
 GARBAGE_SENTENCES = ['',
                      "",
                      "。",
                      "\n"]
 
-logger = logging.getLogger('autoanki.bookcleaner')
-logger.setLevel(logging.INFO)
 
 
 class BookCleaner:
 
-    def __init__(self):
+    def __init__(self, debug_level):
         """ Internal tool used to sanatize input
         Use `clean(bookpath)` to sanatize files and remove junk data
         """
+        self.logger = logging.getLogger('autoanki.bookcleaner')
+        self.logger.setLevel(debug_level)
         self.file_list = []
         self.bookpath = ""
 
     def clean(self, bookpath: str) -> None | list[str]:
         """
         Cleans the files contained in the bookpath. If bookpath is a single file, clean it.
         Args: 
             `bookpath: filepath of files to be cleaned`
         Return: 
             `str: list of cleaned file(s)`
         """
         if not os.path.exists(bookpath):
-            logger.warning("Cannot find path [" + str(bookpath) + "]")
+            self.logger.warning("Cannot find path [" + str(bookpath) + "]")
             return None
 
         # If the bookpath is a single file, clean and return it
         if os.path.isfile(bookpath):
             cleaned_files = [self._clean_file(bookpath, cleaned_files_root=None)]
             return cleaned_files
         else:
@@ -73,17 +73,14 @@
         if not os.path.exists(cleaned_files_root):
             os.mkdir(cleaned_files_root)
 
         for file in dirty_files:
             cleaned_filepath = self._clean_file(file, cleaned_files_root=cleaned_files_root)
             cleaned_files.append(cleaned_filepath)
 
-        # print(dirty_files)
-        # print(cleaned_files)
-
         return cleaned_files
 
     @staticmethod
     def _clean_file(filepath, cleaned_files_root):
         """
         Takes a txt file and cleans it up, putting every sentence on a new line
         :param filepath: The txt file to clean
```

### Comparing `autoanki-1.1.0/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.1.5/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,183 +4,163 @@
 import sqlite3
 import logging
 import unicodedata
 
 from pathlib import Path
 import jieba
 
-logger = logging.getLogger('autoanki.dbmngr')
-#TODO: Set logging level from autoanki
-# logger.setLevel(logging.INFO)
-
 FILTERED_WORDS = [
     '\n',
     ' ',
     '。',
     '"',
     "‘",
     "’",
     "“",
     "”",
     "，",
     "、",
+    "·",
 ]
 
 class DatabaseManager:
 
-    def __init__(self, database_path):
+    def __init__(self, database_path, debug_level):
+        self.logger = logging.getLogger('autoanki.dbmngr')
+        self.logger.setLevel(debug_level)
         if not os.path.exists(database_path):
-            logger.warning("The database [", database_path, "] does not exist.")
+            self.logger.warning("The database [", database_path, "] does not exist.")
             raise Exception("Cannot create DatabaseManager with invalid database path.")
         self.database_path = database_path
         self.books = []
         path = os.path.join(os.getcwd(), self.database_path)
         self.connection = sqlite3.connect(path)
         self.cursor = self.connection.cursor()
 
     @staticmethod
     def convert_to_tablename(name: str):
         """
         Converts a string to a sql-valid table name.
-        :param name: The name to convert
-        :return: A tablename valid for an sql table
+        `param name` The name to convert
+        `return` A tablename valid for an sql table
         """
-        # TODO Look more into table name conventions (- vs. _ etc.)
-        #   : in sql table name?
         value = unicodedata.normalize('NFKC', name)
         # value.replace("：",":")
         value = value.replace("：", "__")
         value = re.sub(r'[^\w\s-]', '', value.lower())
         return re.sub(r'[-\s]+', '_', value).strip('-_')
 
     @staticmethod
-    def is_database(database_name):
+    def is_database(database_name:str):
+        if not database_name.endswith(".db"):
+            return False
+        if not os.path.exists(database_name):
+            return False
         try:
-            if database_name.split(".")[1] != "db":
-                return False
-            if not os.path.exists(database_name):
-                return False
-
             connection = sqlite3.connect(database_name)
-
             cursor = connection.cursor()
             # This will fail if dictionary table does not exist
             cursor.execute("SELECT word FROM dictionary")
             connection.close()
-        except:
+        except sqlite3.OperationalError:
             return False
         return True
 
     @staticmethod
     def create_autoanki_db(database_path):
         """
         Creates an autoanki database file, including all tables needed for autoanki
-        :param database_path: The path to the database to create.
-        :return:
+        `database_path` The path to the database to create
         """
+        logger = logging.getLogger('autoanki.dbmngr')
         logger.info("Creating database [" + database_path + "]")
         path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
         try:
             with open(path, 'r') as sql_file:
                 sql_script = sql_file.read()
             connection = sqlite3.connect(database_path)
             cursor = connection.cursor()
             cursor.executescript(sql_script)
             connection.commit()
         except FileNotFoundError:
-            logger.warning("Could not create database: Missing sql files")
+            logger.warning("Could not create database: Missing SQL files")
             return False
-        # # Create book_table
-        # path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
-        # with open(path, 'r') as sql_file:
-        #     sql_script = sql_file.read()
-        # connection = sqlite3.connect(database_path)
-        # cursor = connection.cursor()
-        # cursor.executescript(sql_script)
-        # connection.commit()
 
-    def _create_book_table(self, book_name, table_name):
+    def _create_book_table(self, book_name, table_name) -> bool:
         """
         Creates a new entry in the book_list table
-        :param table_name: The name of the new entry to create
-        :return: False if error
+        `table_name` The name of the new entry to create
+        `return` False if error
         """
         self.cursor.execute("SELECT table_name FROM book_list")
         book_list = self.cursor.fetchall()
 
-        # Check if the book is already there
-        # If not, add the book to the table
-        if (table_name,) not in book_list:
-            # print("Inserting")
-            self.cursor.execute(f"INSERT INTO book_list VALUES(\"{book_name}\",\"{table_name}\",'cn')")
-            self.connection.commit()
-            fname = 'book_table.sql'
-            this_file = os.path.abspath(__file__)
-            this_dir = os.path.dirname(this_file)
-            wanted_file = os.path.join(this_dir, fname)
-            fd = open(wanted_file, 'r')
-            book_table_file = fd.read()
-            print(type(book_table_file))
-            book_table_file = book_table_file.replace("BOOK_NAME", table_name)
-            fd.close()
-            # Create the new table
-            self.cursor.execute(book_table_file)
-            self.connection.commit()
-
-        else:
-            logger.warning("The book is already in database. Not adding")
+        if (table_name,) in book_list:
+            self.logger.warning("The book is already in database. Not adding")
             return False
+
+        # self.logger.debug("Inserting")
+        self.cursor.execute(f"INSERT INTO book_list VALUES(\"{book_name}\",\"{table_name}\",'cn')")
+        self.connection.commit()
+        fname = 'book_table.sql'
+        this_file = os.path.abspath(__file__)
+        this_dir = os.path.dirname(this_file)
+        wanted_file = os.path.join(this_dir, fname)
+        fd = open(wanted_file, 'r')
+        book_table_file = fd.read()
+        book_table_file = book_table_file.replace("BOOK_NAME", table_name)
+        fd.close()
+        # Create the new table
+        self.cursor.execute(book_table_file)
+        self.connection.commit()
         return True
 
     def add_file_to_database(self, filepath, table_name):
         """
         Adds every word in a file to both the dictionary table and the book's table
-        :param filepath: The path to the file
-        :param table_name: The name of the table to add the words to.
+        `filepath` The path to the file
+        `table_name` The name of the table to add the words to.
             This should be the same for every wile in a given book
-        :return:
         """
-        logger.info(f"Adding file {filepath} to database...")
+        self.logger.info(f"Adding file {filepath} to database...")
 
         # Get number of appearances for each word in the file, and put it into a dictionary
         word_appearances = {}
         # As we add words to the definitions table, get the id. This is for the book table
         word_ids = {}
         with open(filepath,'r',encoding='utf-8') as f:
             line = " "
-            i = 0
             while line:
                 line = f.readline()
-                i += 1
                 if line:
                     # print("Line: ", line)
                     tokenized_line = jieba.lcut(line)
                     # print("Tokenized line: ", tokenized_line)
                     for word in tokenized_line:
 
                         is_ascii = len(word) == len(word.encode())
                         if word not in FILTERED_WORDS and not is_ascii:
                             # print("Word: ",word)
                             if word_appearances.get(word) == None:
                                 word_appearances[word] = 1
                             else:
                                 word_appearances[word] += 1
 
-        logger.info(f"Found {str(len(word_appearances.items()))} words in file.")
+        self.logger.info(f"Found {str(len(word_appearances.items()))} words in file.")
 
         # Add the words to the dictionary if they are not already there
         self.cursor.execute(f"SELECT word FROM dictionary")
         self.connection.commit()
         dictionary_words = self.cursor.fetchall()
 
-        logger.info(f"Found {str(len(dictionary_words))} words in dictionary.")
+        self.logger.info(f"Found {str(len(dictionary_words))} words in dictionary.")
 
         for word, appearances in word_appearances.items():
             if (word,) not in dictionary_words:
-                # logger.info("Adding word...")
+                # self.logger.debug("Adding word...")
 
                 self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
                 self.connection.commit()
 
         # Make a dictionary of word ids from dictionary
         self.cursor.execute(f"SELECT word_id, word FROM dictionary")
         result = self.cursor.fetchall()
@@ -200,31 +180,29 @@
         # Add all words to the book_table
         for word, appearances in word_appearances.items():
 
             dictionary_word_id = word_id_dict[word]
 
             # If the word is already in the dictionary, add the number of appearances to it
             if dictionary_word_id in book_table_appearances:
-                # number_of_apprearances_in_table =
-                # print("HIT")
                 file_appearances = word_appearances[word]
                 db_appearances = book_table_appearances[dictionary_word_id]
                 print("File app:", file_appearances)
                 print("Book app:", book_table_appearances[dictionary_word_id])
                 sum = file_appearances + db_appearances
                 self.cursor.execute(f"UPDATE {table_name} SET number_of_appearances = ? "
                                     f"WHERE dictionary_word_id = ?", [sum, dictionary_word_id])
                 self.connection.commit()
 
             else:
                 self.cursor.execute(f"INSERT INTO {table_name} (dictionary_word_id, number_of_appearances) "
                                     f"VALUES (?,?)", [dictionary_word_id, word_appearances[word]])
                 self.connection.commit()
 
-        logger.info("Done adding file to database")
+        self.logger.info("Done adding file to database")
 
     def add_book(self, bookpath: str, book_name: str):
         """
         Adds a file to the autoanki database. This involves the following steps:\n
         1 - Add book to the book_list table
         2 - Add all the files in "bookpath" to the definitions table and book table
         3 - Add book to book_list property
@@ -233,33 +211,33 @@
 
         if not already there, adding the
         :param bookpath: The filepath to the book. This is file, or a directory of files
         :param book_name: The name of the book. This will show up in the Anki deck
         :return: None
         """
         # TODO Make this work for multiple files. Right now only works for one filepath
-        logger.info("Adding book...")
+        self.logger.info("Adding book...")
         # Gets a 'table name' clean version of the book name
         book_tablename = self.convert_to_tablename(book_name)
 
         # Add the name of the book to the book_list table
         success = self._create_book_table(book_name, book_tablename)
         if not success:
-            logger.error("Failed to create book table")
+            self.logger.error("Failed to create book table")
             return
 
         # Add all the words in the book to the 'definitions' table
         self.add_file_to_database(bookpath, book_tablename)
 
         # # Add all the words in the bookpath to a new table with the name of the book.
         # success = self.add_book_table_to_db(bookpath, table_book_name)
         # if success is False:
         #     return
 
-        logger.info("Done adding book.")
+        self.logger.info("Done adding book.")
         return True
 
     def print_info(self):
         """
         Print basic information about the database
         :return:
         """
@@ -334,14 +312,19 @@
             # print(word["word"])
             # pprint.pp(word)
             # words.append(word)
             words.append(word)
         # pprint.pp(words)
         return words
 
+    def unfinished_definitions(self) -> int:
+        self.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
+        unfinished_rows = self.cursor.fetchall()
+        return len(unfinished_rows)
+
     @property
     def books(self):
         connection = sqlite3.connect(self.database_path)
         cursor = connection.cursor()
         cursor.execute("SELECT book_name FROM book_list")
         return_array = []
         for table in cursor.fetchall():
```

### Comparing `autoanki-1.1.0/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.1.5/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.0/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.1.5/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.0/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.1.5/src/autoanki.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.0
+Version: 1.1.5
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,25 +15,27 @@
 
 > **❗️** <br>
 Pull requests welcome! If you think you can improve AA in any way, open a PR!
 
 # autoanki
 Tool for generating Anki flashcards to learn Chinese.
 
-<img src="media/images/example.jpg" alt="Text to Anki" width="80%"/>
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
 
 ## Motivation
 
-When learning Chinese, usually the advice given is to learn the top X most common words.
-This is good advice, as you can get pretty far with this, however it's not perfect.
+When learning Chinese, advice is to learn the top X most common words.
+This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
-For example, Harry Potter. This book will have normal distrobution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
+For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
+With autoanki, you selectivley add words to an Anki file to continue progressing with your lanuage learning skills.
+
 ## Usage
 
 autoanki is both a library and a command-line tool.
 
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
@@ -47,24 +49,29 @@
 Then create an instance of autoanki using the database
 ```
 aa = AutoAnki(db_path)
 ```
 Add whatever books you want in your deck. These can be a single file, or a folder
 ```
 bookpath = 'short-story.txt'
-aa.add_book(bookpath, 'My first book😆')
+aa.add_book(bookpath, 'My first book🍎')
 ```
 Once all of your books are added, the definitions need to be found, and then you can create a deck!
 ```
 aa.complete_unfinished_definitions()
 aa.create_deck("AutoAnki Deck", "output")
 ```
 This will automatically have the .apkg extension, which Anki uses. 
 Import this file into Anki, and you're all set.
 
+#### Other commands
+If you want to see the status of the database, use:
+```
+aa.print_database_info()
+```
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
 1. BookCleaner: Cleans the input coming in from files that the user supplies 
 2. DatabaseManager: Takes the cleaned input and puts it into the database
 3. Dictionary: Finds definitions for words in the database
 4. DeckManager: Creates Decks
@@ -87,33 +94,31 @@
 - frequency
 - hsk_level
 - top_level
 - audio_path
 - image_path
 - definition
 
-![Dictionary table](media/images/dictionary-table.jpg "Dictionary table") 
-*Dictionary table*  
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/dictionary-table.jpg?raw=true" alt="Dictionary table" width="80%"/>
 
 #### book_list:
 - book_name
 - book_table_name
 - language
 
-![Book list table](media/images/book_list_table.jpg "Book list table")
-*Book list table*
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_list_table.jpg?raw=true" alt="Book list table" width="50%"/>
 
 ### book
  - book_table_word_id
  - dictionary_word_id
  - number_of_appearances 
 
-![Book table](media/images/book_table.jpg "Book table")
-*Book table*
+<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/book_table.jpg?raw=true" alt="Book table" width="80%"/>
 
 ## Planned features
 - See ROADMAP.md
 
 ## Other Info
 
 If you would like to get involved, or learn more information, reading Anki documentation is really important, especially the [Getting Started](https://docs.ankiweb.net/getting-started.html)
 
+To get definitions, this autoanki uses the [CC-CEDICT](https://www.mdbg.net/chinese/dictionary?page=cedict) under the creative commons licence.
```

### Comparing `autoanki-1.1.0/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.1.5/src/autoanki.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 src/autoanki/BookCleaner/BookCleaner.py
 src/autoanki/BookCleaner/__init__.py
 src/autoanki/DatabaseManager/DatabaseManager.py
 src/autoanki/DatabaseManager/__init__.py
 src/autoanki/DatabaseManager/book_table.sql
 src/autoanki/DatabaseManager/book_table_view.sql
 src/autoanki/DatabaseManager/databases_init.sql
+src/autoanki/DeckManager/DeckManager.py
 src/autoanki/DeckManager/__init__.py
+src/autoanki/DeckManager/template_decks.py
 src/autoanki/Dictionary/CEDictionary.py
 src/autoanki/Dictionary/Dictionary.py
 src/autoanki/Dictionary/YellowBridgeDictionary.py
 src/autoanki/Dictionary/__init__.py
```

