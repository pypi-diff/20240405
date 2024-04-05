# Comparing `tmp/turning_points-0.0.3.tar.gz` & `tmp/turning_points-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turning_points-0.0.3.tar", last modified: Fri Apr  5 04:39:15 2024, max compression
+gzip compressed data, was "turning_points-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `turning_points-0.0.3.tar` & `turning_points-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,5 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.554109 turning_points-0.0.3/
--rw-rw-rw-   0        0        0     1070 2024-04-05 03:12:32.000000 turning_points-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3313 2024-04-05 04:39:15.553108 turning_points-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1898 2024-04-05 03:45:54.000000 turning_points-0.0.3/README.md
--rw-rw-rw-   0        0        0     1261 2024-04-05 04:37:56.000000 turning_points-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 04:39:15.554109 turning_points-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      703 2024-04-05 04:37:56.000000 turning_points-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.535081 turning_points-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.552108 turning_points-0.0.3/src/turning_points.egg-info/
--rw-rw-rw-   0        0        0     3313 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 04:39:15.000000 turning_points-0.0.3/src/turning_points.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 04:39:15.550108 turning_points-0.0.3/tests/
--rw-rw-rw-   0        0        0      325 2024-04-05 03:35:58.000000 turning_points-0.0.3/tests/test_turning_point_analyzer.py
+-rw-r--r--   0        0        0     1898 2024-04-05 03:45:54.203857 turning_points-0.0.4/README.md
+-rw-r--r--   0        0        0     1258 2024-04-05 04:41:55.065171 turning_points-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-05 04:33:29.236696 turning_points-0.0.4/src/turning_points/__init__.py
+-rw-r--r--   0        0        0    22753 2024-04-05 03:35:50.289929 turning_points-0.0.4/src/turning_points/turning_points.py
+-rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 turning_points-0.0.4/PKG-INFO
```

### Comparing `turning_points-0.0.3/PKG-INFO` & `turning_points-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,102 @@
-Metadata-Version: 2.1
-Name: turning_points
-Version: 0.0.3
-Summary: A package to find turing points in tracks, andd plot
-Home-page: https://github.com/lesptizami/turning_points
-Author: Your Name
-Author-email: Charles Fosseprez <charles.fosseprez.me@gmail.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/lesptizami/turning_points
-Project-URL: Issues, https://github.com/lesptizami/turning_points/issues
-Keywords: trajectory-analysis,turning-points,transition-probabilities,data-science
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama==0.4.6
-Requires-Dist: contourpy==1.2.1
-Requires-Dist: cycler==0.12.1
-Requires-Dist: exceptiongroup==1.2.0
-Requires-Dist: fonttools==4.50.0
-Requires-Dist: importlib_resources==6.4.0
-Requires-Dist: iniconfig==2.0.0
-Requires-Dist: kiwisolver==1.4.5
-Requires-Dist: matplotlib==3.8.4
-Requires-Dist: numpy==1.26.4
-Requires-Dist: packaging==24.0
-Requires-Dist: pillow==10.3.0
-Requires-Dist: pluggy==1.4.0
-Requires-Dist: pyparsing==3.1.2
-Requires-Dist: pytest==8.1.1
-Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: scipy==1.13.0
-Requires-Dist: six==1.16.0
-Requires-Dist: tomli==2.0.1
-Requires-Dist: zipp==3.18.1
-
-# Turning Point Analyzer
-
-## Overview
-The Turning Point Analyzer is a Python package for analyzing turning points in trajectories and calculating transition probabilities.
-
-## Installation
-You can install the Turning Point Analyzer package using pip:
-```bash
-pip install turning_point_analyzer
-```
-
-## Usage
-To use the Turning Point Analyzer in your Python code, you can import it as follows:
-
-```pytho
-from turning_points import TurningPointAnalyzer
-```
-
-Analyzing Turning Points
-```python
-from turning_points import TurningPointAnalyzer
-
-# Example trajectory data
-trajectories = [
-    [(0, 0), (1, 1), (2, 2), (3, 1), (4, 0)],  # Example trajectory 1
-    [(0, 0), (1, -1), (2, -2), (3, -1), (4, 0)]  # Example trajectory 2
-]
-
-# Create a TurningPointAnalyzer instance
-analyzer = TurningPointAnalyzer(trajectories)
-
-# Plot transition directions
-analyzer.plot_transition()
-
-# Plot frequency distribution of time between turns
-analyzer.plot_frequency()
-
-# Get the probability of same turn direction
-probability = analyzer.get_proba_same_turn()
-print("Probability of same turn direction:", probability)
-
-# Get the results
-results = analyzer.get_results()
-print("Results:", results)
-```
-
-## Testing
-To run tests for the Turning Point Analyzer, you can use the following command:
-
-```bash
-pytest
-```
-
-## Contributing
-Contributions are welcome! Please feel free to submit issues or pull requests.
-
-## License
-This project is licensed under the MIT License - see the LICENSE file for details.
-
-## Citing
-If you use this package for your publication, don't hesitate to cite it.
-example provided in citations.md
-
-
-## thanks for the RDP algorythm
-
-The package use the [Ramer–Douglas–Peucker](http://en.wikipedia.org/wiki/Ramer%E2%80%93Douglas%E2%80%93Peucker_algorithm) algorithm.
-It was obtained from: https://github.com/fhirschmann/rdp
+Metadata-Version: 2.1
+Name: turning_points
+Version: 0.0.4
+Summary: A package to find turing points in tracks, andd plot
+Keywords: trajectory-analysis,turning-points,transition-probabilities,data-science
+Author-email: Charles Fosseprez <charles.fosseprez.me@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Dist: colorama==0.4.6
+Requires-Dist: contourpy==1.2.1
+Requires-Dist: cycler==0.12.1
+Requires-Dist: exceptiongroup==1.2.0
+Requires-Dist: fonttools==4.50.0
+Requires-Dist: importlib_resources==6.4.0
+Requires-Dist: iniconfig==2.0.0
+Requires-Dist: kiwisolver==1.4.5
+Requires-Dist: matplotlib==3.8.4
+Requires-Dist: numpy==1.26.4
+Requires-Dist: packaging==24.0
+Requires-Dist: pillow==10.3.0
+Requires-Dist: pluggy==1.4.0
+Requires-Dist: pyparsing==3.1.2
+Requires-Dist: pytest==8.1.1
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: scipy==1.13.0
+Requires-Dist: six==1.16.0
+Requires-Dist: tomli==2.0.1
+Requires-Dist: zipp==3.18.1
+Project-URL: Homepage, https://github.com/lesptizami/turning_points
+Project-URL: Issues, https://github.com/lesptizami/turning_points/issues
+
+# Turning Point Analyzer
+
+## Overview
+The Turning Point Analyzer is a Python package for analyzing turning points in trajectories and calculating transition probabilities.
+
+## Installation
+You can install the Turning Point Analyzer package using pip:
+```bash
+pip install turning_point_analyzer
+```
+
+## Usage
+To use the Turning Point Analyzer in your Python code, you can import it as follows:
+
+```pytho
+from turning_points import TurningPointAnalyzer
+```
+
+Analyzing Turning Points
+```python
+from turning_points import TurningPointAnalyzer
+
+# Example trajectory data
+trajectories = [
+    [(0, 0), (1, 1), (2, 2), (3, 1), (4, 0)],  # Example trajectory 1
+    [(0, 0), (1, -1), (2, -2), (3, -1), (4, 0)]  # Example trajectory 2
+]
+
+# Create a TurningPointAnalyzer instance
+analyzer = TurningPointAnalyzer(trajectories)
+
+# Plot transition directions
+analyzer.plot_transition()
+
+# Plot frequency distribution of time between turns
+analyzer.plot_frequency()
+
+# Get the probability of same turn direction
+probability = analyzer.get_proba_same_turn()
+print("Probability of same turn direction:", probability)
+
+# Get the results
+results = analyzer.get_results()
+print("Results:", results)
+```
+
+## Testing
+To run tests for the Turning Point Analyzer, you can use the following command:
+
+```bash
+pytest
+```
+
+## Contributing
+Contributions are welcome! Please feel free to submit issues or pull requests.
+
+## License
+This project is licensed under the MIT License - see the LICENSE file for details.
+
+## Citing
+If you use this package for your publication, don't hesitate to cite it.
+example provided in citations.md
+
+
+## thanks for the RDP algorythm
+
+The package use the [Ramer–Douglas–Peucker](http://en.wikipedia.org/wiki/Ramer%E2%80%93Douglas%E2%80%93Peucker_algorithm) algorithm.
+It was obtained from: https://github.com/fhirschmann/rdp
```

### Comparing `turning_points-0.0.3/README.md` & `turning_points-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `turning_points-0.0.3/pyproject.toml` & `turning_points-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 [project]
 name = "turning_points"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Charles Fosseprez", email="charles.fosseprez.me@gmail.com" },
 ]
 description = "A package to find turing points in tracks, andd plot"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

