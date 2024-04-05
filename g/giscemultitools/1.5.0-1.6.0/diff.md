# Comparing `tmp/giscemultitools-1.5.0.tar.gz` & `tmp/giscemultitools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giscemultitools-1.5.0.tar", last modified: Tue Mar  5 08:58:56 2024, max compression
+gzip compressed data, was "giscemultitools-1.6.0.tar", last modified: Fri Apr  5 12:12:07 2024, max compression
```

## Comparing `giscemultitools-1.5.0.tar` & `giscemultitools-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/giscemultitools/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/giscemultitools/githubutils/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/githubutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/githubutils/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/giscemultitools/githubutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/githubutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/githubutils/scripts/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/githubutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/giscemultitools/slackutils/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/slackutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/giscemultitools/slackutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/slackutils/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/slackutils/scripts/slack_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/giscemultitools/slackutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/giscemultitools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-05 08:58:56.000000 giscemultitools-1.5.0/giscemultitools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-05 08:58:56.000000 giscemultitools-1.5.0/giscemultitools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 08:58:56.000000 giscemultitools-1.5.0/giscemultitools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-05 08:58:56.000000 giscemultitools-1.5.0/giscemultitools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-05 08:58:56.000000 giscemultitools-1.5.0/giscemultitools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-05 08:58:56.000000 giscemultitools-1.5.0/giscemultitools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 08:58:56.062219 giscemultitools-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-05 08:58:52.000000 giscemultitools-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/giscemultitools/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/giscemultitools/githubutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/githubutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/githubutils/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/giscemultitools/githubutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/githubutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/githubutils/scripts/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/githubutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/giscemultitools/slackutils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/slackutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/giscemultitools/slackutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/slackutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/slackutils/scripts/slack_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/giscemultitools/slackutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/giscemultitools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 12:12:07.000000 giscemultitools-1.6.0/giscemultitools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-05 12:12:07.000000 giscemultitools-1.6.0/giscemultitools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:12:07.000000 giscemultitools-1.6.0/giscemultitools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-05 12:12:07.000000 giscemultitools-1.6.0/giscemultitools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 12:12:07.000000 giscemultitools-1.6.0/giscemultitools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 12:12:07.000000 giscemultitools-1.6.0/giscemultitools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:12:07.794021 giscemultitools-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 12:12:03.000000 giscemultitools-1.6.0/setup.py
```

### Comparing `giscemultitools-1.5.0/giscemultitools/githubutils/objects.py` & `giscemultitools-1.6.0/giscemultitools/githubutils/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,15 @@
 
     def get_pull_request_projects_and_commits(self, pull_request_number):
         # mergeCommit.oid is the hash
         query = """
             query {
                 repository(owner: "%s", name: "%s") {
                     pullRequest(number: %s) {
+                        id
                         baseRefName
                         number
                         state
                         url
                         title
                         mergedAt
                         createdAt
@@ -289,14 +290,26 @@
                   }
                 }
             }
 
         """ % (project_id, item_id, field_column_id, value)
         return self._graphql_request(dumps({'query': query}))
 
+    def add_item_to_project_v2(self, project_id, item_id):
+        query = """
+            mutation {
+              addProjectV2ItemById(input: {projectId: "%s", contentId: "%s"}) {
+                item {
+                  id
+                }
+              }
+            }
+        """ % (project_id, item_id)
+        return self._graphql_request(dumps({'query': query}))
+
     def get_pr_checks(self, pull_request_number):
         query = """
             query {
               repository(owner: "%s", name: "%s") {
                 pullRequest(number: %s) {
                   commits(last: 1) {
                     nodes {
```

### Comparing `giscemultitools-1.5.0/giscemultitools/githubutils/scripts/github_cli.py` & `giscemultitools-1.6.0/giscemultitools/githubutils/scripts/github_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,14 +94,36 @@
 @click.option("--value", help="Text value", required=True, type=click.STRING)
 def update_projectv2_card_from_id(owner, repository, project_id, item_id, field_id, value):
     from giscemultitools.githubutils.utils import GithubUtils
     res = GithubUtils.update_projectv2_item_field_value(owner, repository, project_id, item_id, field_id, value)
     print(dumps(res))
 
 
+@click.command('add-item-to-projectv2')
+@click.option('--owner', help='GitHub owner name', default='gisce', show_default=True)
+@click.option('--repository', help='GitHub repository name', default='erp', show_default=True)
+@click.option("--project-id", help="Project ID", required=True, type=click.STRING)
+@click.option("--item-id", help="Item ID", required=True, type=click.STRING)
+def add_item_to_projectv2(owner, repository, project_id, item_id):
+    from giscemultitools.githubutils.utils import GithubUtils
+    res = GithubUtils.add_item_to_project(owner, repository, project_id, item_id)
+    print(dumps(res))
+
+
+@click.command('add-prs-to-projectv2')
+@click.option('--owner', help='GitHub owner name', default='gisce', show_default=True)
+@click.option('--repository', help='GitHub repository name', default='erp', show_default=True)
+@click.option("--project-name", help="Project name", required=True, type=click.STRING)
+@click.option("--prs", help="List of prs separated", required=True, type=click.STRING)
+def add_prs_to_projectv2(owner, repository, project_name, prs):
+    prs = [_pr.replace(' ', '') for _pr in prs.split(',')]
+    from giscemultitools.githubutils.utils import GithubUtils
+    GithubUtils.add_prs_to_project_by_name(owner, repository, project_name, prs)
+
+
 @click.command('project-changelog')
 @click.option('--owner', help='GitHub owner name', default='gisce', show_default=True)
 @click.option('--repository', help='GitHub repository name', default='erp', show_default=True)
 @click.option("--project-name", help="Project ID", required=True, type=click.STRING)
 @click.option('--date-since', help='Change log date from ex. 2022-12-27', default=None, show_default=True, type=click.STRING)
 def project_changelog(owner, repository, project_name, date_since):
     from giscemultitools.githubutils.utils import GithubUtils
@@ -152,11 +174,13 @@
 github_cli.add_command(get_pullrequest_checks)
 github_cli.add_command(get_pr_from_sha_merge_commit)
 github_cli.add_command(get_pullrequest_check_status)
 github_cli.add_command(get_pullrequest_context_checks)
 github_cli.add_command(get_pullrequest_context_check_status)
 github_cli.add_command(get_pullrequests_from_project_by_status)
 github_cli.add_command(get_pullrequests_commits_from_project_by_status)
+github_cli.add_command(add_item_to_projectv2)
+github_cli.add_command(add_prs_to_projectv2)
 
 
 if __name__ == "__main__":
     github_cli()
```

### Comparing `giscemultitools-1.5.0/giscemultitools/githubutils/utils.py` & `giscemultitools-1.6.0/giscemultitools/githubutils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     @staticmethod
     def plain_get_commits_sha_from_merge_commit(response):
         res = {
             'commits': [
                 commit['commit']['oid'] for commit in response['data']['repository']['pullRequest']['commits']['nodes']
             ],
             'pullRequest': {
+                'id': response['data']['repository']['pullRequest']['id'],
                 'number': response['data']['repository']['pullRequest']['number'],
                 'state': response['data']['repository']['pullRequest']['state'],
                 'milestone': response['data']['repository']['pullRequest']['milestone'] and response['data']['repository']['pullRequest']['milestone']['title'] or '',
                 'url': response['data']['repository']['pullRequest']['url'],
                 'title': response['data']['repository']['pullRequest']['title'],
                 'baseRefName': response['data']['repository']['pullRequest']['baseRefName'],
                 'mergedAt': response['data']['repository']['pullRequest']['mergedAt'],
@@ -154,24 +155,46 @@
     @staticmethod
     def update_projectv2_item_field_value(owner, repository, project_id, item_id, field_column_id, value):
         from .objects import GHAPIRequester
         requester = GHAPIRequester(owner, repository)
         return requester.update_projectv2_item_field_value(project_id, item_id, field_column_id, value)
 
     @staticmethod
+    def add_item_to_project(owner, repository, project_id, item_id):
+        from .objects import GHAPIRequester
+        requester = GHAPIRequester(owner, repository)
+        return requester.add_item_to_project_v2(project_id, item_id)
+
+    @staticmethod
+    def add_prs_to_project_by_name(owner, repository, project_name, prs_list):
+        from giscemultitools.githubutils.objects import GHAPIRequester
+        requester = GHAPIRequester(owner, repository)
+        res = requester.get_project_info_from_project_name(project_name, only_one=True)
+        project_id = res['id']
+        for _pr in prs_list:
+            human_pr = GithubUtils.plain_get_commits_sha_from_merge_commit(
+                requester.get_pull_request_projects_and_commits(_pr)
+            )
+            pr_id = human_pr['pullRequest']['id']
+            if project_id not in [x['project_id'] for x in human_pr['projectItems']]:
+                res = GithubUtils.add_item_to_project(owner, repository, project_id, pr_id)
+                print('Added {} to project {}'.format(_pr, project_name))
+            else:
+                print('{} already in project {}'.format(_pr, project_name))
+
+    @staticmethod
     def get_pulls_from_project_and_column(owner, repository, project_name, card_status):
         from .objects import GHAPIRequester
         requester = GHAPIRequester(owner, repository)
         res = []
         for _pr_state in ('merged', 'open'):
             included_prs = requester.get_pulls_from_project(project_name, pr_states=(_pr_state,), project_status=(card_status,))
             res.extend(included_prs)
         return res
 
-
     @staticmethod
     def project_changelog(
             owner, repository, project_name,
             categories=('comer', 'distri'),
             sub_categories=('Eléctrico', 'Gas', 'oficinavirtual'),
             top_labels=('ATR', 'facturacio', 'core', 'GIS', 'medidas'),
             skip_labels=('custom',),
```

### Comparing `giscemultitools-1.5.0/giscemultitools/slackutils/scripts/slack_cli.py` & `giscemultitools-1.6.0/giscemultitools/slackutils/scripts/slack_cli.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.5.0/giscemultitools/slackutils/utils.py` & `giscemultitools-1.6.0/giscemultitools/slackutils/utils.py`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.5.0/giscemultitools.egg-info/SOURCES.txt` & `giscemultitools-1.6.0/giscemultitools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giscemultitools-1.5.0/setup.py` & `giscemultitools-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     name='giscemultitools',
     description='Llibreria d\'utilitats',
     author='GISCE',
     author_email='devel@gisce.net',
     url='http://www.gisce.net',
-    version='1.5.0',
+    version='1.6.0',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['giscemultitools'],
     install_requires=[
         "requests",
         "click"
     ],
```

