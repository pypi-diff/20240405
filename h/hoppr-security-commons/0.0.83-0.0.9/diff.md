# Comparing `tmp/hoppr_security_commons-0.0.83.tar.gz` & `tmp/hoppr_security_commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_security_commons-0.0.83.tar", max compression
+gzip compressed data, was "hoppr_security_commons-0.0.9.tar", max compression
```

## Comparing `hoppr_security_commons-0.0.83.tar` & `hoppr_security_commons-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1084 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/LICENSE.md
--rw-r--r--   0        0        0     1100 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/README.md
--rw-r--r--   0        0        0       94 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/py.typed
--rw-r--r--   0        0        0    12132 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/__init__.py
--rw-r--r--   0        0        0      851 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/models.py
--rw-r--r--   0        0        0        0 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/py.typed
--rw-r--r--   0        0        0      393 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/reporting.py
--rw-r--r--   0        0        0    13776 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/assets/vulnerabilities.css
--rw-r--r--   0        0        0    62408 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/package-lock.json
--rw-r--r--   0        0        0       56 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/package.json
--rw-r--r--   0        0        0      135 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/tailwind.config.js
--rw-r--r--   0        0        0     3241 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/vulnerabilities.html
--rw-r--r--   0        0        0       58 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/vulnerability.css
--rw-r--r--   0        0        0    10820 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/vulnerability_details.html
--rw-r--r--   0        0        0     6441 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/utils.py
--rw-r--r--   0        0        0     4336 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/vulnerability_combiner.py
--rw-r--r--   0        0        0     3945 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/hoppr_security_commons/vulnerability_scanner.py
--rw-r--r--   0        0        0     4641 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/pyproject.toml
--rw-r--r--   0        0        0      449 2024-04-05 02:06:30.000000 hoppr_security_commons-0.0.83/security_commons/__init__.py
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.83/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0      615 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/__init__.py
+-rw-r--r--   0        0        0     1100 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/__init__.py
+-rw-r--r--   0        0        0      814 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/models.py
+-rw-r--r--   0        0        0    12906 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/reporting.py
+-rw-r--r--   0        0        0    13776 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/assets/vulnerabilities.css
+-rw-r--r--   0        0        0    50446 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/package-lock.json
+-rw-r--r--   0        0        0       56 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/package.json
+-rw-r--r--   0        0        0      135 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/tailwind.config.js
+-rw-r--r--   0        0        0     3241 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerabilities.html
+-rw-r--r--   0        0        0       58 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerability.css
+-rw-r--r--   0        0        0    10820 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerability_details.html
+-rw-r--r--   0        0        0     7260 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/utils.py
+-rw-r--r--   0        0        0     5438 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/vulnerability_combiner.py
+-rw-r--r--   0        0        0     3688 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/vulnerability_scanner.py
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.9/setup.py
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.9/PKG-INFO
```

### Comparing `hoppr_security_commons-0.0.83/LICENSE.md` & `hoppr_security_commons-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/README.md` & `hoppr_security_commons-0.0.9/security_commons/common/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/__init__.py` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/reporting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Provides vulnerability reporting."""
+"""Provides vulnerability reporting"""
 # This file is part of hoppr-security-commons
 #
 # Licensed under the MIT License;
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://opensource.org/licenses/MIT
@@ -11,289 +11,311 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # Copyright (c) 2022 Lockheed Martin CorporationØ
-from __future__ import annotations
-
 import json
+import pkgutil
 import uuid
-
 from collections import defaultdict
 from pathlib import Path
-from typing import Any
+from typing import List, Optional
 
 import jinja2
 import typer
-
 from hoppr_cyclonedx_models.cyclonedx_1_4 import (
-    Advisory,
-    Affect,
     CyclonedxSoftwareBillOfMaterialsStandard as Bom_1_4,
-    Rating,
-    ScoreMethod,
-    Severity,
-    Vulnerability,
 )
+from hoppr_cyclonedx_models.cyclonedx_1_4 import Vulnerability, Affect, Rating, Advisory
 from packageurl import PackageURL
 from tabulate import tabulate
 
-from hoppr_security_commons.reporting.models import ReportFormat
+from security_commons.common.reporting.models import ReportFormat
 
 
 class Reporting:
-    """Generates reports in multiple formats from a list of vulnerabilities."""
+    """Generates reports in multiple formats from a list of vulnerabilities"""
 
     output_path: Path
     base_name: str
 
     def __init__(self, output_path: Path, base_name: str):
         self.output_path = output_path
         self.base_name = base_name
 
     def generate_vulnerability_reports(
         self,
-        formats: list[ReportFormat],
-        vulnerabilities: dict[str, list[Vulnerability] | None],
-        bom: Bom_1_4 | None = None,
+        formats: List[ReportFormat],
+        vulnerabilities: dict[str, Optional[list[Vulnerability]]],
+        bom: Optional[Bom_1_4] = None,
     ):
-        """Generates various vulnerability reports based on specified formats."""
-        flattened_vulnerabilties = self.__add_purl_as_bom_ref_and_flatten(vulnerabilities)
-
+        """Generates various vulnerability reports based on specified formats"""
+        flattened_vulnerabilties = self.__add_purl_as_bom_ref_and_flatten(
+            vulnerabilities
+        )
+        if ReportFormat.TABLE in formats:
+            findings = self.__get_fields_from_vulnerabilities(flattened_vulnerabilties)
+            typer.echo(
+                tabulate(
+                    findings,
+                    headers=["type", "name", "version", "id", "severity", "found by"],
+                )
+            )
         if ReportFormat.CYCLONE_DX in formats and bom is not None:
-            self.output_path.mkdir(parents=True, exist_ok=True)
             self.add_vulnerabilities_to_bom(bom, flattened_vulnerabilties)
-
-            (self.output_path / f"{Path(self.base_name).name}-enhanced.json").write_text(
-                bom.json(indent=2), encoding="utf-8"
-            )
-
-        if ReportFormat.GITLAB in formats:
-            self.generate_gitlab_vulnerability_report(flattened_vulnerabilties)
-
+            with open(
+                self.output_path / f"{self.base_name}-enhanced.json",
+                "w",
+                encoding="UTF-8",
+            ) as file:
+                file.write(bom.json(exclude_none=True, by_alias=True))
+                file.close()
         if ReportFormat.HTML in formats:
             self.__generate_html_report(flattened_vulnerabilties)
 
-        if ReportFormat.TABLE in formats:
-            findings = self.__get_fields_from_vulnerabilities(flattened_vulnerabilties)
-            typer.echo(tabulate(findings, headers=["type", "name", "version", "id", "severity", "found by"]))
+        if ReportFormat.GITLAB in formats:
+            self.generate_gitlab_vulnerability_report(flattened_vulnerabilties)
 
     @staticmethod
-    def add_vulnerabilities_to_bom(bom: Bom_1_4, vulnerabilities: list[Vulnerability]) -> Bom_1_4:
-        """Adds the vulnerabilities found by various scanners to cyclone 1.4+ compliant BOM."""
+    def add_vulnerabilities_to_bom(
+        bom: Bom_1_4, vulnerabilities: List[Vulnerability]
+    ) -> Bom_1_4:
+        """Adds the vulnerabilities found by various scanners to cyclone 1.4+ compliant BOM"""
         if isinstance(bom, Bom_1_4):
-            bom.vulnerabilities = vulnerabilities
+            bom.vulnerabilities = []
+            bom.vulnerabilities = bom.vulnerabilities + vulnerabilities
         else:
-            typer.echo("Cannot add vulnerabilities to a bom earlier than cyclone version 1.4")
-
+            typer.echo(
+                "Cannot add vulnerabilities to a bom earlier than cyclone version 1.4"
+            )
         return bom
 
     @staticmethod
-    def link_vulnerabilities_to_bom(vulnerabilities: list[Vulnerability]) -> Bom_1_4:
-        """Creates/Adds the vulnerabilities found by various scanners to cyclone 1.4+ compliant VEX BOM."""
+    def link_vulnerabilities_to_bom(vulnerabilities: List[Vulnerability]) -> Bom_1_4:
+        """Creates/Adds the vulnerabilities found by various scanners to cyclone 1.4+ compliant VEX BOM"""
         vex_bom = Bom_1_4(bomFormat="CycloneDX", specVersion="1.4", version=1)
         vex_bom.serialNumber = f"urn:uuid:{uuid.uuid4()}"
-        vex_bom.vulnerabilities = vulnerabilities
+        vex_bom.vulnerabilties = vulnerabilities
 
         return vex_bom
 
     def __add_purl_as_bom_ref_and_flatten(
-        self, vulnerabilities: dict[str, list[Vulnerability] | None]
-    ) -> list[Vulnerability]:
-        flattened_vulnerabilities: list[Vulnerability] = []
+        self, vulnerabilities: dict[str, Optional[list[Vulnerability]]]
+    ) -> List[Vulnerability]:
+        flattened_vulnerabilities: List[Vulnerability] = []
 
         for purl in vulnerabilities:
-            for vuln in vulnerabilities[purl] or []:
-                vuln.affects = vuln.affects or []
-                vuln.affects.append(Affect(ref=purl))
+            for vuln in vulnerabilities[purl]:
+                vuln.affects = [] if vuln.affects is None else vuln.affects
+                vuln.affects.append(Affect(**{"ref": purl}))
                 flattened_vulnerabilities.append(vuln)
 
         flattened_vulnerabilities.sort(key=self.get_score, reverse=True)
         return flattened_vulnerabilities
 
     def get_score(self, vuln_to_score: Vulnerability) -> float:
-        """Return best score of specified Vulnerability."""
         best_rating = self.__get_best_rating(vuln_to_score.ratings)
-
         if best_rating is None or best_rating.score is None:
             return 0.0
-
         return best_rating.score
 
-    def __get_fields_from_vulnerabilities(self, vulnerabilities: list[Vulnerability]) -> list[list[str | None]]:
+    def __get_fields_from_vulnerabilities(self, vulnerabilities: List[Vulnerability]):
         findings = []
 
-        def get_fields(vuln: Vulnerability) -> list[str | None]:
-            tools = [f"{tool.vendor} {tool.name}" for tool in vuln.tools or []]
+        def get_fields(vuln: Vulnerability) -> List:
+            tools = [] if vuln.tools is None else vuln.tools
+            tools = list(map(lambda x: f"{x.vendor} {x.name}", tools))
             severity = self.__get_severity(vuln.ratings)
-
             if severity == "critical":
                 severity = typer.style(severity, fg=typer.colors.RED)
             elif severity == "high":
                 severity = typer.style(severity, fg=typer.colors.BRIGHT_YELLOW)
-
-            if not vulnerability.affects:
-                return []
-
-            purl = PackageURL.from_string(vulnerability.affects[0].ref)
-
-            return [purl.type, purl.name, purl.version, vuln.id, severity, " | ".join(tools)]
+            purl = PackageURL.from_string(str(vulnerability.affects[0].ref.__root__))
+            return [
+                purl.type,
+                purl.name,
+                purl.version,
+                vuln.id,
+                severity,
+                " | ".join(tools),
+            ]
 
         for vulnerability in vulnerabilities:
             findings.append(get_fields(vulnerability))
 
         return findings
 
     def __copy_assets(self):
-        assets_dir = Path(__file__).parent / "templates" / "assets"
         assets = ["vulnerabilities.css"]
-
         output_path = self.output_path / "assets"
         output_path.mkdir(exist_ok=True, parents=True)
-
         for asset in assets:
-            template_data = (assets_dir / asset).read_text(encoding="utf-8")
-            (output_path / asset).write_text(template_data)
+            output_path = output_path / asset
+            template_data = pkgutil.get_data(
+                __name__, f"templates/assets/{asset}"
+            ).decode("utf-8")
+            with open(output_path, "w", encoding="utf-8") as out:
+                out.write(template_data)
+            out.close()
+
+    def __generate_html_report(self, combined_list: List[Vulnerability]):
+        output_path = self.output_path / f"{self.base_name}-vulnerabilities.html"
+        template_data = pkgutil.get_data(
+            __name__, "templates/vulnerabilities.html"
+        ).decode("utf-8")
 
-    def __generate_html_report(self, combined_list: list[Vulnerability]):
-        self.output_path.mkdir(parents=True, exist_ok=True)
-        output_path = self.output_path / f"{Path(self.base_name).name}-vulnerabilities.html"
-
-        env = jinja2.Environment(loader=jinja2.FileSystemLoader(Path(__file__).parent / "templates"))
+        env = jinja2.Environment()
         env.filters["severity"] = self.__get_severity
-        template = env.get_template("vulnerabilities.html")
+        template = env.from_string(template_data)
+        # template = Template(template_data)
 
         self.__copy_assets()
 
         severity_classes = {
             "critical": "bg-red-100 rounded-lg py-5 px-6 mb-4 text-base text-red-700 mb-3",
             "high": "bg-yellow-100 rounded-lg py-5 px-6 mb-4 text-base text-yellow-700 mb-3",
             "medium": "bg-gray-50 rounded-lg py-5 px-6 mb-4 text-base text-gray-500 mb-3",
             "info": "bg-gray-50 rounded-lg py-5 px-6 mb-4 text-base text-gray-500 mb-3",
             "low": "bg-gray-50 rounded-lg py-5 px-6 mb-4 text-base text-gray-500 mb-3",
             "unknown": "bg-gray-50 rounded-lg py-5 px-6 mb-4 text-base text-gray-500 mb-3",
             "none": "bg-gray-50 rounded-lg py-5 px-6 mb-4 text-base text-gray-500 mb-3",
         }
 
         result = template.render(
-            {"findings": combined_list, "severity_classes": severity_classes, "base_name": self.base_name},
+            {
+                "findings": combined_list,
+                "severity_classes": severity_classes,
+                "base_name": self.base_name,
+            }
         )
-
-        output_path.write_text(result, encoding="utf-8")
-
+        with open(output_path, "w", encoding="utf-8") as out:
+            out.write(result)
+            out.close()
         self.__generate_vuln_detail_reports(combined_list, severity_classes)
 
-    def __generate_vuln_detail_reports(self, vulnerabilities: list[Vulnerability], severity_classes: dict[str, str]):
-        output_path = self.output_path / f"{Path(self.base_name).name}-details"
-        env = jinja2.Environment(loader=jinja2.FileSystemLoader(Path(__file__).parent / "templates"))
+    def __generate_vuln_detail_reports(
+        self, vulnerabilities: List[Vulnerability], severity_classes
+    ):
+        output_path = self.output_path / f"{self.base_name}-details"
+        output_path.mkdir(exist_ok=True)
+        template_data = pkgutil.get_data(
+            __name__, "templates/vulnerability_details.html"
+        ).decode("utf-8")
+        env = jinja2.Environment()
         env.filters["featured_link"] = self.__get_featured_link
-        template = env.get_template("vulnerability_details.html")
-
+        template = env.from_string(template_data)
         for vuln in vulnerabilities:
-            if not vuln.affects:
-                continue
-
-            purl = PackageURL.from_string(vuln.affects[0].ref)
+            purl = PackageURL.from_string(str(vuln.affects[0].ref.__root__))
             result = template.render(
                 {
                     "type": purl.type,
                     "namespace": purl.namespace,
                     "name": purl.name,
                     "version": purl.version,
                     "severity_classes": severity_classes,
                     "vulnerability": vuln,
                     "purl": purl.to_string(),
                     "base_name": self.base_name,
-                },
+                }
             )
+            file_name = output_path / f"{vuln.id}.html"
+            with open(file_name, "w", encoding="utf-8") as out:
+                out.write(result)
+                out.close()
 
-            (output_path / f"{vuln.id}.html").write_text(result, encoding="utf-8")
-
-    def generate_gitlab_vulnerability_report(self, vulnerabilities: list[Vulnerability]):
-        """Renders the vulnerabilities report for gitlab."""
+    def generate_gitlab_vulnerability_report(
+        self, vulnerabilities: List[Vulnerability]
+    ):
+        """Renders the vulnerabilities report for gitlab"""
         # Note the JSON schema for this report can be found at
         # https://gitlab.com/gitlab-org/security-products/security-report-schemas/-/blob/master/dist/dependency-scanning-report-format.json
-        report: dict[str, Any] = {
+        report = {
             "version": "14.1.2",
             "vulnerabilities": [],
             "remediations": [],
             "dependency_files": [],
         }
-
-        dependencies_by_format: dict[str, list[Any]] = defaultdict(list, {})
-
-        purls = list({vuln.affects[0].ref for vuln in vulnerabilities if vuln.affects})
-
-        self.output_path.mkdir(parents=True, exist_ok=True)
+        dependencies_by_format = defaultdict(lambda: [], {})
+        purls = list(
+            set(map(lambda x: str(x.affects[0].ref.__root__), vulnerabilities))
+        )
         output_path = self.output_path / "gl-dependency-scanning-report.json"
-
-        for purl_str in purls:
-            purl = PackageURL.from_string(purl_str)
-            dependencies_by_format[purl.type].append({"package": {"name": purl.name}, "version": purl.version})
+        for purl in purls:
+            purl = PackageURL.from_string(purl)
+            dependencies_by_format[purl.type].append(
+                {
+                    "package": {"name": purl.name},
+                    "version": purl.version,
+                }
+            )
 
         for vuln in vulnerabilities:
             report["vulnerabilities"].append(self.__generate_gitlab_row(vuln))
 
         for repo_format in dependencies_by_format:
             report["dependency_files"].append(
                 {
                     "package_manager": repo_format,
                     "path": "cyclonedx.bom",
                     "dependencies": dependencies_by_format[repo_format],
-                },
+                }
             )
 
-        output_path.write_text(json.dumps(report, indent=4, sort_keys=True, default=str), encoding="utf-8")
+        with open(output_path, "w", encoding="utf-8") as out:
+            out.write(json.dumps(report, indent=4, sort_keys=True, default=str))
+            out.close()
 
     @staticmethod
-    def __get_featured_link(advisories: list[Advisory] | None) -> str | None:
+    def __get_featured_link(advisories: Optional[List[Advisory]]) -> Optional[str]:
         if advisories is not None:
             for adv in advisories:
                 url = "" if adv.url is None else adv.url
                 if "https://snyk.io/" in url:
                     return url
         return None
 
-    def __get_severity(self, ratings: list[Rating] | None) -> str:
+    def __get_severity(self, ratings: Optional[List[Rating]]) -> str:
         best_rating = self.__get_best_rating(ratings)
         if best_rating is None or best_rating.severity is None:
             return "none"
 
-        return Severity(best_rating.severity).value
+        return str(best_rating.severity.value)
 
     @staticmethod
-    def __get_best_rating(ratings: list[Rating] | None) -> Rating | None:
-        default_rating = ratings[0] if ratings else None
-
-        methods = [ScoreMethod(rating.method).value if rating.method else "none" for rating in ratings or []]
-
+    def __get_best_rating(ratings: Optional[List[Rating]]):
+        default_rating = None if ratings is None or len(ratings) == 0 else ratings[0]
+        methods = list(
+            map(
+                lambda x: str(x.method.value) if x.method is not None else "none",
+                ratings,
+            )
+        )
         preferred_method = None
         if "CVSSv31" in methods:
             preferred_method = "CVSSv31"
         elif "CVSSv3" in methods:
             preferred_method = "CVSSv3"
         elif "CVSSv2" in methods:
             preferred_method = "CVSSv2"
 
-        return next(
-            filter(lambda rating: rating.method and (str(rating.method) == preferred_method), ratings or []),
-            default_rating,
-        )
-
-    def __generate_gitlab_row(self, vuln: Vulnerability) -> dict[str, Any] | None:
-        """Generates a report row."""
-        # Ensure `affects` and `tools` are non-empty lists
-        if not vuln.affects or not vuln.tools:
-            return None
-
-        purl = PackageURL.from_string(vuln.affects[0].ref)
+        for rating in ratings:
+            if (
+                rating.method is not None
+                and str(rating.method.value) == preferred_method
+                and preferred_method is not None
+            ):
+                return rating
+        return default_rating
+
+    def __generate_gitlab_row(self, vuln: Vulnerability):
+        """Generates a report row"""
+        purl = PackageURL.from_string(str(vuln.affects[0].ref.__root__))
         severity = self.__get_severity(vuln.ratings).title()
-
         return {
             "category": "dependency_scanning",
             "name": vuln.description,
             "description": vuln.description,
             "cve": vuln.id,
             "severity": severity if severity != "none" else "Info",
             "confidence": "Unknown",
```

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/models.py` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""The available reporting formats."""
+"""The available reporting formats"""
 # This file is part of hoppr-cop
 #
 # Licensed under the MIT License;
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://opensource.org/licenses/MIT
@@ -11,19 +11,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # Copyright (c) 2022 Lockheed Martin Corporation
-from __future__ import annotations
 
 from enum import Enum
 
 
 class ReportFormat(Enum):
-    """The available reporting formats."""
+    """The available reporting formats"""
 
     TABLE = "table"
     HTML = "html"
     CYCLONE_DX = "cyclone_dx"
     GITLAB = "gitlab"
```

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/assets/vulnerabilities.css` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/assets/vulnerabilities.css`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/package-lock.json` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/package-lock.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8120807312639094%*

 * *Differences: {"'dependencies'": "{'fast-glob': {'version': '3.2.11', 'resolved': "*

 * *                   "'https://nexus.global.lmco.com/repository/npm-proxy/fast-glob/-/fast-glob-3.2.11.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-xrO3+1bxSo3ZVHAnqzyuewYT6aMFHRAd4Kcs92MAonjwQZLsK9d0SF1IyQ3k5PoirxTW0Oe/RqFgMQ6TcNE5Ew=='}, "*

 * *                   "'function-bind': {'resolved': "*

 * *                   "'https://nexus.global.lmco.com/repository/npm-proxy/function-bind/-/function-bind-1.1.1.tgz'}, "*

 * *        […]*

```diff
@@ -1,55 +1,9 @@
 {
     "dependencies": {
-        "@alloc/quick-lru": {
-            "integrity": "sha512-UrcABB+4bUrFABwbluTIBErXwvbsU/V7TZWfmbgJfbkwiBuziS9gxdODUyuiecfdGQ85jglMW6juS3+z5TsKLw==",
-            "resolved": "https://registry.npmjs.org/@alloc/quick-lru/-/quick-lru-5.2.0.tgz",
-            "version": "5.2.0"
-        },
-        "@jridgewell/gen-mapping": {
-            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
-            "requires": {
-                "@jridgewell/set-array": "^1.0.1",
-                "@jridgewell/sourcemap-codec": "^1.4.10",
-                "@jridgewell/trace-mapping": "^0.3.9"
-            },
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
-            "version": "0.3.3"
-        },
-        "@jridgewell/resolve-uri": {
-            "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz",
-            "version": "3.1.0"
-        },
-        "@jridgewell/set-array": {
-            "integrity": "sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.2.tgz",
-            "version": "1.1.2"
-        },
-        "@jridgewell/sourcemap-codec": {
-            "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz",
-            "version": "1.4.15"
-        },
-        "@jridgewell/trace-mapping": {
-            "dependencies": {
-                "@jridgewell/sourcemap-codec": {
-                    "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
-                    "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
-                    "version": "1.4.14"
-                }
-            },
-            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
-            "requires": {
-                "@jridgewell/resolve-uri": "3.1.0",
-                "@jridgewell/sourcemap-codec": "1.4.14"
-            },
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
-            "version": "0.3.18"
-        },
         "@nodelib/fs.scandir": {
             "integrity": "sha512-vq24Bq3ym5HEQm2NKCr3yXDwjc7vTsEThRDnkp2DK9p1uqLR+DHurm/NOTo0KG7HYHU7eppKZj3MyqYuMBf62g==",
             "requires": {
                 "@nodelib/fs.stat": "2.0.5",
                 "run-parallel": "^1.1.9"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/@nodelib/fs.scandir/-/fs.scandir-2.1.5.tgz",
@@ -65,18 +19,33 @@
             "requires": {
                 "@nodelib/fs.scandir": "2.1.5",
                 "fastq": "^1.6.0"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/@nodelib/fs.walk/-/fs.walk-1.2.8.tgz",
             "version": "1.2.8"
         },
-        "any-promise": {
-            "integrity": "sha512-7UvmKalWRt1wgjL1RrGxoSJW/0QZFIegpeGvZG9kjp8vrRu55XTHbwnqq2GpXm9uLbcuhxm3IqX9OB4MZR1b2A==",
-            "resolved": "https://registry.npmjs.org/any-promise/-/any-promise-1.3.0.tgz",
-            "version": "1.3.0"
+        "acorn": {
+            "integrity": "sha512-nQyp0o1/mNdbTO1PO6kHkwSrmgZ0MT/jCCpNiwbUjGoRN4dlBhqJtoQuCnEOKzgTVwg0ZWiCoQy6SxMebQVh8A==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/acorn/-/acorn-7.4.1.tgz",
+            "version": "7.4.1"
+        },
+        "acorn-node": {
+            "integrity": "sha512-8mt+fslDufLYntIoPAaIMUe/lrbrehIiwmR3t2k9LljIzoigEPF27eLk2hy8zSGzmR/ogr7zbRKINMo1u0yh5A==",
+            "requires": {
+                "acorn": "^7.0.0",
+                "acorn-walk": "^7.0.0",
+                "xtend": "^4.0.2"
+            },
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/acorn-node/-/acorn-node-1.8.2.tgz",
+            "version": "1.8.2"
+        },
+        "acorn-walk": {
+            "integrity": "sha512-OPdCF6GsMIP+Az+aWfAAOEt2/+iVDKE7oy6lJ098aoe59oAmK76qV6Gw60SbZ8jHuG2wH058GF4pLFbYamYrVA==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/acorn-walk/-/acorn-walk-7.2.0.tgz",
+            "version": "7.2.0"
         },
         "anymatch": {
             "integrity": "sha512-P43ePfOAIupkguHUycrc4qJ9kz8ZiuOUijaETwX7THt0Y/GNK7v0aa8rY816xWjZ7rJdA5XdMcpVFTKMq+RvWg==",
             "requires": {
                 "normalize-path": "^3.0.0",
                 "picomatch": "^2.0.4"
             },
@@ -84,33 +53,19 @@
             "version": "3.1.2"
         },
         "arg": {
             "integrity": "sha512-PYjyFOLKQ9y57JvQ6QLo8dAgNqswh8M1RMJYdQduT6xbWSgK36P/Z/v+p888pM69jMMfS8Xd8F6I1kQ/I9HUGg==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/arg/-/arg-5.0.2.tgz",
             "version": "5.0.2"
         },
-        "balanced-match": {
-            "integrity": "sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==",
-            "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "binary-extensions": {
             "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/binary-extensions/-/binary-extensions-2.2.0.tgz",
             "version": "2.2.0"
         },
-        "brace-expansion": {
-            "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
-            "requires": {
-                "balanced-match": "^1.0.0",
-                "concat-map": "0.0.1"
-            },
-            "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-1.1.11.tgz",
-            "version": "1.1.11"
-        },
         "braces": {
             "integrity": "sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==",
             "requires": {
                 "fill-range": "^7.0.1"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/braces/-/braces-3.0.2.tgz",
             "version": "3.0.2"
@@ -141,29 +96,39 @@
                 "is-glob": "~4.0.1",
                 "normalize-path": "~3.0.0",
                 "readdirp": "~3.6.0"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/chokidar/-/chokidar-3.5.3.tgz",
             "version": "3.5.3"
         },
-        "commander": {
-            "integrity": "sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==",
-            "resolved": "https://registry.npmjs.org/commander/-/commander-4.1.1.tgz",
-            "version": "4.1.1"
-        },
-        "concat-map": {
-            "integrity": "sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==",
-            "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
-            "version": "0.0.1"
+        "color-name": {
+            "integrity": "sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/color-name/-/color-name-1.1.4.tgz",
+            "version": "1.1.4"
         },
         "cssesc": {
             "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/cssesc/-/cssesc-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "defined": {
+            "integrity": "sha512-Y2caI5+ZwS5c3RiNDJ6u53VhQHv+hHKwhkI1iHvceKUHw9Df6EK2zRLfjejRgMuCuxK7PfSWIMwWecceVvThjQ==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/defined/-/defined-1.0.0.tgz",
+            "version": "1.0.0"
+        },
+        "detective": {
+            "integrity": "sha512-v9XE1zRnz1wRtgurGu0Bs8uHKFSTdteYZNbIPFVhUZ39L/S79ppMpdmVOZAnoz1jfEFodc48n6MX483Xo3t1yw==",
+            "requires": {
+                "acorn-node": "^1.8.2",
+                "defined": "^1.0.0",
+                "minimist": "^1.2.6"
+            },
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/detective/-/detective-5.2.1.tgz",
+            "version": "5.2.1"
+        },
         "didyoumean": {
             "integrity": "sha512-gxtyfqMg7GKyhQmb056K7M3xszy/myH8w+B4RT+QXBQsvAOdc3XymqDDPHx1BgPgsdAA5SIifona89YtRATDzw==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/didyoumean/-/didyoumean-1.2.2.tgz",
             "version": "1.2.2"
         },
         "dlv": {
             "integrity": "sha512-+HlytyjlPKnIG8XuRG8WvmBP8xs8P71y+SKKS6ZXWoEgLuePxtDoUEiH7WkdePWrQ5JBpE6aoVqfZfJUQkjXwA==",
@@ -177,24 +142,24 @@
                     "requires": {
                         "is-glob": "^4.0.1"
                     },
                     "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/glob-parent/-/glob-parent-5.1.2.tgz",
                     "version": "5.1.2"
                 }
             },
-            "integrity": "sha512-kNFPyjhh5cKjrUltxs+wFx+ZkbRaxxmZ+X0ZU31SOsxCEtP9VPgtq2teZw1DebupL5GmDaNQ6yKMMVcM41iqDg==",
+            "integrity": "sha512-xrO3+1bxSo3ZVHAnqzyuewYT6aMFHRAd4Kcs92MAonjwQZLsK9d0SF1IyQ3k5PoirxTW0Oe/RqFgMQ6TcNE5Ew==",
             "requires": {
                 "@nodelib/fs.stat": "^2.0.2",
                 "@nodelib/fs.walk": "^1.2.3",
                 "glob-parent": "^5.1.2",
                 "merge2": "^1.3.0",
                 "micromatch": "^4.0.4"
             },
-            "resolved": "https://registry.npmjs.org/fast-glob/-/fast-glob-3.3.1.tgz",
-            "version": "3.3.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fast-glob/-/fast-glob-3.2.11.tgz",
+            "version": "3.2.11"
         },
         "fastq": {
             "integrity": "sha512-YpkpUnK8od0o1hmeSc7UUs/eB/vIPWJYjKck2QKIzAf71Vm1AAQ3EbuZB3g2JIy+pg+ERD0vqI79KyZiB2e2Nw==",
             "requires": {
                 "reusify": "^1.0.4"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fastq/-/fastq-1.13.0.tgz",
@@ -204,88 +169,56 @@
             "integrity": "sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==",
             "requires": {
                 "to-regex-range": "^5.0.1"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fill-range/-/fill-range-7.0.1.tgz",
             "version": "7.0.1"
         },
-        "fs.realpath": {
-            "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
-            "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "fsevents": {
             "integrity": "sha512-xiqMQR4xAeHTuB9uWm+fFRcIOgKBMiOBP+eXiyT7jsgVCq1bkVygt00oASowB7EdtpOHaaPgKt812P9ab+DDKA==",
             "optional": true,
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fsevents/-/fsevents-2.3.2.tgz",
             "version": "2.3.2"
         },
         "function-bind": {
             "integrity": "sha512-yIovAzMX49sF8Yl58fSCWJ5svSLuaibPxXQJFLmBObTuCr0Mf1KiPopGM9NiFjiYBCbfaa2Fh6breQ6ANVTI0A==",
-            "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/function-bind/-/function-bind-1.1.1.tgz",
             "version": "1.1.1"
         },
-        "glob": {
-            "integrity": "sha512-LwaxwyZ72Lk7vZINtNNrywX0ZuLyStrdDtabefZKAY5ZGJhVtgdznluResxNmPitE0SAO+O26sWTHeKSI2wMBA==",
-            "requires": {
-                "fs.realpath": "^1.0.0",
-                "inflight": "^1.0.4",
-                "inherits": "2",
-                "minimatch": "^3.0.4",
-                "once": "^1.3.0",
-                "path-is-absolute": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/glob/-/glob-7.1.6.tgz",
-            "version": "7.1.6"
-        },
         "glob-parent": {
             "integrity": "sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==",
             "requires": {
                 "is-glob": "^4.0.3"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/glob-parent/-/glob-parent-6.0.2.tgz",
             "version": "6.0.2"
         },
         "has": {
             "integrity": "sha512-f2dvO0VU6Oej7RkWJGrehjbzMAjFp5/VKPp5tTpWIV4JHHZK1/BxbFRtf/siA2SWTe09caDmVtYYzWEIbBS4zw==",
             "requires": {
                 "function-bind": "^1.1.1"
             },
-            "resolved": "https://registry.npmjs.org/has/-/has-1.0.3.tgz",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/has/-/has-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "inflight": {
-            "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
-            "requires": {
-                "once": "^1.3.0",
-                "wrappy": "1"
-            },
-            "resolved": "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz",
-            "version": "1.0.6"
-        },
-        "inherits": {
-            "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
-            "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
-            "version": "2.0.4"
-        },
         "is-binary-path": {
             "integrity": "sha512-ZMERYes6pDydyuGidse7OsHxtbI7WVeUEozgR/g7rd0xUimYNlvZRE/K2MgZTjWy725IfelLeVcEM97mmtRGXw==",
             "requires": {
                 "binary-extensions": "^2.0.0"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/is-binary-path/-/is-binary-path-2.1.0.tgz",
             "version": "2.1.0"
         },
         "is-core-module": {
-            "integrity": "sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==",
+            "integrity": "sha512-Erxj2n/LDAZ7H8WNJXd9tw38GYM3dv8rk8Zcs+jJuxYTW7sozH+SS8NtrSjVL1/vpLvWi1hxy96IzjJ3EHTJJg==",
             "requires": {
                 "has": "^1.0.3"
             },
-            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.0.tgz",
-            "version": "2.12.0"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/is-core-module/-/is-core-module-2.10.0.tgz",
+            "version": "2.10.0"
         },
         "is-extglob": {
             "integrity": "sha1-qIwCU1eR8C7TfHahueqXc8gz+MI=",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/is-extglob/-/is-extglob-2.1.1.tgz",
             "version": "2.1.1"
         },
         "is-glob": {
@@ -297,28 +230,18 @@
             "version": "4.0.3"
         },
         "is-number": {
             "integrity": "sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/is-number/-/is-number-7.0.0.tgz",
             "version": "7.0.0"
         },
-        "jiti": {
-            "integrity": "sha512-gFqAIbuKyyso/3G2qhiO2OM6shY6EPP/R0+mkDbyspxKazh8BXDC5FiFsUjlczgdNz/vfra0da2y+aHrusLG/Q==",
-            "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.21.0.tgz",
-            "version": "1.21.0"
-        },
         "lilconfig": {
-            "integrity": "sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==",
-            "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-2.1.0.tgz",
-            "version": "2.1.0"
-        },
-        "lines-and-columns": {
-            "integrity": "sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==",
-            "resolved": "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz",
-            "version": "1.2.4"
+            "integrity": "sha512-9JROoBW7pobfsx+Sq2JsASvCo6Pfo6WWoUW79HuB1BCoBXD4PLWJPqDF6fNj67pqBYTbAHkE57M1kS/+L1neOg==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/lilconfig/-/lilconfig-2.0.6.tgz",
+            "version": "2.0.6"
         },
         "merge2": {
             "integrity": "sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/merge2/-/merge2-1.4.1.tgz",
             "version": "1.4.1"
         },
         "micromatch": {
@@ -326,65 +249,34 @@
             "requires": {
                 "braces": "^3.0.2",
                 "picomatch": "^2.3.1"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/micromatch/-/micromatch-4.0.5.tgz",
             "version": "4.0.5"
         },
-        "minimatch": {
-            "integrity": "sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==",
-            "requires": {
-                "brace-expansion": "^1.1.7"
-            },
-            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz",
-            "version": "3.1.2"
-        },
-        "mz": {
-            "integrity": "sha512-z81GNO7nnYMEhrGh9LeymoE4+Yr0Wn5McHIZMK5cfQCl+NDX08sCZgUc9/6MHni9IWuFLm1Z3HTCXu2z9fN62Q==",
-            "requires": {
-                "any-promise": "^1.0.0",
-                "object-assign": "^4.0.1",
-                "thenify-all": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/mz/-/mz-2.7.0.tgz",
-            "version": "2.7.0"
+        "minimist": {
+            "integrity": "sha512-Jsjnk4bw3YJqYzbdyBiNsPWHPfO++UGG749Cxs6peCu5Xg4nrena6OVxOYxrQTqww0Jmwt+Ref8rggumkTLz9Q==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/minimist/-/minimist-1.2.6.tgz",
+            "version": "1.2.6"
         },
         "nanoid": {
-            "integrity": "sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.6.tgz",
-            "version": "3.3.6"
+            "integrity": "sha512-MqBkQh/OHTS2egovRtLk45wEyNXwF+cokD+1YPf9u5VfJiRdAiRwB2froX5Co9Rh20xs4siNPm8naNotSD6RBw==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/nanoid/-/nanoid-3.3.4.tgz",
+            "version": "3.3.4"
         },
         "normalize-path": {
             "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/normalize-path/-/normalize-path-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "object-assign": {
-            "integrity": "sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==",
-            "resolved": "https://registry.npmjs.org/object-assign/-/object-assign-4.1.1.tgz",
-            "version": "4.1.1"
-        },
         "object-hash": {
             "integrity": "sha512-RSn9F68PjH9HqtltsSnqYC1XXoWe9Bju5+213R98cNGttag9q9yAOTzdbsqvIa7aNm5WffBZFpWYr2aWrklWAw==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/object-hash/-/object-hash-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "once": {
-            "integrity": "sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==",
-            "requires": {
-                "wrappy": "1"
-            },
-            "resolved": "https://registry.npmjs.org/once/-/once-1.4.0.tgz",
-            "version": "1.4.0"
-        },
-        "path-is-absolute": {
-            "integrity": "sha512-AVbw3UJ2e9bq64vSaS9Am0fje1Pa8pbGqTTsmXfaIiMpnr5DlDhfJOuLj9Sf95ZPVDAUerDfEk88MPmPe7UCQg==",
-            "resolved": "https://registry.npmjs.org/path-is-absolute/-/path-is-absolute-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "path-parse": {
             "integrity": "sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/path-parse/-/path-parse-1.0.7.tgz",
             "version": "1.0.7"
         },
         "picocolors": {
             "integrity": "sha512-1fygroTLlHu66zi26VoTDv8yRgm0Fccecssto+MhsZ0D/DGW2sm8E8AjW7NU5VVTRt5GxbeZ5qBuJr+HyLYkjQ==",
@@ -397,83 +289,83 @@
             "version": "2.3.1"
         },
         "pify": {
             "integrity": "sha512-udgsAY+fTnvv7kI7aaxbqwWNb0AHiB0qBO89PZKPkoTmGOgdbrHDKD+0B2X4uTfJ/FT1R09r9gTsjUjNJotuog==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/pify/-/pify-2.3.0.tgz",
             "version": "2.3.0"
         },
-        "pirates": {
-            "integrity": "sha512-8V9+HQPupnaXMA23c5hvl69zXvTwTzyAYasnkb0Tts4XvO4CliqONMOnvlq26rkhLC3nWDFBJf73LU1e1VZLaQ==",
-            "resolved": "https://registry.npmjs.org/pirates/-/pirates-4.0.5.tgz",
-            "version": "4.0.5"
-        },
         "postcss": {
-            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
+            "integrity": "sha512-ipHE1XBvKzm5xI7hiHCZJCSugxvsdq2mPnsq5+UF+VHCjiBvtDrlxJfMBToWaP9D5XlgNmcFGqoHmUn0EYEaRQ==",
             "requires": {
-                "nanoid": "^3.3.6",
+                "nanoid": "^3.3.4",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
-            "version": "8.4.23"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss/-/postcss-8.4.16.tgz",
+            "version": "8.4.16"
         },
         "postcss-import": {
-            "integrity": "sha512-hpr+J05B2FVYUAXHeK1YyI267J/dDDhMU6B6civm8hSY1jYJnBXxzKDKDswzJmtLHryrjhnDjqqp/49t8FALew==",
+            "integrity": "sha512-flwI+Vgm4SElObFVPpTIT7SU7R3qk2L7PyduMcokiaVKuWv9d/U+Gm/QAd8NDLuykTWTkcrjOeD2Pp1rMeBTGw==",
             "requires": {
                 "postcss-value-parser": "^4.0.0",
                 "read-cache": "^1.0.0",
                 "resolve": "^1.1.7"
             },
-            "resolved": "https://registry.npmjs.org/postcss-import/-/postcss-import-15.1.0.tgz",
-            "version": "15.1.0"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-import/-/postcss-import-14.1.0.tgz",
+            "version": "14.1.0"
         },
         "postcss-js": {
-            "integrity": "sha512-dDLF8pEO191hJMtlHFPRa8xsizHaM82MLfNkUHdUtVEV3tgTp5oj+8qbEqYM57SLfc74KSbw//4SeJma2LRVIw==",
+            "integrity": "sha512-77QESFBwgX4irogGVPgQ5s07vLvFqWr228qZY+w6lW599cRlK/HmnlivnnVUxkjHnCu4J16PDMHcH+e+2HbvTQ==",
             "requires": {
                 "camelcase-css": "^2.0.1"
             },
-            "resolved": "https://registry.npmjs.org/postcss-js/-/postcss-js-4.0.1.tgz",
-            "version": "4.0.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-js/-/postcss-js-4.0.0.tgz",
+            "version": "4.0.0"
         },
         "postcss-load-config": {
-            "integrity": "sha512-vEJIc8RdiBRu3oRAI0ymerOn+7rPuMvRXslTvZUKZonDHFIczxztIyJ1urxM1x9JXEikvpWWTUUqal5j/8QgvA==",
+            "integrity": "sha512-6DiM4E7v4coTE4uzA8U//WhtPwyhiim3eyjEMFCnUpzbrkK9wJHgKDT2mR+HbtSrd/NubVaYTOpSpjUl8NQeRg==",
             "requires": {
                 "lilconfig": "^2.0.5",
-                "yaml": "^2.1.1"
+                "yaml": "^1.10.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss-load-config/-/postcss-load-config-4.0.1.tgz",
-            "version": "4.0.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-load-config/-/postcss-load-config-3.1.4.tgz",
+            "version": "3.1.4"
         },
         "postcss-nested": {
-            "integrity": "sha512-mEp4xPMi5bSWiMbsgoPfcP74lsWLHkQbZc3sY+jWYd65CUwXrUaTp0fmNpa01ZcETKlIgUdFN/MpS2xZtqL9dQ==",
+            "integrity": "sha512-rKqm2Fk0KbA8Vt3AdGN0FB9OBOMDVajMG6ZCf/GoHgdxUJ4sBFp0A/uMIRm+MJUdo33YXEtjqIz8u7DAp8B7DA==",
             "requires": {
-                "postcss-selector-parser": "^6.0.11"
+                "postcss-selector-parser": "^6.0.6"
             },
-            "resolved": "https://registry.npmjs.org/postcss-nested/-/postcss-nested-6.0.1.tgz",
-            "version": "6.0.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-nested/-/postcss-nested-5.0.6.tgz",
+            "version": "5.0.6"
         },
         "postcss-selector-parser": {
-            "integrity": "sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==",
+            "integrity": "sha512-IQ7TZdoaqbT+LCpShg46jnZVlhWD2w6iQYAcYXfHARZ7X1t/UGhhceQDs5X0cGqKvYlHNOuv7Oa1xmb0oQuA3w==",
             "requires": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.11.tgz",
-            "version": "6.0.11"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-selector-parser/-/postcss-selector-parser-6.0.10.tgz",
+            "version": "6.0.10"
         },
         "postcss-value-parser": {
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
         "queue-microtask": {
             "integrity": "sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/queue-microtask/-/queue-microtask-1.2.3.tgz",
             "version": "1.2.3"
         },
+        "quick-lru": {
+            "integrity": "sha512-WuyALRjWPDGtt/wzJiadO5AXY+8hZ80hVpe6MyivgraREW751X3SbhRvG3eLKOYN+8VEvqLcf3wdnt44Z4S4SA==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/quick-lru/-/quick-lru-5.1.1.tgz",
+            "version": "5.1.1"
+        },
         "read-cache": {
             "integrity": "sha512-Owdv/Ft7IjOgm/i0xvNDZ1LrRANRfew4b2prF3OWMQLxLfu3bS8FVhCsrSCMK4lR56Y9ya+AThoTpDCTxCmpRA==",
             "requires": {
                 "pify": "^2.3.0"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/read-cache/-/read-cache-1.0.0.tgz",
             "version": "1.0.0"
@@ -483,22 +375,22 @@
             "requires": {
                 "picomatch": "^2.2.1"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/readdirp/-/readdirp-3.6.0.tgz",
             "version": "3.6.0"
         },
         "resolve": {
-            "integrity": "sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==",
+            "integrity": "sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==",
             "requires": {
-                "is-core-module": "^2.11.0",
+                "is-core-module": "^2.9.0",
                 "path-parse": "^1.0.7",
                 "supports-preserve-symlinks-flag": "^1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.2.tgz",
-            "version": "1.22.2"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/resolve/-/resolve-1.22.1.tgz",
+            "version": "1.22.1"
         },
         "reusify": {
             "integrity": "sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/reusify/-/reusify-1.0.4.tgz",
             "version": "1.0.4"
         },
         "run-parallel": {
@@ -510,174 +402,80 @@
             "version": "1.2.0"
         },
         "source-map-js": {
             "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/source-map-js/-/source-map-js-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "sucrase": {
-            "integrity": "sha512-ydQOU34rpSyj2TGyz4D2p8rbktIOZ8QY9s+DGLvFU1i5pWJE8vkpruCjGCMHsdXwnD7JDcS+noSwM/a7zyNFDQ==",
-            "requires": {
-                "@jridgewell/gen-mapping": "^0.3.2",
-                "commander": "^4.0.0",
-                "glob": "7.1.6",
-                "lines-and-columns": "^1.1.6",
-                "mz": "^2.7.0",
-                "pirates": "^4.0.1",
-                "ts-interface-checker": "^0.1.9"
-            },
-            "resolved": "https://registry.npmjs.org/sucrase/-/sucrase-3.32.0.tgz",
-            "version": "3.32.0"
-        },
         "supports-preserve-symlinks-flag": {
             "integrity": "sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/supports-preserve-symlinks-flag/-/supports-preserve-symlinks-flag-1.0.0.tgz",
             "version": "1.0.0"
         },
         "tailwindcss": {
-            "integrity": "sha512-U7sxQk/n397Bmx4JHbJx/iSOOv5G+II3f1kpLpY2QeUv5DcPdcTsYLlusZfq1NthHS1c1cZoyFmmkex1rzke0A==",
+            "integrity": "sha512-YSneUCZSFDYMwk+TGq8qYFdCA3yfBRdBlS7txSq0LUmzyeqRe3a8fBQzbz9M3WS/iFT4BNf/nmw9mEzrnSaC0g==",
             "requires": {
-                "@alloc/quick-lru": "^5.2.0",
                 "arg": "^5.0.2",
                 "chokidar": "^3.5.3",
+                "color-name": "^1.1.4",
+                "detective": "^5.2.1",
                 "didyoumean": "^1.2.2",
                 "dlv": "^1.1.3",
-                "fast-glob": "^3.3.0",
+                "fast-glob": "^3.2.11",
                 "glob-parent": "^6.0.2",
                 "is-glob": "^4.0.3",
-                "jiti": "^1.21.0",
-                "lilconfig": "^2.1.0",
-                "micromatch": "^4.0.5",
+                "lilconfig": "^2.0.6",
                 "normalize-path": "^3.0.0",
                 "object-hash": "^3.0.0",
                 "picocolors": "^1.0.0",
-                "postcss": "^8.4.23",
-                "postcss-import": "^15.1.0",
-                "postcss-js": "^4.0.1",
-                "postcss-load-config": "^4.0.1",
-                "postcss-nested": "^6.0.1",
-                "postcss-selector-parser": "^6.0.11",
-                "resolve": "^1.22.2",
-                "sucrase": "^3.32.0"
-            },
-            "resolved": "https://registry.npmjs.org/tailwindcss/-/tailwindcss-3.4.3.tgz",
-            "version": "3.4.3"
-        },
-        "thenify": {
-            "integrity": "sha512-RVZSIV5IG10Hk3enotrhvz0T9em6cyHBLkH/YAZuKqd8hRkKhSfCGIcP2KUY0EPxndzANBmNllzWPwak+bheSw==",
-            "requires": {
-                "any-promise": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/thenify/-/thenify-3.3.1.tgz",
-            "version": "3.3.1"
-        },
-        "thenify-all": {
-            "integrity": "sha512-RNxQH/qI8/t3thXJDwcstUO4zeqo64+Uy/+sNVRBx4Xn2OX+OZ9oP+iJnNFqplFra2ZUVeKCSa2oVWi3T4uVmA==",
-            "requires": {
-                "thenify": ">= 3.1.0 < 4"
+                "postcss": "^8.4.14",
+                "postcss-import": "^14.1.0",
+                "postcss-js": "^4.0.0",
+                "postcss-load-config": "^3.1.4",
+                "postcss-nested": "5.0.6",
+                "postcss-selector-parser": "^6.0.10",
+                "postcss-value-parser": "^4.2.0",
+                "quick-lru": "^5.1.1",
+                "resolve": "^1.22.1"
             },
-            "resolved": "https://registry.npmjs.org/thenify-all/-/thenify-all-1.6.0.tgz",
-            "version": "1.6.0"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/tailwindcss/-/tailwindcss-3.1.8.tgz",
+            "version": "3.1.8"
         },
         "to-regex-range": {
             "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
             "requires": {
                 "is-number": "^7.0.0"
             },
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/to-regex-range/-/to-regex-range-5.0.1.tgz",
             "version": "5.0.1"
         },
-        "ts-interface-checker": {
-            "integrity": "sha512-Y/arvbn+rrz3JCKl9C4kVNfTfSm2/mEp5FSz5EsZSANGPSlQrpRI5M4PKF+mJnE52jOO90PnPSc3Ur3bTQw0gA==",
-            "resolved": "https://registry.npmjs.org/ts-interface-checker/-/ts-interface-checker-0.1.13.tgz",
-            "version": "0.1.13"
-        },
         "util-deprecate": {
             "integrity": "sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/util-deprecate/-/util-deprecate-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "wrappy": {
-            "integrity": "sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==",
-            "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
-            "version": "1.0.2"
+        "xtend": {
+            "integrity": "sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/xtend/-/xtend-4.0.2.tgz",
+            "version": "4.0.2"
         },
         "yaml": {
-            "integrity": "sha512-CBKFWExMn46Foo4cldiChEzn7S7SRV+wqiluAb6xmueD/fGyRHIhX8m14vVGgeFWjN540nKCNVj6P21eQjgTuA==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-2.2.2.tgz",
-            "version": "2.2.2"
+            "integrity": "sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/yaml/-/yaml-1.10.2.tgz",
+            "version": "1.10.2"
         }
     },
     "lockfileVersion": 2,
-    "name": "templates",
+    "name": "security-plugins",
     "packages": {
         "": {
             "dependencies": {
                 "tailwindcss": "^3.1.8"
             }
         },
-        "node_modules/@alloc/quick-lru": {
-            "engines": {
-                "node": ">=10"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/sindresorhus"
-            },
-            "integrity": "sha512-UrcABB+4bUrFABwbluTIBErXwvbsU/V7TZWfmbgJfbkwiBuziS9gxdODUyuiecfdGQ85jglMW6juS3+z5TsKLw==",
-            "resolved": "https://registry.npmjs.org/@alloc/quick-lru/-/quick-lru-5.2.0.tgz",
-            "version": "5.2.0"
-        },
-        "node_modules/@jridgewell/gen-mapping": {
-            "dependencies": {
-                "@jridgewell/set-array": "^1.0.1",
-                "@jridgewell/sourcemap-codec": "^1.4.10",
-                "@jridgewell/trace-mapping": "^0.3.9"
-            },
-            "engines": {
-                "node": ">=6.0.0"
-            },
-            "integrity": "sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/gen-mapping/-/gen-mapping-0.3.3.tgz",
-            "version": "0.3.3"
-        },
-        "node_modules/@jridgewell/resolve-uri": {
-            "engines": {
-                "node": ">=6.0.0"
-            },
-            "integrity": "sha512-F2msla3tad+Mfht5cJq7LSXcdudKTWCVYUgw6pLFOOHSTtZlj6SWNYAp+AhuqLmWdBO2X5hPrLcu8cVP8fy28w==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/resolve-uri/-/resolve-uri-3.1.0.tgz",
-            "version": "3.1.0"
-        },
-        "node_modules/@jridgewell/set-array": {
-            "engines": {
-                "node": ">=6.0.0"
-            },
-            "integrity": "sha512-xnkseuNADM0gt2bs+BvhO0p78Mk762YnZdsuzFV018NoG1Sj1SCQvpSqa7XUaTam5vAGasABV9qXASMKnFMwMw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/set-array/-/set-array-1.1.2.tgz",
-            "version": "1.1.2"
-        },
-        "node_modules/@jridgewell/sourcemap-codec": {
-            "integrity": "sha512-eF2rxCRulEKXHTRiDrDy6erMYWqNw4LPdQ8UQA4huuxaQsVeRPFl2oM8oDGxMFhJUWZf9McpLtJasDDZb/Bpeg==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.15.tgz",
-            "version": "1.4.15"
-        },
-        "node_modules/@jridgewell/trace-mapping": {
-            "dependencies": {
-                "@jridgewell/resolve-uri": "3.1.0",
-                "@jridgewell/sourcemap-codec": "1.4.14"
-            },
-            "integrity": "sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.18.tgz",
-            "version": "0.3.18"
-        },
-        "node_modules/@jridgewell/trace-mapping/node_modules/@jridgewell/sourcemap-codec": {
-            "integrity": "sha512-XPSJHWmi394fuUuzDnGz1wiKqWfo1yXecHQMRf2l6hztTO+nPru658AyDngaBe7isIxEkRsPR3FZh+s7iVa4Uw==",
-            "resolved": "https://registry.npmjs.org/@jridgewell/sourcemap-codec/-/sourcemap-codec-1.4.14.tgz",
-            "version": "1.4.14"
-        },
         "node_modules/@nodelib/fs.scandir": {
             "dependencies": {
                 "@nodelib/fs.stat": "2.0.5",
                 "run-parallel": "^1.1.9"
             },
             "engines": {
                 "node": ">= 8"
@@ -705,18 +503,45 @@
                 "node": ">= 8"
             },
             "integrity": "sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/@nodelib/fs.walk/-/fs.walk-1.2.8.tgz",
             "version": "1.2.8"
         },
-        "node_modules/any-promise": {
-            "integrity": "sha512-7UvmKalWRt1wgjL1RrGxoSJW/0QZFIegpeGvZG9kjp8vrRu55XTHbwnqq2GpXm9uLbcuhxm3IqX9OB4MZR1b2A==",
-            "resolved": "https://registry.npmjs.org/any-promise/-/any-promise-1.3.0.tgz",
-            "version": "1.3.0"
+        "node_modules/acorn": {
+            "bin": {
+                "acorn": "bin/acorn"
+            },
+            "engines": {
+                "node": ">=0.4.0"
+            },
+            "integrity": "sha512-nQyp0o1/mNdbTO1PO6kHkwSrmgZ0MT/jCCpNiwbUjGoRN4dlBhqJtoQuCnEOKzgTVwg0ZWiCoQy6SxMebQVh8A==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/acorn/-/acorn-7.4.1.tgz",
+            "version": "7.4.1"
+        },
+        "node_modules/acorn-node": {
+            "dependencies": {
+                "acorn": "^7.0.0",
+                "acorn-walk": "^7.0.0",
+                "xtend": "^4.0.2"
+            },
+            "integrity": "sha512-8mt+fslDufLYntIoPAaIMUe/lrbrehIiwmR3t2k9LljIzoigEPF27eLk2hy8zSGzmR/ogr7zbRKINMo1u0yh5A==",
+            "license": "Apache-2.0",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/acorn-node/-/acorn-node-1.8.2.tgz",
+            "version": "1.8.2"
+        },
+        "node_modules/acorn-walk": {
+            "engines": {
+                "node": ">=0.4.0"
+            },
+            "integrity": "sha512-OPdCF6GsMIP+Az+aWfAAOEt2/+iVDKE7oy6lJ098aoe59oAmK76qV6Gw60SbZ8jHuG2wH058GF4pLFbYamYrVA==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/acorn-walk/-/acorn-walk-7.2.0.tgz",
+            "version": "7.2.0"
         },
         "node_modules/anymatch": {
             "dependencies": {
                 "normalize-path": "^3.0.0",
                 "picomatch": "^2.0.4"
             },
             "engines": {
@@ -729,37 +554,23 @@
         },
         "node_modules/arg": {
             "integrity": "sha512-PYjyFOLKQ9y57JvQ6QLo8dAgNqswh8M1RMJYdQduT6xbWSgK36P/Z/v+p888pM69jMMfS8Xd8F6I1kQ/I9HUGg==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/arg/-/arg-5.0.2.tgz",
             "version": "5.0.2"
         },
-        "node_modules/balanced-match": {
-            "integrity": "sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==",
-            "resolved": "https://registry.npmjs.org/balanced-match/-/balanced-match-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "node_modules/binary-extensions": {
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/binary-extensions/-/binary-extensions-2.2.0.tgz",
             "version": "2.2.0"
         },
-        "node_modules/brace-expansion": {
-            "dependencies": {
-                "balanced-match": "^1.0.0",
-                "concat-map": "0.0.1"
-            },
-            "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
-            "resolved": "https://registry.npmjs.org/brace-expansion/-/brace-expansion-1.1.11.tgz",
-            "version": "1.1.11"
-        },
         "node_modules/braces": {
             "dependencies": {
                 "fill-range": "^7.0.1"
             },
             "engines": {
                 "node": ">=8"
             },
@@ -812,39 +623,55 @@
                 "node": ">= 6"
             },
             "integrity": "sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==",
             "license": "ISC",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/glob-parent/-/glob-parent-5.1.2.tgz",
             "version": "5.1.2"
         },
-        "node_modules/commander": {
-            "engines": {
-                "node": ">= 6"
-            },
-            "integrity": "sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==",
-            "resolved": "https://registry.npmjs.org/commander/-/commander-4.1.1.tgz",
-            "version": "4.1.1"
-        },
-        "node_modules/concat-map": {
-            "integrity": "sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==",
-            "resolved": "https://registry.npmjs.org/concat-map/-/concat-map-0.0.1.tgz",
-            "version": "0.0.1"
+        "node_modules/color-name": {
+            "integrity": "sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/color-name/-/color-name-1.1.4.tgz",
+            "version": "1.1.4"
         },
         "node_modules/cssesc": {
             "bin": {
                 "cssesc": "bin/cssesc"
             },
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/cssesc/-/cssesc-3.0.0.tgz",
             "version": "3.0.0"
         },
+        "node_modules/defined": {
+            "integrity": "sha512-Y2caI5+ZwS5c3RiNDJ6u53VhQHv+hHKwhkI1iHvceKUHw9Df6EK2zRLfjejRgMuCuxK7PfSWIMwWecceVvThjQ==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/defined/-/defined-1.0.0.tgz",
+            "version": "1.0.0"
+        },
+        "node_modules/detective": {
+            "bin": {
+                "detective": "bin/detective.js"
+            },
+            "dependencies": {
+                "acorn-node": "^1.8.2",
+                "defined": "^1.0.0",
+                "minimist": "^1.2.6"
+            },
+            "engines": {
+                "node": ">=0.8.0"
+            },
+            "integrity": "sha512-v9XE1zRnz1wRtgurGu0Bs8uHKFSTdteYZNbIPFVhUZ39L/S79ppMpdmVOZAnoz1jfEFodc48n6MX483Xo3t1yw==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/detective/-/detective-5.2.1.tgz",
+            "version": "5.2.1"
+        },
         "node_modules/didyoumean": {
             "integrity": "sha512-gxtyfqMg7GKyhQmb056K7M3xszy/myH8w+B4RT+QXBQsvAOdc3XymqDDPHx1BgPgsdAA5SIifona89YtRATDzw==",
             "license": "Apache-2.0",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/didyoumean/-/didyoumean-1.2.2.tgz",
             "version": "1.2.2"
         },
         "node_modules/dlv": {
@@ -860,17 +687,18 @@
                 "glob-parent": "^5.1.2",
                 "merge2": "^1.3.0",
                 "micromatch": "^4.0.4"
             },
             "engines": {
                 "node": ">=8.6.0"
             },
-            "integrity": "sha512-kNFPyjhh5cKjrUltxs+wFx+ZkbRaxxmZ+X0ZU31SOsxCEtP9VPgtq2teZw1DebupL5GmDaNQ6yKMMVcM41iqDg==",
-            "resolved": "https://registry.npmjs.org/fast-glob/-/fast-glob-3.3.1.tgz",
-            "version": "3.3.1"
+            "integrity": "sha512-xrO3+1bxSo3ZVHAnqzyuewYT6aMFHRAd4Kcs92MAonjwQZLsK9d0SF1IyQ3k5PoirxTW0Oe/RqFgMQ6TcNE5Ew==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fast-glob/-/fast-glob-3.2.11.tgz",
+            "version": "3.2.11"
         },
         "node_modules/fast-glob/node_modules/glob-parent": {
             "dependencies": {
                 "is-glob": "^4.0.1"
             },
             "engines": {
                 "node": ">= 6"
@@ -897,19 +725,14 @@
                 "node": ">=8"
             },
             "integrity": "sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fill-range/-/fill-range-7.0.1.tgz",
             "version": "7.0.1"
         },
-        "node_modules/fs.realpath": {
-            "integrity": "sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==",
-            "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "node_modules/fsevents": {
             "engines": {
                 "node": "^8.16.0 || ^10.6.0 || >=11.0.0"
             },
             "hasInstallScript": true,
             "integrity": "sha512-xiqMQR4xAeHTuB9uWm+fFRcIOgKBMiOBP+eXiyT7jsgVCq1bkVygt00oASowB7EdtpOHaaPgKt812P9ab+DDKA==",
             "license": "MIT",
@@ -918,36 +741,18 @@
                 "darwin"
             ],
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/fsevents/-/fsevents-2.3.2.tgz",
             "version": "2.3.2"
         },
         "node_modules/function-bind": {
             "integrity": "sha512-yIovAzMX49sF8Yl58fSCWJ5svSLuaibPxXQJFLmBObTuCr0Mf1KiPopGM9NiFjiYBCbfaa2Fh6breQ6ANVTI0A==",
-            "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/function-bind/-/function-bind-1.1.1.tgz",
             "version": "1.1.1"
         },
-        "node_modules/glob": {
-            "dependencies": {
-                "fs.realpath": "^1.0.0",
-                "inflight": "^1.0.4",
-                "inherits": "2",
-                "minimatch": "^3.0.4",
-                "once": "^1.3.0",
-                "path-is-absolute": "^1.0.0"
-            },
-            "engines": {
-                "node": "*"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/isaacs"
-            },
-            "integrity": "sha512-LwaxwyZ72Lk7vZINtNNrywX0ZuLyStrdDtabefZKAY5ZGJhVtgdznluResxNmPitE0SAO+O26sWTHeKSI2wMBA==",
-            "resolved": "https://registry.npmjs.org/glob/-/glob-7.1.6.tgz",
-            "version": "7.1.6"
-        },
         "node_modules/glob-parent": {
             "dependencies": {
                 "is-glob": "^4.0.3"
             },
             "engines": {
                 "node": ">=10.13.0"
             },
@@ -960,31 +765,18 @@
             "dependencies": {
                 "function-bind": "^1.1.1"
             },
             "engines": {
                 "node": ">= 0.4.0"
             },
             "integrity": "sha512-f2dvO0VU6Oej7RkWJGrehjbzMAjFp5/VKPp5tTpWIV4JHHZK1/BxbFRtf/siA2SWTe09caDmVtYYzWEIbBS4zw==",
-            "resolved": "https://registry.npmjs.org/has/-/has-1.0.3.tgz",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/has/-/has-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "node_modules/inflight": {
-            "dependencies": {
-                "once": "^1.3.0",
-                "wrappy": "1"
-            },
-            "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
-            "resolved": "https://registry.npmjs.org/inflight/-/inflight-1.0.6.tgz",
-            "version": "1.0.6"
-        },
-        "node_modules/inherits": {
-            "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
-            "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
-            "version": "2.0.4"
-        },
         "node_modules/is-binary-path": {
             "dependencies": {
                 "binary-extensions": "^2.0.0"
             },
             "engines": {
                 "node": ">=8"
             },
@@ -996,17 +788,18 @@
         "node_modules/is-core-module": {
             "dependencies": {
                 "has": "^1.0.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-RECHCBCd/viahWmwj6enj19sKbHfJrddi/6cBDsNTKbNq0f7VeaUkBo60BqzvPqo/W54ChS62Z5qyun7cfOMqQ==",
-            "resolved": "https://registry.npmjs.org/is-core-module/-/is-core-module-2.12.0.tgz",
-            "version": "2.12.0"
+            "integrity": "sha512-Erxj2n/LDAZ7H8WNJXd9tw38GYM3dv8rk8Zcs+jJuxYTW7sozH+SS8NtrSjVL1/vpLvWi1hxy96IzjJ3EHTJJg==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/is-core-module/-/is-core-module-2.10.0.tgz",
+            "version": "2.10.0"
         },
         "node_modules/is-extglob": {
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha1-qIwCU1eR8C7TfHahueqXc8gz+MI=",
             "license": "MIT",
@@ -1030,34 +823,22 @@
                 "node": ">=0.12.0"
             },
             "integrity": "sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/is-number/-/is-number-7.0.0.tgz",
             "version": "7.0.0"
         },
-        "node_modules/jiti": {
-            "bin": {
-                "jiti": "bin/jiti.js"
-            },
-            "integrity": "sha512-gFqAIbuKyyso/3G2qhiO2OM6shY6EPP/R0+mkDbyspxKazh8BXDC5FiFsUjlczgdNz/vfra0da2y+aHrusLG/Q==",
-            "resolved": "https://registry.npmjs.org/jiti/-/jiti-1.21.0.tgz",
-            "version": "1.21.0"
-        },
         "node_modules/lilconfig": {
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==",
-            "resolved": "https://registry.npmjs.org/lilconfig/-/lilconfig-2.1.0.tgz",
-            "version": "2.1.0"
-        },
-        "node_modules/lines-and-columns": {
-            "integrity": "sha512-7ylylesZQ/PV29jhEDl3Ufjo6ZX7gCqJr5F7PKrqc93v7fzSymt1BpwEU8nAUXs8qzzvqhbjhK5QZg6Mt/HkBg==",
-            "resolved": "https://registry.npmjs.org/lines-and-columns/-/lines-and-columns-1.2.4.tgz",
-            "version": "1.2.4"
+            "integrity": "sha512-9JROoBW7pobfsx+Sq2JsASvCo6Pfo6WWoUW79HuB1BCoBXD4PLWJPqDF6fNj67pqBYTbAHkE57M1kS/+L1neOg==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/lilconfig/-/lilconfig-2.0.6.tgz",
+            "version": "2.0.6"
         },
         "node_modules/merge2": {
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-8q7VEgMJW4J8tcfVPy8g09NcQwZdbwFEqhe/WZkoIzjn/3TGDwtOCYtXGxA3O8tPzpczCCDgv+P2P5y00ZJOOg==",
             "license": "MIT",
@@ -1073,94 +854,50 @@
                 "node": ">=8.6"
             },
             "integrity": "sha512-DMy+ERcEW2q8Z2Po+WNXuw3c5YaUSFjAO5GsJqfEl7UjvtIuFKO6ZrKvcItdy98dwFI2N1tg3zNIdKaQT+aNdA==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/micromatch/-/micromatch-4.0.5.tgz",
             "version": "4.0.5"
         },
-        "node_modules/minimatch": {
-            "dependencies": {
-                "brace-expansion": "^1.1.7"
-            },
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==",
-            "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.1.2.tgz",
-            "version": "3.1.2"
-        },
-        "node_modules/mz": {
-            "dependencies": {
-                "any-promise": "^1.0.0",
-                "object-assign": "^4.0.1",
-                "thenify-all": "^1.0.0"
-            },
-            "integrity": "sha512-z81GNO7nnYMEhrGh9LeymoE4+Yr0Wn5McHIZMK5cfQCl+NDX08sCZgUc9/6MHni9IWuFLm1Z3HTCXu2z9fN62Q==",
-            "resolved": "https://registry.npmjs.org/mz/-/mz-2.7.0.tgz",
-            "version": "2.7.0"
+        "node_modules/minimist": {
+            "integrity": "sha512-Jsjnk4bw3YJqYzbdyBiNsPWHPfO++UGG749Cxs6peCu5Xg4nrena6OVxOYxrQTqww0Jmwt+Ref8rggumkTLz9Q==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/minimist/-/minimist-1.2.6.tgz",
+            "version": "1.2.6"
         },
         "node_modules/nanoid": {
             "bin": {
                 "nanoid": "bin/nanoid.cjs"
             },
             "engines": {
                 "node": "^10 || ^12 || ^13.7 || ^14 || >=15.0.1"
             },
-            "funding": [
-                {
-                    "type": "github",
-                    "url": "https://github.com/sponsors/ai"
-                }
-            ],
-            "integrity": "sha512-BGcqMMJuToF7i1rt+2PWSNVnWIkGCU78jBG3RxO/bZlnZPK2Cmi2QaffxGO/2RvWi9sL+FAiRiXMgsyxQ1DIDA==",
-            "resolved": "https://registry.npmjs.org/nanoid/-/nanoid-3.3.6.tgz",
-            "version": "3.3.6"
+            "integrity": "sha512-MqBkQh/OHTS2egovRtLk45wEyNXwF+cokD+1YPf9u5VfJiRdAiRwB2froX5Co9Rh20xs4siNPm8naNotSD6RBw==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/nanoid/-/nanoid-3.3.4.tgz",
+            "version": "3.3.4"
         },
         "node_modules/normalize-path": {
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/normalize-path/-/normalize-path-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "node_modules/object-assign": {
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==",
-            "resolved": "https://registry.npmjs.org/object-assign/-/object-assign-4.1.1.tgz",
-            "version": "4.1.1"
-        },
         "node_modules/object-hash": {
             "engines": {
                 "node": ">= 6"
             },
             "integrity": "sha512-RSn9F68PjH9HqtltsSnqYC1XXoWe9Bju5+213R98cNGttag9q9yAOTzdbsqvIa7aNm5WffBZFpWYr2aWrklWAw==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/object-hash/-/object-hash-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "node_modules/once": {
-            "dependencies": {
-                "wrappy": "1"
-            },
-            "integrity": "sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==",
-            "resolved": "https://registry.npmjs.org/once/-/once-1.4.0.tgz",
-            "version": "1.4.0"
-        },
-        "node_modules/path-is-absolute": {
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-AVbw3UJ2e9bq64vSaS9Am0fje1Pa8pbGqTTsmXfaIiMpnr5DlDhfJOuLj9Sf95ZPVDAUerDfEk88MPmPe7UCQg==",
-            "resolved": "https://registry.npmjs.org/path-is-absolute/-/path-is-absolute-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "node_modules/path-parse": {
             "integrity": "sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/path-parse/-/path-parse-1.0.7.tgz",
             "version": "1.0.7"
         },
         "node_modules/picocolors": {
@@ -1186,140 +923,134 @@
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-udgsAY+fTnvv7kI7aaxbqwWNb0AHiB0qBO89PZKPkoTmGOgdbrHDKD+0B2X4uTfJ/FT1R09r9gTsjUjNJotuog==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/pify/-/pify-2.3.0.tgz",
             "version": "2.3.0"
         },
-        "node_modules/pirates": {
-            "engines": {
-                "node": ">= 6"
-            },
-            "integrity": "sha512-8V9+HQPupnaXMA23c5hvl69zXvTwTzyAYasnkb0Tts4XvO4CliqONMOnvlq26rkhLC3nWDFBJf73LU1e1VZLaQ==",
-            "resolved": "https://registry.npmjs.org/pirates/-/pirates-4.0.5.tgz",
-            "version": "4.0.5"
-        },
         "node_modules/postcss": {
             "dependencies": {
-                "nanoid": "^3.3.6",
+                "nanoid": "^3.3.4",
                 "picocolors": "^1.0.0",
                 "source-map-js": "^1.0.2"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/postcss/"
                 },
                 {
                     "type": "tidelift",
                     "url": "https://tidelift.com/funding/github/npm/postcss"
-                },
-                {
-                    "type": "github",
-                    "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==",
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.23.tgz",
-            "version": "8.4.23"
+            "integrity": "sha512-ipHE1XBvKzm5xI7hiHCZJCSugxvsdq2mPnsq5+UF+VHCjiBvtDrlxJfMBToWaP9D5XlgNmcFGqoHmUn0EYEaRQ==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss/-/postcss-8.4.16.tgz",
+            "version": "8.4.16"
         },
         "node_modules/postcss-import": {
             "dependencies": {
                 "postcss-value-parser": "^4.0.0",
                 "read-cache": "^1.0.0",
                 "resolve": "^1.1.7"
             },
             "engines": {
-                "node": ">=14.0.0"
+                "node": ">=10.0.0"
             },
-            "integrity": "sha512-hpr+J05B2FVYUAXHeK1YyI267J/dDDhMU6B6civm8hSY1jYJnBXxzKDKDswzJmtLHryrjhnDjqqp/49t8FALew==",
+            "integrity": "sha512-flwI+Vgm4SElObFVPpTIT7SU7R3qk2L7PyduMcokiaVKuWv9d/U+Gm/QAd8NDLuykTWTkcrjOeD2Pp1rMeBTGw==",
+            "license": "MIT",
             "peerDependencies": {
                 "postcss": "^8.0.0"
             },
-            "resolved": "https://registry.npmjs.org/postcss-import/-/postcss-import-15.1.0.tgz",
-            "version": "15.1.0"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-import/-/postcss-import-14.1.0.tgz",
+            "version": "14.1.0"
         },
         "node_modules/postcss-js": {
             "dependencies": {
                 "camelcase-css": "^2.0.1"
             },
             "engines": {
                 "node": "^12 || ^14 || >= 16"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/postcss/"
             },
-            "integrity": "sha512-dDLF8pEO191hJMtlHFPRa8xsizHaM82MLfNkUHdUtVEV3tgTp5oj+8qbEqYM57SLfc74KSbw//4SeJma2LRVIw==",
+            "integrity": "sha512-77QESFBwgX4irogGVPgQ5s07vLvFqWr228qZY+w6lW599cRlK/HmnlivnnVUxkjHnCu4J16PDMHcH+e+2HbvTQ==",
+            "license": "MIT",
             "peerDependencies": {
-                "postcss": "^8.4.21"
+                "postcss": "^8.3.3"
             },
-            "resolved": "https://registry.npmjs.org/postcss-js/-/postcss-js-4.0.1.tgz",
-            "version": "4.0.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-js/-/postcss-js-4.0.0.tgz",
+            "version": "4.0.0"
         },
         "node_modules/postcss-load-config": {
             "dependencies": {
                 "lilconfig": "^2.0.5",
-                "yaml": "^2.1.1"
+                "yaml": "^1.10.2"
             },
             "engines": {
-                "node": ">= 14"
+                "node": ">= 10"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/postcss/"
             },
-            "integrity": "sha512-vEJIc8RdiBRu3oRAI0ymerOn+7rPuMvRXslTvZUKZonDHFIczxztIyJ1urxM1x9JXEikvpWWTUUqal5j/8QgvA==",
+            "integrity": "sha512-6DiM4E7v4coTE4uzA8U//WhtPwyhiim3eyjEMFCnUpzbrkK9wJHgKDT2mR+HbtSrd/NubVaYTOpSpjUl8NQeRg==",
+            "license": "MIT",
             "peerDependencies": {
                 "postcss": ">=8.0.9",
                 "ts-node": ">=9.0.0"
             },
             "peerDependenciesMeta": {
                 "postcss": {
                     "optional": true
                 },
                 "ts-node": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/postcss-load-config/-/postcss-load-config-4.0.1.tgz",
-            "version": "4.0.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-load-config/-/postcss-load-config-3.1.4.tgz",
+            "version": "3.1.4"
         },
         "node_modules/postcss-nested": {
             "dependencies": {
-                "postcss-selector-parser": "^6.0.11"
+                "postcss-selector-parser": "^6.0.6"
             },
             "engines": {
                 "node": ">=12.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/postcss/"
             },
-            "integrity": "sha512-mEp4xPMi5bSWiMbsgoPfcP74lsWLHkQbZc3sY+jWYd65CUwXrUaTp0fmNpa01ZcETKlIgUdFN/MpS2xZtqL9dQ==",
+            "integrity": "sha512-rKqm2Fk0KbA8Vt3AdGN0FB9OBOMDVajMG6ZCf/GoHgdxUJ4sBFp0A/uMIRm+MJUdo33YXEtjqIz8u7DAp8B7DA==",
+            "license": "MIT",
             "peerDependencies": {
                 "postcss": "^8.2.14"
             },
-            "resolved": "https://registry.npmjs.org/postcss-nested/-/postcss-nested-6.0.1.tgz",
-            "version": "6.0.1"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-nested/-/postcss-nested-5.0.6.tgz",
+            "version": "5.0.6"
         },
         "node_modules/postcss-selector-parser": {
             "dependencies": {
                 "cssesc": "^3.0.0",
                 "util-deprecate": "^1.0.2"
             },
             "engines": {
                 "node": ">=4"
             },
-            "integrity": "sha512-zbARubNdogI9j7WY4nQJBiNqQf3sLS3wCP4WfOidu+p28LofJqDH1tcXypGrcmMHhDk2t9wGhCsYe/+szLTy1g==",
-            "resolved": "https://registry.npmjs.org/postcss-selector-parser/-/postcss-selector-parser-6.0.11.tgz",
-            "version": "6.0.11"
+            "integrity": "sha512-IQ7TZdoaqbT+LCpShg46jnZVlhWD2w6iQYAcYXfHARZ7X1t/UGhhceQDs5X0cGqKvYlHNOuv7Oa1xmb0oQuA3w==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-selector-parser/-/postcss-selector-parser-6.0.10.tgz",
+            "version": "6.0.10"
         },
         "node_modules/postcss-value-parser": {
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
@@ -1339,14 +1070,26 @@
                 }
             ],
             "integrity": "sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/queue-microtask/-/queue-microtask-1.2.3.tgz",
             "version": "1.2.3"
         },
+        "node_modules/quick-lru": {
+            "engines": {
+                "node": ">=10"
+            },
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-WuyALRjWPDGtt/wzJiadO5AXY+8hZ80hVpe6MyivgraREW751X3SbhRvG3eLKOYN+8VEvqLcf3wdnt44Z4S4SA==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/quick-lru/-/quick-lru-5.1.1.tgz",
+            "version": "5.1.1"
+        },
         "node_modules/read-cache": {
             "dependencies": {
                 "pify": "^2.3.0"
             },
             "integrity": "sha512-Owdv/Ft7IjOgm/i0xvNDZ1LrRANRfew4b2prF3OWMQLxLfu3bS8FVhCsrSCMK4lR56Y9ya+AThoTpDCTxCmpRA==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/read-cache/-/read-cache-1.0.0.tgz",
@@ -1365,24 +1108,25 @@
             "version": "3.6.0"
         },
         "node_modules/resolve": {
             "bin": {
                 "resolve": "bin/resolve"
             },
             "dependencies": {
-                "is-core-module": "^2.11.0",
+                "is-core-module": "^2.9.0",
                 "path-parse": "^1.0.7",
                 "supports-preserve-symlinks-flag": "^1.0.0"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-Sb+mjNHOULsBv818T40qSPeRiuWLyaGMa5ewydRLFimneixmVy2zdivRl+AF6jaYPC8ERxGDmFSiqui6SfPd+g==",
-            "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.22.2.tgz",
-            "version": "1.22.2"
+            "integrity": "sha512-nBpuuYuY5jFsli/JIs1oldw6fOQCBioohqWZg/2hiaOybXOft4lonv85uDOKXdf8rhyK159cxU5cDcK/NKk8zw==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/resolve/-/resolve-1.22.1.tgz",
+            "version": "1.22.1"
         },
         "node_modules/reusify": {
             "engines": {
                 "iojs": ">=1.0.0",
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==",
@@ -1418,35 +1162,14 @@
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
             "license": "BSD-3-Clause",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/source-map-js/-/source-map-js-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "node_modules/sucrase": {
-            "bin": {
-                "sucrase": "bin/sucrase",
-                "sucrase-node": "bin/sucrase-node"
-            },
-            "dependencies": {
-                "@jridgewell/gen-mapping": "^0.3.2",
-                "commander": "^4.0.0",
-                "glob": "7.1.6",
-                "lines-and-columns": "^1.1.6",
-                "mz": "^2.7.0",
-                "pirates": "^4.0.1",
-                "ts-interface-checker": "^0.1.9"
-            },
-            "engines": {
-                "node": ">=8"
-            },
-            "integrity": "sha512-ydQOU34rpSyj2TGyz4D2p8rbktIOZ8QY9s+DGLvFU1i5pWJE8vkpruCjGCMHsdXwnD7JDcS+noSwM/a7zyNFDQ==",
-            "resolved": "https://registry.npmjs.org/sucrase/-/sucrase-3.32.0.tgz",
-            "version": "3.32.0"
-        },
         "node_modules/supports-preserve-symlinks-flag": {
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
@@ -1457,95 +1180,80 @@
         },
         "node_modules/tailwindcss": {
             "bin": {
                 "tailwind": "lib/cli.js",
                 "tailwindcss": "lib/cli.js"
             },
             "dependencies": {
-                "@alloc/quick-lru": "^5.2.0",
                 "arg": "^5.0.2",
                 "chokidar": "^3.5.3",
+                "color-name": "^1.1.4",
+                "detective": "^5.2.1",
                 "didyoumean": "^1.2.2",
                 "dlv": "^1.1.3",
-                "fast-glob": "^3.3.0",
+                "fast-glob": "^3.2.11",
                 "glob-parent": "^6.0.2",
                 "is-glob": "^4.0.3",
-                "jiti": "^1.21.0",
-                "lilconfig": "^2.1.0",
-                "micromatch": "^4.0.5",
+                "lilconfig": "^2.0.6",
                 "normalize-path": "^3.0.0",
                 "object-hash": "^3.0.0",
                 "picocolors": "^1.0.0",
-                "postcss": "^8.4.23",
-                "postcss-import": "^15.1.0",
-                "postcss-js": "^4.0.1",
-                "postcss-load-config": "^4.0.1",
-                "postcss-nested": "^6.0.1",
-                "postcss-selector-parser": "^6.0.11",
-                "resolve": "^1.22.2",
-                "sucrase": "^3.32.0"
+                "postcss": "^8.4.14",
+                "postcss-import": "^14.1.0",
+                "postcss-js": "^4.0.0",
+                "postcss-load-config": "^3.1.4",
+                "postcss-nested": "5.0.6",
+                "postcss-selector-parser": "^6.0.10",
+                "postcss-value-parser": "^4.2.0",
+                "quick-lru": "^5.1.1",
+                "resolve": "^1.22.1"
             },
             "engines": {
-                "node": ">=14.0.0"
-            },
-            "integrity": "sha512-U7sxQk/n397Bmx4JHbJx/iSOOv5G+II3f1kpLpY2QeUv5DcPdcTsYLlusZfq1NthHS1c1cZoyFmmkex1rzke0A==",
-            "resolved": "https://registry.npmjs.org/tailwindcss/-/tailwindcss-3.4.3.tgz",
-            "version": "3.4.3"
-        },
-        "node_modules/thenify": {
-            "dependencies": {
-                "any-promise": "^1.0.0"
+                "node": ">=12.13.0"
             },
-            "integrity": "sha512-RVZSIV5IG10Hk3enotrhvz0T9em6cyHBLkH/YAZuKqd8hRkKhSfCGIcP2KUY0EPxndzANBmNllzWPwak+bheSw==",
-            "resolved": "https://registry.npmjs.org/thenify/-/thenify-3.3.1.tgz",
-            "version": "3.3.1"
-        },
-        "node_modules/thenify-all": {
-            "dependencies": {
-                "thenify": ">= 3.1.0 < 4"
-            },
-            "engines": {
-                "node": ">=0.8"
+            "integrity": "sha512-YSneUCZSFDYMwk+TGq8qYFdCA3yfBRdBlS7txSq0LUmzyeqRe3a8fBQzbz9M3WS/iFT4BNf/nmw9mEzrnSaC0g==",
+            "license": "MIT",
+            "peerDependencies": {
+                "postcss": "^8.0.9"
             },
-            "integrity": "sha512-RNxQH/qI8/t3thXJDwcstUO4zeqo64+Uy/+sNVRBx4Xn2OX+OZ9oP+iJnNFqplFra2ZUVeKCSa2oVWi3T4uVmA==",
-            "resolved": "https://registry.npmjs.org/thenify-all/-/thenify-all-1.6.0.tgz",
-            "version": "1.6.0"
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/tailwindcss/-/tailwindcss-3.1.8.tgz",
+            "version": "3.1.8"
         },
         "node_modules/to-regex-range": {
             "dependencies": {
                 "is-number": "^7.0.0"
             },
             "engines": {
                 "node": ">=8.0"
             },
             "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/to-regex-range/-/to-regex-range-5.0.1.tgz",
             "version": "5.0.1"
         },
-        "node_modules/ts-interface-checker": {
-            "integrity": "sha512-Y/arvbn+rrz3JCKl9C4kVNfTfSm2/mEp5FSz5EsZSANGPSlQrpRI5M4PKF+mJnE52jOO90PnPSc3Ur3bTQw0gA==",
-            "resolved": "https://registry.npmjs.org/ts-interface-checker/-/ts-interface-checker-0.1.13.tgz",
-            "version": "0.1.13"
-        },
         "node_modules/util-deprecate": {
             "integrity": "sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==",
             "license": "MIT",
             "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/util-deprecate/-/util-deprecate-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "node_modules/wrappy": {
-            "integrity": "sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==",
-            "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
-            "version": "1.0.2"
+        "node_modules/xtend": {
+            "engines": {
+                "node": ">=0.4"
+            },
+            "integrity": "sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==",
+            "license": "MIT",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/xtend/-/xtend-4.0.2.tgz",
+            "version": "4.0.2"
         },
         "node_modules/yaml": {
             "engines": {
-                "node": ">= 14"
+                "node": ">= 6"
             },
-            "integrity": "sha512-CBKFWExMn46Foo4cldiChEzn7S7SRV+wqiluAb6xmueD/fGyRHIhX8m14vVGgeFWjN540nKCNVj6P21eQjgTuA==",
-            "resolved": "https://registry.npmjs.org/yaml/-/yaml-2.2.2.tgz",
-            "version": "2.2.2"
+            "integrity": "sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==",
+            "license": "ISC",
+            "resolved": "https://nexus.global.lmco.com/repository/npm-proxy/yaml/-/yaml-1.10.2.tgz",
+            "version": "1.10.2"
         }
     },
     "requires": true
 }
```

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/vulnerabilities.html` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/reporting/templates/vulnerability_details.html` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerability_details.html`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/utils.py` & `hoppr_security_commons-0.0.9/security_commons/common/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This provides a set of utility functions for working with vulnerabilities and boms."""
+"""This provides a set of utility functions for working with vulnerabilities and boms"""
 # This file is part of hoppr-cop
 #
 # Licensed under the MIT License;
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://opensource.org/licenses/MIT
@@ -11,170 +11,193 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # Copyright (c) 2022 Lockheed Martin Corporation
-from __future__ import annotations
 
 import json
 import os
 import stat
 import tempfile
 import uuid
-
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import Optional, Union, List, Dict
 
 import requests
-import typer
-
 from hoppr_cyclonedx_models.cyclonedx_1_3 import (
     CyclonedxSoftwareBillOfMaterialSpecification as Bom_1_3,
 )
 from hoppr_cyclonedx_models.cyclonedx_1_4 import (
-    Advisory,
-    Component,
     CyclonedxSoftwareBillOfMaterialsStandard as Bom_1_4,
-    Reference,
     VulnerabilitySource,
+    Reference,
+    Advisory,
 )
-
-
-if TYPE_CHECKING:
-    from packageurl import PackageURL
+import typer
+from packageurl import PackageURL
 
 
 def convert_xml_to_json(file_path: Path) -> Path:
-    """Function to convert a xml file to json format."""
+    """
+    Function to convert a xml file to json format.
+    """
     typer.echo("xml format detected, attempt to convert with cyclonedx tools")
-
     # Default to the path specified in the hoppr-cop docker file or define the local filename to save data
     docker_image_path = Path("/usr/local/bin/cyclone-dx")
-    cyclone_dx_path = docker_image_path if docker_image_path.exists() else Path(tempfile.gettempdir()) / "cyclonedx"
+    cyclone_dx_path = (
+        docker_image_path
+        if docker_image_path.exists()
+        else Path(tempfile.gettempdir()) / "cyclonedx"
+    )
     if not cyclone_dx_path.exists():
         typer.echo("cyclonedx tools not found Attempting to download")
-        if url := os.getenv("CYCLONE_INSTALL_URL"):
+        if "CYCLONE_INSTALL_URL" in os.environ:
+            url = os.environ.get("CYCLONE_INSTALL_URL")
             # Make http request for remote file datae
-            data = requests.get(url, timeout=60)
-
+            data = requests.get(url)
             # Save file data to local copy
-            cyclone_dx_path.write_bytes(data.content)
+            with open(cyclone_dx_path, "wb") as file:
+                file.write(data.content)
         else:
             msg = typer.style(
                 "In order to support xml boms, you must set 'CYCLONE_INSTALL_URL' to "
                 "the correct release of cyclone-dx cli. https://github.com/CycloneDX/cyclonedx-cli/releases",
                 fg=typer.colors.RED,
             )
             typer.echo(msg)
             raise typer.Exit(code=1)
-
-    cyclone_dx_path.chmod(stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH | stat.S_IXOTH)
-
+    os.chmod(
+        cyclone_dx_path,
+        stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH | stat.S_IXOTH,
+    )
     os.system(
         f"{cyclone_dx_path.absolute()} convert --input-file {file_path} \
-            --output-file {tempfile.gettempdir()}/{file_path.name}.json --output-format json",
+            --output-file {tempfile.gettempdir()}/{file_path.name}.json --output-format json"
     )
     return Path(f"{tempfile.gettempdir()}/{file_path.name}.json")
 
 
-def parse_sbom(sbom_file: Path) -> Bom_1_4 | Bom_1_3:
-    """Parses a Software Bill of Materials File."""
+def parse_sbom(sbom_file: Path) -> Optional[Union[Bom_1_4, Bom_1_3]]:
+    """Parses a Software Bill of Materials File"""
+    sbom = None
     if sbom_file.is_file() and sbom_file.exists():
-        typer.echo(f"processing {sbom_file}")
-
-        if sbom_file.suffix == ".xml":
+        typer.echo(f"processing {str(sbom_file)}")
+        if str(sbom_file).endswith(".xml"):
             sbom_file = convert_xml_to_json(sbom_file)
 
-        sbom_json_object = json.loads(sbom_file.read_text(encoding="utf-8"))
-        sbom = create_sbom_object(sbom_json_object, str(sbom_file))
+        with open(sbom_file, encoding="utf-8") as sbom_file_json:
+            sbom_json_object = json.load(sbom_file_json)
+            sbom = create_sbom_object(sbom_json_object, str(sbom_file))
     else:
-        typer.secho(f"{sbom_file!s} is not a file", fg=typer.colors.RED)
+        typer.secho(f"{str(sbom_file)} is not a file", fg=typer.colors.RED)
         raise typer.Exit
-
     return sbom
 
 
-def parse_sbom_json_string(sbom_file_json: str, sbom_info: str) -> Bom_1_4 | Bom_1_3:
-    """Parses a Software Bill of Materials JSON String."""
+def parse_sbom_json_string(
+    sbom_file_json: str, sbom_info: str
+) -> Optional[Union[Bom_1_4, Bom_1_3]]:
+    """Parses a Software Bill of Materials JSON String"""
     sbom_json_object = json.loads(sbom_file_json)
     return create_sbom_object(sbom_json_object, sbom_info)
 
 
-def create_sbom_object(sbom_json_object: dict, sbom_info: str) -> Bom_1_4 | Bom_1_3:
-    """Creates a Software Bill of Materials Object."""
+def create_sbom_object(
+    sbom_json_object: Dict, sbom_info: str
+) -> Optional[Union[Bom_1_4, Bom_1_3]]:
+    """Creates a Software Bill of Materials Object"""
+    sbom = None
     spec_version = sbom_json_object.get("specVersion", "")
-    sbom_json_object.pop("$schema", None)
-
-    sbom: Bom_1_4 | Bom_1_3
+    if "$schema" in sbom_json_object:
+        del sbom_json_object["$schema"]
     if spec_version == "1.4":
         sbom = Bom_1_4(**sbom_json_object)
     elif spec_version == "1.3":
         sbom = Bom_1_3(**sbom_json_object)
     else:
         typer.secho(f"{sbom_info} is an unknown spec version ({spec_version})")
         raise typer.Exit
 
     return sbom
 
 
-def get_vulnerability_source(vulnerability_id: str) -> VulnerabilitySource | None:
-    """Generate the source for a vulnerability based on a given ID."""
+def get_vulnerability_source(vulnerability_id: str) -> Optional[VulnerabilitySource]:
+    """Generate the source for a vulnerability based on a given ID"""
     if vulnerability_id.startswith("CVE-"):
-        return VulnerabilitySource(name="NVD", url=f"https://nvd.nist.gov/vuln/detail/{vulnerability_id}")
+        return VulnerabilitySource(
+            name="NVD", url=f"https://nvd.nist.gov/vuln/detail/{vulnerability_id}"
+        )
     if vulnerability_id.startswith("GHSA"):
-        return VulnerabilitySource(name="Github Advisories", url=f"https://github.com/advisories/{vulnerability_id}")
+        return VulnerabilitySource(
+            name="Github Advisories",
+            url=f"https://github.com/advisories/{vulnerability_id}",
+        )
     if vulnerability_id.startswith("GMS"):
-        return VulnerabilitySource(name="Github Advisories", url=f"https://github.com/advisories/{vulnerability_id}")
+        return VulnerabilitySource(
+            name="Github Advisories",
+            url=f"https://github.com/advisories/{vulnerability_id}",
+        )
     if vulnerability_id.startswith("sonatype"):
         return VulnerabilitySource(
             name="OSS Index",
             url=f"https://ossindex.sonatype.org/vulnerability/{vulnerability_id}",
         )
 
     return None
+    # else:
+    #     efoss_vuln.source = Source(name="Gitlab Advisories",
+    #                                url=f"https://gitlab.com/gitlab-org/security-products/gemnasium-db/-/tree/master/{path_slug}/{filename}",
+    #                                scanner="gemnasium")
 
 
-def get_advisories_from_urls(urls: list[str]) -> list[Advisory]:
+def get_advisories_from_urls(urls: List[str]) -> List[Advisory]:
     """Generates a list of advisories for the given set of urls."""
     urls = list(set(urls))
-    return [Advisory(url=x) for x in urls]
+    return list((map(lambda x: Advisory(url=x), urls)))
 
 
-def get_references_from_ids(ids: list[str], primary_id: str) -> list[Reference]:
-    """Builds a list of Reference objects to the given vulnerability IDs."""
+def get_references_from_ids(ids: List[str], primary_id: str) -> List[Reference]:
+    """Builds a list of Reference objects to the given vulnerability IDs"""
+    unique_ids = list(set(ids))
     references = []
-
-    for ident in list(set(ids)):
-        if ident != primary_id and (source := get_vulnerability_source(ident)):
-            references.append(Reference(id=ident, source=source))
-
+    for ident in unique_ids:
+        if ident != primary_id:
+            references.append(
+                Reference(id=ident, source=get_vulnerability_source(ident))
+            )
     return references
 
 
-def build_bom_dict_from_purls(purls: list[PackageURL]) -> dict:
-    """Create SBOM dictionary from PackageURL list."""
-    sbom = Bom_1_4(specVersion="1.4", serialNumber=uuid.uuid1().urn)
-    sbom.components = []  # assign explicitly for type checkers
+def __build_bom_dict_from_purls(purls: List[PackageURL]) -> Dict:
+    bom = {
+        "bomFormat": "CycloneDX",
+        "specVersion": "1.4",
+        "serialNumber": f"urn:uuid:{str(uuid.uuid1())}",
+        "version": 1,
+        "components": [],
+    }
 
     for purl in purls:
-        component = Component(
-            type="library",
-            name=purl.name,
-            version=purl.version,
-            purl=purl.to_string(),
-            group=purl.namespace,
-            bom_ref=purl.to_string(),
-            description="test",
-            author="test",
-            externalReferences=[],
-        )
-
-        sbom.components.append(component)
-
-    return sbom.dict()
-
-
-def build_bom_from_purls(purls: list[PackageURL]) -> Bom_1_4:
-    """Creates a skeleton BOM from a list of purls."""
-    return Bom_1_4(**build_bom_dict_from_purls(purls))
+        component = {
+            "type": "library",
+            # "bom-ref": "610e35f2-175c-437d-bb20-7740c8205601",
+            "name": purl.name,
+            "version": purl.version,
+            "purl": purl.to_string(),
+            "group": purl.namespace,
+            "bom-ref": purl.to_string(),
+            "description": "test",
+            "author": "test",
+            "externalReferences": [],
+        }
+        if purl.namespace is not None:
+            component["group"] = purl.namespace
+
+        bom["components"].append(component)
+    return bom
+
+
+def build_bom_from_purls(purls: List[PackageURL]) -> Bom_1_4:
+    """Creates a skeleton bOM from a list of purls"""
+    return Bom_1_4(**__build_bom_dict_from_purls(purls))
```

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/vulnerability_combiner.py` & `hoppr_security_commons-0.0.9/security_commons/common/vulnerability_combiner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This file provides the ability to combine vulnerabilities from multiple sources into a single model."""
+"""This file provides the ability to combine vulnerabilities from multiple sources into a single model"""
 # This file is part of hoppr-cop
 #
 # Licensed under the MIT License;
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://opensource.org/licenses/MIT
@@ -11,109 +11,128 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # Copyright (c) 2022 Lockheed Martin Corporation
-from __future__ import annotations
+from typing import List, Optional, Dict
 
-from typing import TYPE_CHECKING
+from hoppr_cyclonedx_models.cyclonedx_1_4 import Vulnerability
 
 
-if TYPE_CHECKING:
-    from hoppr_cyclonedx_models.cyclonedx_1_4 import Vulnerability
-
-
-def __get_all_ids_from_vulnerability(from_vulnerability: Vulnerability) -> list[str]:
-    ids = list(filter(None, [from_vulnerability.id]))
-
+def __get_all_ids_from_vulnerability(from_vulnerability: Vulnerability):
+    ids = [from_vulnerability.id]
     if from_vulnerability.references is not None:
-        ids.extend(reference.id for reference in from_vulnerability.references)
-
+        for reference in from_vulnerability.references:
+            ids.append(reference.id)
     return list(set(ids))
 
 
-def __combine_vulnerabilities(existing: Vulnerability, new: Vulnerability) -> Vulnerability:
+def __combine_vunerabilities(
+    existing: Vulnerability, new: Vulnerability
+) -> Vulnerability:
+
+    # pylint: disable=cell-var-from-loop
+
     if existing.cwes is None or len(existing.cwes) == 0:
         existing.cwes = new.cwes
 
-    # Combine advisories
-    existing.advisories = existing.advisories or []
-    new.advisories = new.advisories or []
-
-    existing.advisories = list(
-        {advisory.url: advisory for advisory in [*existing.advisories, *new.advisories]}.values(),
-    )
+    ## Combine advisories
+    if existing.advisories is None and new.advisories is not None:
+        existing.advisories = new.advisories
+    elif new.advisories is not None:
+        existing_urls = list(map(lambda x: x.url, existing.advisories))
+        new_advisories = list(
+            filter(lambda x: x.url not in existing_urls, new.advisories)
+        )
+        existing.advisories = existing.advisories + new_advisories
 
     # Combine Tools
-    existing.tools = existing.tools or []
-    new.tools = new.tools or []
-
-    existing.tools = list({tool.name: tool for tool in [*existing.tools, *new.tools]}.values())
+    existing.tools = [] if existing.tools is None else existing.tools
+    if new.tools is not None:
+        existing_tool_names = list(map(lambda x: x.name, existing.tools))
+        new_tools = list(filter(lambda x: x.name not in existing_tool_names, new.tools))
+        existing.tools = new_tools + existing.tools
 
     # Combine Ratings
-    existing.ratings = existing.ratings or []
-    new.ratings = new.ratings or []
-
-    existing_reference_ids = [x.vector for x in existing.ratings]
-    existing.ratings.extend(rating for rating in new.ratings if rating.vector not in existing_reference_ids)
-
-    for new_rating in [rating for rating in new.ratings if rating.source is not None]:
-        existing_rating = next(ex_rtng for ex_rtng in existing.ratings if ex_rtng.vector == new_rating.vector)
-
-        if existing_rating and (not existing_rating.source or not existing_rating.source.name):
-            existing_rating.source = new_rating.source
+    existing.ratings = [] if existing.ratings is None else existing.ratings
+    if new.ratings is not None:
+        existing_reference_ids = list(map(lambda x: str(x.vector), existing.ratings))
+        new_ratings = list(
+            filter(lambda x: str(x.vector) not in existing_reference_ids, new.ratings)
+        )
+        existing.ratings = new_ratings + existing.ratings
+        for rating in new.ratings:
+            if rating.source is not None:
+                existing_rating = list(
+                    filter(lambda x: x.vector == rating.vector, existing.ratings)
+                )[0]
+                if (
+                    existing_rating.source is None
+                    or existing_rating.source.name is None
+                ):
+                    existing_rating.source = rating.source
 
     # Combine References
-    existing.references = existing.references or []
-    new.references = new.references or []
-
-    existing.references = list({ref.id: ref for ref in [*existing.references, *new.references]}.values())
+    existing.references = [] if existing.references is None else existing.references
+    if new.references is not None:
+        existing_reference_ids = list(map(lambda x: str(x.id), existing.references))
+        new_references = list(
+            filter(lambda x: str(x.id) not in existing_reference_ids, new.references)
+        )
+        existing.references = new_references + existing.references
 
     # Combine Recommendation
-    existing.recommendation = existing.recommendation or ""
-
-    if new.recommendation:
-        existing.recommendation = f"{existing.recommendation}.  ||  {new.recommendation}"
+    existing.recommendation = (
+        "" if existing.recommendation is None else existing.recommendation
+    )
+    if new.recommendation is not None and new.recommendation != "":
+        existing.recommendation = (
+            f"{existing.recommendation}.  ||  {new.recommendation}"
+        )
 
     return existing
 
 
-def __does_id_exist_in_both(existing_id_list: list[str], new_id_list: list[str]) -> bool:
-    return len([value for value in existing_id_list if value in new_id_list]) > 0
+def __does_id_exist_in_both(
+    existing_id_list: List[str], new_id_list: List[str]
+) -> bool:
+    length = len([value for value in existing_id_list if value in new_id_list]) > 0
+
+    return length
 
 
 def __get_matching_vulnerability_from_list(
-    combined_list: list[Vulnerability], new_finding: Vulnerability
-) -> Vulnerability | None:
+    combined_list: List[Vulnerability], new_finding: Vulnerability
+) -> Optional[Vulnerability]:
     new_finding_ids = __get_all_ids_from_vulnerability(new_finding)
     for vuln in combined_list:
         existing_finding_ids = __get_all_ids_from_vulnerability(vuln)
+        # if "CVE-2021-23926" in existing_finding_ids or "CVE-2021-23926" in new_finding_ids:
+        #     print(f"{existing_finding_ids} new = {new_finding_ids}  in both = {__does_id_exist_in_both(existing_finding_ids, new_finding_ids)}")
 
         if __does_id_exist_in_both(existing_finding_ids, new_finding_ids):
             return vuln
-
     return None
 
 
 def combine_vulnerabilities(
-    vulnerabilities_list: list[dict[str, list[Vulnerability] | None]],
-) -> dict[str, list[Vulnerability]]:
-    """Intelligently combines the lists of vulnerabilities found by different scanners."""
-    combined_result: dict[str, list[Vulnerability]] = {}
-
+    vulnerabilities_list: List[Dict[str, Optional[List[Vulnerability]]]]
+) -> Dict[str, Optional[List[Vulnerability]]]:
+    """Intelligently combines the lists of vulnerabilities found by different scanners"""
+    combined_result = {}
     for result in vulnerabilities_list:
         for purl in result:
-            tool_vulnerabilities = result.get(purl)
-
+            tool_vulnerabilities = result[purl]
             if purl not in combined_result:
                 combined_result[purl] = []
 
-            for vulnerability in tool_vulnerabilities or []:
-                existing = __get_matching_vulnerability_from_list(combined_result[purl], vulnerability)
-
-                combined_result[purl].append(
-                    __combine_vulnerabilities(existing, vulnerability) if existing else vulnerability,
+            for vulnerability in tool_vulnerabilities:
+                exisiting = __get_matching_vulnerability_from_list(
+                    combined_result[purl], vulnerability
                 )
-
+                if exisiting is None:
+                    combined_result[purl].append(vulnerability)
+                else:
+                    __combine_vunerabilities(exisiting, vulnerability)
     return combined_result
```

### Comparing `hoppr_security_commons-0.0.83/hoppr_security_commons/vulnerability_scanner.py` & `hoppr_security_commons-0.0.9/security_commons/common/vulnerability_scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Defines the common interface for a vulnerability scanner."""
+"""Defines the common interface for a vulnerability scanner"""
 # This file is part of hoppr-cop
 #
 # Licensed under the MIT License;
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://opensource.org/licenses/MIT
@@ -11,95 +11,82 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # Copyright (c) 2022 Lockheed Martin Corporation
-from __future__ import annotations
-
+# pylint: disable=deprecated-module
 import distutils.spawn
 import os
-
-from typing import TYPE_CHECKING, ClassVar
+from typing import Optional, Union
 
 import typer
-
+from hoppr_cyclonedx_models.cyclonedx_1_3 import (
+    CyclonedxSoftwareBillOfMaterialSpecification as Bom_1_3,
+)
+from hoppr_cyclonedx_models.cyclonedx_1_4 import (
+    CyclonedxSoftwareBillOfMaterialsStandard as Bom_1_4,
+)
+from hoppr_cyclonedx_models.cyclonedx_1_4 import Vulnerability
 from packageurl import PackageURL
 
 
-if TYPE_CHECKING:
-    from hoppr_cyclonedx_models.cyclonedx_1_3 import (
-        CyclonedxSoftwareBillOfMaterialSpecification as Bom_1_3,
-    )
-    from hoppr_cyclonedx_models.cyclonedx_1_4 import (
-        CyclonedxSoftwareBillOfMaterialsStandard as Bom_1_4,
-        Vulnerability,
-    )
-
-
 class VulnerabilityMeta(type):
-    """a meta class to define interface expectations of a vulnerability scanner."""
+    """a meta class to define interface expectations of a vulnerability scanner"""
 
-    @classmethod
-    def __instancecheck__(cls, instance: object) -> bool:
+    def __instancecheck__(cls, instance):
+        # pylint: disable=no-value-for-parameter
         return cls.__subclasscheck__(type(instance))
 
-    @classmethod
-    def __subclasscheck__(cls, subclass: type) -> bool:
+    def __subclasscheck__(cls, subclass):
         return (
             hasattr(subclass, "get_vulnerabilities_by_purl")
             and callable(subclass.get_vulnerabilities_by_purl)
             and hasattr(subclass, "get_vulnerabilities_by_sbom")
             and callable(subclass.get_vulnerabilities_by_sbom)
             and hasattr(subclass, "should_activate")
             and callable(subclass.should_activate)
         )
 
 
 class VulnerabilitySuper(metaclass=VulnerabilityMeta):
-    """A super class that defines the expected interface for a vulnerability scanner."""
-
-    required_tools_on_path: ClassVar[list[str]] = []
-    required_environment_variables: ClassVar[list[str]] = []
-    offline_mode_supported = False
-    offline_mode = False
+    """A super class that defines the expected interface for a vulnerability scanner"""
 
-    def get_vulnerabilities_by_purl(self, purls: list[PackageURL]) -> dict[str, list[Vulnerability] | None]:
-        """Get the vulnerabilities for a list of package URLS (purls).
+    required_tools_on_path = []
+    required_environment_variables = []
 
-        Return a dictionary of package URL to vulnerabilities or none if no vulnerabilities are found.
+    def get_vulnerabilities_by_purl(
+        self, purls: list[PackageURL]
+    ) -> dict[str, Optional[list[Vulnerability]]]:
+        """Get the vulnerabilities for a list of package URLS (purls)
+        This function will return a dictionary of package URL to vulnerabilities or none if no vulnerabilities are found
         """
-        return {}
 
-    def get_vulnerabilities_by_sbom(self, bom: Bom_1_4 | Bom_1_3) -> dict[str, list[Vulnerability] | None]:
-        """Accepts a cyclone dx compatible BOM and returns a list of vulnerabilities.
-
-        Return a dictionary of package URL to vulnerabilities or none if no vulnerabilities are found.
+    def get_vulnerabilities_by_sbom(
+        self, bom: [Union[Bom_1_4, Bom_1_3]]
+    ) -> dict[str, Optional[list[Vulnerability]]]:
+        """Accepts a cyclone dx compatible BOM and returns a list of vulnerabilities "
+        This function will return a dictionary of package URL to vulnerabilities or none if no vulnerabilities are found
         """
-        purls = [
-            PackageURL.from_string(component.purl)
-            for component in bom.components or []
-            if component.purl is not None and component.purl != ""
-        ]
-
+        purls = []
+        for component in bom.components:
+            if component.purl is not None and component.purl != "":
+                purls.append(PackageURL.from_string(component.purl))
         return self.get_vulnerabilities_by_purl(purls)
 
     def should_activate(self) -> bool:
-        """Checks if the vulnerability scanner should activate based on it's requirements."""
+        """checks if the vulnerability scanner should activate based on it's requirements"""
         activate = True
         for tool in self.required_tools_on_path:
             if not distutils.spawn.find_executable(tool):
                 activate = False
-                typer.echo(f"{type(self).__name__} is not activated because {tool} is not on the PATH")
+                typer.echo(
+                    f"{type(self).__name__} is not activated because {tool} is not on the PATH"
+                )
         for env in self.required_environment_variables:
             if env not in os.environ:
                 activate = False
                 typer.echo(
-                    f"{type(self).__name__} is not activated because required environment variable {env} is not set",
+                    f"{type(self).__name__} is not activated because required environment variable {env} is not set"
                 )
-
-        if self.offline_mode and not self.offline_mode_supported:
-            activate = False
-            typer.echo(f"{type(self).__name__} is not activated because offline mode is not supported by this scanner")
-
         return activate
```

### Comparing `hoppr_security_commons-0.0.83/PKG-INFO` & `hoppr_security_commons-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: hoppr-security-commons
-Version: 0.0.83
+Version: 0.0.9
 Summary: Common Library For hoppr-cop
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hoppr-cyclonedx-models (==0.*)
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: packageurl-python (==0.*)
-Requires-Dist: requests (>=2.29.0,<3.0.0)
-Requires-Dist: tabulate (==0.*)
-Requires-Dist: typer (==0.*)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: cvss (>=2.5,<3.0)
+Requires-Dist: hoppr-cyclonedx-models (>=0.3.0,<0.4.0)
+Requires-Dist: packageurl-python (>=0.10.1,<0.11.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tinydb (>=4.7.0,<5.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
```

