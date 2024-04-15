# Comparing `tmp/issx-0.1.0.tar.gz` & `tmp/issx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.1.0.tar", max compression
+gzip compressed data, was "issx-0.2.0.tar", max compression
```

## Comparing `issx-0.1.0.tar` & `issx-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1101 2024-04-14 20:28:03.222558 issx-0.1.0/LICENCE
--rw-r--r--   0        0        0     4817 2024-04-14 20:28:03.222558 issx-0.1.0/README.md
--rw-r--r--   0        0        0     3102 2024-04-14 20:28:03.222558 issx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/__init__.py
--rw-r--r--   0        0        0     3917 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/cli.py
--rw-r--r--   0        0        0      200 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/clients/__init__.py
--rw-r--r--   0        0        0      317 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/clients/exceptions.py
--rw-r--r--   0        0        0     2800 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0     1547 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0     2865 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/clients/redmine.py
--rw-r--r--   0        0        0        0 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/domain/__init__.py
--rw-r--r--   0        0        0      205 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/domain/issues.py
--rw-r--r--   0        0        0     2442 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/instance_managers.py
--rw-r--r--   0        0        0        0 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/py.typed
--rw-r--r--   0        0        0     1390 2024-04-14 20:28:03.222558 issx-0.1.0/src/issx/services.py
--rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 issx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-15 20:46:01.645835 issx-0.2.0/LICENCE
+-rw-r--r--   0        0        0     4817 2024-04-15 20:46:01.645835 issx-0.2.0/README.md
+-rw-r--r--   0        0        0     3102 2024-04-15 20:46:01.645835 issx-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/__init__.py
+-rw-r--r--   0        0        0     4342 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/cli.py
+-rw-r--r--   0        0        0      200 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     3206 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     1797 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     3352 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/domain/issues.py
+-rw-r--r--   0        0        0     2442 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/instance_managers.py
+-rw-r--r--   0        0        0        0 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/py.typed
+-rw-r--r--   0        0        0     2200 2024-04-15 20:46:01.645835 issx-0.2.0/src/issx/services.py
+-rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 issx-0.2.0/PKG-INFO
```

### Comparing `issx-0.1.0/LICENCE` & `issx-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.1.0/README.md` & `issx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `issx-0.1.0/pyproject.toml` & `issx-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.1.0"
+version = "0.2.0"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `issx-0.1.0/src/issx/cli.py` & `issx-0.2.0/src/issx/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,14 +57,24 @@
         typer.Option(
             "--description-format",
             "-D",
             help="Template of a new issue description. Can contain placeholders of the"
             " issue attributes: {id}, {title}, {description}, {web_url}, {reference}",
         ),
     ] = "{description}",
+    allow_duplicates: Annotated[
+        bool,
+        typer.Option(
+            "--allow-duplicates",
+            "-A",
+            help="Allow for duplicate issues. If set, the command will return the first"
+            " issue found with the same title. If no issues are found,"
+            " a new issue will be created.",
+        ),
+    ] = False,
 ) -> int:
     console.print(
         Text.assemble(
             f"Copying issue {issue_id} from project ",
             (source_project_name, "bold magenta"),
             " to project ",
             (target_project_name, "bold magenta"),
@@ -77,15 +87,18 @@
         target_client = instance_manager.get_project_client(target_project_name)
     except Exception as e:
         console.print_exception()
         console.print("Error when configuring client instance.\n", style="red")
         raise typer.Exit(1) from e
     new_issue = asyncio.run(
         CopyIssueService(source_client, target_client).copy(
-            issue_id, title_format, description_format
+            issue_id,
+            title_format,
+            description_format,
+            allow_duplicates=allow_duplicates,
         )
     )
     console.print(f"Success!\n{new_issue}", style="green")
     return 0
 
 
 @app.command()
```

### Comparing `issx-0.1.0/src/issx/clients/gitlab.py` & `issx-0.2.0/src/issx/clients/gitlab.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,18 @@
             id=issue.iid,
             title=issue.title,
             description=issue.description,
             web_url=issue.web_url,
             reference=issue.references["full"],
         )
 
+    @classmethod
+    def issues_to_domain_list(cls, issues: list[ProjectIssue]) -> list[Issue]:
+        return [cls.issue_to_domain(issue) for issue in issues]
+
 
 class GitlabInstanceClient(InstanceClientInterface):
     @classmethod
     def from_config(cls, config: dict) -> Self:
         return cls(Gitlab(config["url"], private_token=config["token"]))
 
     def __init__(self, client: Gitlab):
@@ -56,14 +60,19 @@
         )
         return IssueMapper.issue_to_domain(issue)
 
     async def get_issue(self, issue_id: int) -> Issue:
         issue: ProjectIssue = await self._get_issue(issue_id)
         return IssueMapper.issue_to_domain(issue)
 
+    async def find_issues(self, title: str) -> list[Issue]:
+        project = await self._get_project()
+        issues = cast(list[ProjectIssue], list(project.issues.list(search=title)))
+        return IssueMapper.issues_to_domain_list(issues)
+
     async def _get_project(self) -> Project:
         if self._project is None:
             try:
                 self._project = self.client.projects.get(self.project_id)
             except GitlabGetError as e:
                 raise ProjectDoesNotExistError(
                     f"Project with id={self.project_id} does not exist"
```

### Comparing `issx-0.1.0/src/issx/clients/interfaces.py` & `issx-0.2.0/src/issx/clients/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,11 +48,20 @@
         """
         pass
 
     @abc.abstractmethod
     async def create_issue(self, title: str, description: str) -> Issue:
         pass
 
+    @abc.abstractmethod
+    async def find_issues(self, title: str) -> list[Issue]:
+        """
+        Find issues by title using an exact match.
+        :param title: The title of the issue
+        :return: List of issues
+        """
+        pass
+
     @classmethod
     @abc.abstractmethod
     def from_config(cls, config: dict) -> Self:
         pass
```

### Comparing `issx-0.1.0/src/issx/clients/redmine.py` & `issx-0.2.0/src/issx/clients/redmine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Self
 
 from redminelib import Redmine
 from redminelib.exceptions import ResourceNotFoundError
 from redminelib.resources import Issue as RedmineIssue
 from redminelib.resources import Project
+from redminelib.resultsets import ResourceSet
 
 from issx.clients.exceptions import IssueDoesNotExistError, ProjectDoesNotExistError
 from issx.clients.interfaces import InstanceClientInterface, IssueClientInterface
 from issx.domain.issues import Issue
 
 
 class RedmineIssueMapper:
@@ -21,14 +22,18 @@
             id=issue.id,
             title=issue.subject,
             description=issue.description,
             web_url=issue.url,
             reference=issue.id,
         )
 
+    @classmethod
+    def issues_to_domain_list(cls, issues: ResourceSet) -> list[Issue]:  # type: ignore[no-any-unimported]
+        return [cls.issue_to_domain(issue) for issue in issues]
+
 
 class RedmineInstanceClient(InstanceClientInterface):
     def __init__(self, client: Redmine):  # type: ignore[no-any-unimported]
         self.client = client
 
     async def auth(self) -> str | None:
         return str(self.client.auth())
@@ -63,14 +68,21 @@
     async def get_issue(self, issue_id: int) -> Issue:
         try:
             issue = self.client.issue.get(issue_id)
         except ResourceNotFoundError as e:
             raise IssueDoesNotExistError(issue_id) from e
         return RedmineIssueMapper.issue_to_domain(issue)
 
+    async def find_issues(self, title: str) -> list[Issue]:
+        return RedmineIssueMapper.issues_to_domain_list(
+            self.client.issue.filter(
+                project_id=(await self.get_project()).id, subject=title
+            )
+        )
+
     async def get_project(self) -> Project:  # type: ignore[no-any-unimported]
         if self._project is None:
             try:
                 self._project = self.client.project.get(self._project_id)
             except ResourceNotFoundError as e:
                 raise ProjectDoesNotExistError(
                     f"Project with id={self._project_id} does not exist"
```

### Comparing `issx-0.1.0/src/issx/instance_managers.py` & `issx-0.2.0/src/issx/instance_managers.py`

 * *Files identical despite different names*

### Comparing `issx-0.1.0/PKG-INFO` & `issx-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

