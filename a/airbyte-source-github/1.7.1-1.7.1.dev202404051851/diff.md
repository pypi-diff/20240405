# Comparing `tmp/airbyte_source_github-1.7.1.tar.gz` & `tmp/airbyte_source_github-1.7.1.dev202404051851.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_github-1.7.1.tar", max compression
+gzip compressed data, was "airbyte_source_github-1.7.1.dev202404051851.tar", max compression
```

## Comparing `airbyte_source_github-1.7.1.tar` & `airbyte_source_github-1.7.1.dev202404051851.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     4496 2024-03-26 18:36:58.177088 airbyte_source_github-1.7.1/README.md
--rw-r--r--   0        0        0      797 2024-03-26 18:40:11.543877 airbyte_source_github-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1134 2024-03-26 18:36:58.181088 airbyte_source_github-1.7.1/source_github/__init__.py
--rw-r--r--   0        0        0     3849 2024-03-26 18:36:58.181088 airbyte_source_github-1.7.1/source_github/config_migrations.py
--rw-r--r--   0        0        0      238 2024-03-26 18:36:58.181088 airbyte_source_github-1.7.1/source_github/constants.py
--rw-r--r--   0        0        0  1600314 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/github_schema.py
--rw-r--r--   0        0        0    11625 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/graphql.py
--rw-r--r--   0        0        0      407 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/run.py
--rw-r--r--   0        0        0     1232 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/assignees.json
--rw-r--r--   0        0        0     1487 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/branches.json
--rw-r--r--   0        0        0     1724 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/collaborators.json
--rw-r--r--   0        0        0     2191 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/comments.json
--rw-r--r--   0        0        0       87 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/commit_comment_reactions.json
--rw-r--r--   0        0        0      984 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/commit_comments.json
--rw-r--r--   0        0        0     2772 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/commits.json
--rw-r--r--   0        0        0     2348 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/contributor_activity.json
--rw-r--r--   0        0        0     1478 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/deployments.json
--rw-r--r--   0        0        0     1228 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/events.json
--rw-r--r--   0        0        0       87 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issue_comment_reactions.json
--rw-r--r--   0        0        0    10180 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issue_events.json
--rw-r--r--   0        0        0      543 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issue_labels.json
--rw-r--r--   0        0        0     1168 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issue_milestones.json
--rw-r--r--   0        0        0      516 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issue_reactions.json
--rw-r--r--   0        0        0    26850 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issue_timeline_events.json
--rw-r--r--   0        0        0     6210 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/issues.json
--rw-r--r--   0        0        0     4605 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/organizations.json
--rw-r--r--   0        0        0      910 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/project_cards.json
--rw-r--r--   0        0        0      698 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/project_columns.json
--rw-r--r--   0        0        0      921 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/projects.json
--rw-r--r--   0        0        0     1608 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/projects_v2.json
--rw-r--r--   0        0        0      504 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/pull_request_comment_reactions.json
--rw-r--r--   0        0        0     2619 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/pull_request_commits.json
--rw-r--r--   0        0        0     1717 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/pull_request_stats.json
--rw-r--r--   0        0        0     8128 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/pull_requests.json
--rw-r--r--   0        0        0     2682 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/releases.json
--rw-r--r--   0        0        0     6878 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/repositories.json
--rw-r--r--   0        0        0     2394 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/review_comments.json
--rw-r--r--   0        0        0     1374 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/reviews.json
--rw-r--r--   0        0        0     7387 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/events/comment.json
--rw-r--r--   0        0        0     4197 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/events/commented.json
--rw-r--r--   0        0        0     1443 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/events/committed.json
--rw-r--r--   0        0        0    36914 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/events/cross_referenced.json
--rw-r--r--   0        0        0     2764 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/events/reviewed.json
--rw-r--r--   0        0        0      449 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/reaction.json
--rw-r--r--   0        0        0      616 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/reactions.json
--rw-r--r--   0        0        0     1135 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/user.json
--rw-r--r--   0        0        0      453 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/shared/user_graphql.json
--rw-r--r--   0        0        0      336 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/stargazers.json
--rw-r--r--   0        0        0      601 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/tags.json
--rw-r--r--   0        0        0     1273 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/team_members.json
--rw-r--r--   0        0        0      403 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/team_memberships.json
--rw-r--r--   0        0        0      984 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/teams.json
--rw-r--r--   0        0        0     1254 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/users.json
--rw-r--r--   0        0        0     2089 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/workflow_jobs.json
--rw-r--r--   0        0        0    10171 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/workflow_runs.json
--rw-r--r--   0        0        0      753 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/schemas/workflows.json
--rw-r--r--   0        0        0    13879 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/source.py
--rw-r--r--   0        0        0     7074 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/spec.json
--rw-r--r--   0        0        0    77006 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/streams.py
--rw-r--r--   0        0        0     5462 2024-03-26 18:36:58.185088 airbyte_source_github-1.7.1/source_github/utils.py
--rw-r--r--   0        0        0     5228 1970-01-01 00:00:00.000000 airbyte_source_github-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     4496 2024-04-05 18:49:00.394111 airbyte_source_github-1.7.1.dev202404051851/README.md
+-rw-r--r--   0        0        0      817 2024-04-05 18:51:34.161467 airbyte_source_github-1.7.1.dev202404051851/pyproject.toml
+-rw-r--r--   0        0        0     1134 2024-04-05 18:49:00.398111 airbyte_source_github-1.7.1.dev202404051851/source_github/__init__.py
+-rw-r--r--   0        0        0     3849 2024-04-05 18:49:00.398111 airbyte_source_github-1.7.1.dev202404051851/source_github/config_migrations.py
+-rw-r--r--   0        0        0      238 2024-04-05 18:49:00.398111 airbyte_source_github-1.7.1.dev202404051851/source_github/constants.py
+-rw-r--r--   0        0        0  1600314 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/github_schema.py
+-rw-r--r--   0        0        0    11625 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/graphql.py
+-rw-r--r--   0        0        0      407 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/run.py
+-rw-r--r--   0        0        0     1232 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/assignees.json
+-rw-r--r--   0        0        0     1487 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/branches.json
+-rw-r--r--   0        0        0     1724 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/collaborators.json
+-rw-r--r--   0        0        0     2191 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/comments.json
+-rw-r--r--   0        0        0       87 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/commit_comment_reactions.json
+-rw-r--r--   0        0        0      984 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/commit_comments.json
+-rw-r--r--   0        0        0     2772 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/commits.json
+-rw-r--r--   0        0        0     2348 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/contributor_activity.json
+-rw-r--r--   0        0        0     1478 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/deployments.json
+-rw-r--r--   0        0        0     1228 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/events.json
+-rw-r--r--   0        0        0       87 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_comment_reactions.json
+-rw-r--r--   0        0        0    10180 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_events.json
+-rw-r--r--   0        0        0      543 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_labels.json
+-rw-r--r--   0        0        0     1168 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_milestones.json
+-rw-r--r--   0        0        0      516 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_reactions.json
+-rw-r--r--   0        0        0    26850 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_timeline_events.json
+-rw-r--r--   0        0        0     6210 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issues.json
+-rw-r--r--   0        0        0     4605 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/organizations.json
+-rw-r--r--   0        0        0      910 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/project_cards.json
+-rw-r--r--   0        0        0      698 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/project_columns.json
+-rw-r--r--   0        0        0      921 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/projects.json
+-rw-r--r--   0        0        0     1608 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/projects_v2.json
+-rw-r--r--   0        0        0      504 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_request_comment_reactions.json
+-rw-r--r--   0        0        0     2619 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_request_commits.json
+-rw-r--r--   0        0        0     1717 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_request_stats.json
+-rw-r--r--   0        0        0     8128 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_requests.json
+-rw-r--r--   0        0        0     2682 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/releases.json
+-rw-r--r--   0        0        0     6878 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/repositories.json
+-rw-r--r--   0        0        0     2394 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/review_comments.json
+-rw-r--r--   0        0        0     1374 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/reviews.json
+-rw-r--r--   0        0        0     7387 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/comment.json
+-rw-r--r--   0        0        0     4197 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/commented.json
+-rw-r--r--   0        0        0     1443 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/committed.json
+-rw-r--r--   0        0        0    36914 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/cross_referenced.json
+-rw-r--r--   0        0        0     2764 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/reviewed.json
+-rw-r--r--   0        0        0      449 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/reaction.json
+-rw-r--r--   0        0        0      616 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/reactions.json
+-rw-r--r--   0        0        0     1135 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/user.json
+-rw-r--r--   0        0        0      453 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/user_graphql.json
+-rw-r--r--   0        0        0      336 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/stargazers.json
+-rw-r--r--   0        0        0      601 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/tags.json
+-rw-r--r--   0        0        0     1273 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/team_members.json
+-rw-r--r--   0        0        0      403 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/team_memberships.json
+-rw-r--r--   0        0        0      984 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/teams.json
+-rw-r--r--   0        0        0     1254 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/users.json
+-rw-r--r--   0        0        0     2089 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/workflow_jobs.json
+-rw-r--r--   0        0        0    10171 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/workflow_runs.json
+-rw-r--r--   0        0        0      753 2024-04-05 18:49:00.402111 airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/workflows.json
+-rw-r--r--   0        0        0    13879 2024-04-05 18:49:00.406111 airbyte_source_github-1.7.1.dev202404051851/source_github/source.py
+-rw-r--r--   0        0        0     7074 2024-04-05 18:49:00.406111 airbyte_source_github-1.7.1.dev202404051851/source_github/spec.json
+-rw-r--r--   0        0        0    77006 2024-04-05 18:49:00.406111 airbyte_source_github-1.7.1.dev202404051851/source_github/streams.py
+-rw-r--r--   0        0        0     5462 2024-04-05 18:49:00.406111 airbyte_source_github-1.7.1.dev202404051851/source_github/utils.py
+-rw-r--r--   0        0        0     5246 1970-01-01 00:00:00.000000 airbyte_source_github-1.7.1.dev202404051851/PKG-INFO
```

### Comparing `airbyte_source_github-1.7.1/README.md` & `airbyte_source_github-1.7.1.dev202404051851/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/pyproject.toml` & `airbyte_source_github-1.7.1.dev202404051851/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.7.1"
+version = "1.7.1.dev202404051851"
 name = "airbyte-source-github"
 description = "Source implementation for GitHub."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_github" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.72.1"
 sgqlc = "==16.3"
 
 [tool.poetry.scripts]
 source-github = "source_github.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
```

### Comparing `airbyte_source_github-1.7.1/source_github/__init__.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/config_migrations.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/github_schema.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/github_schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/graphql.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/assignees.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/assignees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/branches.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/branches.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/collaborators.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/collaborators.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/comments.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/commit_comments.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/commit_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/commits.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/contributor_activity.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/contributor_activity.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/deployments.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/deployments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/events.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/issue_events.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/issue_labels.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/issue_milestones.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_milestones.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/issue_reactions.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/issue_timeline_events.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issue_timeline_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/issues.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/organizations.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/project_cards.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/project_cards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/project_columns.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/project_columns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/projects.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/projects_v2.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/projects_v2.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/pull_request_commits.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_request_commits.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/pull_request_stats.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_request_stats.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/pull_requests.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/pull_requests.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/releases.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/releases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/repositories.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/repositories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/review_comments.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/review_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/reviews.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/events/comment.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/comment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/events/commented.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/commented.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/events/committed.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/committed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/events/cross_referenced.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/cross_referenced.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/events/reviewed.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/events/reviewed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/reactions.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/reactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/shared/user.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/tags.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/tags.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/team_members.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/team_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/teams.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/users.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/workflow_jobs.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/workflow_jobs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/workflow_runs.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/workflow_runs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/schemas/workflows.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/source.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/spec.json` & `airbyte_source_github-1.7.1.dev202404051851/source_github/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/streams.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/source_github/utils.py` & `airbyte_source_github-1.7.1.dev202404051851/source_github/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_github-1.7.1/PKG-INFO` & `airbyte_source_github-1.7.1.dev202404051851/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-github
-Version: 1.7.1
+Version: 1.7.1.dev202404051851
 Summary: Source implementation for GitHub.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.72.1)
 Requires-Dist: sgqlc (==16.3)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/github
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Github source connector
```

