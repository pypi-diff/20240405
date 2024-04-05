# Comparing `tmp/configure_dms_viz-1.2.2.tar.gz` & `tmp/configure_dms_viz-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configure_dms_viz-1.2.2.tar", max compression
+gzip compressed data, was "configure_dms_viz-1.3.2.tar", max compression
```

## Comparing `configure_dms_viz-1.2.2.tar` & `configure_dms_viz-1.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1095 2024-03-29 17:35:22.213986 configure_dms_viz-1.2.2/LICENSE
--rw-r--r--   0        0        0      621 2024-03-29 17:35:22.213986 configure_dms_viz-1.2.2/README.md
--rw-r--r--   0        0        0        0 2024-03-29 17:35:22.213986 configure_dms_viz-1.2.2/configure_dms_viz/__init__.py
--rwxr-xr-x   0        0        0    37893 2024-03-29 17:35:22.213986 configure_dms_viz-1.2.2/configure_dms_viz/configure_dms_viz.py
--rw-r--r--   0        0        0     7948 2024-03-29 17:35:22.213986 configure_dms_viz-1.2.2/configure_dms_viz/pdb_utils.py
--rw-r--r--   0        0        0     1120 2024-03-29 17:35:22.213986 configure_dms_viz-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 configure_dms_viz-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/LICENSE
+-rw-r--r--   0        0        0      621 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/configure_dms_viz/__init__.py
+-rwxr-xr-x   0        0        0    38645 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/configure_dms_viz/configure_dms_viz.py
+-rw-r--r--   0        0        0     8500 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/configure_dms_viz/pdb_utils.py
+-rw-r--r--   0        0        0     1120 2024-04-05 20:19:22.027565 configure_dms_viz-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 configure_dms_viz-1.3.2/PKG-INFO
```

### Comparing `configure_dms_viz-1.2.2/LICENSE` & `configure_dms_viz-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.2.2/README.md` & `configure_dms_viz-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `configure_dms_viz-1.2.2/configure_dms_viz/configure_dms_viz.py` & `configure_dms_viz-1.3.2/configure_dms_viz/configure_dms_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,22 +130,14 @@
         A list of the protein chains to include in the visualization.
 
     Returns
     -------
     pandas.DataFrame
     """
 
-    # Coerce values to floats to check if they are numeric
-    def is_numeric(value):
-        try:
-            float(value)
-            return True
-        except ValueError:
-            return False
-
     # Check that required columns are present in the sitemap data
     missing_sitemap_columns = {"sequential_site", "reference_site"} - set(
         sitemap_df.columns
     )
     if missing_sitemap_columns:
         raise ValueError(
             f"The following columns do not exist in the sitemap: {list(missing_sitemap_columns)}"
@@ -200,14 +192,19 @@
         )
 
     # Drop the columns that aren't needed for the visualization
     sitemap_df = sitemap_df[
         ["reference_site", "protein_site", "sequential_site", "chains"]
     ]
 
+    # If a column is of type float, convert it to an integer
+    for col in sitemap_df.columns:
+        if sitemap_df[col].dtype == "float64":
+            sitemap_df[col] = sitemap_df[col].astype(int)
+
     return sitemap_df
 
 
 # Join the additional dataframes to the main dataframe
 def join_additional_data(mut_metric_df, join_data):
     """Join additional dataframes to the main mutation dataframe.
 
@@ -379,18 +376,18 @@
 
     Parameters
     ---------
     mut_metric_df: pandas.DataFrame
         A dataframe containing site- and mutation-level data for visualization.
     metric_col: str
         The name of the column the contains the metric for visualization.
-    sitemap_df: pandas.DataFrame
-        A dataframe mapping sequential sites to reference sites to protein sites.
     structure: str
         An RCSB PDB ID (i.e. 6UDJ) or the path to a file with a *.pdb extension.
+    sitemap_df: pandas.DataFrame or None
+        A dataframe mapping sequential sites to reference sites to protein sites.
     metric_name: str or None
         Rename the metric column to this name if desired. This name shows up in the plot.
     condition_col: str or None
         The name of the column the contains the condition if there are multiple measurements per mutation.
     condition_name: str or None
         Rename or format the condition column if desired.
     join_data: list or None
@@ -433,14 +430,29 @@
         excluded_chains = "none"
 
     # Check that the necessary columns are present in the mut_metric dataframe and format
     mut_metric_df = format_mutation_data(
         mut_metric_df, metric_col, condition_col, alphabet
     )
 
+    # If there is no sitemap dataframe, create a default one
+    if sitemap_df is None:
+        click.secho(
+            message="Warning: No sitemap dataframe was provided. Creating a default sitemap.",
+            fg="yellow",
+        )
+        sitemap_df = pd.DataFrame(
+            {
+                "reference_site": mut_metric_df["reference_site"].unique(),
+                "sequential_site": range(
+                    1, len(mut_metric_df["reference_site"].unique()) + 1
+                ),
+            }
+        )
+
     # Check that the necessary columns are present in the sitemap dataframe and format
     sitemap_df = format_sitemap_data(sitemap_df, mut_metric_df, included_chains)
 
     # Keep track of the required columns to cut down on the final total data size
     cols_to_keep = ["reference_site", "wildtype", "mutant", metric_col]
 
     # Join the additional data to the main dataframe if there is any
@@ -599,31 +611,33 @@
         condition_col = condition_name
 
     # Check that the chains and wildtype residues are in the structure
     if check_pdb:
         if included_chains != "polymer":
             check_chains(get_structure(structure), included_chains.split(" "))
         # Check that the wildtype residues are in the structure
-        perc_matching, perc_missing = check_wildtype_residues(
-            get_structure(structure), mut_metric_df, sitemap_df, excluded_chains
+        perc_matching, perc_missing, count_matching, count_missing = (
+            check_wildtype_residues(
+                get_structure(structure), mut_metric_df, sitemap_df, excluded_chains
+            )
         )
         # Alert the user about the missing and matching residues
         if perc_matching < 0.5:
             color = "red"
-            message = f"Warning: Fewer than {perc_matching*100:.2F}% of the wildtype residues in the data match the corresponding residues in the structure."
+            message = f"Warning: Fewer than {perc_matching*100:.2F}% {count_matching} of the wildtype residues in the data match the corresponding residues in the structure."
         else:
             color = "yellow"
-            message = f"About {perc_matching*100:.2F}% of the wildtype residues in the data match the corresponding residues in the structure."
+            message = f"About {perc_matching*100:.2F}% {count_matching} of the wildtype residues in the data match the corresponding residues in the structure."
         click.secho(message=message, fg=color)
         if perc_missing >= 0.5:
             color = "red"
-            message = f"Warning: {perc_missing*100:.2F}% of the data sites are missing from the structure."
+            message = f"Warning: {perc_missing*100:.2F}% {count_missing} of the data sites are missing from the structure."
         else:
             color = "yellow"
-            message = f"About {perc_missing*100:.2F}% of the data sites are missing from the structure."
+            message = f"About {perc_missing*100:.2F}% {count_missing} of the data sites are missing from the structure."
         click.secho(message=message, fg=color)
 
     # Make a dictionary holding the experiment data
     experiment_dict = {
         "mut_metric_df": json.loads(mut_metric_df.to_json(orient="records")),
         "sitemap": sitemap_df.set_index("reference_site").to_dict(orient="index"),
         "metric_col": metric_col,
@@ -681,32 +695,33 @@
 @click.option(
     "--input",
     type=click.Path(exists=True),
     required=True,
     help="Path to a csv with site- and mutation-level data to visualize on a protein structure.",
 )
 @click.option(
-    "--sitemap",
-    type=click.Path(exists=True),
-    required=True,
-    help="Path to a csv with a mapping of sequential sites to reference sites to protein sites.",
-)
-@click.option(
     "--metric",
     type=str,
     required=True,
     help="The name of the column that contains the metric for visualization.",
 )
 @click.option(
     "--structure",
     type=str,
     required=True,
     help="An RCSB PDB ID (i.e. 6UDJ) or the path to a file with a *.pdb extension.",
 )
 @click.option(
+    "--sitemap",
+    type=click.Path(exists=True),
+    required=False,
+    default=None,
+    help="Path to a csv with a mapping of sequential sites to reference sites to protein sites.",
+)
+@click.option(
     "--name",
     type=str,
     required=True,
     help="The name of the experiment. This will be used when concatenating multiple experiments.",
 )
 @click.option(
     "--output",
@@ -865,16 +880,19 @@
         click.secho(
             message=f"\nJoining data from {len(join_data)} dataframe.", fg="green"
         )
     else:
         join_data_dfs = None
 
     # Read in the sitemap data
-    sitemap_df = pd.read_csv(sitemap)
-    click.secho(message=f"\nUsing sitemap from '{sitemap}'.", fg="green")
+    if sitemap is not None:
+        sitemap_df = pd.read_csv(sitemap)
+        click.secho(message=f"\nUsing sitemap from '{sitemap}'.", fg="green")
+    else:
+        sitemap_df = None
 
     # Create the dictionary to save as a json
     experiment_dict = make_experiment_dictionary(
         mut_metric_df,
         metric,
         sitemap_df,
         structure,
```

### Comparing `configure_dms_viz-1.2.2/configure_dms_viz/pdb_utils.py` & `configure_dms_viz-1.3.2/configure_dms_viz/pdb_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -193,12 +193,27 @@
             except KeyError:
                 site_not_in_structure.append(True)
         if matches_wildtype_at_site and all(matches_wildtype_at_site):
             matching_residues += 1
         if site_not_in_structure and all(site_not_in_structure):
             missing_sites += 1
 
-    # Calculate the matching and missing sites
-    total_matching_residues = matching_residues / total_sites
+    # How many residues match at sites present in the structure?
+    assert matching_residues <= total_sites - missing_sites
+    if total_sites == missing_sites:
+        total_matching_residues = 0
+        total_matching_string = "(0 of 0)"
+    else:
+        total_matching_residues = matching_residues / (total_sites - missing_sites)
+        total_matching_string = (
+            f"({matching_residues} of {total_sites - missing_sites})"
+        )
+    # How many sites in the data are missing in the structure?
     total_missing_sites = missing_sites / total_sites
+    total_missing_string = f"({missing_sites} of {total_sites})"
 
-    return (total_matching_residues, total_missing_sites)
+    return (
+        total_matching_residues,
+        total_missing_sites,
+        total_matching_string,
+        total_missing_string,
+    )
```

### Comparing `configure_dms_viz-1.2.2/pyproject.toml` & `configure_dms_viz-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configure-dms-viz"
-version = "1.2.2"
+version = "1.3.2"
 description = "Configure your data for visualization with dms-viz.github.io"
 authors = ["Will Hannon <hannonww@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "configure_dms_viz" }]
 
 [tool.poetry.dependencies]
```

### Comparing `configure_dms_viz-1.2.2/PKG-INFO` & `configure_dms_viz-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configure-dms-viz
-Version: 1.2.2
+Version: 1.3.2
 Summary: Configure your data for visualization with dms-viz.github.io
 License: MIT
 Author: Will Hannon
 Author-email: hannonww@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

