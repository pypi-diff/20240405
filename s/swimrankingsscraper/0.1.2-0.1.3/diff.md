# Comparing `tmp/swimrankingsscraper-0.1.2.tar.gz` & `tmp/swimrankingsscraper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swimrankingsscraper-0.1.2.tar", last modified: Mon Apr  1 18:13:25 2024, max compression
+gzip compressed data, was "swimrankingsscraper-0.1.3.tar", last modified: Fri Apr  5 17:12:14 2024, max compression
```

## Comparing `swimrankingsscraper-0.1.2.tar` & `swimrankingsscraper-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/swimrankingsscraper/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/swimrankingsscraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35478 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/swimrankingsscraper/swimrankingsscraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 18:13:25.000000 swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:25.322904 swimrankingsscraper-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22660 2024-04-01 18:13:08.000000 swimrankingsscraper-0.1.2/tests/test_swimrankingsscraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:12:14.923788 swimrankingsscraper-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-05 17:12:03.000000 swimrankingsscraper-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 17:12:14.923788 swimrankingsscraper-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-05 17:12:03.000000 swimrankingsscraper-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:12:14.923788 swimrankingsscraper-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-05 17:12:03.000000 swimrankingsscraper-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:12:14.919788 swimrankingsscraper-0.1.3/swimrankingsscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 17:12:03.000000 swimrankingsscraper-0.1.3/swimrankingsscraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35551 2024-04-05 17:12:03.000000 swimrankingsscraper-0.1.3/swimrankingsscraper/swimrankingsscraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:12:14.923788 swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-05 17:12:14.000000 swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-05 17:12:14.000000 swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:12:14.000000 swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 17:12:14.000000 swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 17:12:14.000000 swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:12:14.923788 swimrankingsscraper-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23328 2024-04-05 17:12:03.000000 swimrankingsscraper-0.1.3/tests/test_swimrankingsscraper.py
```

### Comparing `swimrankingsscraper-0.1.2/LICENSE` & `swimrankingsscraper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swimrankingsscraper-0.1.2/PKG-INFO` & `swimrankingsscraper-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swimrankingsscraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A scraper for swimrankings.net
 Home-page: https://swimrankingsscraper.readthedocs.io/
 Author: Bas Neeleman
 Author-email: bas@neeleman-mail.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `swimrankingsscraper-0.1.2/setup.py` & `swimrankingsscraper-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 
 setup(
     name='swimrankingsscraper',
-    version='0.1.2',
+    version='0.1.3',
     description='A scraper for swimrankings.net',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://swimrankingsscraper.readthedocs.io/',
     author='Bas Neeleman',
     author_email='bas@neeleman-mail.nl',
     license='MIT',
```

### Comparing `swimrankingsscraper-0.1.2/swimrankingsscraper/swimrankingsscraper.py` & `swimrankingsscraper-0.1.3/swimrankingsscraper/swimrankingsscraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,35 +356,35 @@
         - `athlete_id` (str): The ID of the athlete.
         - `sessionManager` (SessionManager): The requests session to be used for making HTTP requests.
         - `update_interval` (int): The minimum time interval (in seconds) between consecutive updates.
         """
         super().__init__(sessionManager, update_interval)
         self.athlete_id = athlete_id
 
-    def list_personal_bests(self) -> list:
+    def list_personal_bests(self, season="") -> list:
         """
         Retrieves a list of personal bests for the athlete.
 
         Returns:
         - `list`: A list of dictionaries containing information about each personal best.
         """
-        params = {'page': 'athleteDetail', 'athleteId': self.athlete_id}
+        params = {'page': 'athleteDetail', 'athleteId': self.athlete_id, 'pbest': season}
         try:
             soup = self._get_page_content(params)
             table = soup.find('table', {'class': 'athleteBest'})
         except AttributeError:
             return []
 
         data = []
         for row in table.find_all('tr', {'class': ['athleteBest0', 'athleteBest1']}):
             event_cell = row.find('td', {'class': 'event'})
             event_name = event_cell.find('a').get_text(strip=True)
             course_cell = row.find('td', {'class': 'course'})
             course_length = course_cell.get_text(strip=True)
-            time_cell = row.find('td', {'class': 'time'})
+            time_cell = row.find('td', {'class': ['time', 'swimtimeImportant']})
             time = convert_time(time_cell.get_text(strip=True))
             result_url = time_cell.find('a')['href']
             result_id = int(parse_qs(urlparse(result_url).query)['id'][0])
             fina_points = row.find('td', {'class': 'code'}).get_text(strip=True)
             data.append({'result_id': result_id, 'event_name': event_name, 'course_length': course_length, 'time': time, 'FINA Points': fina_points})
         return data
 
@@ -825,8 +825,8 @@
         return athletes   
 
 
 if __name__ == '__main__':
     # Example usage
     scraper = SwimrankingsScraper()
     athelete = scraper.get_athlete('4292888')
-    print(athelete.list_meets())
+    print(athelete.list_personal_bests(season='2024'))
```

### Comparing `swimrankingsscraper-0.1.2/swimrankingsscraper.egg-info/PKG-INFO` & `swimrankingsscraper-0.1.3/swimrankingsscraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swimrankingsscraper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A scraper for swimrankings.net
 Home-page: https://swimrankingsscraper.readthedocs.io/
 Author: Bas Neeleman
 Author-email: bas@neeleman-mail.nl
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `swimrankingsscraper-0.1.2/tests/test_swimrankingsscraper.py` & `swimrankingsscraper-0.1.3/tests/test_swimrankingsscraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
     def test_get_athlete(self):
         athlete_id = 123456
         athlete_instance = self.scraper.get_athlete(athlete_id)
         # Ensure that the Athlete instance is created with the correct parameters
         self.assertEqual(athlete_instance.athlete_id, athlete_id)
         self.assertEqual(athlete_instance.sessionManager, self.mock_session_manager)
-        
 
     def test_get_meet(self):
         meet_id = 789012
         meet_instance = self.scraper.get_meet(meet_id)
         # Ensure that the Meet instance is created with the correct parameters
         self.assertEqual(meet_instance.meet_id, meet_id)
         self.assertEqual(meet_instance.sessionManager, self.mock_session_manager)
@@ -183,28 +182,39 @@
         # Mock the _get_page_content method to avoid making actual requests
         self.athlete._get_page_content = MagicMock()
         self.athlete._get_page_content.return_value = values_for_testing.athlete_detail_page
         # Call the list_personal_bests method
         self.personal_best = self.athlete.list_personal_bests()
 
         # Assertions 
-        self.athlete._get_page_content.assert_called_once_with({'page': 'athleteDetail', 'athleteId': self.athete_id})
+        self.athlete._get_page_content.assert_called_once_with({'page': 'athleteDetail', 'athleteId': self.athete_id, 'pbest': ''})
         self.assertEqual(self.personal_best, values_for_testing.athlete_personal_best)
 
     def test_list_personal_bests_failure(self):
         # Mock the _get_page_content method to avoid making actual requests
         self.athlete._get_page_content = MagicMock()
         self.athlete._get_page_content.return_value = None
         # Call the list_personal_bests method
         self.personal_best = self.athlete.list_personal_bests()
 
         # Assertions 
-        self.athlete._get_page_content.assert_called_once_with({'page': 'athleteDetail', 'athleteId': self.athete_id})
+        self.athlete._get_page_content.assert_called_once_with({'page': 'athleteDetail', 'athleteId': self.athete_id, 'pbest': ''})
         self.assertEqual(self.personal_best, [])
 
+    def test_list_personal_bests_season_succes(self):
+        # Mock the _get_page_content method to avoid making actual requests
+        self.athlete._get_page_content = MagicMock()
+        self.athlete._get_page_content.return_value = values_for_testing.athlete_detail_season_page
+        # Call the list_personal_bests method
+        self.personal_best = self.athlete.list_personal_bests(season='2024')
+
+        # Assertions 
+        self.athlete._get_page_content.assert_called_once_with({'page': 'athleteDetail', 'athleteId': self.athete_id, 'pbest': '2024'})
+        self.assertEqual(self.personal_best, values_for_testing.athlete_season_best)
+
     def test_list_meets_succes(self):
         # Mock the _get_page_content method to avoid making actual requests
         self.athlete._get_page_content = MagicMock()
         self.athlete._get_page_content.return_value = values_for_testing.athlete_meets_page
         # Call the list_meets method
         self.meets = self.athlete.list_meets()
```

