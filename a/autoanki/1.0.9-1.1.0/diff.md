# Comparing `tmp/autoanki-1.0.9.tar.gz` & `tmp/autoanki-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.0.9.tar", last modified: Fri May  5 21:40:56 2023, max compression
+gzip compressed data, was "autoanki-1.1.0.tar", last modified: Thu Apr  4 21:59:39 2024, max compression
```

## Comparing `autoanki-1.0.9.tar` & `autoanki-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.483939 autoanki-1.0.9/
--rw-r--r--   0 owner      (501) staff       (20)     1061 2023-04-17 18:57:35.000000 autoanki-1.0.9/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.0.9/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     4335 2023-05-05 21:40:56.484000 autoanki-1.0.9/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     3802 2023-04-19 00:15:21.000000 autoanki-1.0.9/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.0.9/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      662 2023-05-05 21:40:56.484219 autoanki-1.0.9/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.478092 autoanki-1.0.9/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.479828 autoanki-1.0.9/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     5171 2023-04-27 16:28:13.000000 autoanki-1.0.9/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.481406 autoanki-1.0.9/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     7268 2023-04-17 17:53:21.000000 autoanki-1.0.9/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.482600 autoanki-1.0.9/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    13282 2023-05-05 17:57:22.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.482838 autoanki-1.0.9/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     6413 2023-04-17 18:46:28.000000 autoanki-1.0.9/src/autoanki/DeckManager/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.483694 autoanki-1.0.9/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)      122 2023-04-17 18:22:48.000000 autoanki-1.0.9/src/autoanki/Dictionary/CC-CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      232 2023-04-17 16:36:34.000000 autoanki-1.0.9/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5580 2023-04-17 17:53:21.000000 autoanki-1.0.9/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       58 2023-04-17 18:23:02.000000 autoanki-1.0.9/src/autoanki/Dictionary/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.0.9/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2023-05-05 21:40:56.480956 autoanki-1.0.9/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     4335 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)      798 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.0.9/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:40:56.000000 autoanki-1.0.9/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.914944 autoanki-1.1.0/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.0/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)       75 2023-05-05 18:09:43.000000 autoanki-1.1.0/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     4165 2024-04-04 21:59:39.914877 autoanki-1.1.0/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     3632 2024-04-04 21:52:38.000000 autoanki-1.1.0/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.0/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      699 2024-04-04 21:59:39.915222 autoanki-1.1.0/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.907486 autoanki-1.1.0/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.909363 autoanki-1.1.0/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     5514 2024-04-01 00:05:03.000000 autoanki-1.1.0/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.910960 autoanki-1.1.0/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     7312 2024-03-31 20:22:09.000000 autoanki-1.1.0/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.912651 autoanki-1.1.0/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13541 2024-04-01 14:40:06.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.0/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.912893 autoanki-1.1.0/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     5924 2024-04-04 21:35:35.000000 autoanki-1.1.0/src/autoanki/DeckManager/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.914193 autoanki-1.1.0/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     2178 2024-04-01 00:02:43.000000 autoanki-1.1.0/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      270 2024-03-31 23:26:31.000000 autoanki-1.1.0/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)     5561 2024-03-31 20:00:33.000000 autoanki-1.1.0/src/autoanki/Dictionary/YellowBridgeDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.0/src/autoanki/Dictionary/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.0/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-04-04 21:59:39.914615 autoanki-1.1.0/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     4165 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)      795 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.0/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-04-04 21:59:39.000000 autoanki-1.1.0/src/autoanki.egg-info/top_level.txt
```

### Comparing `autoanki-1.0.9/LICENSE.txt` & `autoanki-1.1.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Copyright 2023 Jarvis Coghlin
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `autoanki-1.0.9/setup.cfg` & `autoanki-1.1.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.0.9
+version = 1.1.0
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls = 
@@ -13,16 +13,19 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 include_package_data = True
 zip_safe = False
-packages = find:
 package_dir = 
 	= src
+packages = find:
 python_requires = >=3.6
 
+[options.packages.find]
+where = src
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `autoanki-1.0.9/src/autoanki/AutoAnki.py` & `autoanki-1.1.0/src/autoanki/AutoAnki.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,119 @@
 import logging
 
 from .BookCleaner import BookCleaner
 from .DatabaseManager import DatabaseManager
-from .Dictionary import YellowBridgeDictionary
+from .Dictionary import CEDictionary
 from .DeckManager import DeckManager
 
+BLACK = "\u001b[30m"
+RED = "\u001b[31m"
+GREEN = "\u001b[32m"
+YELLOW = "\u001b[33m"
+BLUE = "\u001b[34m"
+MAGENTA = "\u001b[35m"
+CYAN = "\u001b[36m"
+WHITE = "\u001b[37m"
+RESET = "\u001b[0m"
+# Add this to see the function name:
+#%(funcName)s
+logging.basicConfig(
+    # filename='HISTORYlistener.log',
+    level=logging.DEBUG,
+    format=f'{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)18s{RESET}: %(message)s',
+    datefmt='%Y-%m-%d %H:%M:%S',
+)
+
 logger = logging.getLogger('autoanki')
 logger.setLevel(logging.INFO)
+logger.debug(f"logger active")
+
 logging.basicConfig(
     # filename='HISTORYlistener.log',
-    level=logging.DEBUG,
-    format='%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s',
+    level=logging.CRITICAL,
+    format=f'--{GREEN}%(asctime)s{RESET} {RED}%(levelname)8s{RESET} {YELLOW}%(name)18s{RESET}: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 
+
 class AutoAnki:
 
-    def __init__(self, database_filepath='autoanki.db'):
+    def __init__(self, database_filepath='autoanki.db', logging_level=20):
         """
         Creates an instance of autoanki.
         This creates a book cleaner, database connection, and deck maker
         :param database_filepath: The filepath for the database
+        :param logging_level: between 0 (DEBUG) and 50(CRITICAL)
         """
-        logger.info("autoanki: Connecting to database...")
+        logger.setLevel(logging_level)
+        logger.info("Connecting to database...")
 
         self.database_filepath = database_filepath
 
         self.book_cleaner = BookCleaner()
         if not DatabaseManager.is_database(database_filepath):
             logger.info("Creating database...")
             DatabaseManager.create_autoanki_db(database_filepath)
             logger.info("Done creating database.")
         self.database_manager = DatabaseManager(database_filepath)
-        self.dictionary = YellowBridgeDictionary()
+        self.dictionary = CEDictionary()
         self.deck_manager = DeckManager()
 
-        logger.info("autoanki: Connected!")
+        logger.info("Connected!")
 
     def add_book(self, book_path: str, book_name: str = 'New Book'):
         """
-        Add a directory ful of files to the database
+        Add a directory full of files to the database
         :param book_path: The filepath to the directory that contains the files to add. e.g. lost_prince.txt
         :param book_name: The name of the book being added e.g. "Lost Prince"
         :return:
         """
 
         logger.debug(f"autoanki: Adding book from [{book_path}]")
 
         # Clean the book
         if not self.book_cleaner.clean(book_path):
-            logger.warning("autoanki: Unable to clean book [" + book_name + "].")
+            #logger.warning("autoanki: Unable to clean book [" + book_name + "].")
             return
 
         # Add the book to the database
         if not self.database_manager.add_book(book_path, book_name):
-            logger.warning("Unable to add [" + book_name + "] to database.")
+            #logger.warning("Unable to add [" + book_name + "] to database.")
             return
 
         logger.info("autoanki: Added [" + book_path + "].")
 
     def complete_unfinished_definitions(self):
         """
-        autoanki contains an internal definitions' table that is scraped from the internet. As words are added to
+        autoanki contains an internal definitions table that is scraped from the internet. As words are added to
         autoanki, their definitions must be found. This function passively finds definitions and adds them to the table
         :return: None
         """
 
-        # TODO Make progress par for unfinished records
+        # TODO Make progress bar for unfinished records
         logger.info("Checking for records...")
         self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         response_rows = self.database_manager.cursor.fetchall()
-        while len(response_rows) > 0:
-            self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
-            response_rows = self.database_manager.cursor.fetchall()
-            if len(response_rows) > 0:
-                logger.info("Adding " + str(len(response_rows)) + " rows to dictionary table")
-                for row in response_rows:
-                    word = row[0]
-
-                    # TODO This is a bad way of doing it, but find word is returning all of the parameters to
-                    #     add to the database
-                    # TODO create a dictionary that gets words from a file, not the internet
-                    params = self.dictionary.find_word(word)
-                    self.database_manager.complete_definition(params)
+        #while len(response_rows) > 0:
+        self.database_manager.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
+        response_rows = self.database_manager.cursor.fetchall()
+        if len(response_rows) > 0:
+            logger.info("Adding " + str(len(response_rows)) + " rows to dictionary table")
+            for row in response_rows:
+                word = row[0]
+
+                logger.debug(f"Finding: [{word}]...")
+                params = self.dictionary.find_word(word)
+                if not params:
+                    logger.info(f"Could not find: [{word}]")
+                else:
+                    self.database_manager.update_definition(params)
 
-            else:
-                logger.info("No new rows to complete in dictionary table")
+        else:
+            logger.info("No new rows to complete in dictionary table")
             # time.sleep(2)
 
     @staticmethod
     def is_database(db_path):
         return DatabaseManager.is_database(db_path)
 
     @staticmethod
@@ -97,44 +121,42 @@
         DatabaseManager.create_autoanki_db(db_path)
 
     def create_deck(self, deck_name: str, filepath: str):
         """
         Creates a deck file in the directory of the main file.
         :return:
         """
-        # FEATURE Add more options for how the deck looks
-        # FEATURE get files from only one book, not the whole database
 
-        logger.info("Generating deck file [" + deck_name + ".apk ]")
+        logger.info("Generating deck file [" + deck_name + ".apk]")
         words = self.database_manager.get_all_completed_definitions()
 
         deck_path = self.deck_manager.generate_deck_file(words, deck_name, filepath)
         if deck_path is None:
             logger.warning("Was not able to create deck file for [", deck_name, "]")
         else:
             logger.info("Generated deck file [" + deck_path + "]")
 
     @property
     def book_list(self):
         """
         Get a list of the books in the database
         :return: List of book names
         """
-        return self.database_manager.book_list
+        return self.database_manager.books
 
     @book_list.setter
-    def book_list(self, value):
+    def book_list(self, _):
         pass
 
     @property
     def unfinished_entries(self):
         return self.database_manager.unfinished_definitions()
 
     @unfinished_entries.setter
-    def unfinished_entries(self, value):
+    def unfinished_entries(self, _):
         pass
 
 
 if __name__ == '__main__':
 
     aa = AutoAnki()
     print(aa.book_list)
```

### Comparing `autoanki-1.0.9/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.1.0/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,52 +16,56 @@
 CLEANED_FILES_SUFFIX = '_cleaned'
 # Sentences That should not be added to the completed file.
 GARBAGE_SENTENCES = ['',
                      "",
                      "。",
                      "\n"]
 
-logger = logging.getLogger('autoanki')
+logger = logging.getLogger('autoanki.bookcleaner')
 logger.setLevel(logging.INFO)
 
 
 class BookCleaner:
 
     def __init__(self):
+        """ Internal tool used to sanatize input
+        Use `clean(bookpath)` to sanatize files and remove junk data
+        """
         self.file_list = []
         self.bookpath = ""
 
-    def clean(self, bookpath: str):
+    def clean(self, bookpath: str) -> None | list[str]:
         """
         Cleans the files contained in the bookpath. If bookpath is a single file, clean it.
-        :return: The path to the cleaned file(s)
+        Args: 
+            `bookpath: filepath of files to be cleaned`
+        Return: 
+            `str: list of cleaned file(s)`
         """
         if not os.path.exists(bookpath):
-            # PRACTICE Should I raise an error here, or let the caller raise one?
-            logger.warning("BookCleaner: Cannot find path [" + str(bookpath) + "]")
+            logger.warning("Cannot find path [" + str(bookpath) + "]")
             return None
 
         # If the bookpath is a single file, clean and return it
         if os.path.isfile(bookpath):
-            cleaned_path = self._clean_file(bookpath, cleaned_files_root=None)
-            return cleaned_path
-        # Otherwise, get a list of files to clean, and return the cleaned files directory
+            cleaned_files = [self._clean_file(bookpath, cleaned_files_root=None)]
+            return cleaned_files
         else:
             dirty_files = []
             for root, dirs, files in os.walk(bookpath):
                 for file in files:
                     # Only clean files that are not in cleaned_files directory
                     in_cleaned = str(root).find(CLEANED_FILES_DIRECTORY) != -1
                     if not in_cleaned:
                         if '.txt' in file:
                             dirty_files.append(os.path.join(root, file))
 
             # Check this cleaning won't be mean to the CPU
             if len(dirty_files) > 50:
-                yn = input("The number of files is very large. Are you sure you want to convert this many files? (Y/N)")
+                yn = input("Over 50 files. Are you sure you want to convert this many files? (Y/N)")
                 if yn.lower() != 'y':
                     return None
 
         # Now we have a list of files to convert in a list
         cleaned_files = []
 
         # Create directory for files
@@ -175,8 +179,8 @@
     #         "w",
     #         encoding="utf-8")
     #     for line in current_compacted_file_text.split("\n"):
     #         current_file.write(line + "\n")
     #     current_file.close()
     #
     #     print("Done compacting")
-    #     return True
+    #     return True
```

### Comparing `autoanki-1.0.9/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.1.0/src/autoanki/DatabaseManager/DatabaseManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,39 @@
 import sqlite3
 import logging
 import unicodedata
 
 from pathlib import Path
 import jieba
 
-logger = logging.getLogger('autoanki')
-logger.setLevel(logging.INFO)
-
+logger = logging.getLogger('autoanki.dbmngr')
+#TODO: Set logging level from autoanki
+# logger.setLevel(logging.INFO)
+
+FILTERED_WORDS = [
+    '\n',
+    ' ',
+    '。',
+    '"',
+    "‘",
+    "’",
+    "“",
+    "”",
+    "，",
+    "、",
+]
 
 class DatabaseManager:
 
     def __init__(self, database_path):
         if not os.path.exists(database_path):
             logger.warning("The database [", database_path, "] does not exist.")
             raise Exception("Cannot create DatabaseManager with invalid database path.")
         self.database_path = database_path
-        self.book_list = []
+        self.books = []
         path = os.path.join(os.getcwd(), self.database_path)
         self.connection = sqlite3.connect(path)
         self.cursor = self.connection.cursor()
 
     @staticmethod
     def convert_to_tablename(name: str):
         """
@@ -60,15 +73,15 @@
     @staticmethod
     def create_autoanki_db(database_path):
         """
         Creates an autoanki database file, including all tables needed for autoanki
         :param database_path: The path to the database to create.
         :return:
         """
-        logger.info("DatabaseManager: Creating database [" + database_path + "]")
+        logger.info("Creating database [" + database_path + "]")
         path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
         try:
             with open(path, 'r') as sql_file:
                 sql_script = sql_file.read()
             connection = sqlite3.connect(database_path)
             cursor = connection.cursor()
             cursor.executescript(sql_script)
@@ -140,15 +153,16 @@
                 i += 1
                 if line:
                     # print("Line: ", line)
                     tokenized_line = jieba.lcut(line)
                     # print("Tokenized line: ", tokenized_line)
                     for word in tokenized_line:
 
-                        if word != '\n':
+                        is_ascii = len(word) == len(word.encode())
+                        if word not in FILTERED_WORDS and not is_ascii:
                             # print("Word: ",word)
                             if word_appearances.get(word) == None:
                                 word_appearances[word] = 1
                             else:
                                 word_appearances[word] += 1
 
         logger.info(f"Found {str(len(word_appearances.items()))} words in file.")
@@ -205,19 +219,19 @@
                 self.cursor.execute(f"INSERT INTO {table_name} (dictionary_word_id, number_of_appearances) "
                                     f"VALUES (?,?)", [dictionary_word_id, word_appearances[word]])
                 self.connection.commit()
 
         logger.info("Done adding file to database")
 
     def add_book(self, bookpath: str, book_name: str):
-        f"""
+        """
         Adds a file to the autoanki database. This involves the following steps:\n
-        1 - Add book to the book_list table\n
-        2 - Add all the files in "bookpath" to the definitions table and book table\n
-        3 - Add book to book_list property\n
+        1 - Add book to the book_list table
+        2 - Add all the files in "bookpath" to the definitions table and book table
+        3 - Add book to book_list property
 
         If given a directory, it will recursively search for all files in the directory and add them.
 
         if not already there, adding the
         :param bookpath: The filepath to the book. This is file, or a directory of files
         :param book_name: The name of the book. This will show up in the Anki deck
         :return: None
@@ -226,48 +240,49 @@
         logger.info("Adding book...")
         # Gets a 'table name' clean version of the book name
         book_tablename = self.convert_to_tablename(book_name)
 
         # Add the name of the book to the book_list table
         success = self._create_book_table(book_name, book_tablename)
         if not success:
+            logger.error("Failed to create book table")
             return
 
         # Add all the words in the book to the 'definitions' table
         self.add_file_to_database(bookpath, book_tablename)
 
         # # Add all the words in the bookpath to a new table with the name of the book.
         # success = self.add_book_table_to_db(bookpath, table_book_name)
         # if success is False:
         #     return
 
         logger.info("Done adding book.")
         return True
 
-    def print_database_status(self):
+    def print_info(self):
         """
         Print basic information about the database
         :return:
         """
         self.cursor.execute("SELECT word FROM dictionary")
         all_rows = self.cursor.fetchall()
         self.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         unfinished_rows = self.cursor.fetchall()
         format_string_int = "{:<30} | {:>8}"
         format_string_dec = "{:<30} | {:>8.2}"
         print("------------------------")
         print(self.database_path)
         print("------------------------")
-        print(format_string_int.format("Number of books:", len(self.book_list)))
+        print(format_string_int.format("Number of books:", len(self.books)))
         print(format_string_dec.format("Database size (MB):", Path(self.database_path).stat().st_size / (1024 * 1024)))
         print("Dictionary Table:")
         print(format_string_int.format("Number of rows:", len(all_rows)))
         print(format_string_int.format("Number of unfinished rows:", len(unfinished_rows)))
 
-    def complete_definition(self, params: list):
+    def update_definition(self, params: list):
         f"""
         Complete a definition for one word in the dictionary table\n
         traditional_script = params[0]\n
         word_type = params[1]\n
         pinyin = params[2]\n
         pinyin_numbers = params[3]\n
         sub_components = params[4]\n
@@ -319,24 +334,20 @@
             # print(word["word"])
             # pprint.pp(word)
             # words.append(word)
             words.append(word)
         # pprint.pp(words)
         return words
 
-   
-
-
-
     @property
-    def book_list(self):
+    def books(self):
         connection = sqlite3.connect(self.database_path)
         cursor = connection.cursor()
         cursor.execute("SELECT book_name FROM book_list")
         return_array = []
         for table in cursor.fetchall():
             return_array.append(table[0])
         return return_array
 
-    @book_list.setter
-    def book_list(self, value):
-        self._book_list = value
+    @books.setter
+    def books(self, value):
+        self._books= value
```

### Comparing `autoanki-1.0.9/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.1.0/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.0.9/src/autoanki/DeckManager/__init__.py` & `autoanki-1.1.0/src/autoanki/DeckManager/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 
 import genanki
 from genanki import Model
 from pprint import pprint
 
-logger = logging.getLogger('autoanki')
+logger = logging.getLogger('autoanki.dckmngr')
 logger.setLevel(logging.INFO)
 
+# TODO If the user included .apkg at the end, ignore it
+
 # TODO Add this somewhere
 # # All the resources for finding the
 #         CHINESE_CARD_MODEL = Model(
 #             1559383145,
 #             'Chinese Card (autoanki)',
 #             fields=[
 #                 {
@@ -89,35 +91,14 @@
         # 'qfmt': '{{FrontSide}}\n\n<hr id=answer>\n{{Pinyin}}\n{{Back}}',
         # 'afmt': '{{Front}}',
         # },
     ],
     css='.card {\n font-family: arial;\n font-size: 30px;\n text-align: center;\n color: black;\n background-color: white;\n}\n',
 )
 
-
-def _create_test_deck():
-    """
-    Used for testing
-    :return:
-    """
-
-    print("Generating card")
-    my_note = genanki.Note(
-        model=CHINESE_CARD_MODEL,
-        fields=['Capital of Canada', 'Ottawa'],
-        sort_field=1
-    )
-    my_deck = genanki.Deck(
-        2023480110,
-        'Country Capitals'
-    )
-    my_deck.add_note(my_note)
-    genanki.Package(my_deck).write_to_file('output.apkg')
-
-
 class DeckManager:
     """
     The class to make anki decks. Create the file using generate_deck_file()
     One of the most important concepts is the id. No matter what deck the word is in, it should have the same id so the
     same card in different decks can be remembered.
     This class makes extensive use of genanki, so understanding how genanki works
         is pretty significant for understanding this.
@@ -136,33 +117,34 @@
     def generate_deck_file(self, words, deck_name: str, filename: str):
         """
         Generates a deck file from the database
         :param deck_name: The name of the deck to be created
         :param definitions_filename: The name of the file containing the definitions.
         :return:
         """
-        # TODO This is a legacy function. Update this to use the database, rather than text file
-        # Has not been changed to use the object, which it should.
 
         # Number of valid cards that have been added to the deck
         num_of_valid_cards_added = 0
 
         # length = general_functions.file_len(definitions_filename)
         # self.deck.add_note()
         self.deck = genanki.Deck(
             2020000110,
             deck_name
         )
 
         for row in words:
             word = row["word"]
             word_traditional = row["word_traditional"]
-            if word_traditional == 'Same':
+            if word_traditional == word:
                 word_traditional = "-"
-            pinyin = row["pinyin"]
+            if row["pinyin"]:
+                pinyin = row["pinyin"]
+            else:
+                pinyin = row["pinyin_numbers"]
             definition = "<br>" + row["definition"]
             # word["word_id"]
             # word["word"]
             # word["word_traditional"]
             # word["word_type"]
             # word["pinyin"]
             # word["pinyin_numbers"]
@@ -189,16 +171,13 @@
                 fields=[word, word_traditional, pinyin, definition],
                 # sort_field can be used to sort when the cards appear.
                 # By default they are shown in the order they are addeed, so this is not currently used
                 sort_field=1,
 
             )
             self.deck.add_note(note)
+            num_of_valid_cards_added += 1
 
         genanki.Package(self.deck).write_to_file(filename + ".apkg")
         logger.info("Deck " + deck_name + " created with " + str(num_of_valid_cards_added) + " cards")
         return filename + ".apkg"
 
-
-if __name__ == '__main__':
-    maker = DeckManager()
-    maker.generate_deck_file('autoanki.apkg', 'example.txt')
```

### Comparing `autoanki-1.0.9/src/autoanki/Dictionary/YellowBridgeDictionary.py` & `autoanki-1.1.0/src/autoanki/Dictionary/YellowBridgeDictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         :param cache_number: The secondary page number for a word with multiple definitions. (See comments in body of
         function)
         :return:
         '''
         print(repr(word))
         if word == None or word == '':
             print("There is no page on Yellowbridge page for null")
-            logger
             return
 
         urlx = "http://www.yellowbridge.com/chinese/dictionary.php?word="
         url = urlx + urllib.parse.quote(word)
         if cache_number is not None:
             url += "&cache=" + cache_number
```

### Comparing `autoanki-1.0.9/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.1.0/src/autoanki.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 src/autoanki/BookCleaner/__init__.py
 src/autoanki/DatabaseManager/DatabaseManager.py
 src/autoanki/DatabaseManager/__init__.py
 src/autoanki/DatabaseManager/book_table.sql
 src/autoanki/DatabaseManager/book_table_view.sql
 src/autoanki/DatabaseManager/databases_init.sql
 src/autoanki/DeckManager/__init__.py
-src/autoanki/Dictionary/CC-CEDictionary.py
+src/autoanki/Dictionary/CEDictionary.py
 src/autoanki/Dictionary/Dictionary.py
 src/autoanki/Dictionary/YellowBridgeDictionary.py
 src/autoanki/Dictionary/__init__.py
```

