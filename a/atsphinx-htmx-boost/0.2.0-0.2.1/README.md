# Comparing `tmp/atsphinx_htmx_boost-0.2.0.tar.gz` & `tmp/atsphinx_htmx_boost-0.2.1.tar.gz`

## Comparing `atsphinx_htmx_boost-0.2.0.tar` & `atsphinx_htmx_boost-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,44 @@
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/.editorconfig
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/.python-version
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/CHANGES.rst
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/requirements.lock
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/.gitignore
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/.ruff.toml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/Makefile
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/changelogs.rst
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/conf.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/make.bat
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/usage.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/changelogs/v0.1.0.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/changelogs/v0.1.1.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/changelogs/v0.1.2.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/changelogs/v0.1.3.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/doc/changelogs/v0.1.4.rst
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/src/atsphinx/htmx_boost/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/tests/.ruff.toml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/tests/test_it.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/tests/test-root/conf.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/tests/test-root/index.rst
--rwxr-xr-x   0        0        0     2636 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/tools/release-commit.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/LICENSE
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/README.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.age.toml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.editorconfig
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.python-version
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/CHANGES.rst
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/requirements.lock
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.github/workflows/deploy-doc.yml
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/.gitignore
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/.ruff.toml
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/Makefile
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs.rst
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/conf.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/make.bat
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/usage.rst
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/changelogs.po
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/index.po
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/usage.po
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/changelogs/v0.1.0.po
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/changelogs/v0.1.1.po
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/changelogs/v0.1.2.po
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/changelogs/v0.1.3.po
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/_locales/ja/LC_MESSAGES/changelogs/v0.1.4.po
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs/v0.1.0.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs/v0.1.1.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs/v0.1.2.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs/v0.1.3.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs/v0.1.4.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/doc/changelogs/v0.2.0.rst
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/src/atsphinx/htmx_boost/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/tests/.ruff.toml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/tests/test_it.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/tests/test-root/conf.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/tests/test-root/index.rst
+-rwxr-xr-x   0        0        0     2552 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/tools/release-commit.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/LICENSE
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/README.rst
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 atsphinx_htmx_boost-0.2.1/PKG-INFO
```

### Comparing `atsphinx_htmx_boost-0.2.0/.editorconfig` & `atsphinx_htmx_boost-0.2.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `atsphinx_htmx_boost-0.2.0/requirements-dev.lock` & `atsphinx_htmx_boost-0.2.1/requirements-dev.lock`

 * *Files 17% similar despite different names*

```diff
@@ -8,77 +8,88 @@
 #   with-sources: false
 
 -e file:.
 alabaster==0.7.16
     # via sphinx
 atsphinx-helper==0.1.0
     # via atsphinx-htmx-boost
+atsphinx-mini18n==0.2.1
 attrs==23.2.0
     # via cattrs
     # via lsprotocol
 babel==2.14.0
     # via sphinx
+    # via sphinx-intl
 beautifulsoup4==4.12.3
     # via atsphinx-htmx-boost
     # via furo
 cattrs==23.2.3
     # via lsprotocol
     # via pygls
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
+click==8.1.7
+    # via sphinx-intl
 docutils==0.20.1
     # via sphinx
     # via sphinx-rtd-theme
 esbonio==0.16.4
 furo==2024.1.29
-idna==3.6
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.3
     # via sphinx
 lsprotocol==2023.0.1
     # via pygls
+lxml==5.2.1
+    # via atsphinx-htmx-boost
 markupsafe==2.1.5
     # via jinja2
-packaging==23.2
+packaging==24.0
     # via pytest
     # via sphinx
 platformdirs==4.2.0
     # via esbonio
 pluggy==1.4.0
     # via pytest
-pygls==1.3.0
+pygls==1.3.1
     # via esbonio
 pygments==2.17.2
     # via furo
     # via sphinx
 pyspellchecker==0.8.1
     # via esbonio
 pytest==8.0.2
 requests==2.31.0
     # via sphinx
+setuptools==69.5.1
+    # via sphinx-intl
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.2.6
     # via atsphinx-helper
     # via atsphinx-htmx-boost
+    # via atsphinx-mini18n
     # via esbonio
     # via furo
     # via sphinx-basic-ng
+    # via sphinx-intl
     # via sphinx-rtd-theme
     # via sphinxcontrib-jquery
 sphinx-basic-ng==1.0.0b2
     # via furo
+sphinx-intl==2.1.0
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
```

### Comparing `atsphinx_htmx_boost-0.2.0/requirements.lock` & `atsphinx_htmx_boost-0.2.1/requirements.lock`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     # via sphinx
 idna==3.6
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.3
     # via sphinx
+lxml==5.2.1
+    # via atsphinx-htmx-boost
 markupsafe==2.1.5
     # via jinja2
 packaging==23.2
     # via sphinx
 pygments==2.17.2
     # via sphinx
 requests==2.31.0
```

### Comparing `atsphinx_htmx_boost-0.2.0/.github/workflows/main.yml` & `atsphinx_htmx_boost-0.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `atsphinx_htmx_boost-0.2.0/doc/make.bat` & `atsphinx_htmx_boost-0.2.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx_htmx_boost-0.2.0/doc/usage.rst` & `atsphinx_htmx_boost-0.2.1/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `atsphinx_htmx_boost-0.2.0/src/atsphinx/htmx_boost/__init__.py` & `atsphinx_htmx_boost-0.2.1/src/atsphinx/htmx_boost/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from atsphinx.helper.decorators import emit_only
 from bs4 import BeautifulSoup
 from sphinx.application import Sphinx
 from sphinx.jinja2glue import BuiltinTemplateLoader
 from sphinx.util.docutils import nodes
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 class WithHtmxTemplateLoader(BuiltinTemplateLoader):  # noqa: D101
     def render(self, template: str, context: dict) -> str:  # noqa: D102
         out = super().render(template, context)
         if not template.endswith(".html"):
             return out
-        soup = BeautifulSoup(out, "html.parser")
+        soup = BeautifulSoup(out, "lxml")
         preload = context.get("htmx_boost_preload", "")
         if preload:
             soup.body.attrs["hx-ext"] = "preload"
         for a in soup.find_all("a", {"class": "internal"}):
             a["hx-boost"] = "true"
             a["preload"] = preload
-        return soup.prettify()
+        return str(soup)
 
 
 @emit_only(formats=["html"])
 def setup_custom_loader(app: Sphinx):
     """Inject extra values about htmx-boost into generated config."""
     app.config.template_bridge = "atsphinx.htmx_boost.WithHtmxTemplateLoader"
     app.builder.init()
@@ -50,9 +50,9 @@
     """Load as Sphinx-extension."""
     app.connect("builder-inited", setup_custom_loader)
     app.connect("html-page-context", pass_extra_context)
     app.add_config_value("htmx_boost_preload", "", "env", [str])
     return {
         "version": __version__,
         "env_version": 1,
-        "paralell_read_safe": True,
+        "parallel_read_safe": True,
     }
```

### Comparing `atsphinx_htmx_boost-0.2.0/tests/test_it.py` & `atsphinx_htmx_boost-0.2.1/tests/test_it.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,14 @@
         if "internal" not in a.attrs.get("class", []):
             assert "hx-boost" not in a.attrs
 
 
 @pytest.mark.sphinx("html", confoverrides={"html_use_opensearch": True})
 def test__with_opensearch(app: SphinxTestApp, status: StringIO, warning: StringIO):
     app.build()
+
+
+@pytest.mark.sphinx("html")
+def test__inline_code(app: SphinxTestApp):
+    app.build()
+    html = (app.outdir / "index.html").read_text()
+    assert "</span></code>" in html
```

### Comparing `atsphinx_htmx_boost-0.2.0/tools/release-commit.py` & `atsphinx_htmx_boost-0.2.1/tools/release-commit.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,16 @@
     cmd = ["rye", "version"]
     proc = subprocess.run(cmd, stdout=subprocess.PIPE)
     return proc.stdout.decode("utf-8").strip()
 
 
 def bump_version(level: str) -> str:  # noqa: D103
     """Bump version for sources."""
-    cmd = ["rye", "version", "--bump", level]
+    cmd = ["age", level]
     subprocess.run(cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE)
-    return get_version()
 
 
 def replace_version(target, current_version: str, new_version: str):
     """Change old/new version text from source."""
     src = root / target["filename"]
     lines = []
     from_ = target["search"].format(current_version=current_version)
@@ -74,20 +73,19 @@
     move_to.parent.mkdir(parents=True, exist_ok=True)
     shutil.copy(target, move_to)
     target.write_text(CHANGELOG_TEMPLATE.render(version=new_version, now=now))
 
 
 def main(args: argparse.Namespace):
     """Handle multi functions."""
-    pyproject = tomllib.loads((root / "pyproject.toml").read_text())
-    current_version = get_version()
+    pyproject_toml = root / "pyproject.toml"
+    current_version = tomllib.loads(pyproject_toml.read_text())["project"]["version"]
     print(f"Current version: v{current_version}")
-    new_version = bump_version(args.level)
+    bump_version(args.level)
+    new_version = tomllib.loads(pyproject_toml.read_text())["project"]["version"]
     print(f"Next version:    v{new_version}")
-    for target in pyproject["tool"]["local"]["bumpversion"]["files"]:
-        replace_version(target, current_version, new_version)
     update_changes(current_version, new_version)
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     main(args)
```

### Comparing `atsphinx_htmx_boost-0.2.0/.gitignore` & `atsphinx_htmx_boost-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx_htmx_boost-0.2.0/LICENSE` & `atsphinx_htmx_boost-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx_htmx_boost-0.2.0/pyproject.toml` & `atsphinx_htmx_boost-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [project]
 name = "atsphinx-htmx-boost"
-version = "0.2.0"
+version = "0.2.1"
 description = "[EXPERIMENTAL] Improve user-experience for Sphinx document."
 authors = [
     { name = "Kazuya Takei", email = "myself@attakei.net" }
 ]
 dependencies = [
     "beautifulsoup4",
+    "lxml",
     "sphinx",
     "atsphinx-helper",
 ]
 readme = "README.rst"
 requires-python = ">= 3.8"
 license = "Apache-2.0"
 classifiers = [
@@ -48,14 +49,16 @@
 dev-dependencies = [
     "furo~=2024.1.29",
     "jinja2~=3.1.3",
     "pytest~=8.0.2",
     "sphinx~=7.2.6",
     "sphinx-rtd-theme~=2.0.0",
     "esbonio~=0.16.4",
+    "sphinx-intl~=2.1.0",
+    "atsphinx-mini18n~=0.2.0",
 ]
 
 [tool.rye.scripts]
 setup = {chain = ["setup:sync", "setup:pre-commit"]}
 "setup:sync" = "rye sync --no-lock --all-features"
 "setup:pre-commit" = "pre-commit install"
 bump = "./tools/release-commit.py"
@@ -63,18 +66,13 @@
 
 [tool.ruff.lint]
 select = ["C90", "D", "E", "F", "I", "W"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
-[[tool.local.bumpversion.files]]
-filename = "src/atsphinx/htmx_boost/__init__.py"
-search = "__version__ = \"{current_version}\""
-replace = "__version__ = \"{new_version}\""
-
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/atsphinx"]
 only-includes = ["src/atsphinx"]
```

### Comparing `atsphinx_htmx_boost-0.2.0/PKG-INFO` & `atsphinx_htmx_boost-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atsphinx-htmx-boost
-Version: 0.2.0
+Version: 0.2.1
 Summary: [EXPERIMENTAL] Improve user-experience for Sphinx document.
 Project-URL: Home, https://github.com/atsphinx/htmx-boost
 Project-URL: Repository, https://github.com/atsphinx/htmx-boost
 Project-URL: Issues, https://github.com/atsphinx/htmx-boost/issues
 Project-URL: Changelog, https://github.com/atsphinx/htmx-boost/blob/main/CHANGES.rst
 Author-email: Kazuya Takei <myself@attakei.net>
 License-Expression: Apache-2.0
@@ -25,14 +25,15 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Requires-Python: >=3.8
 Requires-Dist: atsphinx-helper
 Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
 Requires-Dist: sphinx
 Description-Content-Type: text/x-rst
 
 ===================
 atsphinx-htmx-boost
 ===================
```

