# Comparing `tmp/oca_port-0.15.tar.gz` & `tmp/oca_port-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oca_port-0.15.tar", last modified: Mon Apr 15 14:24:13 2024, max compression
+gzip compressed data, was "oca_port-0.9.tar", last modified: Sun Sep 18 10:11:31 2022, max compression
```

## Comparing `oca_port-0.15.tar` & `oca_port-0.9.tar`

### file list

```diff
@@ -1,47 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.879995 oca_port-0.15/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 14:24:09.000000 oca_port-0.15/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.867995 oca_port-0.15/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.871995 oca_port-0.15/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-15 14:24:09.000000 oca_port-0.15/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-15 14:24:09.000000 oca_port-0.15/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-15 14:24:09.000000 oca_port-0.15/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-15 14:24:09.000000 oca_port-0.15/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 14:24:09.000000 oca_port-0.15/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-15 14:24:09.000000 oca_port-0.15/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-15 14:24:09.000000 oca_port-0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-15 14:24:13.875995 oca_port-0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-15 14:24:09.000000 oca_port-0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.871995 oca_port-0.15/oca_port/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.875995 oca_port-0.15/oca_port/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/cli/pr.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/migrate_addon.py
--rw-r--r--   0 runner    (1001) docker     (127)    28196 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/port_addon_pr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.875995 oca_port-0.15/oca_port/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.875995 oca_port-0.15/oca_port/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/tests/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6568 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/tests/test_utils_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/tests/test_utils_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.875995 oca_port-0.15/oca_port/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-15 14:24:09.000000 oca_port-0.15/oca_port/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:24:13.875995 oca_port-0.15/oca_port.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-15 14:24:13.000000 oca_port-0.15/oca_port.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 14:24:13.000000 oca_port-0.15/oca_port.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:24:13.000000 oca_port-0.15/oca_port.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 14:24:13.000000 oca_port-0.15/oca_port.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 14:24:13.000000 oca_port-0.15/oca_port.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 14:24:13.000000 oca_port-0.15/oca_port.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 14:24:09.000000 oca_port-0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:24:13.879995 oca_port-0.15/setup.cfg
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.473864 oca_port-0.9/
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.465864 oca_port-0.9/.github/
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.469864 oca_port-0.9/.github/workflows/
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      607 2022-09-18 10:09:49.000000 oca_port-0.9/.github/workflows/publish.yml
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      212 2022-08-31 11:45:14.000000 oca_port-0.9/.gitignore
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     7652 2022-08-31 11:45:14.000000 oca_port-0.9/LICENSE
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    11314 2022-09-18 10:11:31.473864 oca_port-0.9/PKG-INFO
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     1660 2022-08-31 11:45:14.000000 oca_port-0.9/README.md
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.469864 oca_port-0.9/oca_port/
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     7287 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/__init__.py
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)     7485 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/migrate_addon.py
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    11336 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/misc.py
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    26227 2022-08-31 11:45:14.000000 oca_port-0.9/oca_port/port_addon_pr.py
+drwxrwxr-x   0 sbi-local  (1000) sbi-local  (1000)        0 2022-09-18 10:11:31.473864 oca_port-0.9/oca_port.egg-info/
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)    11314 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/PKG-INFO
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      357 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/SOURCES.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)        1 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/dependency_links.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       43 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/entry_points.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       25 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/requires.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       14 2022-09-18 10:11:31.000000 oca_port-0.9/oca_port.egg-info/top_level.txt
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)      995 2022-09-18 10:09:49.000000 oca_port-0.9/pyproject.toml
+-rw-rw-r--   0 sbi-local  (1000) sbi-local  (1000)       38 2022-09-18 10:11:31.473864 oca_port-0.9/setup.cfg
```

### Comparing `oca_port-0.15/LICENSE` & `oca_port-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oca_port-0.15/PKG-INFO` & `oca_port-0.9/oca_port.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: oca_port
-Version: 0.15
+Name: oca-port
+Version: 0.9
 Summary: OCA tool to help with modules migration
 Author: Odoo Community Association (OCA)
-Author-email: Sébastien Alix <sebastien.alix@camptocamp.com>, Simone Orsi <simone.orsi@camptocamp.com>
+Author-email: Sébastien Alix <sebastien.alix@camptocamp.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -176,41 +176,21 @@
 Keywords: odoo,oca,port,migration,modules,addons
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Odoo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: gitpython
-Requires-Dist: requests
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: coverage; extra == "test"
-
-[![Pre-commit Status](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml/badge.svg?branch=main)](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml?query=branch%3Amain)
 
 oca-port
 ========
 
 Tool helping to port an addon or missing commits of an addon from one branch
 to another.
 
-Installing
-----------
-
-    $ pipx install oca-port
-    $ #OR
-    $ git clone git@github.com:oca/oca-port.git
-    $ cd oca-port
-    $ pipx install .
-
-Using
------
-
 If the addon does not exist on the target branch, it will assist the user in
 the migration, following the OCA migration guide.
 
 If the addon already exists on the target branch, it will retrieve missing
 commits to port. If a Pull Request exists for a missing commit, it will be
 ported with all its commits if they were not yet (fully) ported.
 
@@ -219,86 +199,30 @@
     $ export GITHUB_TOKEN=<token>
     $ oca-port 14.0 15.0 shopfloor --verbose
 
 To effectively migrate the addon or port its commits, use the `--fork` option:
 
     $ oca-port 14.0 15.0 shopfloor --fork camptocamp
 
-You can also directly blacklist a bunch of PRs on a given branch thanks to the
-`oca-port-pr` tool:
-
-    $ oca-port-pr blacklist OCA/wms#250,OCA/wms#251 15.0 shopfloor
-
-You could give a more detailed reason of this blacklist with `--reason` parameter:
-
-    $ oca-port-pr blacklist OCA/wms#250,OCA/wms#251 15.0 shopfloor --reason "Refactored in 15.0, not needed anymore"
-
-And if the module has been moved to another repository, you can specify its remote as well:
-
-    $ git remote add new_repo git@github.com:OCA/new-repo.git
-    $ oca-port-pr blacklist OCA/wms#250,OCA/wms#251 15.0 shopfloor --remote new_repo
-
 Migration of addon
 ------------------
 
 The tool follows the usual OCA migration guide to port commits of an addon,
 and will invite the user to fullfill the mentionned steps that can't be
 performed automatically.
 
 **Output example:**
 ![image](https://user-images.githubusercontent.com/5315285/129355442-f863adff-33c0-4c91-b0cb-b6882312e340.png)
 
-If used with the `--non-interactive` option, the returned exit code is `100`
-if an addon could be migrated.
-
 Port of commits/Pull Requests
 -----------------------------
 
 The tool will ask the user if he wants to open draft pull requests against
 the upstream repository.
 
 If there are several Pull Requests to port, it will ask the user if he wants
 to base the next PR on the previous one, allowing the user to cumulate ported
 PRs in one branch and creating a draft PR against the upstream repository
 with all of them.
 
-More details here : [OCA Days 2022 - Sébastien Alix and Simone Orsi: oca-port:new OCA tool to help with modules migration](https://www.youtube.com/watch?v=idGLkQiJ5N0)
-
 **Output example (with --verbose):**
 ![oca_port_pr_verbose](https://user-images.githubusercontent.com/5315285/129207041-12ac6c4a-ea96-4b8c-bd68-ae661531ad92.png)
-
-If used with the `--non-interactive` option, the returned exit code is `110`
-if some pull requests/commits could be ported.
-
-API
----
-
-You can also use `oca-port` as a Python package:
-
-```python
->>> import oca_port
->>> app = oca_port.App(
-...     from_branch="14.0",
-...     to_branch="16.0",
-...     addon="stock_move_auto_assign",
-...     from_org": "OCA",
-...     from_remote": "origin",
-...     repo_path": "/home/odoo/OCA/stock-logistics-warehouse",
-...     output": "json",
-...     fetch": True,
-...     github_token: "ghp_sheeXai3xu1yoopheiquoo3ohch0AefooSob"
-... )
->>> json_data = app.run()
->>> data = json.loads(json_data)
->>> from pprint import pprint as pp
->>> pp(data)
-{'process': 'port_commits',
- 'results': {'1631': {'author': 'TDu',
-                      'merged_at': '2023-04-04T17:06:03Z',
-                      'missing_commits': ['41416c1d7dad15ce4745e07d0541c79e938c2710',
-                                          'd43985a443e29641447a3811f2310d54b886ab3d',
-                                          '6bd9fcff3e814a6802c7aefadb9c646194cde42b'],
-                      'ref': 'OCA/stock-logistics-warehouse#1631',
-                      'title': '[14][ADD] stock_move_auto_assign_auto_release '
-                               '- backport',
-                      'url': 'https://github.com/OCA/stock-logistics-warehouse/pull/1631'}}}
-```
```

### Comparing `oca_port-0.15/oca_port/app.py` & `oca_port-0.9/oca_port/migrate_addon.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,197 +1,197 @@
 # Copyright 2022 Camptocamp SA
 # License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl)
-import os
-import pathlib
-from dataclasses import dataclass
 
-import git
+import click
+import os
+import subprocess
+import tempfile
+import urllib.parse
 
-from . import utils
-from .exceptions import ForkValueError, RemoteBranchValueError
-from .migrate_addon import MigrateAddon
+from . import misc
+from .misc import bcolors as bc
 from .port_addon_pr import PortAddonPullRequest
-from .utils.git import Branch
-from .utils.github import GitHub
-from .utils.misc import Output, bcolors as bc
-
-
-@dataclass
-class App(Output):
-    """'oca-port' application centralizing settings and operations.
-
-    Parameters:
-
-        from_branch:
-            the source branch (e.g. '15.0')
-        to_branch:
-            the source branch (e.g. '16.0')
-        addon:
-            the name of the module to process
-        repo_path:
-            local path to the Git repository
-        fork:
-            name of the Git remote used as fork
-        repo_name:
-            name of the repository on the upstream organization (e.g. 'server-tools')
-        user_org:
-            name of the user's GitHub organization where the fork is hosted
-        from_org:
-            name of the upstream GitHub organization (default = 'OCA')
-        from_remote:
-            name of the Git remote considered as the upstream (default = 'origin')
-        verbose:
-            returns more details to the user
-        non_interactive:
-            flag to not wait for user input and to return a error code to the shell.
-            Returns 100 if an addon could be migrated, 110 if pull requests/commits
-            could be ported, 0 if the history of the addon is the same on both branches.
-        output:
-            returns a parsable output. This implies the 'non-interactive' mode
-            defined above but without returning any special exit code.
-            Possible values: 'json'
-        fetch:
-            always fetch source and target branches from upstream
-        no_cache:
-            flag to disable the user's cache
-        clear_cache:
-            flag to remove the user's cache once the process is done
-        github_token:
-            Token to use when requesting GitHub API (highly recommended
-            to not trigger the "API rate limit exceeded" error).
-    """
-
-    from_branch: str
-    to_branch: str
-    addon: str
-    repo_path: str
-    fork: str = None
-    repo_name: str = None
-    user_org: str = None
-    from_org: str = "OCA"
-    from_remote: str = "origin"
-    verbose: bool = False
-    non_interactive: bool = False
-    output: str = None
-    fetch: bool = False
-    no_cache: bool = False
-    clear_cache: bool = False
-    github_token: str = None
-    cli: bool = False  # Not documented, should not be used outside of the CLI
-
-    _available_outputs = ("json",)
-
-    def __post_init__(self):
-        # Handle with repo_path and repo_name
-        if self.repo_path:
-            self.repo_path = pathlib.Path(self.repo_path)
-        else:
-            raise ValueError("'repo_path' has to be set.")
-        if not self.repo_name:
-            self.repo_name = self.repo_path.name
-        # Handle Git repository
-        self.repo = git.Repo(self.repo_path)
-        if self.repo.is_dirty(untracked_files=True):
-            raise ValueError("changes not committed detected in this repository.")
-        # Handle user's organization and fork
-        if not self.user_org:
-            # Assume that the fork remote has the same name than the user organization
-            self.user_org = self.fork
-        if self.fork:
-            if self.fork not in self.repo.remotes:
-                raise ForkValueError(self.repo_name, self.fork)
-        # Transform branch strings to Branch objects
-        try:
-            self.from_branch = Branch(
-                self.repo, self.from_branch, default_remote=self.from_remote
-            )
-            self.to_branch = Branch(
-                self.repo, self.to_branch, default_remote=self.from_remote
-            )
-        except ValueError as exc:
-            if exc.args[1] not in self.repo.remotes:
-                raise RemoteBranchValueError(self.repo_name, exc.args[1]) from exc
-        # Force non-interactive mode:
-        #   - if we are not in CLI mode
-        if not self.cli:
-            self.non_interactive = True
-        #   - if an output has been defined
-        if self.output:
-            if self.output.lower() not in self._available_outputs:
-                outputs = ", ".join(self._available_outputs)
-                raise ValueError(f"Supported outputs are: {outputs}")
-            self.non_interactive = True
-        # Fetch branches if they can't be resolved locally
-        # NOTE: required for the storage below to retrieve data
-        remote_branches = self.repo.git.branch("-r").split()
-        if (
-            self.fetch
-            or (
-                self.from_branch.remote
-                and self.from_branch.ref() not in remote_branches
-            )
-            or (self.to_branch.remote and self.to_branch.ref() not in remote_branches)
-        ):
-            self.fetch_branches()
-        # GitHub API helper
-        self.github = GitHub(self.github_token or os.environ.get("GITHUB_TOKEN"))
-        # Initialize storage & cache
-        self.storage = utils.storage.InputStorage(self.to_branch, self.addon)
-        self.cache = utils.cache.UserCacheFactory(self).build()
-
-    def fetch_branches(self):
-        for branch in (self.from_branch, self.to_branch):
-            if not branch.remote:
-                continue
-            remote_url = branch.repo.remotes[branch.remote].url
-            if self.verbose:
-                self._print(f"Fetch {bc.BOLD}{branch.ref()}{bc.END} from {remote_url}")
-            branch.repo.remotes[branch.remote].fetch(branch.name)
-
-    def _check_addon_exists(self, branch, raise_exc=False):
-        repo = self.repo
-        addon = self.addon
-        branch_addons = [t.path for t in repo.commit(branch.ref()).tree.trees]
-        if addon not in branch_addons:
-            if not raise_exc:
-                return False
-            error = f"{addon} does not exist on {branch.ref()}"
-            if self.cli:
-                error = f"{bc.FAIL}{addon}{bc.ENDC} does not exist on {branch.ref()}"
-            raise ValueError(error)
-        return True
-
-    def check_addon_exists_from_branch(self, raise_exc=False):
-        """Check that `addon` exists on the source branch`."""
-        return self._check_addon_exists(self.from_branch, raise_exc=raise_exc)
-
-    def check_addon_exists_to_branch(self, raise_exc=False):
-        """Check that `addon` exists on the target branch`."""
-        return self._check_addon_exists(self.to_branch, raise_exc=raise_exc)
+
+MIG_BRANCH_NAME = (
+    "{branch}-mig-{addon}"
+)
+MIG_MERGE_COMMITS_URL = (
+    "https://github.com/OCA/maintainer-tools/wiki/Merge-commits-in-pull-requests"
+)
+MIG_TASKS_URL = (
+    "https://github.com/OCA/maintainer-tools/wiki/Migration-to-version-{branch}"
+    "#tasks-to-do-in-the-migration"
+)
+MIG_NEW_PR_TITLE = "[{to_branch}][MIG] {addon}"
+MIG_NEW_PR_URL = (
+    "https://github.com/{upstream_org}/{repo_name}/compare/"
+    "{to_branch}...{user_org}:{mig_branch}?expand=1&title={title}"
+)
+MIG_TIPS = "\n".join([
+    f"\n{bc.BOLD}{bc.OKCYAN}The next steps are:{bc.END}",
+    (
+        "\t1) Reduce the number of commits "
+        f"('{bc.DIM}OCA Transbot...{bc.END}'):"
+    ),
+    f"\t\t=> {bc.BOLD}{MIG_MERGE_COMMITS_URL}{bc.END}",
+    "\t2) Adapt the module to the {to_branch} version:",
+    f"\t\t=> {bc.BOLD}" "{mig_tasks_url}" f"{bc.END}",
+    (
+        "\t3) On a shell command, type this for uploading the content to GitHub:\n"
+        f"{bc.DIM}"
+        "\t\t$ git add --all\n"
+        "\t\t$ git commit -m \"[MIG] {addon}: Migration to {to_branch}\"\n"
+        "\t\t$ git push {fork} {mig_branch} --set-upstream"
+        f"{bc.END}"
+    ),
+    "\t4) Create the PR against {upstream_org}/{repo_name}:",
+    f"\t\t=> {bc.BOLD}" "{new_pr_url}" f"{bc.END}",
+])
+
+
+class MigrateAddon():
+    def __init__(
+            self, repo, upstream_org, repo_name, from_branch, to_branch,
+            fork, user_org, addon, storage, verbose=False, non_interactive=False
+            ):
+        self.repo = repo
+        self.upstream_org = upstream_org
+        self.repo_name = repo_name
+        self.from_branch = from_branch
+        self.to_branch = to_branch
+        self.fork = fork
+        self.user_org = user_org
+        self.addon = addon
+        self.storage = storage
+        self.mig_branch = misc.Branch(
+            repo, MIG_BRANCH_NAME.format(branch=to_branch.name[:4], addon=addon)
+        )
+        self.verbose = verbose
+        self.non_interactive = non_interactive
 
     def run(self):
-        """Run 'oca-port' to migrate an addon or to port its pull requests."""
-        self.check_addon_exists_from_branch(raise_exc=True)
-        # Check if some PRs could be ported
-        res, output = self.run_port()
-        if not res:
-            # If not, migrate the addon
-            res, output = self.run_migrate()
-        if self.cli and self.output:
-            if not output:
-                output = self._render_output(self.output, {})
-            print(output)
-        if self.clear_cache:
-            self.cache.clear()
-        if self.output:
-            return output
-        return res
-
-    def run_port(self):
-        """Port pull requests of an addon (if any)."""
-        # Check if the addon (folder) exists on the target branch
-        #   - if it already exists, check if some PRs could be ported
-        return PortAddonPullRequest(self).run()
-
-    def run_migrate(self):
-        """Migrate an addon."""
-        return MigrateAddon(self).run()
+        if self.storage.is_addon_blacklisted(
+                self.from_branch.name, self.to_branch.name, self.addon
+                ):
+            print(
+                f"{bc.DIM}Migration to {self.to_branch.name} for "
+                f"{bc.BOLD}{self.addon}{bc.END} {bc.DIM}blacklisted{bc.ENDD}")
+            return
+        if self.non_interactive:
+            # Exit with an error code if the addon is eligible for a migration
+            raise SystemExit(1)
+        confirm = (
+            f"Migrate {bc.BOLD}{self.addon}{bc.END} "
+            f"from {bc.BOLD}{self.from_branch.name}{bc.END} "
+            f"to {bc.BOLD}{self.to_branch.name}{bc.END}?"
+        )
+        if not click.confirm(confirm):
+            self.storage.blacklist_addon(
+                self.from_branch.name, self.to_branch.name,
+                self.addon, confirm=True
+            )
+            return
+        # Check if a migration PR already exists
+        # TODO
+        if not self.fork:
+            raise click.UsageError("Please set the '--fork' option")
+        if self.repo.untracked_files:
+            raise click.ClickException("Untracked files detected, abort")
+        self._checkout_base_branch()
+        if self._create_mig_branch():
+            with tempfile.TemporaryDirectory() as patches_dir:
+                self._generate_patches(patches_dir)
+                self._apply_patches(patches_dir)
+            self._run_pre_commit()
+        # Check if the addon has commits that update neighboring addons to
+        # make it work properly
+        PortAddonPullRequest(
+            self.repo, self.upstream_org, self.repo_name,
+            self.from_branch, self.mig_branch, self.fork, self.user_org,
+            self.addon, self.storage, self.verbose,
+            create_branch=False, push_branch=False
+        ).run()
+        self._print_tips()
+
+    def _checkout_base_branch(self):
+        # Ensure to not start to work from a working branch
+        if self.to_branch.name in self.repo.heads:
+            self.repo.heads[self.to_branch.name].checkout()
+        else:
+            self.repo.git.checkout(
+                "--no-track", "-b", self.to_branch.name, self.to_branch.ref()
+            )
+
+    def _create_mig_branch(self):
+        create_branch = True
+        if self.mig_branch.name in self.repo.heads:
+            confirm = (
+                f"Branch {bc.BOLD}{self.mig_branch.name}{bc.END} already exists, "
+                "recreate it?\n(⚠️  you will lose the existing branch)"
+            )
+            if click.confirm(confirm):
+                self.repo.delete_head(self.mig_branch.name, "-f")
+            else:
+                create_branch = False
+        if create_branch:
+            # Create branch
+            print(
+                f"\tCreate branch {bc.BOLD}{self.mig_branch.name}{bc.END} "
+                f"from {self.to_branch.ref()}..."
+            )
+            self.repo.git.checkout(
+                "--no-track", "-b", self.mig_branch.name, self.to_branch.ref()
+            )
+        return create_branch
+
+    def _generate_patches(self, patches_dir):
+        print("\tGenerate patches...")
+        self.repo.git.format_patch(
+            "--keep-subject", "-o", patches_dir,
+            f"{self.to_branch.ref()}..{self.from_branch.ref()}",
+            "--", self.addon
+        )
+
+    def _apply_patches(self, patches_dir):
+        patches = [
+            os.path.join(patches_dir, f) for f in sorted(os.listdir(patches_dir))
+        ]
+        # Apply patches with git-am
+        print(f"\tApply {len(patches)} patches...")
+        self.repo.git.am("-3", "--keep", *patches)
+        print(
+            f"\t\tCommits history of {bc.BOLD}{self.addon}{bc.END} "
+            f"has been migrated."
+        )
+
+    def _run_pre_commit(self):
+        # Run pre-commit
+        print(
+            f"\tRun {bc.BOLD}pre-commit{bc.END} and commit changes if any..."
+        )
+        # First ensure that 'pre-commit' is initialized for the repository,
+        # then run it (without checking the return code on purpose)
+        subprocess.check_call("pre-commit install", shell=True)
+        subprocess.run("pre-commit run -a", shell=True)
+        if self.repo.untracked_files or self.repo.is_dirty():
+            self.repo.git.add("-A")
+            self.repo.git.commit(
+                "-m", f"[IMP] {self.addon}: black, isort, prettier", "--no-verify"
+            )
+
+    def _print_tips(self):
+        mig_tasks_url = MIG_TASKS_URL.format(branch=self.to_branch.name)
+        pr_title_encoded = urllib.parse.quote(
+            MIG_NEW_PR_TITLE.format(to_branch=self.to_branch.name[:4], addon=self.addon)
+        )
+        new_pr_url = MIG_NEW_PR_URL.format(
+            upstream_org=self.upstream_org, repo_name=self.repo_name,
+            to_branch=self.to_branch.name, user_org=self.user_org,
+            mig_branch=self.mig_branch.name, title=pr_title_encoded
+        )
+        tips = MIG_TIPS.format(
+            upstream_org=self.upstream_org, repo_name=self.repo_name,
+            addon=self.addon, to_branch=self.to_branch.name, fork=self.fork,
+            mig_branch=self.mig_branch.name, mig_tasks_url=mig_tasks_url,
+            new_pr_url=new_pr_url
+        )
+        print(tips)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oca_port-0.15/oca_port/port_addon_pr.py` & `oca_port-0.9/oca_port/port_addon_pr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,287 +1,255 @@
 # Copyright 2022 Camptocamp SA
 # License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl)
 
-import os
+from collections import defaultdict
 import shutil
 import tempfile
-from collections import defaultdict
+import os
 
 import click
 import git
 
-from .utils import git as g, misc
-from .utils.misc import Output, bcolors as bc
+from . import misc
+from .misc import bcolors as bc
 
 AUTHOR_EMAILS_TO_SKIP = [
     "transbot@odoo-community.org",
-    "noreply@weblate.org",
     "oca-git-bot@odoo-community.org",
     "oca+oca-travis@odoo-community.org",
     "oca-ci@odoo-community.org",
     "shopinvader-git-bot@shopinvader.com",
 ]
 
 SUMMARY_TERMS_TO_SKIP = [
     "Translated using Weblate",
     "Added translation using Weblate",
 ]
 
-PR_BRANCH_NAME = "oca-port-from-{from_branch}-to-{to_branch}-pr-{pr_number}"
+PR_BRANCH_NAME = (
+    "oca-port-pr-{pr_number}-from-{from_branch}-to-{to_branch}"
+)
 
 FOLDERS_TO_SKIP = [
     "setup",
     ".github",
 ]
 
 FILES_TO_KEEP = [
     "requirements.txt",
     "test-requirements.txt",
     "oca_dependencies.txt",
 ]
 
-BOT_FILES_TO_SKIP = [
-    "README.rst",
-    "static/description/index.html",
-]
-
-# Fake PR for commits w/o any PR (used as fallback)
-FAKE_PR = g.PullRequest(*[""] * 6)
-
 
 def path_to_skip(commit_path):
     """Return True if the commit path should not be ported."""
     # Allows all folders (addons!) excepted those like 'setup/' generated
     # automatically by pre-commit.
     if commit_path.isdir:
         return commit_path in FOLDERS_TO_SKIP
     # Forbid all files excepted those that developers could update
     return commit_path not in FILES_TO_KEEP
 
 
-class PortAddonPullRequest(Output):
-    def __init__(self, app, create_branch=True, push_branch=True):
-        """Port pull requests of an addon."""
-        self.app = app
+class PortAddonPullRequest():
+    def __init__(
+            self, repo, upstream_org, repo_name,
+            from_branch, to_branch, fork, user_org, addon, storage,
+            verbose=False, non_interactive=False,
+            create_branch=True, push_branch=True
+            ):
+        """Port pull requests of `addon`."""
+        self.repo = repo
+        self.upstream_org = upstream_org
+        self.repo_name = repo_name
+        self.from_branch = from_branch
+        self.to_branch = to_branch
+        self.fork = fork
+        self.user_org = user_org
+        self.addon = addon
+        self.storage = storage
+        self.verbose = verbose
+        self.non_interactive = non_interactive
         self.create_branch = create_branch
         self.push_branch = push_branch
-        self._results = {"process": "port_commits", "results": {}}
 
     def run(self):
-        if not self.app.check_addon_exists_to_branch():
-            if self.app.non_interactive:
-                if self.app.output:
-                    return False, self._render_output(self.app.output, {})
-            return False, None
-        self._print(
-            f"{bc.BOLD}{self.app.addon}{bc.END} already exists "
-            f"on {bc.BOLD}{self.app.to_branch.name}{bc.END}, "
+        print(
+            f"{bc.BOLD}{self.addon}{bc.END} already exists "
+            f"on {bc.BOLD}{self.to_branch.name}{bc.END}, "
             "checking PRs to port..."
         )
-        branches_diff = BranchesDiff(self.app)
-        branches_diff.print_diff(self.app.verbose)
-        if self.app.non_interactive:
+        branches_diff = BranchesDiff(
+            self.repo, self.upstream_org, self.repo_name, self.addon,
+            self.from_branch, self.to_branch, self.storage
+        )
+        branches_diff.print_diff(self.verbose)
+        if self.non_interactive:
             if branches_diff.commits_diff:
-                # If an output is defined we return the result in the expected format
-                if self.app.output:
-                    self._results["results"] = branches_diff.serialized_diff
-                    return True, self._render_output(self.app.output, self._results)
-                if self.app.cli:
-                    # Exit with an error code if commits are eligible for (back)porting
-                    # User-defined exit codes should be defined between 64 and 113.
-                    # Allocate 110 for 'PortAddonPullRequest'.
-                    raise SystemExit(110)
-                return True, None
-            if self.app.output:
-                # Nothing to port -> return an empty output
-                return False, self._render_output(self.app.output, {})
-            return False, None
-        if self.app.fork:
-            self._print()
+                # Exit with an error code if commits are eligible for (back)porting
+                raise SystemExit(1)
+            return
+        if self.fork:
+            print()
             self._port_pull_requests(branches_diff)
-        return True, None
 
     def _port_pull_requests(self, branches_diff):
         """Open new Pull Requests (if it doesn't exist) on the GitHub repository."""
-        base_ref = branches_diff.app.to_branch  # e.g. 'origin/14.0'
+        base_ref = branches_diff.to_branch  # e.g. 'origin/14.0'
         previous_pr = previous_pr_branch = None
         processed_prs = []
         last_pr = (
             list(branches_diff.commits_diff.keys())[-1]
-            if branches_diff.commits_diff
-            else None
+            if branches_diff.commits_diff else None
         )
         for pr, commits in branches_diff.commits_diff.items():
-            current_commit = self.app.repo.commit(self.app.to_branch.ref())
+            current_commit = self.repo.commit(self.to_branch.ref())
             pr_branch, based_on_previous = self._port_pull_request_commits(
-                pr,
-                commits,
-                base_ref,
-                previous_pr,
-                previous_pr_branch,
+                pr, commits, base_ref, previous_pr, previous_pr_branch,
             )
             if pr_branch:
-                # Check if commits have been ported.
-                # If none has been ported, blacklist automatically the current PR.
-                if self.app.repo.commit(pr_branch.ref()) == current_commit:
-                    self._print("\tℹ️  Nothing has been ported, skipping")
-                    self.app.storage.blacklist_pr(
-                        pr.number,
-                        confirm=True,
-                        reason=f"(auto) Nothing to port from PR #{pr.number}",
+                # Check if commits have been ported
+                if self.repo.commit(pr_branch.ref()) == current_commit:
+                    print("\tℹ️  Nothing has been ported, skipping")
+                    self.storage.blacklist_pr(
+                        self.from_branch.name, self.to_branch.name,
+                        self.addon, pr.number
                     )
-                    if self.app.storage.dirty:
-                        self.app.storage.commit()
                     msg = (
                         f"\t{bc.DIM}PR #{pr.number} has been"
-                        if pr.number
-                        else "Orphaned commits have been"
+                        if pr.number else "Orphaned commits have been"
                     ) + f" automatically blacklisted{bc.ENDD}"
-                    self._print(msg)
+                    print(msg)
                     continue
                 previous_pr = pr
                 previous_pr_branch = pr_branch
                 if based_on_previous:
                     processed_prs.append(pr)
                 else:
                     processed_prs = [pr]
                 if pr == last_pr:
-                    self._print("\t🎉 Last PR processed! 🎉")
+                    print("\t🎉 Last PR processed! 🎉")
+                if not self.push_branch:
+                    continue
                 is_pushed = self._push_branch_to_remote(pr_branch)
                 if not is_pushed:
                     continue
                 pr_data = self._prepare_pull_request_data(processed_prs, pr_branch)
                 pr_url = self._search_pull_request(pr_data["base"], pr_data["title"])
                 if pr_url:
-                    self._print(f"\tExisting PR has been refreshed => {pr_url}")
+                    print(f"\tExisting PR has been refreshed => {pr_url}")
                 else:
                     self._create_pull_request(pr_branch, pr_data, processed_prs)
 
     def _port_pull_request_commits(
-        self,
-        pr,
-        commits,
-        base_ref,
-        previous_pr=None,
-        previous_pr_branch=None,
-    ):
+            self, pr, commits, base_ref, previous_pr=None, previous_pr_branch=None,
+            ):
         """Port commits of a Pull Request in a new branch."""
         if pr.number:
-            self._print(
+            print(
                 f"- {bc.BOLD}{bc.OKCYAN}Port PR #{pr.number}{bc.END} "
                 f"({pr.url}) {bc.OKCYAN}{pr.title}{bc.ENDC}..."
             )
         else:
-            self._print(f"- {bc.BOLD}{bc.OKCYAN}Port commits w/o PR{bc.END}...")
+            print(f"- {bc.BOLD}{bc.OKCYAN}Port commits w/o PR{bc.END}...")
         based_on_previous = False
         # Ensure to not start to work from a working branch
-        if self.app.to_branch.name in self.app.repo.heads:
-            self.app.repo.heads[self.app.to_branch.name].checkout()
+        if self.to_branch.name in self.repo.heads:
+            self.repo.heads[self.to_branch.name].checkout()
         else:
-            self.app.repo.git.checkout(
-                "--no-track",
-                "-b",
-                self.app.to_branch.name,
-                self.app.to_branch.ref(),
+            self.repo.git.checkout(
+                "--no-track", "-b", self.to_branch.name, self.to_branch.ref()
             )
-        # Ask the user if he wants to port the PR (or orphaned commits)
         if not click.confirm("\tPort it?" if pr.number else "\tPort them?"):
-            self.app.storage.blacklist_pr(pr.ref, confirm=True)
-            if not self.app.storage.dirty:
-                return None, based_on_previous
+            self.storage.blacklist_pr(
+                self.from_branch.name, self.to_branch.name,
+                self.addon, pr.number, confirm=True
+            )
+            return None, based_on_previous
         # Create a local branch based on upstream
         if self.create_branch:
             branch_name = PR_BRANCH_NAME.format(
-                from_branch=self.app.from_branch.name,
-                to_branch=self.app.to_branch.name,
                 pr_number=pr.number,
+                from_branch=self.from_branch.name,
+                to_branch=self.to_branch.name,
             )
-            if branch_name in self.app.repo.heads:
+            if branch_name in self.repo.heads:
                 # If the local branch already exists, ask the user if he wants
                 # to recreate it + check if this existing branch is based on
                 # the previous PR branch
                 if previous_pr_branch:
-                    based_on_previous = self.app.repo.is_ancestor(
-                        previous_pr_branch.name, branch_name
+                    based_on_previous = self.repo.is_ancestor(
+                        previous_pr_branch, branch_name
                     )
                 confirm = (
                     f"\tBranch {bc.BOLD}{branch_name}{bc.END} already exists, "
                     "recreate it?\n\t(⚠️  you will lose the existing branch)"
                 )
                 if not click.confirm(confirm):
-                    return g.Branch(self.app.repo, branch_name), based_on_previous
-                self.app.repo.delete_head(branch_name, "-f")
+                    return misc.Branch(self.repo, branch_name), based_on_previous
+                self.repo.delete_head(branch_name, "-f")
             if previous_pr and click.confirm(
-                f"\tUse the previous {bc.BOLD}PR #{previous_pr.number}{bc.END} "
-                "branch as base?"
-            ):
+                    f"\tUse the previous {bc.BOLD}PR #{previous_pr.number}{bc.END} "
+                    "branch as base?"
+                    ):
                 base_ref = previous_pr_branch
                 based_on_previous = True
-                # Set the new branch name the same than the previous one
-                # but with the PR number as suffix.
-                branch_name = f"{previous_pr_branch.name}-{pr.number}"
-            self._print(
+            print(
                 f"\tCreate branch {bc.BOLD}{branch_name}{bc.END} from {base_ref.ref()}..."
             )
-            self.app.repo.git.checkout("--no-track", "-b", branch_name, base_ref.ref())
+            self.repo.git.checkout("--no-track", "-b", branch_name, base_ref.ref())
         else:
-            branch_name = self.app.to_branch.name
-        # If the PR has been blacklisted we need to commit this information
-        if self.app.storage.dirty:
-            self.app.storage.commit()
-            return g.Branch(self.app.repo, branch_name), based_on_previous
+            branch_name = self.to_branch.name
 
         # Cherry-pick commits of the source PR
         for commit in commits:
-            self._print(
+            print(
                 f"\t\tApply {bc.OKCYAN}{commit.hexsha[:8]}{bc.ENDC} "
                 f"{commit.summary}..."
             )
             # Port only relevant diffs/paths from the commit
             paths_to_port = set(commit.paths_to_port)
             for diff in commit.diffs:
                 skip, message = self._skip_diff(commit, diff)
                 if skip:
                     if message:
-                        self._print(f"\t\t\t{message}")
+                        print(f"\t\t\t{message}")
                     if diff.a_path in paths_to_port:
                         paths_to_port.remove(diff.a_path)
                     if diff.b_path in paths_to_port:
                         paths_to_port.remove(diff.b_path)
                     continue
             if not paths_to_port:
-                self._print("\t\t\tℹ️  Nothing to port from this commit, skipping")
+                print(
+                    "\t\t\tℹ️  Nothing to port from this commit, skipping"
+                )
                 continue
             try:
                 patches_dir = tempfile.mkdtemp()
-                self.app.repo.git.format_patch(
-                    "--keep-subject",
-                    "-o",
-                    patches_dir,
-                    "-1",
-                    commit.hexsha,
-                    "--",
-                    *paths_to_port,
+                self.repo.git.format_patch(
+                    "--keep-subject", "-o", patches_dir, "-1", commit.hexsha,
+                    "--", *paths_to_port
                 )
                 patches = [
                     os.path.join(patches_dir, f)
                     for f in sorted(os.listdir(patches_dir))
                 ]
-                self.app.repo.git.am("-3", "--keep", *patches)
+                self.repo.git.am("-3", "--keep", *patches)
                 shutil.rmtree(patches_dir)
             except git.exc.GitCommandError as exc:
-                self._print(f"{bc.FAIL}ERROR:{bc.ENDC}\n{exc}\n")
+                print(f"{bc.FAIL}ERROR:{bc.ENDC}\n{exc}\n")
                 # High chance a conflict occurs, ask the user to resolve it
                 if not click.confirm(
-                    "⚠️  A conflict occurs, please resolve it and "
-                    "confirm to continue the process (y) or skip this commit (N)."
-                ):
-                    self.app.repo.git.am("--abort")
+                        "⚠️  A conflict occurs, please resolve it and "
+                        "confirm to continue the process (y) or skip this commit (N)."
+                        ):
+                    self.repo.git.am("--abort")
                     continue
-        return g.Branch(self.app.repo, branch_name), based_on_previous
+        return misc.Branch(self.repo, branch_name), based_on_previous
 
     @staticmethod
     def _skip_diff(commit, diff):
         """Check if a commit diff should be skipped or not.
 
         A skipped diff won't have its file path ported through 'git format-path'.
 
@@ -291,180 +259,156 @@
             if diff.a_path not in commit.paths_to_port:
                 return True, ""
         if diff.b_path not in commit.paths_to_port:
             return True, ""
         if diff.renamed:
             return False, ""
         diff_path = diff.b_path.split("/", maxsplit=1)[0]
-        # Skip diff updating auto-generated files (pre-commit, bot...)
-        if any(file_path in diff_path for file_path in BOT_FILES_TO_SKIP):
-            return (
-                True,
-                f"SKIP: '{diff.change_type} {diff.b_path}' diff relates "
-                "to an auto-generated file, skip to avoid conflict",
-            )
         # Do not accept diff on unported addons
-        if (
-            not misc.get_manifest_path(diff_path)
-            and diff_path not in commit.addons_created
-        ):
+        if not misc.get_manifest_path(diff_path) and diff_path not in commit.addons_created:
             return (
                 True,
                 (
                     f"{bc.WARNING}SKIP diff "
                     f"{bc.BOLD}{diff.change_type} {diff.b_path}{bc.END}: "
                     "relates to an unported addon"
-                ),
+                )
             )
         if diff.change_type in ("M", "D"):
             # Do not accept update and deletion on non-existing files
             if not os.path.exists(diff.b_path):
                 return (
                     True,
                     (
                         f"SKIP: '{diff.change_type} {diff.b_path}' diff relates "
                         "to a non-existing file"
-                    ),
+                    )
                 )
         return False, ""
 
     def _push_branch_to_remote(self, branch):
         """Force push the local branch to remote fork."""
-        if not self.push_branch:
-            return False
         confirm = (
             f"\tPush branch '{bc.BOLD}{branch.name}{bc.END}' "
-            f"to remote '{bc.BOLD}{self.app.fork}{bc.END}'?"
+            f"to remote '{bc.BOLD}{self.fork}{bc.END}'?"
         )
         if click.confirm(confirm):
-            branch.repo.git.push(self.app.fork, branch.name, "--force-with-lease")
-            branch.remote = self.app.fork
+            branch.repo.git.push(self.fork, branch.name, "--force-with-lease")
+            branch.remote = self.fork
             return True
-        return False
 
     def _prepare_pull_request_data(self, processed_prs, pr_branch):
         if len(processed_prs) > 1:
             title = (
-                f"[{self.app.to_branch.name}][FW] {self.app.addon}: multiple ports "
-                f"from {self.app.from_branch.name}"
+                f"[{self.to_branch.name}][FW] {self.addon}: multiple ports "
+                f"from {self.from_branch.name}"
             )
             lines = [f"- #{pr.number}" for pr in processed_prs]
             body = "\n".join(
                 [
-                    f"Port of the following PRs from {self.app.from_branch.name} "
-                    f"to {self.app.to_branch.name}:"
+                    f"Port of the following PRs from {self.from_branch.name} "
+                    f"to {self.to_branch.name}:"
                 ]
                 + lines
             )
         else:
             pr = processed_prs[0]
-            title = f"[{self.app.to_branch.name}][FW] {pr.title}"
+            title = f"[{self.to_branch.name}][FW] {pr.title}"
             body = (
-                f"Port of #{pr.number} from {self.app.from_branch.name} "
-                f"to {self.app.to_branch.name}."
+                f"Port of #{pr.number} from {self.from_branch.name} "
+                f"to {self.to_branch.name}."
             )
         return {
             "draft": True,
             "title": title,
-            "head": f"{self.app.user_org}:{pr_branch.name}",
-            "base": self.app.to_branch.name,
+            "head": f"{self.user_org}:{pr_branch.name}",
+            "base": self.to_branch.name,
             "body": body,
         }
 
     def _search_pull_request(self, base_branch, title):
         params = {
             "q": (
-                f"is:pr "
-                f"repo:{self.app.from_org}/{self.app.repo_name} "
-                f"base:{base_branch} "
+                f"is:pr repo:{self.upstream_org}/{self.repo_name} base:{base_branch} "
                 f"state:open {title} in:title"
             ),
         }
-        response = self.app.github.request("search/issues", params=params)
+        response = misc._request_github("search/issues", params=params)
         if response["items"]:
             return response["items"][0]["html_url"]
 
     def _create_pull_request(self, pr_branch, pr_data, processed_prs):
         if len(processed_prs) > 1:
-            self._print(
+            print(
                 "\tPR(s) ported locally:",
                 ", ".join(
                     [f"{bc.OKCYAN}#{pr.number}{bc.ENDC}" for pr in processed_prs]
-                ),
+                )
             )
         if click.confirm(
-            f"\tCreate a draft PR from '{bc.BOLD}{pr_branch.name}{bc.END}' "
-            f"to '{bc.BOLD}{self.app.to_branch.name}{bc.END}' "
-            f"against {bc.BOLD}{self.app.from_org}/{self.app.repo_name}{bc.END}?"
-        ):
-            response = self.app.github.request(
-                f"repos/{self.app.from_org}/{self.app.repo_name}/pulls",
+                f"\tCreate a draft PR from '{bc.BOLD}{pr_branch.name}{bc.END}' "
+                f"to '{bc.BOLD}{self.to_branch.name}{bc.END}' "
+                f"against {bc.BOLD}{self.upstream_org}/{self.repo_name}{bc.END}?"
+                ):
+            response = misc._request_github(
+                f"repos/{self.upstream_org}/{self.repo_name}/pulls",
                 method="post",
-                json=pr_data,
+                json=pr_data
             )
             pr_url = response["html_url"]
-            self._print(
-                f"\t\t{bc.BOLD}{bc.OKCYAN}PR created =>" f"{bc.ENDC} {pr_url}{bc.END}"
+            print(
+                f"\t\t{bc.BOLD}{bc.OKCYAN}PR created =>"
+                f"{bc.ENDC} {pr_url}{bc.END}"
             )
             return pr_url
 
 
-class BranchesDiff(Output):
+class BranchesDiff():
     """Helper to compare easily commits (and related PRs) between two branches."""
-
-    def __init__(self, app):
-        self.app = app
-        self.path = self.app.addon
+    def __init__(
+            self, repo, upstream_org, repo_name, path, from_branch, to_branch, storage
+            ):
+        self.repo = repo
+        self.upstream_org = upstream_org
+        self.repo_name = repo_name
+        self.path = path
+        self.from_branch, self.to_branch = from_branch, to_branch
         self.from_branch_path_commits, _ = self._get_branch_commits(
-            self.app.from_branch.ref(), self.path
+            self.from_branch.ref(), path
         )
         self.from_branch_all_commits, _ = self._get_branch_commits(
-            self.app.from_branch.ref()
+            self.from_branch.ref()
         )
         self.to_branch_path_commits, _ = self._get_branch_commits(
-            self.app.to_branch.ref(), self.path
-        )
-        self.to_branch_all_commits, _ = self._get_branch_commits(
-            self.app.to_branch.ref()
+            self.to_branch.ref(), self.path
         )
+        self.to_branch_all_commits, _ = self._get_branch_commits(self.to_branch.ref())
+        self.storage = storage
         self.commits_diff = self.get_commits_diff()
-        self.serialized_diff = self._serialize_diff(self.commits_diff)
-
-    def _serialize_diff(self, commits_diff):
-        data = {}
-        for pr, commits in commits_diff.items():
-            data[pr.number] = pr.to_dict()
-            data[pr.number]["missing_commits"] = [commit.hexsha for commit in commits]
-        return data
 
     def _get_branch_commits(self, branch, path="."):
         """Get commits from the local repository for the given `branch`.
 
         An optional `path` parameter can be set to limit commits to a given folder.
         This function also filters out undesirable commits (merge or translation
         commits...).
 
         Return two data structures:
             - a list of Commit objects `[Commit, ...]`
             - a dict of Commits objects grouped by SHA `{SHA: Commit, ...}`
         """
-        commits = self.app.repo.iter_commits(branch, paths=path)
+        commits = self.repo.iter_commits(branch, paths=path)
         commits_list = []
         commits_by_sha = {}
         for commit in commits:
-            if self.app.cache.is_commit_ported(commit.hexsha):
-                continue
-            com = g.Commit(commit)
+            com = misc.Commit(commit)
             if self._skip_commit(com):
                 continue
             commits_list.append(com)
             commits_by_sha[commit.hexsha] = com
-        # Put ancestors at the beginning of the list to loop with
-        # the expected order
-        commits_list.reverse()
         return commits_list, commits_by_sha
 
     @staticmethod
     def _skip_commit(commit):
         """Check if a commit should be skipped or not.
 
         Merge or translations commits are skipped for instance, or commits
@@ -487,182 +431,196 @@
             if pr.number:
                 lines_to_print.append(
                     f"{i}) {bc.BOLD}{bc.OKBLUE}PR #{pr.number}{bc.END} "
                     f"({pr.url or 'w/o PR'}) {bc.OKBLUE}{pr.title}{bc.ENDC}:"
                 )
                 lines_to_print.append(f"\tBy {pr.author}, merged at {pr.merged_at}")
             else:
-                lines_to_print.append(f"{i}) {bc.BOLD}{bc.OKBLUE}w/o PR{bc.END}:")
+                lines_to_print.append(
+                    f"{i}) {bc.BOLD}{bc.OKBLUE}w/o PR{bc.END}:"
+                )
                 fake_pr = pr
             if verbose:
-                pr_paths = ", ".join([f"{bc.DIM}{path}{bc.ENDD}" for path in pr.paths])
-                lines_to_print.append(f"\t=> Updates: {pr_paths}")
+                pr_paths = ", ".join(
+                    [f"{bc.DIM}{path}{bc.ENDD}" for path in pr.paths]
+                )
+                lines_to_print.append(
+                    f"\t=> Updates: {pr_paths}"
+                )
             if pr.number:
                 pr_paths_not_ported = ", ".join(
-                    [f"{bc.OKBLUE}{path}{bc.ENDC}" for path in pr.paths_not_ported]
+                    [
+                        f"{bc.OKBLUE}{path}{bc.ENDC}"
+                        for path in pr.paths_not_ported
+                    ]
+                )
+                lines_to_print.append(
+                    f"\t=> Not ported: {pr_paths_not_ported}"
                 )
-                lines_to_print.append(f"\t=> Not ported: {pr_paths_not_ported}")
             lines_to_print.append(
                 f"\t=> {bc.BOLD}{bc.OKBLUE}{len(self.commits_diff[pr])} "
                 f"commit(s){bc.END} not (fully) ported"
             )
             if verbose or not pr.number:
                 for commit in self.commits_diff[pr]:
                     lines_to_print.append(
-                        f"\t\t{bc.DIM}{commit.hexsha[:8]} " f"{commit.summary}{bc.ENDD}"
+                        f"\t\t{bc.DIM}{commit.hexsha[:8]} "
+                        f"{commit.summary}{bc.ENDD}"
                     )
         if fake_pr:
             # We have commits without PR, adapt the message
             i -= 1
             nb_commits = len(self.commits_diff[fake_pr])
             message = (
                 f"{bc.BOLD}{bc.OKBLUE}{i} pull request(s){bc.END} "
                 f"and {bc.BOLD}{bc.OKBLUE}{nb_commits} commit(s) w/o "
                 f"PR{bc.END} related to '{bc.OKBLUE}{self.path}"
-                f"{bc.ENDC}' to port from {self.app.from_branch.ref()} "
-                f"to {self.app.to_branch.ref()}"
+                f"{bc.ENDC}' to port from {self.from_branch.ref()} "
+                f"to {self.to_branch.ref()}"
             )
         else:
             message = (
                 f"{bc.BOLD}{bc.OKBLUE}{i} pull request(s){bc.END} "
                 f"related to '{bc.OKBLUE}{self.path}{bc.ENDC}' to port from "
-                f"{self.app.from_branch.ref()} to {self.app.to_branch.ref()}"
+                f"{self.from_branch.ref()} to {self.to_branch.ref()}"
             )
         lines_to_print.insert(0, message)
-        self._print("\n".join(lines_to_print))
+        print("\n".join(lines_to_print))
 
     def get_commits_diff(self):
         """Returns the commits which do not exist in `to_branch`, grouped by
         their related Pull Request.
 
         :return: a dict {PullRequest: {Commit: data, ...}, ...}
         """
         commits_by_pr = defaultdict(list)
         for commit in self.from_branch_path_commits:
             if commit in self.to_branch_all_commits:
-                self.app.cache.mark_commit_as_ported(commit.hexsha)
                 continue
             # Get related Pull Request if any
-            pr = self._get_original_pr(commit)
-            if pr:
-                for pr_commit_sha in pr.commits:
-                    try:
-                        raw_commit = self.app.repo.commit(pr_commit_sha)
-                    except ValueError:
-                        # Ignore commits referenced by a PR but not present
-                        # in the stable branches
-                        continue
-                    pr_commit = g.Commit(raw_commit)
-                    if self._skip_commit(pr_commit):
-                        continue
-                    pr_commit_paths = {
-                        path for path in pr_commit.paths if not path_to_skip(path)
-                    }
-                    pr.paths.update(pr_commit_paths)
-                    # Check that this PR commit does not change the current
-                    # addon we are interested in, in such case also check
-                    # for each updated addons that the commit has already
-                    # been ported.
-                    # Indeed a commit could have been ported partially
-                    # in the past (with git-format-patch), and we now want
-                    # to port the remaining chunks.
-                    if pr_commit not in self.to_branch_path_commits:
-                        paths = set(pr_commit_paths)
-                        # A commit could have been ported several times
-                        # if it was impacting several addons and the
-                        # migration has been done with git-format-patch
-                        # on each addon separately
-                        to_branch_all_commits = self.to_branch_all_commits[:]
-                        skip_pr_commit = False
-                        with g.no_strict_commit_equality():
-                            while pr_commit in to_branch_all_commits:
-                                index = to_branch_all_commits.index(pr_commit)
-                                ported_commit = to_branch_all_commits.pop(index)
-                                ported_commit_paths = {
-                                    path
-                                    for path in ported_commit.paths
-                                    if not path_to_skip(path)
-                                }
-                                pr.ported_paths.update(ported_commit_paths)
-                                pr_commit.ported_commits.append(ported_commit)
-                                paths -= ported_commit_paths
-                                if not paths:
-                                    # The ported commits have already updated
-                                    # the same addons than the original one,
-                                    # we can skip it.
-                                    skip_pr_commit = True
-                        if skip_pr_commit:
+            if any("github.com" in remote.url for remote in self.repo.remotes):
+                gh_commit_pulls = misc._request_github(
+                    f"repos/{self.upstream_org}/{self.repo_name}"
+                    f"/commits/{commit.hexsha}/pulls"
+                )
+                full_repo_name = f"{self.upstream_org}/{self.repo_name}"
+                gh_commit_pull = [
+                    data for data in gh_commit_pulls
+                    if data["base"]["repo"]["full_name"] == full_repo_name
+                ]
+                # Fake PR for commits w/o related PR
+                pr = misc.PullRequest(*[""] * 6, tuple(), tuple())
+                if gh_commit_pull:
+                    pr = self._new_pull_request_from_github_data(gh_commit_pull[0])
+                    # Get all commits of the related PR as they could update
+                    # others addons than the one the user is interested in
+                    gh_pr_commits = misc._request_github(
+                        f"repos/{self.upstream_org}/{self.repo_name}"
+                        f"/pulls/{pr.number}/commits"
+                    )
+                    for gh_pr_commit in gh_pr_commits:
+                        try:
+                            raw_commit = self.repo.commit(gh_pr_commit["sha"])
+                        except ValueError:
+                            # Ignore commits referenced by a PR but not present
+                            # in the stable branches
                             continue
-                    # We want to port commits that were still not ported
-                    # for the addon we are interested in.
-                    # If the commit has already been included, skip it.
-                    if (
-                        pr_commit in self.to_branch_path_commits
-                        and pr_commit in self.to_branch_all_commits
-                    ):
-                        continue
-                    existing_pr_commits = commits_by_pr.get(pr, [])
-                    for existing_pr_commit in existing_pr_commits:
+                        pr_commit = misc.Commit(raw_commit)
+                        if self._skip_commit(pr_commit):
+                            continue
+                        pr_commit_paths = set(
+                            path for path in pr_commit.paths
+                            if not path_to_skip(path)
+                        )
+                        pr.paths.update(pr_commit_paths)
+                        # Check that this PR commit does not change the current
+                        # addon we are interested in, in such case also check
+                        # for each updated addons that the commit has already
+                        # been ported.
+                        # Indeed a commit could have been ported partially
+                        # in the past (with git-format-patch), and we now want
+                        # to port the remaining chunks.
+                        if pr_commit not in self.to_branch_path_commits:
+                            paths = set(pr_commit_paths)
+                            # A commit could have been ported several times
+                            # if it was impacting several addons and the
+                            # migration has been done with git-format-patch
+                            # on each addon separately
+                            to_branch_all_commits = self.to_branch_all_commits[:]
+                            skip_pr_commit = False
+                            with misc.no_strict_commit_equality():
+                                while pr_commit in to_branch_all_commits:
+                                    index = to_branch_all_commits.index(pr_commit)
+                                    ported_commit = to_branch_all_commits.pop(index)
+                                    ported_commit_paths = set(
+                                        path for path in ported_commit.paths
+                                        if not path_to_skip(path)
+                                    )
+                                    pr.ported_paths.update(ported_commit_paths)
+                                    pr_commit.ported_commits.append(ported_commit)
+                                    paths -= ported_commit_paths
+                                    if not paths:
+                                        # The ported commits have already updated
+                                        # the same addons than the original one,
+                                        # we can skip it.
+                                        skip_pr_commit = True
+                            if skip_pr_commit:
+                                continue
+                        # We want to port commits that were still not ported
+                        # for the addon we are interested in.
+                        # If the commit has already been included, skip it.
                         if (
-                            existing_pr_commit == pr_commit
-                            and existing_pr_commit.hexsha == pr_commit.hexsha
+                                pr_commit in self.to_branch_path_commits
+                                and pr_commit in self.to_branch_all_commits
                         ):
-                            # This PR commit has already been appended, skip
-                            break
-                    else:
-                        commits_by_pr[pr].append(pr_commit)
-            # No related PR: add the commit to the fake PR
+                            continue
+                        existing_pr_commits = commits_by_pr.get(pr, [])
+                        for existing_pr_commit in existing_pr_commits:
+                            if (
+                                existing_pr_commit == pr_commit and
+                                existing_pr_commit.hexsha == pr_commit.hexsha
+                            ):
+                                # This PR commit has already been appended, skip
+                                break
+                        else:
+                            commits_by_pr[pr].append(pr_commit)
+                # No related PR: add the current commit anyway
+                else:
+                    commits_by_pr[pr].append(commit)
             else:
-                commits_by_pr[FAKE_PR].append(commit)
+                # FIXME log?
+                pass
         # Sort PRs on the merge date (better to port them in the right order).
         # Do not return blacklisted PR.
         sorted_commits_by_pr = {}
         for pr in sorted(commits_by_pr, key=lambda pr: pr.merged_at or ""):
-            blacklisted = self.app.storage.is_pr_blacklisted(pr.ref)
-            if not blacklisted:
-                # TODO: Backward compat for old tracking only by number
-                blacklisted = self.app.storage.is_pr_blacklisted(pr.number)
-            if blacklisted:
+            if self.storage.is_pr_blacklisted(
+                    self.from_branch.name, self.to_branch.name, self.path, pr.number
+                    ):
                 msg = (
-                    f"{bc.DIM}PR #{pr.number}" if pr.number else "Orphaned commits"
-                ) + f" blacklisted ({blacklisted}){bc.ENDD}"
-                self._print(msg)
+                    f"{bc.DIM}PR #{pr.number}"
+                    if pr.number else "Orphaned commits"
+                ) + f" blacklisted{bc.ENDD}"
+                print(msg)
                 continue
             sorted_commits_by_pr[pr] = commits_by_pr[pr]
         return sorted_commits_by_pr
 
-    def _get_original_pr(self, commit: g.Commit):
-        """Return the original PR of a given commit."""
-        # Try to get the data from the user's cache first
-        data = self.app.cache.get_pr_from_commit(commit.hexsha)
-        if data:
-            return g.PullRequest(**data)
-        # Request GitHub to get them
-        if not any("github.com" in remote.url for remote in self.app.repo.remotes):
-            return
-        raw_data = self.app.github.get_original_pr(
-            self.app.from_org,
-            self.app.repo_name,
-            self.app.from_branch.name,
-            commit.hexsha,
+    @staticmethod
+    def _new_pull_request_from_github_data(data, paths=None, ported_paths=None):
+        """Create a new PullRequest instance from GitHub data."""
+        pr_number = data["number"]
+        pr_url = data["html_url"]
+        pr_author = data["user"].get("login", "")
+        pr_title = data["title"]
+        pr_body = data["body"]
+        pr_merge_at = data["merged_at"]
+        return misc.PullRequest(
+            number=pr_number,
+            url=pr_url,
+            author=pr_author,
+            title=pr_title,
+            body=pr_body,
+            merged_at=pr_merge_at,
+            paths=paths,
+            ported_paths=ported_paths,
         )
-        if raw_data:
-            # Get all commits of the PR as they could update others addons
-            # than the one the user is interested in.
-            # NOTE: commits fetched from PR are already in the right order
-            pr_number = raw_data["number"]
-            pr_commits_data = self.app.github.request(
-                f"repos/{self.app.from_org}/{self.app.repo_name}"
-                f"/pulls/{pr_number}/commits?per_page=100"
-            )
-            pr_commits = [pr["sha"] for pr in pr_commits_data]
-            data = {
-                "number": raw_data["number"],
-                "url": raw_data["html_url"],
-                "author": raw_data["user"].get("login", ""),
-                "title": raw_data["title"],
-                "body": raw_data["body"],
-                "merged_at": raw_data["merged_at"],
-                "commits": pr_commits,
-            }
-            self.app.cache.store_commit_pr(commit.hexsha, data)
-            return g.PullRequest(**data)
```

### Comparing `oca_port-0.15/oca_port.egg-info/PKG-INFO` & `oca_port-0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: oca_port
-Version: 0.15
+Version: 0.9
 Summary: OCA tool to help with modules migration
 Author: Odoo Community Association (OCA)
-Author-email: Sébastien Alix <sebastien.alix@camptocamp.com>, Simone Orsi <simone.orsi@camptocamp.com>
+Author-email: Sébastien Alix <sebastien.alix@camptocamp.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -176,41 +176,21 @@
 Keywords: odoo,oca,port,migration,modules,addons
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Odoo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: gitpython
-Requires-Dist: requests
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: coverage; extra == "test"
-
-[![Pre-commit Status](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml/badge.svg?branch=main)](https://github.com/OCA/oca-port/actions/workflows/pre-commit.yml?query=branch%3Amain)
 
 oca-port
 ========
 
 Tool helping to port an addon or missing commits of an addon from one branch
 to another.
 
-Installing
-----------
-
-    $ pipx install oca-port
-    $ #OR
-    $ git clone git@github.com:oca/oca-port.git
-    $ cd oca-port
-    $ pipx install .
-
-Using
------
-
 If the addon does not exist on the target branch, it will assist the user in
 the migration, following the OCA migration guide.
 
 If the addon already exists on the target branch, it will retrieve missing
 commits to port. If a Pull Request exists for a missing commit, it will be
 ported with all its commits if they were not yet (fully) ported.
 
@@ -219,86 +199,30 @@
     $ export GITHUB_TOKEN=<token>
     $ oca-port 14.0 15.0 shopfloor --verbose
 
 To effectively migrate the addon or port its commits, use the `--fork` option:
 
     $ oca-port 14.0 15.0 shopfloor --fork camptocamp
 
-You can also directly blacklist a bunch of PRs on a given branch thanks to the
-`oca-port-pr` tool:
-
-    $ oca-port-pr blacklist OCA/wms#250,OCA/wms#251 15.0 shopfloor
-
-You could give a more detailed reason of this blacklist with `--reason` parameter:
-
-    $ oca-port-pr blacklist OCA/wms#250,OCA/wms#251 15.0 shopfloor --reason "Refactored in 15.0, not needed anymore"
-
-And if the module has been moved to another repository, you can specify its remote as well:
-
-    $ git remote add new_repo git@github.com:OCA/new-repo.git
-    $ oca-port-pr blacklist OCA/wms#250,OCA/wms#251 15.0 shopfloor --remote new_repo
-
 Migration of addon
 ------------------
 
 The tool follows the usual OCA migration guide to port commits of an addon,
 and will invite the user to fullfill the mentionned steps that can't be
 performed automatically.
 
 **Output example:**
 ![image](https://user-images.githubusercontent.com/5315285/129355442-f863adff-33c0-4c91-b0cb-b6882312e340.png)
 
-If used with the `--non-interactive` option, the returned exit code is `100`
-if an addon could be migrated.
-
 Port of commits/Pull Requests
 -----------------------------
 
 The tool will ask the user if he wants to open draft pull requests against
 the upstream repository.
 
 If there are several Pull Requests to port, it will ask the user if he wants
 to base the next PR on the previous one, allowing the user to cumulate ported
 PRs in one branch and creating a draft PR against the upstream repository
 with all of them.
 
-More details here : [OCA Days 2022 - Sébastien Alix and Simone Orsi: oca-port:new OCA tool to help with modules migration](https://www.youtube.com/watch?v=idGLkQiJ5N0)
-
 **Output example (with --verbose):**
 ![oca_port_pr_verbose](https://user-images.githubusercontent.com/5315285/129207041-12ac6c4a-ea96-4b8c-bd68-ae661531ad92.png)
-
-If used with the `--non-interactive` option, the returned exit code is `110`
-if some pull requests/commits could be ported.
-
-API
----
-
-You can also use `oca-port` as a Python package:
-
-```python
->>> import oca_port
->>> app = oca_port.App(
-...     from_branch="14.0",
-...     to_branch="16.0",
-...     addon="stock_move_auto_assign",
-...     from_org": "OCA",
-...     from_remote": "origin",
-...     repo_path": "/home/odoo/OCA/stock-logistics-warehouse",
-...     output": "json",
-...     fetch": True,
-...     github_token: "ghp_sheeXai3xu1yoopheiquoo3ohch0AefooSob"
-... )
->>> json_data = app.run()
->>> data = json.loads(json_data)
->>> from pprint import pprint as pp
->>> pp(data)
-{'process': 'port_commits',
- 'results': {'1631': {'author': 'TDu',
-                      'merged_at': '2023-04-04T17:06:03Z',
-                      'missing_commits': ['41416c1d7dad15ce4745e07d0541c79e938c2710',
-                                          'd43985a443e29641447a3811f2310d54b886ab3d',
-                                          '6bd9fcff3e814a6802c7aefadb9c646194cde42b'],
-                      'ref': 'OCA/stock-logistics-warehouse#1631',
-                      'title': '[14][ADD] stock_move_auto_assign_auto_release '
-                               '- backport',
-                      'url': 'https://github.com/OCA/stock-logistics-warehouse/pull/1631'}}}
-```
```

### Comparing `oca_port-0.15/pyproject.toml` & `oca_port-0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [project]
 name = "oca_port"
 authors = [
     {name = "Odoo Community Association (OCA)"},
-    {name = "Sébastien Alix", email="sebastien.alix@camptocamp.com"},
-    {name = "Simone Orsi", email="simone.orsi@camptocamp.com"}
+    {name = "Sébastien Alix", email="sebastien.alix@camptocamp.com"}
 ]
 description = "OCA tool to help with modules migration"
 readme = "README.md"
 keywords = ["odoo", "oca", "port", "migration", "modules", "addons"]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
@@ -24,24 +23,17 @@
 
 [project.urls]
 homepage = "https://github.com/OCA/oca-port"
 documentation = "https://github.com/OCA/oca-port"
 repository = "https://github.com/OCA/oca-port"
 
 [project.scripts]
-oca-port = "oca_port.cli.main:main"
-oca-port-pr = "oca_port.cli.pr:cli"
-
-[project.optional-dependencies]
-test = [
-  "pytest",
-  "coverage",
-]
+oca-port = "oca_port:main"
 
 [build-system]
-requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools_scm]
```

