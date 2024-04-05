# Comparing `tmp/edgarquery-0.0.57.tar.gz` & `tmp/edgarquery-0.0.58.tar.gz`

## Comparing `edgarquery-0.0.57.tar` & `edgarquery-0.0.58.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0    24576 2020-02-02 00:00:00.000000 edgarquery-0.0.57/.notes.txt.swp
--rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 edgarquery-0.0.57/genusage.sh
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 edgarquery-0.0.57/notes.txt
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.57/scripts/edgarquery.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.57/scripts/edgartickerstocsv.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/__about__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/concepts.sh
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/ebquery.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarcikperson.py
--rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarcompanyconcepttocsv.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarcompanyfactsshow.py
--rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarcompanyfactstocsv.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarcompanyfactsziptocsv.py
--rw-r--r--   0        0        0     8602 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarlatest10K.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarlatestsubmissions.py
--rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarquery.py
--rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarsubmissions.py
--rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarsubmissionsziptocsv.py
--rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgartickerstocsv.py
--rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/edgarxbrlframestocsv.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/sedfile
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.57/src/edgarquery/tickerd.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.57/tests/__init__.py
--rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.57/tests/p.sh
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.57/tests/s.sh
--rwxr-xr-x   0        0        0     2431 2020-02-02 00:00:00.000000 edgarquery-0.0.57/tests/x.sh
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.57/tests/y.sh
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.57/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.57/LICENSE.txt
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 edgarquery-0.0.57/README.md
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 edgarquery-0.0.57/pyproject.toml
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 edgarquery-0.0.57/PKG-INFO
+-rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 edgarquery-0.0.58/genusage.sh
+-rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.58/notes.txt
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.58/scripts/edgarquery.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.58/scripts/edgartickerstocsv.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/__about__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/__init__.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/concepts.sh
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/ebquery.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcikperson.py
+-rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyconcepttocsv.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsshow.py
+-rwxr-xr-x   0        0        0     5961 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyfactstocsv.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsziptocsv.py
+-rw-r--r--   0        0        0     8602 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarlatest10K.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarlatestsubmissions.py
+-rwxr-xr-x   0        0        0    15138 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarquery.py
+-rw-r--r--   0        0        0    13988 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarsubmissions.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarsubmissionsziptocsv.py
+-rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgartickerstocsv.py
+-rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/edgarxbrlframestocsv.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/sedfile
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.58/src/edgarquery/tickerd.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/__init__.py
+-rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/p.sh
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/s.sh
+-rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/x.sh
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.58/tests/y.sh
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.58/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.58/LICENSE.txt
+-rw-r--r--   0        0        0     8413 2020-02-02 00:00:00.000000 edgarquery-0.0.58/README.md
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 edgarquery-0.0.58/pyproject.toml
+-rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 edgarquery-0.0.58/PKG-INFO
```

### Comparing `edgarquery-0.0.57/genusage.sh` & `edgarquery-0.0.58/genusage.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/notes.txt` & `edgarquery-0.0.58/notes.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
   # SEC data resources
   https://www.sec.gov/sec-data-resources
 
   # SEC webmaster FAQ
   https://www.sec.gov/os/webmaster-faq
 
-  # contaiشs some generalaccess instructions
+  # contains some generalaccess instructions
   #     User-Agent rule
   #     contains urls for daily index and for full index
   #     shows some directory structure
   #     describes format for accession numbers CIK-YY-f#
   #     describes web browsing by CIK or accession number
   #     has links to risk analysis data
   https://www.sec.gov/os/accessing-edgar-data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edgarquery-0.0.57/scripts/edgarquery.py` & `edgarquery-0.0.58/scripts/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/ebquery.py` & `edgarquery-0.0.58/src/edgarquery/ebquery.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,22 +27,25 @@
         while True:
             try:
                 req = urllib.request.Request(url, headers=hdr)
                 resp = urllib.request.urlopen(req)
                 return resp
             except urllib.error.URLError as e:
                 print("Error %s(%s): %s" % ('query', url, e.reason),
-                file=sys.stderr )
+                              file=sys.stderr )
+                if e.reason == 'Not Found':
+                    return None
                 if tries < ntries:
-                    print('retrying in %d seconds' % pause)
+                    print('retrying in %d seconds' % (pause),
+                        file=sys.stderr)
                     time.sleep(pause)
                     tries = tries + 1
                     pause = pause * 2
                     continue
-                sys.exit(1)
+                #sys.exit(1)
 
     def storequery(self, qresp, file):
         """storequery(qresp, file) - store the query response in a file
 
         resp - the query response
         file   - filename that will hold the query response
         """
```

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarcikperson.py` & `edgarquery-0.0.58/src/edgarquery/edgarcikperson.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
         collect cik, name, and relationship from REPORTINGOWNER.tsv
         fznm - name of the form345.zip file
         fzpath - full path of where the file will be stored
         """
 
         url = '%s/%s' % (self.iturl, fznm)
         resp = self.uq.query(url, self.hdr)
+        if not resp:
+            return
         self.uq.storequery(resp, fzpath)
         # resp = self.query(url)
         # self.storequery(resp, fzpath)
         lge = self.form345zipfileiter(fzpath, 'REPORTINGOWNER.tsv')
         hdr = []
         for ln in lge:
             la =  re.split('\t', ln)
@@ -146,15 +148,15 @@
         for y in range(self.y0, self.y1):
             for q in (1,2,3,4):
                 fznm = '%dq%d_form345.zip' % (y,q)
                 print('processform345files %s' % (fznm), file=sys.stderr )
                 if y == now.year:
                     if now.month <=3: return
                     elif q == 1 and now.month <=3: return
-                    elif q == 2 and mpw.month <=6: return
+                    elif q == 2 and now.month <=6: return
                     elif q == 3 and now.month <=9: return
                     elif q == 4: return
                 self.collectform345owners(fznm, fznm)
         #self.reportcikpeople(fp)
 
 def main():
     CP = CIKPerson()
```

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarcompanyconcepttocsv.py` & `edgarquery-0.0.58/src/edgarquery/edgarcompanyconcepttocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarcompanyfactsshow.py` & `edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsshow.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarcompanyfactstocsv.py` & `edgarquery-0.0.58/src/edgarquery/edgarcompanyfactstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarcompanyfactsziptocsv.py` & `edgarquery-0.0.58/src/edgarquery/edgarcompanyfactsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarlatest10K.py` & `edgarquery-0.0.58/src/edgarquery/edgarlatest10K.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarlatestsubmissions.py` & `edgarquery-0.0.58/src/edgarquery/edgarlatestsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarquery.py` & `edgarquery-0.0.58/src/edgarquery/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarsubmissions.py` & `edgarquery-0.0.58/src/edgarquery/edgarsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarsubmissionsziptocsv.py` & `edgarquery-0.0.58/src/edgarquery/edgarsubmissionsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgartickerstocsv.py` & `edgarquery-0.0.58/src/edgarquery/edgartickerstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/edgarxbrlframestocsv.py` & `edgarquery-0.0.58/src/edgarquery/edgarxbrlframestocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/src/edgarquery/tickerd.py` & `edgarquery-0.0.58/src/edgarquery/tickerd.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/tests/p.sh` & `edgarquery-0.0.58/tests/p.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/tests/x.sh` & `edgarquery-0.0.58/tests/x.sh`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 echo $EQDIR
 echo $EQODIR
 
 # big files
 # edgarquery --companyfactsarchivezip \
 #                                             --ticker amzn
 # edgarquery --submissionszip
-#edgarquery  --submissionszip
-#sleep 5
+edgarquery  --submissionszip
+sleep 5
 
 edgarsubmissionsziptocsv --zipfile $EQODIR/submissions.zip \
     --files CIK0000831001.json,CIK0001665650.json,CIK0000019617.json
 
 # SEC needs a user-agent
 curl --user-agent $EQEMAIL --output /private/tmp/sitemap.xml \
      https://www.sec.gov/Archives/edgar/daily-index/sitemap.xml
```

### Comparing `edgarquery-0.0.57/LICENSE.txt` & `edgarquery-0.0.58/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/README.md` & `edgarquery-0.0.58/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 ## edgarquery
 
 ## required environmental variable<br/>
 EQEMAIL - required by the SEC to download some of the files with curl.<br/>
           used as the user-agent in the url request by the scripts.<br/>
 
 These commands retrieve various data from SEC EDGAR. They use a<br/>
-CIK or Central Index Key to identify entities such as companies or<br/>
-insiders - company officers or large stock holders.<br/>
+CIK or Central Index Key or ticker symbol to identify entities<br/>
+such as companies or insiders - company officers or large stock holders.<br/>
+<br/>
 Use edgartickerstocsv and edgarcikperson to find CIKs by name<br/>
-or ticker and then use that CIK to gather the data of interest.<br/>
+or ticker and then use that CIK or ticker  to gather the data of interest.<br/>
 To display facts for a company aggregated by the SEC, invoke<br/>
 
 ## Usage
 
 <br/>
 ##<br/>
 ## edgarcikperson<br/>
```

### Comparing `edgarquery-0.0.57/pyproject.toml` & `edgarquery-0.0.58/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.57/PKG-INFO` & `edgarquery-0.0.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgarquery
-Version: 0.0.57
+Version: 0.0.58
 Summary: Downloads various SEC EDGAR files by CIK or ticker.  companyfactsshow displays company facts in your browser
 Project-URL: Documentation, https://github.com/dfwcnj/edgarquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/edgarquery/issues
 Project-URL: Source, https://github.com/dfwcnj/edgarquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -37,18 +37,19 @@
 ## edgarquery
 
 ## required environmental variable<br/>
 EQEMAIL - required by the SEC to download some of the files with curl.<br/>
           used as the user-agent in the url request by the scripts.<br/>
 
 These commands retrieve various data from SEC EDGAR. They use a<br/>
-CIK or Central Index Key to identify entities such as companies or<br/>
-insiders - company officers or large stock holders.<br/>
+CIK or Central Index Key or ticker symbol to identify entities<br/>
+such as companies or insiders - company officers or large stock holders.<br/>
+<br/>
 Use edgartickerstocsv and edgarcikperson to find CIKs by name<br/>
-or ticker and then use that CIK to gather the data of interest.<br/>
+or ticker and then use that CIK or ticker  to gather the data of interest.<br/>
 To display facts for a company aggregated by the SEC, invoke<br/>
 
 ## Usage
 
 <br/>
 ##<br/>
 ## edgarcikperson<br/>
```

