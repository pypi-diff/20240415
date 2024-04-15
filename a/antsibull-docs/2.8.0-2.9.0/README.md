# Comparing `tmp/antsibull_docs-2.8.0.tar.gz` & `tmp/antsibull_docs-2.9.0.tar.gz`

## Comparing `antsibull_docs-2.8.0.tar` & `antsibull_docs-2.9.0.tar`

### file list

```diff
@@ -1,655 +1,656 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.flake8
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.pylintrc.automated
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.readthedocs.yml
--rw-r--r--   0        0        0    61846 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/CHANGELOG.md.license
--rw-r--r--   0        0        0    38107 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/CHANGELOG.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/LICENSE
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/antsibull-docs.cfg
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/codecov.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/docs-requirements.txt
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/mkdocs.yml
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/noxfile.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.github/patchback.yml
--rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.github/workflows/antsibull-docs.yml
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.github/workflows/build-css.yml
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.reuse/dep5
--rw-r--r--   0        0        0    46168 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/changelogs/fragments/.keep
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/docs/collection-docs.md
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/docs/index.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/docs/package-docs.md
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/docs/schemas.rst
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/_pydantic_compat.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/app_context.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/augment_docs.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/collection_config.py
--rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/collection_links.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/constants.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/env_variables.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/extra_docs.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/lint_extra_docs.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/lint_helpers.py
--rw-r--r--   0        0        0    33601 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/lint_plugin_docs.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/plugin_docs.py
--rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/process_docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/py.typed
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/rstcheck.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/__init__.py
--rw-r--r--   0        0        0    30639 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/antsibull_docs.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/__init__.py
--rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/_build.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/collection.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/collection_plugins.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/current.py
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/devel.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/lint_docs.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/plugin.py
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py
--rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/stable.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/__init__.py
--rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/ansible_2_10_routing.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/collection_links.rst.j2
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2
--rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2
--rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/collection_links.rst.j2
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/_gitignore.j2
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/build_sh.j2
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/conf_py.j2
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/__init__.py
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/ansible_doc.py
--rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/fqcn.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/parsing.py
--rw-r--r--   0        0        0    19479 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/routing.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/jinja2/__init__.py
--rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/jinja2/environment.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/jinja2/filters.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/jinja2/tests.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/markup/__init__.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/markup/_counter.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/markup/htmlify.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/markup/rstify.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/markup/semantic_helper.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/ansible_doc.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/app_context.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/collection_config.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/collection_links.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/ansible_doc.py
--rw-r--r--   0        0        0    25466 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/base.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/callback.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/module.py
--rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/plugin.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/positional.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/role.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/utils/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/utils/collection_name_transformer.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/utils/get_pkg_data.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/utils/rst.py
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/vendored/ansible.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/write_docs/__init__.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/write_docs/collections.py
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/write_docs/hierarchy.py
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/write_docs/indexes.py
--rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/write_docs/plugin_stubs.py
--rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/antsibull_docs/write_docs/plugins.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/__init__.py
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/antsibull-minimal.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/antsibull-minimal.css.license
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/antsibull.sty
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/assets.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default-autodark.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default-autodark.css.license
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default-dark.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default-dark.css.license
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default.css
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default.css.license
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/directive_helper.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/directives.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/nodes.py
--rw-r--r--   0        0        0    14747 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/roles.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/sphinx_helper.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/.gitignore
--rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/browserslistrc
--rwxr-xr-x   0        0        0     1224 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/build.sh
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/colors-default-autodark.scss
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/colors-default-dark.scss
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/colors-default.scss
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/cssnano.config.js
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/default-colors-dark.scss
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/default-colors-light.scss
--rw-r--r--   0        0        0    60996 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/package-lock.json
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/package-lock.json.license
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/package.json
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/package.json.license
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/schemas/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/src/sphinx_antsibull_ext/schemas/ansible_links.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/argcomplete.pyi
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/rstcheck.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/__init__.pyi
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/constants.pyi
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/release.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/cli/__init__.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/cli/arguments.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/collections/list.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/galaxy/collection.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/module_utils/_text.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/module_utils/common/json.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/plugins/loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/utils/collection_loader.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/ansible/utils/plugin_docs.pyi
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/jinja2/utils.pyi
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/rstcheck_core/__init__.pyi
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/rstcheck_core/checker.pyi
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/rstcheck_core/config.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/stubs/rstcheck_core/types.pyi
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/validate-html.py
--rw-r--r--   0        0        0  1061728 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-all-others.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-all-others.json.license
--rw-r--r--   0        0        0  1059812 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-all.json.license
--rw-r--r--   0        0        0  1056490 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns.col2-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns.col2-ns2.col.json.license
--rw-r--r--   0        0        0  1044677 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.col.json.license
--rw-r--r--   0        0        0  1023422 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.flatcol.json.license
--rw-r--r--   0        0        0    57717 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col1-ns.col2-ns2.col-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col1-ns.col2-ns2.col-ns2.flatcol.json.license
--rw-r--r--   0        0        0    45904 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col1-ns2.col-ns2.flatcol.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col1-ns2.col-ns2.flatcol.json.license
--rw-r--r--   0        0        0    29798 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col2.json.license
--rw-r--r--   0        0        0    42582 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns2.col.json.license
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-all-others.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-all-others.json.license
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-all.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-all.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-ns.col2.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-ns.col2.json.license
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-ns2.col.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-galaxy-cache-ns2.col.json.license
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-version.output
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible-version.output.license
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/ansible_doc_caching.py
--rwxr-xr-x   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/antsibull-docs-stub.py
--rwxr-xr-x   0        0        0     4342 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/build-docs-baseline.sh
--rwxr-xr-x   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/build-sphinx-init-baseline.sh
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/sanitize-ansible-doc-dump.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/sanitize-ansible-galaxy-list.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/test.rst
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/test_docs_baseline.py
--rw-r--r--   0        0        0   101489 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/test_docs_linting.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/test_sphinx_init_baseline.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/utils.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/environment_variables.rst
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_become.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_cache.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_callback.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_cliconf.rst
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_connection.rst
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_filter.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_inventory.rst
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_lookup.rst
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_module.rst
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_role.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_shell.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_strategy.rst
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_test.rst
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_vars.rst
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/index.rst
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/index.rst
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index.rst
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_become.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_cache.rst
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_callback.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_cliconf.rst
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_connection.rst
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_filter.rst
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_inventory.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_lookup.rst
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_module.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_role.rst
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_shell.rst
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_strategy.rst
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_test.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_vars.rst
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/index.rst
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col1/index.rst
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst
--rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/index.rst
--rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/index.rst
--rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst
--rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_redirect_module.rst
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/is_bar_test.rst
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/build.sh
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/conf.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/requirements.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      903 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/build.sh
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/conf.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/requirements.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/rst/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/build.sh
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/conf.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/requirements.txt
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/rst/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
--rwxr-xr-x   0        0        0      896 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/build.sh
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/conf.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/requirements.txt
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/rst/index.rst
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/bar_test.rst
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_become.rst
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_module.rst
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_role.rst
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_test.rst
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/index.rst
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_become.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_module.rst
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_role.rst
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_test.rst
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
--rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
--rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
--rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
--rw-r--r--   0        0        0     9261 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/main.yml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/baz.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/test_schema.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_become.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_become.json.license
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_become_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_become_results.json.license
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cache.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cache.json.license
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cache_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cache_results.json.license
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_callback.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_callback.json.license
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_callback_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_callback_results.json.license
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cliconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cliconf.json.license
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cliconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cliconf_results.json.license
--rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_connection.json.license
--rw-r--r--   0        0        0    23771 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_connection_results.json.license
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_filter.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_filter.json.license
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_filter_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_filter_results.json.license
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_httpapi.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_httpapi.json.license
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_httpapi_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_httpapi_results.json.license
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_inventory.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_inventory.json.license
--rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_inventory_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_inventory_results.json.license
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_lookup.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_lookup.json.license
--rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_lookup_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_lookup_results.json.license
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_module.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_module.json.license
--rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_module_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_module_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_netconf.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_netconf.json.license
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_netconf_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_netconf_results.json.license
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_role.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_role.json.license
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_role_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_role_results.json.license
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_shell.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_shell.json.license
--rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_shell_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_shell_results.json.license
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_strategy.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_strategy.json.license
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_strategy_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_strategy_results.json.license
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_test.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_test.json.license
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_test_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_test_results.json.license
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_vars.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_vars.json.license
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_vars_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/one_vars_results.json.license
--rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/ssh_connection.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/ssh_connection.json.license
--rw-r--r--   0        0        0    56416 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/ssh_connection_results.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/functional/schema/good_data/ssh_connection_results.json.license
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/units/test_jinja2.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/units/markup/test_counter.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/units/markup/test_markup.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/tests/units/markup/test_semantic_helper.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/.gitignore
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/README.md
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 antsibull_docs-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.flake8
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.pylintrc.automated
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.readthedocs.yml
+-rw-r--r--   0        0        0    62505 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/CHANGELOG.md.license
+-rw-r--r--   0        0        0    38311 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/LICENSE
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/antsibull-docs.cfg
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/codecov.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/docs-requirements.txt
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/mkdocs.yml
+-rw-r--r--   0        0        0    10034 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/noxfile.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.github/patchback.yml
+-rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.github/workflows/antsibull-docs.yml
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.github/workflows/build-css.yml
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.reuse/dep5
+-rw-r--r--   0        0        0    46445 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/changelogs/fragments/.keep
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/docs/changelog.md -> ../CHANGELOG.md
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/docs/collection-docs.md
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/docs/index.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/docs/package-docs.md
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/docs/schemas.rst
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/_pydantic_compat.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/app_context.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/augment_docs.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/collection_config.py
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/collection_links.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/constants.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/env_variables.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/extra_docs.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/lint_extra_docs.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/lint_helpers.py
+-rw-r--r--   0        0        0    33601 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/lint_plugin_docs.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/plugin_docs.py
+-rw-r--r--   0        0        0    11388 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/process_docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/py.typed
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/rstcheck.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/__init__.py
+-rw-r--r--   0        0        0    30639 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/antsibull_docs.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/__init__.py
+-rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/_build.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/collection.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/collection_plugins.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/current.py
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/devel.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/lint_docs.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/plugin.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py
+-rw-r--r--   0        0        0     7446 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/stable.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/__init__.py
+-rw-r--r--   0        0        0   127036 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/ansible_2_10_routing.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/__init__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/collection_links.rst.j2
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2
+-rw-r--r--   0        0        0    13774 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/collection_links.rst.j2
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/_gitignore.j2
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/build_sh.j2
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/conf_py.j2
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/requirements_txt.j2
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/__init__.py
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/ansible_doc.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/fqcn.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/parsing.py
+-rw-r--r--   0        0        0    19479 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/routing.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/jinja2/__init__.py
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/jinja2/environment.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/jinja2/filters.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/jinja2/tests.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/markup/__init__.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/markup/_counter.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/markup/htmlify.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/markup/rstify.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/markup/semantic_helper.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/ansible_doc.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/app_context.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/collection_config.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/collection_links.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/__init__.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/ansible_doc.py
+-rw-r--r--   0        0        0    25466 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/base.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/callback.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/module.py
+-rw-r--r--   0        0        0     7150 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/plugin.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/positional.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/role.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/utils/collection_name_transformer.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/utils/get_pkg_data.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/utils/rst.py
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/vendored/ansible.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/write_docs/__init__.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/write_docs/collections.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/write_docs/hierarchy.py
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/write_docs/indexes.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/write_docs/plugin_stubs.py
+-rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/antsibull_docs/write_docs/plugins.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/__init__.py
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/antsibull-minimal.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/antsibull-minimal.css.license
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/antsibull.sty
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/assets.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default-autodark.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default-autodark.css.license
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default-dark.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default-dark.css.license
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default.css
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default.css.license
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/directive_helper.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/directives.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/nodes.py
+-rw-r--r--   0        0        0    14747 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/roles.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/sphinx_helper.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/.gitignore
+-rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/browserslistrc
+-rwxr-xr-x   0        0        0     1224 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/build.sh
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/colors-default-autodark.scss
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/colors-default-dark.scss
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/colors-default.scss
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/cssnano.config.js
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/default-colors-dark.scss
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/default-colors-light.scss
+-rw-r--r--   0        0        0    60996 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/package-lock.json
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/package-lock.json.license
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/package.json
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/package.json.license
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/schemas/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/src/sphinx_antsibull_ext/schemas/ansible_links.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/argcomplete.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/rstcheck.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/__init__.pyi
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/constants.pyi
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/release.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/cli/__init__.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/cli/arguments.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/collections/list.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/galaxy/collection.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/module_utils/_text.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/module_utils/common/json.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/plugins/loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/utils/collection_loader.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/ansible/utils/plugin_docs.pyi
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/jinja2/utils.pyi
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/rstcheck_core/__init__.pyi
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/rstcheck_core/checker.pyi
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/rstcheck_core/config.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/stubs/rstcheck_core/types.pyi
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/validate-html.py
+-rw-r--r--   0        0        0  1061728 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-all-others.json.license
+-rw-r--r--   0        0        0  1059812 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-all.json.license
+-rw-r--r--   0        0        0  1056490 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns.col2-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns.col2-ns2.col.json.license
+-rw-r--r--   0        0        0  1044677 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.col.json.license
+-rw-r--r--   0        0        0  1023422 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.flatcol.json.license
+-rw-r--r--   0        0        0    57717 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col1-ns.col2-ns2.col-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col1-ns.col2-ns2.col-ns2.flatcol.json.license
+-rw-r--r--   0        0        0    45904 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col1-ns2.col-ns2.flatcol.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col1-ns2.col-ns2.flatcol.json.license
+-rw-r--r--   0        0        0    29798 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col2.json.license
+-rw-r--r--   0        0        0    42582 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns2.col.json.license
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-all-others.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-all-others.json.license
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-all.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-all.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-ns.col2.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-ns.col2.json.license
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-ns2.col.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-galaxy-cache-ns2.col.json.license
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-version.output
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible-version.output.license
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/ansible_doc_caching.py
+-rwxr-xr-x   0        0        0      488 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/antsibull-docs-stub.py
+-rwxr-xr-x   0        0        0     4342 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/build-docs-baseline.sh
+-rwxr-xr-x   0        0        0     1346 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/build-sphinx-init-baseline.sh
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/sanitize-ansible-doc-dump.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/sanitize-ansible-galaxy-list.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/test.rst
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/test_docs_baseline.py
+-rw-r--r--   0        0        0   101489 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/test_docs_linting.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/test_sphinx_init_baseline.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/utils.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/environment_variables.rst
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_become.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_cache.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_callback.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_connection.rst
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_filter.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_inventory.rst
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_lookup.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_module.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_role.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_shell.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_strategy.rst
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_test.rst
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_vars.rst
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/index.rst
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_become.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_cache.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_callback.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_connection.rst
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_filter.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_role.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_shell.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_test.rst
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_vars.rst
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/index.rst
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index.rst
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_become.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_cache.rst
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_callback.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_connection.rst
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_filter.rst
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_inventory.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_lookup.rst
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_module.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_role.rst
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_shell.rst
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_strategy.rst
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_test.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_vars.rst
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/index.rst
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col1/index.rst
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst
+-rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/index.rst
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/index.rst
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_redirect_module.rst
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/build.sh
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/conf.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/requirements.txt
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      903 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/build.sh
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/conf.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/rst/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/build.sh
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/conf.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/requirements.txt
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/rst/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg
+-rwxr-xr-x   0        0        0      896 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/build.sh
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/conf.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/requirements.txt
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/rst/index.rst
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/bar_test.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_become.rst
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_module.rst
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_role.rst
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_test.rst
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/index.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/callback_index_stdout.rst
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_become.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_cache.rst
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_callback.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_cliconf.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_connection.rst
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_filter.rst
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_inventory.rst
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_lookup.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_module.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_role.rst
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_shell.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_strategy.rst
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_test.rst
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/index_vars.rst
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/index.rst
+-rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst
+-rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst
+-rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst
+-rw-r--r--   0        0        0     9261 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col1/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col1/galaxy.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col1/plugins/module_utils/empty.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/galaxy.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/config.yml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/meta/runtime.yml
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/main.yml
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/baz.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/config.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/extra-docs.yml
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/meta/runtime.yml
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/is_bar.yml -> bar.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/main.yml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/tasks/main.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/COPYING -> ../../../../../../LICENSE
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/galaxy.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/docs/docsite/config.yml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/other-collections/ansible_collections/ext/col/galaxy.yml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/test_schema.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_become.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_become.json.license
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_become_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_become_results.json.license
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cache.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cache.json.license
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cache_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cache_results.json.license
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_callback.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_callback.json.license
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_callback_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_callback_results.json.license
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cliconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cliconf.json.license
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cliconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cliconf_results.json.license
+-rw-r--r--   0        0        0    10708 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_connection.json.license
+-rw-r--r--   0        0        0    23771 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_connection_results.json.license
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_filter.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_filter.json.license
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_filter_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_filter_results.json.license
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_httpapi.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_httpapi.json.license
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_httpapi_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_httpapi_results.json.license
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_inventory.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_inventory.json.license
+-rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_inventory_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_inventory_results.json.license
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_lookup.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_lookup.json.license
+-rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_lookup_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_lookup_results.json.license
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_module.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_module.json.license
+-rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_module_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_module_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_netconf.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_netconf.json.license
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_netconf_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_netconf_results.json.license
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_role.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_role.json.license
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_role_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_role_results.json.license
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_shell.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_shell.json.license
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_shell_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_shell_results.json.license
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_strategy.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_strategy.json.license
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_strategy_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_strategy_results.json.license
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_test.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_test.json.license
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_test_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_test_results.json.license
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_vars.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_vars.json.license
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_vars_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/one_vars_results.json.license
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/ssh_connection.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/ssh_connection.json.license
+-rw-r--r--   0        0        0    56416 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/ssh_connection_results.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/functional/schema/good_data/ssh_connection_results.json.license
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/units/test_jinja2.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/units/markup/test_counter.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/units/markup/test_markup.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/tests/units/markup/test_semantic_helper.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/.gitignore
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/README.md
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0    10542 2020-02-02 00:00:00.000000 antsibull_docs-2.9.0/PKG-INFO
```

### Comparing `antsibull_docs-2.8.0/.pylintrc.automated` & `antsibull_docs-2.9.0/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/CHANGELOG.md` & `antsibull_docs-2.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,143 +1,160 @@
 # antsibull\-docs \-\- Ansible Documentation Build Scripts Release Notes
 
 **Topics**
+
+- <a href="#v2-9-0">v2\.9\.0</a>
+    - <a href="#release-summary">Release Summary</a>
+    - <a href="#minor-changes">Minor Changes</a>
 - <a href="#v2-8-0">v2\.8\.0</a>
-  - <a href="#release-summary">Release Summary</a>
-  - <a href="#minor-changes">Minor Changes</a>
-  - <a href="#bugfixes">Bugfixes</a>
+    - <a href="#release-summary-1">Release Summary</a>
+    - <a href="#minor-changes-1">Minor Changes</a>
+    - <a href="#bugfixes">Bugfixes</a>
 - <a href="#v2-7-0">v2\.7\.0</a>
-  - <a href="#release-summary-1">Release Summary</a>
-  - <a href="#minor-changes-1">Minor Changes</a>
-  - <a href="#bugfixes-1">Bugfixes</a>
+    - <a href="#release-summary-2">Release Summary</a>
+    - <a href="#minor-changes-2">Minor Changes</a>
+    - <a href="#bugfixes-1">Bugfixes</a>
 - <a href="#v2-6-1">v2\.6\.1</a>
-  - <a href="#release-summary-2">Release Summary</a>
-  - <a href="#bugfixes-2">Bugfixes</a>
+    - <a href="#release-summary-3">Release Summary</a>
+    - <a href="#bugfixes-2">Bugfixes</a>
 - <a href="#v2-6-0">v2\.6\.0</a>
-  - <a href="#release-summary-3">Release Summary</a>
-  - <a href="#minor-changes-2">Minor Changes</a>
-  - <a href="#bugfixes-3">Bugfixes</a>
+    - <a href="#release-summary-4">Release Summary</a>
+    - <a href="#minor-changes-3">Minor Changes</a>
+    - <a href="#bugfixes-3">Bugfixes</a>
 - <a href="#v2-5-0">v2\.5\.0</a>
-  - <a href="#release-summary-4">Release Summary</a>
-  - <a href="#minor-changes-3">Minor Changes</a>
+    - <a href="#release-summary-5">Release Summary</a>
+    - <a href="#minor-changes-4">Minor Changes</a>
 - <a href="#v2-4-0">v2\.4\.0</a>
-  - <a href="#release-summary-5">Release Summary</a>
-  - <a href="#minor-changes-4">Minor Changes</a>
-  - <a href="#deprecated-features">Deprecated Features</a>
-  - <a href="#bugfixes-4">Bugfixes</a>
-  - <a href="#known-issues">Known Issues</a>
+    - <a href="#release-summary-6">Release Summary</a>
+    - <a href="#minor-changes-5">Minor Changes</a>
+    - <a href="#deprecated-features">Deprecated Features</a>
+    - <a href="#bugfixes-4">Bugfixes</a>
+    - <a href="#known-issues">Known Issues</a>
 - <a href="#v2-3-1">v2\.3\.1</a>
-  - <a href="#release-summary-6">Release Summary</a>
-  - <a href="#bugfixes-5">Bugfixes</a>
+    - <a href="#release-summary-7">Release Summary</a>
+    - <a href="#bugfixes-5">Bugfixes</a>
 - <a href="#v2-3-0">v2\.3\.0</a>
-  - <a href="#release-summary-7">Release Summary</a>
-  - <a href="#minor-changes-5">Minor Changes</a>
-  - <a href="#bugfixes-6">Bugfixes</a>
+    - <a href="#release-summary-8">Release Summary</a>
+    - <a href="#minor-changes-6">Minor Changes</a>
+    - <a href="#bugfixes-6">Bugfixes</a>
 - <a href="#v2-2-0">v2\.2\.0</a>
-  - <a href="#release-summary-8">Release Summary</a>
-  - <a href="#minor-changes-6">Minor Changes</a>
-  - <a href="#bugfixes-7">Bugfixes</a>
+    - <a href="#release-summary-9">Release Summary</a>
+    - <a href="#minor-changes-7">Minor Changes</a>
+    - <a href="#bugfixes-7">Bugfixes</a>
 - <a href="#v2-1-0">v2\.1\.0</a>
-  - <a href="#release-summary-9">Release Summary</a>
-  - <a href="#minor-changes-7">Minor Changes</a>
-  - <a href="#bugfixes-8">Bugfixes</a>
+    - <a href="#release-summary-10">Release Summary</a>
+    - <a href="#minor-changes-8">Minor Changes</a>
+    - <a href="#bugfixes-8">Bugfixes</a>
 - <a href="#v2-0-0">v2\.0\.0</a>
-  - <a href="#release-summary-10">Release Summary</a>
-  - <a href="#major-changes">Major Changes</a>
-  - <a href="#minor-changes-8">Minor Changes</a>
-  - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
-  - <a href="#bugfixes-9">Bugfixes</a>
+    - <a href="#release-summary-11">Release Summary</a>
+    - <a href="#major-changes">Major Changes</a>
+    - <a href="#minor-changes-9">Minor Changes</a>
+    - <a href="#breaking-changes--porting-guide">Breaking Changes / Porting Guide</a>
+    - <a href="#bugfixes-9">Bugfixes</a>
 - <a href="#v1-11-0">v1\.11\.0</a>
-  - <a href="#release-summary-11">Release Summary</a>
-  - <a href="#minor-changes-9">Minor Changes</a>
+    - <a href="#release-summary-12">Release Summary</a>
+    - <a href="#minor-changes-10">Minor Changes</a>
 - <a href="#v1-10-0">v1\.10\.0</a>
-  - <a href="#release-summary-12">Release Summary</a>
-  - <a href="#major-changes-1">Major Changes</a>
-  - <a href="#minor-changes-10">Minor Changes</a>
-  - <a href="#bugfixes-10">Bugfixes</a>
+    - <a href="#release-summary-13">Release Summary</a>
+    - <a href="#major-changes-1">Major Changes</a>
+    - <a href="#minor-changes-11">Minor Changes</a>
+    - <a href="#bugfixes-10">Bugfixes</a>
 - <a href="#v1-9-0">v1\.9\.0</a>
-  - <a href="#release-summary-13">Release Summary</a>
-  - <a href="#minor-changes-11">Minor Changes</a>
+    - <a href="#release-summary-14">Release Summary</a>
+    - <a href="#minor-changes-12">Minor Changes</a>
 - <a href="#v1-8-2">v1\.8\.2</a>
-  - <a href="#release-summary-14">Release Summary</a>
-  - <a href="#bugfixes-11">Bugfixes</a>
+    - <a href="#release-summary-15">Release Summary</a>
+    - <a href="#bugfixes-11">Bugfixes</a>
 - <a href="#v1-8-1">v1\.8\.1</a>
-  - <a href="#release-summary-15">Release Summary</a>
-  - <a href="#bugfixes-12">Bugfixes</a>
+    - <a href="#release-summary-16">Release Summary</a>
+    - <a href="#bugfixes-12">Bugfixes</a>
 - <a href="#v1-8-0">v1\.8\.0</a>
-  - <a href="#release-summary-16">Release Summary</a>
-  - <a href="#minor-changes-12">Minor Changes</a>
-  - <a href="#bugfixes-13">Bugfixes</a>
+    - <a href="#release-summary-17">Release Summary</a>
+    - <a href="#minor-changes-13">Minor Changes</a>
+    - <a href="#bugfixes-13">Bugfixes</a>
 - <a href="#v1-7-4">v1\.7\.4</a>
-  - <a href="#release-summary-17">Release Summary</a>
-  - <a href="#bugfixes-14">Bugfixes</a>
+    - <a href="#release-summary-18">Release Summary</a>
+    - <a href="#bugfixes-14">Bugfixes</a>
 - <a href="#v1-7-3">v1\.7\.3</a>
-  - <a href="#release-summary-18">Release Summary</a>
-  - <a href="#bugfixes-15">Bugfixes</a>
+    - <a href="#release-summary-19">Release Summary</a>
+    - <a href="#bugfixes-15">Bugfixes</a>
 - <a href="#v1-7-2">v1\.7\.2</a>
-  - <a href="#release-summary-19">Release Summary</a>
-  - <a href="#bugfixes-16">Bugfixes</a>
+    - <a href="#release-summary-20">Release Summary</a>
+    - <a href="#bugfixes-16">Bugfixes</a>
 - <a href="#v1-7-1">v1\.7\.1</a>
-  - <a href="#release-summary-20">Release Summary</a>
-  - <a href="#bugfixes-17">Bugfixes</a>
+    - <a href="#release-summary-21">Release Summary</a>
+    - <a href="#bugfixes-17">Bugfixes</a>
 - <a href="#v1-7-0">v1\.7\.0</a>
-  - <a href="#release-summary-21">Release Summary</a>
-  - <a href="#minor-changes-13">Minor Changes</a>
-  - <a href="#bugfixes-18">Bugfixes</a>
+    - <a href="#release-summary-22">Release Summary</a>
+    - <a href="#minor-changes-14">Minor Changes</a>
+    - <a href="#bugfixes-18">Bugfixes</a>
 - <a href="#v1-6-1">v1\.6\.1</a>
-  - <a href="#release-summary-22">Release Summary</a>
-  - <a href="#bugfixes-19">Bugfixes</a>
+    - <a href="#release-summary-23">Release Summary</a>
+    - <a href="#bugfixes-19">Bugfixes</a>
 - <a href="#v1-6-0">v1\.6\.0</a>
-  - <a href="#release-summary-23">Release Summary</a>
-  - <a href="#minor-changes-14">Minor Changes</a>
-  - <a href="#bugfixes-20">Bugfixes</a>
+    - <a href="#release-summary-24">Release Summary</a>
+    - <a href="#minor-changes-15">Minor Changes</a>
+    - <a href="#bugfixes-20">Bugfixes</a>
 - <a href="#v1-5-0">v1\.5\.0</a>
-  - <a href="#release-summary-24">Release Summary</a>
-  - <a href="#minor-changes-15">Minor Changes</a>
-  - <a href="#bugfixes-21">Bugfixes</a>
+    - <a href="#release-summary-25">Release Summary</a>
+    - <a href="#minor-changes-16">Minor Changes</a>
+    - <a href="#bugfixes-21">Bugfixes</a>
 - <a href="#v1-4-0">v1\.4\.0</a>
-  - <a href="#release-summary-25">Release Summary</a>
-  - <a href="#minor-changes-16">Minor Changes</a>
-  - <a href="#bugfixes-22">Bugfixes</a>
+    - <a href="#release-summary-26">Release Summary</a>
+    - <a href="#minor-changes-17">Minor Changes</a>
+    - <a href="#bugfixes-22">Bugfixes</a>
 - <a href="#v1-3-0">v1\.3\.0</a>
-  - <a href="#release-summary-26">Release Summary</a>
-  - <a href="#minor-changes-17">Minor Changes</a>
-  - <a href="#bugfixes-23">Bugfixes</a>
+    - <a href="#release-summary-27">Release Summary</a>
+    - <a href="#minor-changes-18">Minor Changes</a>
+    - <a href="#bugfixes-23">Bugfixes</a>
 - <a href="#v1-2-2">v1\.2\.2</a>
-  - <a href="#release-summary-27">Release Summary</a>
-  - <a href="#bugfixes-24">Bugfixes</a>
+    - <a href="#release-summary-28">Release Summary</a>
+    - <a href="#bugfixes-24">Bugfixes</a>
 - <a href="#v1-2-1">v1\.2\.1</a>
-  - <a href="#release-summary-28">Release Summary</a>
-  - <a href="#bugfixes-25">Bugfixes</a>
+    - <a href="#release-summary-29">Release Summary</a>
+    - <a href="#bugfixes-25">Bugfixes</a>
 - <a href="#v1-2-0">v1\.2\.0</a>
-  - <a href="#release-summary-29">Release Summary</a>
-  - <a href="#minor-changes-18">Minor Changes</a>
-  - <a href="#bugfixes-26">Bugfixes</a>
+    - <a href="#release-summary-30">Release Summary</a>
+    - <a href="#minor-changes-19">Minor Changes</a>
+    - <a href="#bugfixes-26">Bugfixes</a>
 - <a href="#v1-1-0">v1\.1\.0</a>
-  - <a href="#release-summary-30">Release Summary</a>
-  - <a href="#minor-changes-19">Minor Changes</a>
+    - <a href="#release-summary-31">Release Summary</a>
+    - <a href="#minor-changes-20">Minor Changes</a>
 - <a href="#v1-0-1">v1\.0\.1</a>
-  - <a href="#release-summary-31">Release Summary</a>
-  - <a href="#bugfixes-27">Bugfixes</a>
+    - <a href="#release-summary-32">Release Summary</a>
+    - <a href="#bugfixes-27">Bugfixes</a>
 - <a href="#v1-0-0">v1\.0\.0</a>
-  - <a href="#release-summary-32">Release Summary</a>
-  - <a href="#major-changes-2">Major Changes</a>
-  - <a href="#minor-changes-20">Minor Changes</a>
+    - <a href="#release-summary-33">Release Summary</a>
+    - <a href="#major-changes-2">Major Changes</a>
+    - <a href="#minor-changes-21">Minor Changes</a>
 - <a href="#v0-1-0">v0\.1\.0</a>
-  - <a href="#release-summary-33">Release Summary</a>
+    - <a href="#release-summary-34">Release Summary</a>
+
+<a id="v2-9-0"></a>
+## v2\.9\.0
+
+<a id="release-summary"></a>
+### Release Summary
+
+Maintenance release\.
+
+<a id="minor-changes"></a>
+### Minor Changes
+
+* Add support for the antsibull\-core v3 \([https\://github\.com/ansible\-community/antsibull\-docs/pull/261](https\://github\.com/ansible\-community/antsibull\-docs/pull/261)\)\.
 
 <a id="v2-8-0"></a>
 ## v2\.8\.0
 
-<a id="release-summary"></a>
+<a id="release-summary-1"></a>
 ### Release Summary
 
 Bugfix and feature release\.
 
-<a id="minor-changes"></a>
+<a id="minor-changes-1"></a>
 ### Minor Changes
 
 * Add support for \"dark mode\" to the option table styling \([https\://github\.com/ansible\-community/antsibull\-docs/pull/253](https\://github\.com/ansible\-community/antsibull\-docs/pull/253)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/258](https\://github\.com/ansible\-community/antsibull\-docs/pull/258)\)\.
 * Add support for the latest antsibull\-core v3 pre\-release\, <code>3\.0\.0a1</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/250](https\://github\.com/ansible\-community/antsibull\-docs/pull/250)\)\.
 * Declare support for Python 3\.12 \([https\://github\.com/ansible\-community/antsibull\-docs/pull/255](https\://github\.com/ansible\-community/antsibull\-docs/pull/255)\)\.
 * The colors used by the CSS provided by the Antsibull Sphinx extension can now be overridden \([https\://github\.com/ansible\-community/antsibull\-docs/pull/254](https\://github\.com/ansible\-community/antsibull\-docs/pull/254)\)\.
 
@@ -145,20 +162,20 @@
 ### Bugfixes
 
 * Fix duplicate docs detection \(for aliases\) for latest ansible\-core devel \([https\://github\.com/ansible\-community/antsibull\-docs/pull/257](https\://github\.com/ansible\-community/antsibull\-docs/pull/257)\)\.
 
 <a id="v2-7-0"></a>
 ## v2\.7\.0
 
-<a id="release-summary-1"></a>
+<a id="release-summary-2"></a>
 ### Release Summary
 
 Bugfix and refactoring release\.
 
-<a id="minor-changes-1"></a>
+<a id="minor-changes-2"></a>
 ### Minor Changes
 
 * Explicitly set up Galaxy context instead of relying on deprecated functionality \([https\://github\.com/ansible\-community/antsibull\-docs/pull/234](https\://github\.com/ansible\-community/antsibull\-docs/pull/234)\)\.
 
 <a id="bugfixes-1"></a>
 ### Bugfixes
 
@@ -166,69 +183,69 @@
 * Make error reporting for invalid references in <code>plugin</code> <code>seealso</code> entries more precise \([https\://github\.com/ansible\-community/antsibull\-docs/pull/240](https\://github\.com/ansible\-community/antsibull\-docs/pull/240)\)\.
 * Support new <code>ansible\-doc \-\-json</code> output field <code>plugin\_name</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/242](https\://github\.com/ansible\-community/antsibull\-docs/pull/242)\)\.
 * Use certain fields from library context instead of app context that are deprecated in the app context and will be removed from antsibull\-core 3\.0\.0 \([https\://github\.com/ansible\-community/antsibull\-docs/pull/233](https\://github\.com/ansible\-community/antsibull\-docs/pull/233)\)\.
 
 <a id="v2-6-1"></a>
 ## v2\.6\.1
 
-<a id="release-summary-2"></a>
+<a id="release-summary-3"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-2"></a>
 ### Bugfixes
 
 * For role argument specs\, allow <code>author</code>\, <code>description</code>\, and <code>todo</code> to be a string instead of a list of strings\, similarly as with ansible\-doc and with modules and plugins \([https\://github\.com/ansible\-community/antsibull\-docs/pull/227](https\://github\.com/ansible\-community/antsibull\-docs/pull/227)\)\.
 * Make sure that title underlines have the correct width for wide Unicode characters \([https\://github\.com/ansible\-community/antsibull\-docs/issues/228](https\://github\.com/ansible\-community/antsibull\-docs/issues/228)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/229](https\://github\.com/ansible\-community/antsibull\-docs/pull/229)\)\.
 
 <a id="v2-6-0"></a>
 ## v2\.6\.0
 
-<a id="release-summary-3"></a>
+<a id="release-summary-4"></a>
 ### Release Summary
 
 Fix parsing of <code>EXAMPLES</code> and improve error message
 
-<a id="minor-changes-2"></a>
+<a id="minor-changes-3"></a>
 ### Minor Changes
 
 * Improve error messages when calls to <code>ansible\-doc</code> fail \([https\://github\.com/ansible\-community/antsibull\-docs/pull/223](https\://github\.com/ansible\-community/antsibull\-docs/pull/223)\)\.
 
 <a id="bugfixes-3"></a>
 ### Bugfixes
 
 * When <code>EXAMPLES</code> has the format specified by <code>\# fmt\: \<format\></code>\, this value is used to determine the code block type \([https\://github\.com/ansible\-community/antsibull\-docs/pull/225](https\://github\.com/ansible\-community/antsibull\-docs/pull/225)\)\.
 
 <a id="v2-5-0"></a>
 ## v2\.5\.0
 
-<a id="release-summary-4"></a>
+<a id="release-summary-5"></a>
 ### Release Summary
 
 Release to support the updated Ansible Galaxy codebase\.
 
-<a id="minor-changes-3"></a>
+<a id="minor-changes-4"></a>
 ### Minor Changes
 
 * The default collection URL template has been changed from <code>https\://galaxy\.ansible\.com/\{namespace\}/\{name\}</code> to <code>https\://galaxy\.ansible\.com/ui/repo/published/\{namespace\}/\{name\}/</code> to adjust for the Galaxy codebase change on September 30th\, 2023 \([https\://github\.com/ansible\-community/antsibull\-docs/issues/147](https\://github\.com/ansible\-community/antsibull\-docs/issues/147)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/220](https\://github\.com/ansible\-community/antsibull\-docs/pull/220)\)\.
 
 <a id="v2-4-0"></a>
 ## v2\.4\.0
 
-<a id="release-summary-5"></a>
+<a id="release-summary-6"></a>
 ### Release Summary
 
 Bugfix and feature release\. Improves support for other builders than <code>html</code>\.
 
 There will be a follow\-up release after [Ansible Galaxy](https\://galaxy\.ansible\.com/)
 switched to the new <code>galaxy\_ng</code> codebase\, which is scheduled for September 30th\.
 That release will only adjust the URLs to Galaxy\, except potentially bugfixes\.
 
-<a id="minor-changes-4"></a>
+<a id="minor-changes-5"></a>
 ### Minor Changes
 
 * Add basic support for other HTML based Sphinx builders such as <code>epub</code> and <code>singlehtml</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/201](https\://github\.com/ansible\-community/antsibull\-docs/pull/201)\)\.
 * Adjust default RST output to work better with Spinx\'s LaTeX builder \([https\://github\.com/ansible\-community/antsibull\-docs/pull/195](https\://github\.com/ansible\-community/antsibull\-docs/pull/195)\)\.
 * Allow specifying wildcards for the collection names for the <code>collections</code> subcommand if <code>\-\-use\-current</code> is specified \([https\://github\.com/ansible\-community/antsibull\-docs/pull/219](https\://github\.com/ansible\-community/antsibull\-docs/pull/219)\)\.
 * Antsibull\-docs now depends on antsibull\-core \>\= 2\.1\.0 \([https\://github\.com/ansible\-community/antsibull\-docs/pull/209](https\://github\.com/ansible\-community/antsibull\-docs/pull/209)\)\.
 * Create collection links with a custom directive\. This makes them compatible with builders other than the HTML builder \([https\://github\.com/ansible\-community/antsibull\-docs/pull/200](https\://github\.com/ansible\-community/antsibull\-docs/pull/200)\)\.
@@ -263,33 +280,33 @@
 ### Known Issues
 
 * When using Sphinx builders other than HTML and LaTeX\, the indentation for nested options and return values is missing \([https\://github\.com/ansible\-community/antsibull\-docs/pull/195](https\://github\.com/ansible\-community/antsibull\-docs/pull/195)\)\.
 
 <a id="v2-3-1"></a>
 ## v2\.3\.1
 
-<a id="release-summary-6"></a>
+<a id="release-summary-7"></a>
 ### Release Summary
 
 Bugfix release with a CSS fix for the Sphinx extension\.
 
 <a id="bugfixes-5"></a>
 ### Bugfixes
 
 * Fix antsibull Sphinx extension CSS so that the option/return value anchors for module/plugin/role documentation can also be used on WebKit\-based browsers such as Gnome Web and Safari \([https\://github\.com/ansible\-community/antsibull\-docs/issues/188](https\://github\.com/ansible\-community/antsibull\-docs/issues/188)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/189](https\://github\.com/ansible\-community/antsibull\-docs/pull/189)\)\.
 
 <a id="v2-3-0"></a>
 ## v2\.3\.0
 
-<a id="release-summary-7"></a>
+<a id="release-summary-8"></a>
 ### Release Summary
 
 Bugfix and feature release\.
 
-<a id="minor-changes-5"></a>
+<a id="minor-changes-6"></a>
 ### Minor Changes
 
 * Add a <code>\:ansplugin\:</code> role to the Sphinx extension\. This allows to reference a module\, plugin\, or role with the <code>fqcn\#type</code> syntax from semantic markup instead of having to manually compose a <code>ansible\_collections\.\{fqcn\}\_\{type\}</code> label\. An explicit reference title can also be provided with the <code>title \<fqcn\#type\></code> syntax similar to the <code>\:ref\:</code> role \([https\://github\.com/ansible\-community/antsibull\-docs/pull/180](https\://github\.com/ansible\-community/antsibull\-docs/pull/180)\)\.
 * Add a new subcommand <code>lint\-core\-docs</code> which lints the ansible\-core documentation \([https\://github\.com/ansible\-community/antsibull\-docs/pull/182](https\://github\.com/ansible\-community/antsibull\-docs/pull/182)\)\.
 * Add a new subcommand\, <code>collection\-plugins</code>\, for rendering files for all plugins and roles in a collection without any indexes \([https\://github\.com/ansible\-community/antsibull\-docs/pull/177](https\://github\.com/ansible\-community/antsibull\-docs/pull/177)\)\.
 * Add support for different output formats\. Next to the default format\, <code>ansible\-docsite</code>\, a new <strong>experimental</strong> format <code>simplified\-rst</code> is supported\. Experimental means that it will likely change considerably in the next few releases until it stabilizes\. Such changes will not be considered breaking changes\, and could potentially even be bugfixes \([https\://github\.com/ansible\-community/antsibull\-docs/pull/177](https\://github\.com/ansible\-community/antsibull\-docs/pull/177)\)\.
 * Use Dart sass compiler instead of sassc to compile CSS for Sphinx extension \([https\://github\.com/ansible\-community/antsibull\-docs/issues/185](https\://github\.com/ansible\-community/antsibull\-docs/issues/185)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/186](https\://github\.com/ansible\-community/antsibull\-docs/pull/186)\)\.
@@ -301,20 +318,20 @@
 * Consider module/plugin aliases when linting references to other modules and plugins \([https\://github\.com/ansible\-community/antsibull\-docs/pull/184](https\://github\.com/ansible\-community/antsibull\-docs/pull/184)\)\.
 * Make sure that all aliases are actually listed for plugins \([https\://github\.com/ansible\-community/antsibull\-docs/pull/183](https\://github\.com/ansible\-community/antsibull\-docs/pull/183)\)\.
 * When looking for redirects\, the <code>aliases</code> field and filesystem redirects in ansible\-core were not properly considered\. This ensures that all redirect stubs are created\, and that no duplicates show up\, not depending on whether ansible\-core is installed in editable mode or not \([https\://github\.com/ansible\-community/antsibull\-docs/pull/183](https\://github\.com/ansible\-community/antsibull\-docs/pull/183)\)\.
 
 <a id="v2-2-0"></a>
 ## v2\.2\.0
 
-<a id="release-summary-8"></a>
+<a id="release-summary-9"></a>
 ### Release Summary
 
 Bugfix and feature release improving rendering and linting\.
 
-<a id="minor-changes-6"></a>
+<a id="minor-changes-7"></a>
 ### Minor Changes
 
 * Collection docs linter \- also validate <code>seealso</code> module and plugin destinations \([https\://github\.com/ansible\-community/antsibull\-docs/issues/168](https\://github\.com/ansible\-community/antsibull\-docs/issues/168)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/171](https\://github\.com/ansible\-community/antsibull\-docs/pull/171)\)\.
 * When linting collection plugin docs\, make sure that array stubs <code>\[\.\.\.\]</code> are used when referencing sub\-options or sub\-return values inside lists\, and are not used outside lists and dictionaries \([https\://github\.com/ansible\-community/antsibull\-docs/pull/173](https\://github\.com/ansible\-community/antsibull\-docs/pull/173)\)\.
 
 <a id="bugfixes-7"></a>
 ### Bugfixes
@@ -323,20 +340,20 @@
 * Make sure that <code>\:ansopt\:</code> and <code>\:ansretval\:</code> create the same references as the labels created in the RST files \([https\://github\.com/ansible\-community/antsibull\-docs/issues/167](https\://github\.com/ansible\-community/antsibull\-docs/issues/167)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/172](https\://github\.com/ansible\-community/antsibull\-docs/pull/172)\)\.
 * Make sure that broken <code>\:ansopt\:</code> and <code>\:ansretval\:</code> parameters result in correctly rendered error messages \([https\://github\.com/ansible\-community/antsibull\-docs/pull/175](https\://github\.com/ansible\-community/antsibull\-docs/pull/175)\)\.
 * When trying to copying descriptions of non\-existing plugins to <code>seealso</code>\, references to these non\-existing plugins were added in some cases\, crashing the docs augmentation process \([https\://github\.com/ansible\-community/antsibull\-docs/pull/169](https\://github\.com/ansible\-community/antsibull\-docs/pull/169)\)\.
 
 <a id="v2-1-0"></a>
 ## v2\.1\.0
 
-<a id="release-summary-9"></a>
+<a id="release-summary-10"></a>
 ### Release Summary
 
 Feature and bugfix release with many improvements related to semantic markup and validation\.
 
-<a id="minor-changes-7"></a>
+<a id="minor-changes-8"></a>
 ### Minor Changes
 
 * Add option <code>\-\-disallow\-unknown\-collection\-refs</code> to disallow references to other collections than the one covered by <code>\-\-validate\-collection\-refs</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/157](https\://github\.com/ansible\-community/antsibull\-docs/pull/157)\)\.
 * Add option <code>\-\-validate\-collection\-refs</code> to the <code>lint\-collection\-docs</code> subcommand to also control which references to plugin/module/role names in \(other\) collections and their options and return values should be validated \([https\://github\.com/ansible\-community/antsibull\-docs/pull/157](https\://github\.com/ansible\-community/antsibull\-docs/pull/157)\)\.
 * Add the new collection config field <code>envvar\_directives</code> which allows to declare which environment variables are declared with an <code>\.\. envvar\:\:</code> directive in the collection\'s extra docsite documentation\. This is used\, next to the plugin configuration information and the ansible\-core configuration information\, to determine whether an environment variable is referencable or not \([https\://github\.com/ansible\-community/antsibull\-docs/pull/166](https\://github\.com/ansible\-community/antsibull\-docs/pull/166)\)\.
 * Add the roles <code>\:ansenvvar\:</code> and <code>\:ansenvvarref\:</code> to the antsibull\-docs Sphinx extension \([https\://github\.com/ansible\-community/antsibull\-docs/pull/166](https\://github\.com/ansible\-community/antsibull\-docs/pull/166)\)\.
 * Render <code>E\(\.\.\.\)</code> markup with <code>\:ansenvvarref\:</code> or <code>\:ansenvvar\:</code> depending on whether the environment variable is known to be referencable or not \([https\://github\.com/ansible\-community/antsibull\-docs/pull/166](https\://github\.com/ansible\-community/antsibull\-docs/pull/166)\)\.
@@ -350,25 +367,25 @@
 * Allow role entrypoint deprecations without having to specify the collection the role is removed from \([https\://github\.com/ansible\-community/antsibull\-docs/pull/156](https\://github\.com/ansible\-community/antsibull\-docs/pull/156)\)\.
 * Indent module/plugin and role entrypoint deprecations correctly if \'Why\' or \'Alternative\' texts need more than one line \([https\://github\.com/ansible\-community/antsibull\-docs/pull/156](https\://github\.com/ansible\-community/antsibull\-docs/pull/156)\)\.
 * When collecting collection dependencies for the <code>lint\-collection\-docs</code> subcommand\, a bug prevented the duplicate detection to work \([https\://github\.com/ansible\-community/antsibull\-docs/pull/160](https\://github\.com/ansible\-community/antsibull\-docs/pull/160)\)\.
 
 <a id="v2-0-0"></a>
 ## v2\.0\.0
 
-<a id="release-summary-10"></a>
+<a id="release-summary-11"></a>
 ### Release Summary
 
 Major new release that drops support for older Python and Ansible/ansible\-base/ansible\-core versions\.
 
 <a id="major-changes"></a>
 ### Major Changes
 
 * Change pyproject build backend from <code>poetry\-core</code> to <code>hatchling</code>\. <code>pip install antsibull\-docs</code> works exactly the same as before\, but some users may be affected depending on how they build/install the project \([https\://github\.com/ansible\-community/antsibull\-docs/pull/115](https\://github\.com/ansible\-community/antsibull\-docs/pull/115)\)\.
 
-<a id="minor-changes-8"></a>
+<a id="minor-changes-9"></a>
 ### Minor Changes
 
 * Allow to use the currently installed ansible\-core version for the <code>devel</code> and <code>stable</code> subcommands \([https\://github\.com/ansible\-community/antsibull\-docs/pull/121](https\://github\.com/ansible\-community/antsibull\-docs/pull/121)\)\.
 * Ansibull\-docs now no longer depends directly on <code>sh</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/122](https\://github\.com/ansible\-community/antsibull\-docs/pull/122)\)\.
 * Bump version range of antsibull\-docs requirement written by <code>sphinx\-init</code> subcommand to <code>\>\= 2\.0\.0\, \< 3\.0\.0</code>\. Previously\, this was set to <code>\>\=2\.0\.0a2\, \<3\.0\.0</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/151](https\://github\.com/ansible\-community/antsibull\-docs/pull/151)\)\.
 * Now depends antsibull\-core 2\.0\.0 or newer\; antsibull\-core 1\.x\.y is no longer supported \([https\://github\.com/ansible\-community/antsibull\-docs/pull/122](https\://github\.com/ansible\-community/antsibull\-docs/pull/122)\)\.
 * Remove residual compatability code for Python 3\.6 and 3\.7 \([https\://github\.com/ansible\-community/antsibull\-docs/pulls/70](https\://github\.com/ansible\-community/antsibull\-docs/pulls/70)\)\.
@@ -390,101 +407,101 @@
 
 * Bump version range of antsibull\-docs requirement written by <code>sphinx\-init</code> subcommand to <code>\>\= 2\.0\.0a2\, \< 3\.0\.0</code>\. Previously\, this was set to <code>\>\=2\.0\.0\, \<3\.0\.0</code> which could not be satisfied \([https\://github\.com/ansible\-community/antsibull\-docs/pull/149](https\://github\.com/ansible\-community/antsibull\-docs/pull/149)\)\.
 * Use <code>doc\_parsing\_backend</code> from the application context instead of the library context\. This prevents removal of <code>doc\_parsing\_backend</code> from the antsibull\-core library context \([https\://github\.com/ansible\-community/antsibull\-docs/pull/125](https\://github\.com/ansible\-community/antsibull\-docs/pull/125)\)\.
 
 <a id="v1-11-0"></a>
 ## v1\.11\.0
 
-<a id="release-summary-11"></a>
+<a id="release-summary-12"></a>
 ### Release Summary
 
 Feature release\.
 
-<a id="minor-changes-9"></a>
+<a id="minor-changes-10"></a>
 ### Minor Changes
 
 * Add support for semantic markup in roles \([https\://github\.com/ansible\-community/antsibull\-docs/pull/113](https\://github\.com/ansible\-community/antsibull\-docs/pull/113)\)\.
 * Internal refactoring of markup code \([https\://github\.com/ansible\-community/antsibull\-docs/pull/108](https\://github\.com/ansible\-community/antsibull\-docs/pull/108)\)\.
 * The <code>lint\-collection\-docs</code> subcommand can be told not to run rstcheck when <code>\-\-plugin\-docs</code> is used by passing <code>\-\-skip\-rstcheck</code>\. This speeds up testing for large collections \([https\://github\.com/ansible\-community/antsibull\-docs/pull/112](https\://github\.com/ansible\-community/antsibull\-docs/pull/112)\)\.
 * The <code>lint\-collection\-docs</code> subcommand will now also validate Ansible markup when <code>\-\-plugin\-docs</code> is passed\. It can also ensure that no semantic markup is used with the new <code>\-\-disallow\-semantic\-markup</code> option\. This can for example be used by collections to avoid semantic markup being backported to older stable branches \([https\://github\.com/ansible\-community/antsibull\-docs/pull/112](https\://github\.com/ansible\-community/antsibull\-docs/pull/112)\)\.
 
 <a id="v1-10-0"></a>
 ## v1\.10\.0
 
-<a id="release-summary-12"></a>
+<a id="release-summary-13"></a>
 ### Release Summary
 
 Bugfix and feature release\.
 
 <a id="major-changes-1"></a>
 ### Major Changes
 
 * Support new semantic markup in documentation \([https\://github\.com/ansible\-community/antsibull\-docs/pull/4](https\://github\.com/ansible\-community/antsibull\-docs/pull/4)\)\.
 
-<a id="minor-changes-10"></a>
+<a id="minor-changes-11"></a>
 ### Minor Changes
 
 * Add a note about the ordering of positional and named parameter to the plugin page\. Also mention positional and keyword parameters for lookups \([https\://github\.com/ansible\-community/antsibull\-docs/pull/101](https\://github\.com/ansible\-community/antsibull\-docs/pull/101)\)\.
 * Update schema for roles argument spec to allow specifying attributes on the entrypoint level\. These are now also rendered when present \([https\://github\.com/ansible\-community/antsibull\-docs/pull/103](https\://github\.com/ansible\-community/antsibull\-docs/pull/103)\)\.
 
 <a id="bugfixes-10"></a>
 ### Bugfixes
 
 * Explicitly declare the <code>sh</code> dependency and limit it to before 2\.0\.0\. Also explicitly declare the dependencies on <code>pydantic</code>\, <code>semantic\_version</code>\, <code>aiohttp</code>\, <code>twiggy</code>\, and <code>PyYAML</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/99](https\://github\.com/ansible\-community/antsibull\-docs/pull/99)\)\.
 * Restrict the <code>pydantic</code> dependency to major version 1 \([https\://github\.com/ansible\-community/antsibull\-docs/pull/102](https\://github\.com/ansible\-community/antsibull\-docs/pull/102)\)\.
 
 <a id="v1-9-0"></a>
 ## v1\.9\.0
 
-<a id="release-summary-13"></a>
+<a id="release-summary-14"></a>
 ### Release Summary
 
 Feature release\.
 
-<a id="minor-changes-11"></a>
+<a id="minor-changes-12"></a>
 ### Minor Changes
 
 * Improve build script generated by <code>antsibull\-docs sphinx\-init</code> to change to the directory where the script is located\, instead of hardcoding the script\'s path\. This also fixed the existing bug that the path was not quoted \([https\://github\.com/ansible\-community/antsibull\-docs/issues/91](https\://github\.com/ansible\-community/antsibull\-docs/issues/91)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/92](https\://github\.com/ansible\-community/antsibull\-docs/pull/92)\)\.
 * Show callback plugin type on callback plugin pages\. Also write callback indexes by callback plugin type \([https\://github\.com/ansible\-community/antsibull\-docs/issues/89](https\://github\.com/ansible\-community/antsibull\-docs/issues/89)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/90](https\://github\.com/ansible\-community/antsibull\-docs/pull/90)\)\.
 
 <a id="v1-8-2"></a>
 ## v1\.8\.2
 
-<a id="release-summary-14"></a>
+<a id="release-summary-15"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-11"></a>
 ### Bugfixes
 
 * Fix the new options <code>\-\-extra\-html\-context</code> and <code>\-\-extra\-html\-theme\-options</code> of the <code>sphinx\-init</code> subcommand \([https\://github\.com/ansible\-community/antsibull\-docs/pull/86](https\://github\.com/ansible\-community/antsibull\-docs/pull/86)\)\.
 
 <a id="v1-8-1"></a>
 ## v1\.8\.1
 
-<a id="release-summary-15"></a>
+<a id="release-summary-16"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-12"></a>
 ### Bugfixes
 
 * When creating toctrees for breadcrumbs\, place subtree for a plugin type in the plugin type\'s section \([https\://github\.com/ansible\-community/antsibull\-docs/pull/83](https\://github\.com/ansible\-community/antsibull\-docs/pull/83)\)\.
 
 <a id="v1-8-0"></a>
 ## v1\.8\.0
 
-<a id="release-summary-16"></a>
+<a id="release-summary-17"></a>
 ### Release Summary
 
 Feature and bugfix release\.
 
-<a id="minor-changes-12"></a>
+<a id="minor-changes-13"></a>
 ### Minor Changes
 
 * Add new options <code>\-\-project</code>\, <code>\-\-copyright</code>\, <code>\-\-title</code>\, <code>\-\-html\-short\-title</code>\, <code>\-\-extra\-conf</code>\, <code>\-\-extra\-html\-context</code>\, and <code>\-\-extra\-html\-theme\-options</code> to the <code>sphinx\-init</code> subcommand to allow to customize the generated <code>conf\.py</code> Sphinx configuration \([https\://github\.com/ansible\-community/antsibull\-docs/pull/77](https\://github\.com/ansible\-community/antsibull\-docs/pull/77)\)\.
 * Automatically use a module\'s or plugin\'s short description as the \"See also\" description if no description is provided \([https\://github\.com/ansible\-community/antsibull\-docs/issues/64](https\://github\.com/ansible\-community/antsibull\-docs/issues/64)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/74](https\://github\.com/ansible\-community/antsibull\-docs/pull/74)\)\.
 * It is now possible to provide a path to an existing file to be used as <code>rst/index\.rst</code> for <code>antsibull\-docs sphinx\-init</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/68](https\://github\.com/ansible\-community/antsibull\-docs/pull/68)\)\.
 * Make compatible with antsibull\-core 2\.x\.y \([https\://github\.com/ansible\-community/antsibull\-docs/pull/78](https\://github\.com/ansible\-community/antsibull\-docs/pull/78)\)\.
 * Remove support for <code>forced\_action\_plugin</code>\, a module attribute that was removed during the development phase of attributes \([https\://github\.com/ansible\-community/antsibull\-docs/pull/63](https\://github\.com/ansible\-community/antsibull\-docs/pull/63)\)\.
@@ -496,74 +513,74 @@
 ### Bugfixes
 
 * Make sure that <code>build\.sh</code> created by the <code>sphinx\-init</code> subcommand sets proper permissions for antsibull\-docs on the <code>temp\-rst</code> directory it creates \([https\://github\.com/ansible\-community/antsibull\-docs/pull/79](https\://github\.com/ansible\-community/antsibull\-docs/pull/79)\)\.
 
 <a id="v1-7-4"></a>
 ## v1\.7\.4
 
-<a id="release-summary-17"></a>
+<a id="release-summary-18"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-14"></a>
 ### Bugfixes
 
 * Removed <code>sphinx</code> restriction in <code>requirements\.txt</code> file created by <code>antsibull\-docs sphinx\-init</code> since the bug in <code>sphinx\-rtd\-theme</code> has been fixed \([https\://github\.com/ansible\-community/antsibull\-docs/pull/69](https\://github\.com/ansible\-community/antsibull\-docs/pull/69)\)\.
 * The license header for the template for the <code>rst/index\.rst</code> file created by <code>antsibull\-docs sphinx\-init</code> was commented incorrectly and thus showed up in the templated file \([https\://github\.com/ansible\-community/antsibull\-docs/pull/67](https\://github\.com/ansible\-community/antsibull\-docs/pull/67)\)\.
 * When using <code>\-\-squash\-hierarchy</code>\, do not mention the list of collections on the collection\'s index page \([https\://github\.com/ansible\-community/antsibull\-docs/pull/72](https\://github\.com/ansible\-community/antsibull\-docs/pull/72)\)\.
 
 <a id="v1-7-3"></a>
 ## v1\.7\.3
 
-<a id="release-summary-18"></a>
+<a id="release-summary-19"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-15"></a>
 ### Bugfixes
 
 * Fix rendering of the <code>action\_group</code> attribute \([https\://github\.com/ansible\-community/antsibull\-docs/pull/62](https\://github\.com/ansible\-community/antsibull\-docs/pull/62)\)\.
 
 <a id="v1-7-2"></a>
 ## v1\.7\.2
 
-<a id="release-summary-19"></a>
+<a id="release-summary-20"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-16"></a>
 ### Bugfixes
 
 * Fix <code>version\_added</code> processing for ansible\.builtin 0\.x to represent this as <code>Ansible 0\.x</code> instead of <code>ansible\-core 0\.x</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/61](https\://github\.com/ansible\-community/antsibull\-docs/pull/61)\)\.
 
 <a id="v1-7-1"></a>
 ## v1\.7\.1
 
-<a id="release-summary-20"></a>
+<a id="release-summary-21"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-17"></a>
 ### Bugfixes
 
 * Prevent crash during <code>stable</code> docsite build when <code>\_python</code> entry is present in deps file \([https\://github\.com/ansible\-community/antsibull\-docs/pull/57](https\://github\.com/ansible\-community/antsibull\-docs/pull/57)\)\.
 
 <a id="v1-7-0"></a>
 ## v1\.7\.0
 
-<a id="release-summary-21"></a>
+<a id="release-summary-22"></a>
 ### Release Summary
 
 Bugfix and feature release\.
 
-<a id="minor-changes-13"></a>
+<a id="minor-changes-14"></a>
 ### Minor Changes
 
 * Add <code>\-\-intersphinx</code> option to the <code>sphinx\-init</code> subcommand to allow adding additional <code>intersphinx\_mapping</code> entries to <code>conf\.py</code> \([https\://github\.com/ansible\-community/antsibull\-docs/issues/35](https\://github\.com/ansible\-community/antsibull\-docs/issues/35)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/44](https\://github\.com/ansible\-community/antsibull\-docs/pull/44)\)\.
 * Allow the <code>toctree</code> entries for in a collection\'s <code>docs/docsite/extra\-docs\.yml</code> to be a dictionary with <code>ref</code> and <code>title</code> keys instead of just a reference as a string \([https\://github\.com/ansible\-community/antsibull\-docs/pull/45](https\://github\.com/ansible\-community/antsibull\-docs/pull/45)\)\.
 * Antsibull\-docs now depends on [packaging](https\://pypi\.org/project/packaging/) \([https\://github\.com/ansible\-community/antsibull\-docs/pull/49](https\://github\.com/ansible\-community/antsibull\-docs/pull/49)\)\.
 * The collection index pages now contain the supported versions of ansible\-core of the collection in case collection\'s <code>meta/runtime\.yml</code> specifies <code>requires\_ansible</code> \([https\://github\.com/ansible\-community/antsibull\-docs/issues/48](https\://github\.com/ansible\-community/antsibull\-docs/issues/48)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/49](https\://github\.com/ansible\-community/antsibull\-docs/pull/49)\)\.
 * The output of the <code>lint\-collection\-docs</code> command has been improved\; in particular multi\-line messages are now indented \([https\://github\.com/ansible\-community/antsibull\-docs/pull/52](https\://github\.com/ansible\-community/antsibull\-docs/pull/52)\)\.
@@ -575,33 +592,33 @@
 
 * Avoid long aliases list to make left column too wide \([https\://github\.com/ansible\-collections/amazon\.aws/issues/1101](https\://github\.com/ansible\-collections/amazon\.aws/issues/1101)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/54](https\://github\.com/ansible\-community/antsibull\-docs/pull/54)\)\.
 * Make <code>lint\-collection\-docs \-\-plugin\-docs</code> subcommand actually work \([https\://github\.com/ansible\-community/antsibull\-docs/pull/47](https\://github\.com/ansible\-community/antsibull\-docs/pull/47)\)\.
 
 <a id="v1-6-1"></a>
 ## v1\.6\.1
 
-<a id="release-summary-22"></a>
+<a id="release-summary-23"></a>
 ### Release Summary
 
 Bugfix release for ansible\-core 2\.14\.
 
 <a id="bugfixes-19"></a>
 ### Bugfixes
 
 * Fix formulation of top\-level <code>version\_added</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/43](https\://github\.com/ansible\-community/antsibull\-docs/pull/43)\)\.
 
 <a id="v1-6-0"></a>
 ## v1\.6\.0
 
-<a id="release-summary-23"></a>
+<a id="release-summary-24"></a>
 ### Release Summary
 
 Bugfix and feature release\.
 
-<a id="minor-changes-14"></a>
+<a id="minor-changes-15"></a>
 ### Minor Changes
 
 * Allow to specify choices as dictionary instead of list \([https\://github\.com/ansible\-community/antsibull\-docs/pull/36](https\://github\.com/ansible\-community/antsibull\-docs/pull/36)\)\.
 * Use JSON serializer to format choices \([https\://github\.com/ansible\-community/antsibull\-docs/pull/37](https\://github\.com/ansible\-community/antsibull\-docs/pull/37)\)\.
 * Use special serializer to format INI values in examples \([https\://github\.com/ansible\-community/antsibull\-docs/pull/37](https\://github\.com/ansible\-community/antsibull\-docs/pull/37)\)\.
 
 <a id="bugfixes-20"></a>
@@ -611,59 +628,59 @@
 * For INI examples which have no default\, write <code>VALUE</code> as intended instead of <code>None</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/37](https\://github\.com/ansible\-community/antsibull\-docs/pull/37)\)\.
 * Format lists correctly for INI examples \([https\://github\.com/ansible\-community/antsibull\-docs/pull/37](https\://github\.com/ansible\-community/antsibull\-docs/pull/37)\)\.
 * The <code>sphinx\-init</code> subcommand\'s <code>requirement\.txt</code> file avoids Sphinx 5\.2\.0\.post0\, which triggers a bug in sphinx\-rtd\-theme which happens to be the parent theme of the default theme sphinx\_ansible\_theme used by <code>sphinx\-init</code> \([https\://github\.com/ansible\-community/antsibull\-docs/issues/39](https\://github\.com/ansible\-community/antsibull\-docs/issues/39)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/40](https\://github\.com/ansible\-community/antsibull\-docs/pull/40)\)\.
 
 <a id="v1-5-0"></a>
 ## v1\.5\.0
 
-<a id="release-summary-24"></a>
+<a id="release-summary-25"></a>
 ### Release Summary
 
 Feature and bugfix release\.
 
-<a id="minor-changes-15"></a>
+<a id="minor-changes-16"></a>
 ### Minor Changes
 
 * Detect filter and test plugin aliases and avoid them being emitted multiple times\. Instead insert redirects so that stub pages will be created \([https\://github\.com/ansible\-community/antsibull\-docs/pull/33](https\://github\.com/ansible\-community/antsibull\-docs/pull/33)\)\.
 * Replace <code>ansible\.builtin</code> with <code>ansible\-core</code>\, <code>ansible\-base</code>\, or <code>Ansible</code> in version added collection names\. Also write <code>\<collection\_name\> \<version\></code> instead of <code>\<version\> of \<collection\_name\></code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/34](https\://github\.com/ansible\-community/antsibull\-docs/pull/34)\)\.
 
 <a id="bugfixes-21"></a>
 ### Bugfixes
 
 * Fix escaping of collection names in version added statements\, and fix collection names for roles options \([https\://github\.com/ansible\-community/antsibull\-docs/pull/34](https\://github\.com/ansible\-community/antsibull\-docs/pull/34)\)\.
 
 <a id="v1-4-0"></a>
 ## v1\.4\.0
 
-<a id="release-summary-25"></a>
+<a id="release-summary-26"></a>
 ### Release Summary
 
 Feature and bugfix release\.
 
-<a id="minor-changes-16"></a>
+<a id="minor-changes-17"></a>
 ### Minor Changes
 
 * The <code>sphinx\-init</code> subcommand now also creates an <code>antsibull\-docs\.cfg</code> file and moves configuration settings from CLI flags in <code>build\.sh</code> to this configuration file \([https\://github\.com/ansible\-community/antsibull\-docs/pull/26](https\://github\.com/ansible\-community/antsibull\-docs/pull/26)\)\.
 * There are two new options for explicitly specified configuration files named <code>collection\_url</code> and <code>collection\_install</code>\. These allow to override the URLs pointing to collections \(default link to galaxy\.ansible\.com\)\, and the commands to install collections \(use <code>ansible\-galaxy collection install</code> by default\)\. This can be useful when documenting \(internal\) collections that are not available on Ansible Galaxy\. The default <code>antsibull\-docs\.cfg</code> generated by the <code>sphinx\-init</code> subcommand shows how this can be configured \([https\://github\.com/ansible\-community/antsibull\-docs/issues/15](https\://github\.com/ansible\-community/antsibull\-docs/issues/15)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/26](https\://github\.com/ansible\-community/antsibull\-docs/pull/26)\)\.
 * When generating plugin error pages\, or showing non\-fatal errors in plugins or roles\, link to the collection\'s issue tracker instead of the collection\'s URL if available \([https\://github\.com/ansible\-community/antsibull\-docs/pull/29](https\://github\.com/ansible\-community/antsibull\-docs/pull/29)\)\.
 
 <a id="bugfixes-22"></a>
 ### Bugfixes
 
 * Make handling of bad documentation more robust when certain values are <code>None</code> while the keys are present \([https\://github\.com/ansible\-community/antsibull\-docs/pull/32](https\://github\.com/ansible\-community/antsibull\-docs/pull/32)\)\.
 
 <a id="v1-3-0"></a>
 ## v1\.3\.0
 
-<a id="release-summary-26"></a>
+<a id="release-summary-27"></a>
 ### Release Summary
 
 Feature and bugfix release\.
 
-<a id="minor-changes-17"></a>
+<a id="minor-changes-18"></a>
 ### Minor Changes
 
 * Ensure that values for <code>default</code>\, <code>choices</code>\, and <code>sample</code> use the types specified for the option / return value \([https\://github\.com/ansible\-community/antsibull\-docs/pull/19](https\://github\.com/ansible\-community/antsibull\-docs/pull/19)\)\.
 * If a plugin or module has requirements listed\, add a disclaimer next to the installation line at the top that further requirements are needed \([https\://github\.com/ansible\-community/antsibull\-docs/issues/23](https\://github\.com/ansible\-community/antsibull\-docs/issues/23)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/24](https\://github\.com/ansible\-community/antsibull\-docs/pull/24)\)\.
 * Show the \'you might already have this collection installed if you are using the <code>ansible</code> package\' disclaimer for plugins only for official docsite builds \(subcommands <code>devel</code> and <code>stable</code>\)\. Also include this disclaimer for roles on official docsite builds \([https\://github\.com/ansible\-community/antsibull\-docs/pull/25](https\://github\.com/ansible\-community/antsibull\-docs/pull/25)\)\.
 * Use <code>true</code> and <code>false</code> for booleans instead of <code>yes</code> and <code>no</code> \([https\://github\.com/ansible\-community/community\-topics/issues/116](https\://github\.com/ansible\-community/community\-topics/issues/116)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/19](https\://github\.com/ansible\-community/antsibull\-docs/pull/19)\)\.
 * When processing formatting directives\, make sure to properly escape all other text for RST respectively HTML instead of including it verbatim \([https\://github\.com/ansible\-community/antsibull\-docs/issues/21](https\://github\.com/ansible\-community/antsibull\-docs/issues/21)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/22](https\://github\.com/ansible\-community/antsibull\-docs/pull/22)\)\.
@@ -672,47 +689,47 @@
 ### Bugfixes
 
 * Improve indentation of HTML blocks for tables to avoid edge cases which generate invalid RST \([https\://github\.com/ansible\-community/antsibull\-docs/pull/22](https\://github\.com/ansible\-community/antsibull\-docs/pull/22)\)\.
 
 <a id="v1-2-2"></a>
 ## v1\.2\.2
 
-<a id="release-summary-27"></a>
+<a id="release-summary-28"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-24"></a>
 ### Bugfixes
 
 * Fix rstcheck\-core support \([https\://github\.com/ansible\-community/antsibull\-docs/pull/20](https\://github\.com/ansible\-community/antsibull\-docs/pull/20)\)\.
 
 <a id="v1-2-1"></a>
 ## v1\.2\.1
 
-<a id="release-summary-28"></a>
+<a id="release-summary-29"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-25"></a>
 ### Bugfixes
 
 * Do not escape <code>\<</code>\, <code>\></code>\, <code>\&</code>\, and <code>\'</code> in JSONified defaults and examples as the [Jinja2 tojson filter](https\://jinja\.palletsprojects\.com/en/2\.11\.x/templates/\#tojson) does\. Also improve formatting by making sure <code>\,</code> is followed by a space \([https\://github\.com/ansible\-community/antsibull\-docs/pull/18](https\://github\.com/ansible\-community/antsibull\-docs/pull/18)\)\.
 * The collection filter was ignored when parsing the <code>ansible\-galaxy collection list</code> output for the docs build \([https\://github\.com/ansible\-community/antsibull\-docs/issues/16](https\://github\.com/ansible\-community/antsibull\-docs/issues/16)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/17](https\://github\.com/ansible\-community/antsibull\-docs/pull/17)\)\.
 
 <a id="v1-2-0"></a>
 ## v1\.2\.0
 
-<a id="release-summary-29"></a>
+<a id="release-summary-30"></a>
 ### Release Summary
 
 Feature and bugfix release\.
 
-<a id="minor-changes-18"></a>
+<a id="minor-changes-19"></a>
 ### Minor Changes
 
 * Support plugin <code>seealso</code> from the [semantic markup specification](https\://hackmd\.io/VjN60QSoRSSeRfvGmOH1lQ\?both) \([https\://github\.com/ansible\-community/antsibull\-docs/pull/8](https\://github\.com/ansible\-community/antsibull\-docs/pull/8)\)\.
 * The <code>lint\-collection\-docs</code> subcommand has a new boolean flag <code>\-\-plugin\-docs</code> which renders the plugin docs to RST and validates them with rstcheck\. This can be used as a lighter version of rendering the docsite in CI \([https\://github\.com/ansible\-community/antsibull\-docs/pull/12](https\://github\.com/ansible\-community/antsibull\-docs/pull/12)\)\.
 * The files in the source repository now follow the [REUSE Specification](https\://reuse\.software/spec/)\. The only exceptions are changelog fragments in <code>changelogs/fragments/</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/14](https\://github\.com/ansible\-community/antsibull\-docs/pull/14)\)\.
 
 <a id="bugfixes-26"></a>
@@ -720,61 +737,61 @@
 
 * Make sure that <code>\_input</code> does not show up twice for test or filter arguments when the plugin mentions it in <code>positional</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/10](https\://github\.com/ansible\-community/antsibull\-docs/pull/10)\)\.
 * Mark rstcheck 4\.x and 5\.x as compatible\. Support rstcheck 6\.x as well \([https\://github\.com/ansible\-community/antsibull\-docs/pull/13](https\://github\.com/ansible\-community/antsibull\-docs/pull/13)\)\.
 
 <a id="v1-1-0"></a>
 ## v1\.1\.0
 
-<a id="release-summary-30"></a>
+<a id="release-summary-31"></a>
 ### Release Summary
 
 Feature release with support for ansible\-core 2\.14\'s sidecar docs feature\.
 
-<a id="minor-changes-19"></a>
+<a id="minor-changes-20"></a>
 ### Minor Changes
 
 * If lookup plugins have a single return value starting with <code>\_</code>\, that return value is now labelled <code>Return value</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/6](https\://github\.com/ansible\-community/antsibull\-docs/pull/6)\)\.
 * If lookup plugins have an option called <code>\_terms</code>\, it is now shown in its own section <code>Terms</code>\, and not in the regular <code>Parameters</code> section \([https\://github\.com/ansible\-community/antsibull\-docs/pull/6](https\://github\.com/ansible\-community/antsibull\-docs/pull/6)\)\.
 * More robust handling of parsing errors when ansible\-doc was unable to extract documentation \([https\://github\.com/ansible\-community/antsibull\-docs/pull/6](https\://github\.com/ansible\-community/antsibull\-docs/pull/6)\)\.
 * Support parameter type <code>any</code>\, and show <code>raw</code> as <code>any</code> \([https\://github\.com/ansible\-community/antsibull\-docs/pull/6](https\://github\.com/ansible\-community/antsibull\-docs/pull/6)\)\.
 * Support test and filter plugins when ansible\-core 2\.14\+ is used\. This works with the current <code>devel</code> branch of ansible\-core \([https\://github\.com/ansible\-community/antsibull\-docs/pull/6](https\://github\.com/ansible\-community/antsibull\-docs/pull/6)\)\.
 
 <a id="v1-0-1"></a>
 ## v1\.0\.1
 
-<a id="release-summary-31"></a>
+<a id="release-summary-32"></a>
 ### Release Summary
 
 Bugfix release\.
 
 <a id="bugfixes-27"></a>
 ### Bugfixes
 
 * Make sure that aliases of module/plugin options and return values that result in identical RST labels under docutil\'s normalization are only emitted once \([https\://github\.com/ansible\-community/antsibull\-docs/pull/7](https\://github\.com/ansible\-community/antsibull\-docs/pull/7)\)\.
 * Properly escape module/plugin option and return value slugs in generated HTML \([https\://github\.com/ansible\-community/antsibull\-docs/pull/7](https\://github\.com/ansible\-community/antsibull\-docs/pull/7)\)\.
 
 <a id="v1-0-0"></a>
 ## v1\.0\.0
 
-<a id="release-summary-32"></a>
+<a id="release-summary-33"></a>
 ### Release Summary
 
 First stable release\.
 
 <a id="major-changes-2"></a>
 ### Major Changes
 
 * From version 1\.0\.0 on\, antsibull\-docs is sticking to semantic versioning and aims at providing no backwards compatibility breaking changes <strong>to the command line API \(antsibull\-docs\)</strong> during a major release cycle\. We explicitly exclude code compatibility\. <strong>antsibull\-docs is not supposed to be used as a library\,</strong> and when used as a library it might not conform to semantic versioning \([https\://github\.com/ansible\-community/antsibull\-docs/pull/2](https\://github\.com/ansible\-community/antsibull\-docs/pull/2)\)\.
 
-<a id="minor-changes-20"></a>
+<a id="minor-changes-21"></a>
 ### Minor Changes
 
 * Only mention \'These are the collections with docs hosted on docs\.ansible\.com\' for <code>stable</code> and <code>devel</code> subcommands \([https\://github\.com/ansible\-community/antsibull\-docs/pull/3](https\://github\.com/ansible\-community/antsibull\-docs/pull/3)\)\.
 * Stop using some API from antsibull\-core that is being removed \([https\://github\.com/ansible\-community/antsibull\-docs/pull/1](https\://github\.com/ansible\-community/antsibull\-docs/pull/1)\)\.
 
 <a id="v0-1-0"></a>
 ## v0\.1\.0
 
-<a id="release-summary-33"></a>
+<a id="release-summary-34"></a>
 ### Release Summary
 
 Initial release\. The <code>antsibull\-docs</code> tool is compatible to the one from antsibull 0\.43\.0\.
```

#### html2text {}

```diff
@@ -1,80 +1,85 @@
 # antsibull\-docs \-\- Ansible Documentation Build Scripts Release Notes
-**Topics** - _v_2_\_._8_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._7_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._6_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
-_B_u_g_f_i_x_e_s - _v_2_\_._6_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._5_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_2_\_._4_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
-_D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _B_u_g_f_i_x_e_s - _K_n_o_w_n_ _I_s_s_u_e_s - _v_2_\_._3_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
-_B_u_g_f_i_x_e_s - _v_2_\_._3_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._2_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r
-_C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s
-- _B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g_ _G_u_i_d_e - _B_u_g_f_i_x_e_s - _v_1_\_._1_1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
-_M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._1_0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s -
-_B_u_g_f_i_x_e_s - _v_1_\_._9_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._8_\_._2 - _R_e_l_e_a_s_e
-_S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._8_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._8_\_._0 - _R_e_l_e_a_s_e
-_S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._7_\_._4 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s -
-_v_1_\_._7_\_._3 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._7_\_._2 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s -
-_v_1_\_._7_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._7_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r
-_C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._6_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._6_\_._0 - _R_e_l_e_a_s_e
-_S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._5_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s
-- _B_u_g_f_i_x_e_s - _v_1_\_._4_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._3_\_._0 -
-_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._2 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
-_B_u_g_f_i_x_e_s - _v_1_\_._2_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
-_M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
-_v_1_\_._0_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r
-_C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_0_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y ## v2\.8\.0 ### Release
-Summary Bugfix and feature release\. ### Minor Changes * Add support for \"dark
-mode\" to the option table styling \([https\://github\.com/ansible\-community/
-antsibull\-docs/pull/253](https\://github\.com/ansible\-community/antsibull\-
-docs/pull/253)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/
-258](https\://github\.com/ansible\-community/antsibull\-docs/pull/258)\)\. *
-Add support for the latest antsibull\-core v3 pre\-release\, 3\.0\.0a1 \(
-[https\://github\.com/ansible\-community/antsibull\-docs/pull/250](https\://
-github\.com/ansible\-community/antsibull\-docs/pull/250)\)\. * Declare support
-for Python 3\.12 \([https\://github\.com/ansible\-community/antsibull\-docs/
-pull/255](https\://github\.com/ansible\-community/antsibull\-docs/pull/255)\)\.
-* The colors used by the CSS provided by the Antsibull Sphinx extension can now
-be overridden \([https\://github\.com/ansible\-community/antsibull\-docs/pull/
-254](https\://github\.com/ansible\-community/antsibull\-docs/pull/254)\)\. ###
-Bugfixes * Fix duplicate docs detection \(for aliases\) for latest ansible\-
-core devel \([https\://github\.com/ansible\-community/antsibull\-docs/pull/257]
-(https\://github\.com/ansible\-community/antsibull\-docs/pull/257)\)\. ##
-v2\.7\.0 ### Release Summary Bugfix and refactoring release\. ### Minor Changes
-* Explicitly set up Galaxy context instead of relying on deprecated
-functionality \([https\://github\.com/ansible\-community/antsibull\-docs/pull/
-234](https\://github\.com/ansible\-community/antsibull\-docs/pull/234)\)\. ###
-Bugfixes * Fix schema for seealso in role entrypoints\. Plugin references now
-work \([https\://github\.com/ansible\-community/antsibull\-docs/issues/237]
-(https\://github\.com/ansible\-community/antsibull\-docs/issues/237)\, [https\:
-//github\.com/ansible\-community/antsibull\-docs/pull/240](https\://
-github\.com/ansible\-community/antsibull\-docs/pull/240)\)\. * Make error
-reporting for invalid references in plugin seealso entries more precise \(
-[https\://github\.com/ansible\-community/antsibull\-docs/pull/240](https\://
-github\.com/ansible\-community/antsibull\-docs/pull/240)\)\. * Support new
-ansible\-doc \-\-json output field plugin\_name \([https\://github\.com/
-ansible\-community/antsibull\-docs/pull/242](https\://github\.com/ansible\-
-community/antsibull\-docs/pull/242)\)\. * Use certain fields from library
-context instead of app context that are deprecated in the app context and will
-be removed from antsibull\-core 3\.0\.0 \([https\://github\.com/ansible\-
-community/antsibull\-docs/pull/233](https\://github\.com/ansible\-community/
-antsibull\-docs/pull/233)\)\. ## v2\.6\.1 ### Release Summary Bugfix release\.
-### Bugfixes * For role argument specs\, allow author\, description\, and todo
-to be a string instead of a list of strings\, similarly as with ansible\-doc
-and with modules and plugins \([https\://github\.com/ansible\-community/
-antsibull\-docs/pull/227](https\://github\.com/ansible\-community/antsibull\-
-docs/pull/227)\)\. * Make sure that title underlines have the correct width for
-wide Unicode characters \([https\://github\.com/ansible\-community/antsibull\-
-docs/issues/228](https\://github\.com/ansible\-community/antsibull\-docs/
-issues/228)\, [https\://github\.com/ansible\-community/antsibull\-docs/pull/
-229](https\://github\.com/ansible\-community/antsibull\-docs/pull/229)\)\. ##
-v2\.6\.0 ### Release Summary Fix parsing of EXAMPLES and improve error message
-### Minor Changes * Improve error messages when calls to ansible\-doc fail \(
-[https\://github\.com/ansible\-community/antsibull\-docs/pull/223](https\://
-github\.com/ansible\-community/antsibull\-docs/pull/223)\)\. ### Bugfixes *
-When EXAMPLES has the format specified by \# fmt\: \>
+**Topics** - _v_2_\_._9_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_2_\_._8_\_._0 - _R_e_l_e_a_s_e
+_S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._7_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s
+- _B_u_g_f_i_x_e_s - _v_2_\_._6_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_2_\_._6_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y
+- _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._5_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
+_v_2_\_._4_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _D_e_p_r_e_c_a_t_e_d_ _F_e_a_t_u_r_e_s - _B_u_g_f_i_x_e_s -
+_K_n_o_w_n_ _I_s_s_u_e_s - _v_2_\_._3_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_2_\_._3_\_._0 - _R_e_l_e_a_s_e
+_S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._2_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s
+- _B_u_g_f_i_x_e_s - _v_2_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_2_\_._0_\_._0 -
+_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_r_e_a_k_i_n_g_ _C_h_a_n_g_e_s_ _/_ _P_o_r_t_i_n_g
+_G_u_i_d_e - _B_u_g_f_i_x_e_s - _v_1_\_._1_1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._1_0_\_._0 -
+_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._9_\_._0 - _R_e_l_e_a_s_e
+_S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._8_\_._2 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._8_\_._1 -
+_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._8_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
+_B_u_g_f_i_x_e_s - _v_1_\_._7_\_._4 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._7_\_._3 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
+_B_u_g_f_i_x_e_s - _v_1_\_._7_\_._2 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._7_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
+_B_u_g_f_i_x_e_s - _v_1_\_._7_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._6_\_._1 -
+_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._6_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s -
+_B_u_g_f_i_x_e_s - _v_1_\_._5_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._4_\_._0 -
+_R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._3_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r
+_C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._2 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._1 - _R_e_l_e_a_s_e
+_S_u_m_m_a_r_y - _B_u_g_f_i_x_e_s - _v_1_\_._2_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _B_u_g_f_i_x_e_s -
+_v_1_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_i_n_o_r_ _C_h_a_n_g_e_s - _v_1_\_._0_\_._1 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y -
+_B_u_g_f_i_x_e_s - _v_1_\_._0_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y - _M_a_j_o_r_ _C_h_a_n_g_e_s - _M_i_n_o_r_ _C_h_a_n_g_e_s -
+_v_0_\_._1_\_._0 - _R_e_l_e_a_s_e_ _S_u_m_m_a_r_y ## v2\.9\.0 ### Release Summary Maintenance
+release\. ### Minor Changes * Add support for the antsibull\-core v3 \([https\:
+//github\.com/ansible\-community/antsibull\-docs/pull/261](https\://
+github\.com/ansible\-community/antsibull\-docs/pull/261)\)\. ## v2\.8\.0 ###
+Release Summary Bugfix and feature release\. ### Minor Changes * Add support
+for \"dark mode\" to the option table styling \([https\://github\.com/ansible\-
+community/antsibull\-docs/pull/253](https\://github\.com/ansible\-community/
+antsibull\-docs/pull/253)\, [https\://github\.com/ansible\-community/
+antsibull\-docs/pull/258](https\://github\.com/ansible\-community/antsibull\-
+docs/pull/258)\)\. * Add support for the latest antsibull\-core v3 pre\-
+release\, 3\.0\.0a1 \([https\://github\.com/ansible\-community/antsibull\-docs/
+pull/250](https\://github\.com/ansible\-community/antsibull\-docs/pull/250)\)\.
+* Declare support for Python 3\.12 \([https\://github\.com/ansible\-community/
+antsibull\-docs/pull/255](https\://github\.com/ansible\-community/antsibull\-
+docs/pull/255)\)\. * The colors used by the CSS provided by the Antsibull
+Sphinx extension can now be overridden \([https\://github\.com/ansible\-
+community/antsibull\-docs/pull/254](https\://github\.com/ansible\-community/
+antsibull\-docs/pull/254)\)\. ### Bugfixes * Fix duplicate docs detection \(for
+aliases\) for latest ansible\-core devel \([https\://github\.com/ansible\-
+community/antsibull\-docs/pull/257](https\://github\.com/ansible\-community/
+antsibull\-docs/pull/257)\)\. ## v2\.7\.0 ### Release Summary Bugfix and
+refactoring release\. ### Minor Changes * Explicitly set up Galaxy context
+instead of relying on deprecated functionality \([https\://github\.com/
+ansible\-community/antsibull\-docs/pull/234](https\://github\.com/ansible\-
+community/antsibull\-docs/pull/234)\)\. ### Bugfixes * Fix schema for seealso
+in role entrypoints\. Plugin references now work \([https\://github\.com/
+ansible\-community/antsibull\-docs/issues/237](https\://github\.com/ansible\-
+community/antsibull\-docs/issues/237)\, [https\://github\.com/ansible\-
+community/antsibull\-docs/pull/240](https\://github\.com/ansible\-community/
+antsibull\-docs/pull/240)\)\. * Make error reporting for invalid references in
+plugin seealso entries more precise \([https\://github\.com/ansible\-community/
+antsibull\-docs/pull/240](https\://github\.com/ansible\-community/antsibull\-
+docs/pull/240)\)\. * Support new ansible\-doc \-\-json output field
+plugin\_name \([https\://github\.com/ansible\-community/antsibull\-docs/pull/
+242](https\://github\.com/ansible\-community/antsibull\-docs/pull/242)\)\. *
+Use certain fields from library context instead of app context that are
+deprecated in the app context and will be removed from antsibull\-core 3\.0\.0
+\([https\://github\.com/ansible\-community/antsibull\-docs/pull/233](https\://
+github\.com/ansible\-community/antsibull\-docs/pull/233)\)\. ## v2\.6\.1 ###
+Release Summary Bugfix release\. ### Bugfixes * For role argument specs\, allow
+author\, description\, and todo to be a string instead of a list of strings\,
+similarly as with ansible\-doc and with modules and plugins \([https\://
+github\.com/ansible\-community/antsibull\-docs/pull/227](https\://github\.com/
+ansible\-community/antsibull\-docs/pull/227)\)\. * Make sure that title
+underlines have the correct width for wide Unicode characters \([https\://
+github\.com/ansible\-community/antsibull\-docs/issues/228](https\://
+github\.com/ansible\-community/antsibull\-docs/issues/228)\, [https\://
+github\.com/ansible\-community/antsibull\-docs/pull/229](https\://github\.com/
+ansible\-community/antsibull\-docs/pull/229)\)\. ## v2\.6\.0 ### Release
+Summary Fix parsing of EXAMPLES and improve error message ### Minor Changes *
+Improve error messages when calls to ansible\-doc fail \([https\://github\.com/
+ansible\-community/antsibull\-docs/pull/223](https\://github\.com/ansible\-
+community/antsibull\-docs/pull/223)\)\. ### Bugfixes * When EXAMPLES has the
+format specified by \# fmt\: \>
 \, this value is used to determine the code block type \([https\://github\.com/
 ansible\-community/antsibull\-docs/pull/225](https\://github\.com/ansible\-
 community/antsibull\-docs/pull/225)\)\. ## v2\.5\.0 ### Release Summary Release
 to support the updated Ansible Galaxy codebase\. ### Minor Changes * The
 default collection URL template has been changed from https\://
 galaxy\.ansible\.com/\{namespace\}/\{name\} to https\://galaxy\.ansible\.com/
 ui/repo/published/\{namespace\}/\{name\}/ to adjust for the Galaxy codebase
```

### Comparing `antsibull_docs-2.8.0/CHANGELOG.rst` & `antsibull_docs-2.9.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 ===================================================================
 antsibull-docs -- Ansible Documentation Build Scripts Release Notes
 ===================================================================
 
 .. contents:: Topics
 
+v2.9.0
+======
+
+Release Summary
+---------------
+
+Maintenance release.
+
+Minor Changes
+-------------
+
+- Add support for the antsibull-core v3 (https://github.com/ansible-community/antsibull-docs/pull/261).
+
 v2.8.0
 ======
 
 Release Summary
 ---------------
 
 Bugfix and feature release.
```

### Comparing `antsibull_docs-2.8.0/LICENSE` & `antsibull_docs-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/antsibull-docs.cfg` & `antsibull_docs-2.9.0/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/mkdocs.yml` & `antsibull_docs-2.9.0/mkdocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # REUSE-IgnoreEnd
 markdown_extensions:
   # Builtin
   - admonition
   - toc:
       permalink: true
   # pymdownx
+  - pymdownx.escapeall
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.superfences
 nav:
   - antsibull-docs: index.md
   - Creating a collection docsite: collection-docs.md
   - Official Ansible docsite: package-docs.md
+  - antsibull-docs Release Notes: changelog.md
```

### Comparing `antsibull_docs-2.8.0/noxfile.py` & `antsibull_docs-2.9.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,25 +151,31 @@
     # and spews type errors across the entire codebase.
     if False:
         additional_libraries = []
         for path in others:
             if isinstance(path, Path):
                 additional_libraries.extend(("--search-path", str(path / "src")))
 
-        purelib = session.run(
-            "python",
-            "-c",
-            "import sysconfig; print(sysconfig.get_path('purelib'))",
-            silent=True,
+        purelib = (
+            session.run(
+                "python",
+                "-c",
+                "import sysconfig; print(sysconfig.get_path('purelib'))",
+                silent=True,
+            )
+            or ""
         ).strip()
-        platlib = session.run(
-            "python",
-            "-c",
-            "import sysconfig; print(sysconfig.get_path('platlib'))",
-            silent=True,
+        platlib = (
+            session.run(
+                "python",
+                "-c",
+                "import sysconfig; print(sysconfig.get_path('platlib'))",
+                silent=True,
+            )
+            or ""
         ).strip()
         session.run(
             "pyre",
             "--source-directory",
             "src",
             "--search-path",
             purelib,
@@ -233,15 +239,15 @@
     if len(session.posargs) == 1:
         if not fragment_file.is_file():
             session.error(
                 f"Either {fragment_file} must already exist, "
                 "or two positional arguments must be provided."
             )
     # Needs newer antsibull-changelog for hatch version auto-detection support
-    install(session, "antsibull-changelog[toml] >= 0.24.0", "hatch")
+    install(session, "antsibull-changelog[toml] >= 0.26.0", "hatch")
     current_version = session.run("hatch", "version", silent=True).strip()
     if version != current_version:
         session.run("hatch", "version", version)
     if len(session.posargs) > 1:
         fragment = session.run(
             "python",
             "-c",
```

### Comparing `antsibull_docs-2.8.0/.github/workflows/antsibull-docs.yml` & `antsibull_docs-2.9.0/.github/workflows/antsibull-docs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/.github/workflows/build-css.yml` & `antsibull_docs-2.9.0/.github/workflows/build-css.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/changelogs/changelog.yaml` & `antsibull_docs-2.9.0/changelogs/changelog.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -776,7 +776,16 @@
     - 2.8.0.yml
     - 250-core-3.0.0a1.yaml
     - 253-darkmode-support-to-option-tables.yaml
     - 254-theme-colors.yml
     - 255-python-3.12.yml
     - 257-duplicates.yml
     release_date: '2024-03-12'
+  2.9.0:
+    changes:
+      minor_changes:
+      - Add support for the antsibull-core v3 (https://github.com/ansible-community/antsibull-docs/pull/261).
+      release_summary: Maintenance release.
+    fragments:
+    - 2.9.0.yml
+    - core-v3.yml
+    release_date: '2024-03-17'
```

### Comparing `antsibull_docs-2.8.0/changelogs/config.yaml` & `antsibull_docs-2.9.0/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/docs/collection-docs.md` & `antsibull_docs-2.9.0/docs/collection-docs.md`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/docs/index.md` & `antsibull_docs-2.9.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-docs – Building Ansible documentation
 
+[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
 [![Discuss on Matrix at #docs:ansible.com](https://img.shields.io/matrix/docs:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23docs:ansible.com&logo=matrix)](https://matrix.to/#/#docs:ansible.com)
 
 This package provides tooling for validating and building Ansible documentation. It mainly consists of a CLI tool, `antsibull-docs`, and a Sphinx extension. The main output format are [reStructured Text (RST)](https://en.wikipedia.org/wiki/ReStructuredText) files for consumption by [Sphinx](https://en.wikipedia.org/wiki/Sphinx_\(documentation_generator\)).
 
 **Collection maintainers and authors should look at the [Creating a collection docsite](collection-docs.md) section of this docsite.**
 
 antsibull-docs is covered by the [Ansible Code of Conduct](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html).
```

### Comparing `antsibull_docs-2.8.0/docs/package-docs.md` & `antsibull_docs-2.9.0/docs/package-docs.md`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/docs/schemas.rst` & `antsibull_docs-2.9.0/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/__init__.py` & `antsibull_docs-2.9.0/src/antsibull_docs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """The main antsibull-docs module. Contains versioning information."""
 
 import os
 import warnings
 
 import pydantic
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 
 
 def _filter_pydantic_v2_warnings() -> None:
     """
     Filter DeprecationWarnings from Pydantic v2. We cannot fix these without
     dropping support for v1 entirely, and we don't want to break setups with
     PYTHONWARNINGS=error.
```

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/_pydantic_compat.py` & `antsibull_docs-2.9.0/src/antsibull_docs/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/app_context.py` & `antsibull_docs-2.9.0/src/antsibull_docs/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/augment_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/augment_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/collection_config.py` & `antsibull_docs-2.9.0/src/antsibull_docs/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/collection_links.py` & `antsibull_docs-2.9.0/src/antsibull_docs/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/constants.py` & `antsibull_docs-2.9.0/src/antsibull_docs/constants.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/env_variables.py` & `antsibull_docs-2.9.0/src/antsibull_docs/env_variables.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/extra_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/lint_extra_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/lint_extra_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/lint_helpers.py` & `antsibull_docs-2.9.0/src/antsibull_docs/lint_helpers.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/lint_plugin_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/lint_plugin_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/plugin_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/plugin_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/process_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/process_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/rstcheck.py` & `antsibull_docs-2.9.0/src/antsibull_docs/rstcheck.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/antsibull_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/antsibull_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/_build.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/_build.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/collection.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/collection.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/collection_plugins.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/collection_plugins.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/current.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/current.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/devel.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/devel.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/lint_docs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/lint_docs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/plugin.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/sphinx_init.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/cli/doc_commands/stable.py` & `antsibull_docs-2.9.0/src/antsibull_docs/cli/doc_commands/stable.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/ansible_2_10_routing.yml` & `antsibull_docs-2.9.0/src/antsibull_docs/data/ansible_2_10_routing.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_callback_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_collections_by_namespace.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_env_variables.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/list_of_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-error.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-redirect.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin-tombstone.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugin.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/plugins_by_collection.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/role.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/attributes.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/choiceslist.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/collection_links.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/collection_links.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/deprecates.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/parameters.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/returnvalues.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/ansible-docsite/macros/version_added.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_callback_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_collections_by_namespace.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/list_of_plugins.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-deprecation.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-error.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-redirect.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin-tombstone.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugin.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/plugins_by_collection.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/role.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/attributes.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/choiceslist.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/deprecates.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/parameters.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/returnvalues.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/docsite/simplified-rst/macros/version_added.rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/antsibull-docs_cfg.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/build_sh.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/build_sh.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/conf_py.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/conf_py.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2` & `antsibull_docs-2.9.0/src/antsibull_docs/data/sphinx_init/rst_index_rst.j2`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/__init__.py` & `antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/ansible_doc.py` & `antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py` & `antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/ansible_doc_core_213.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/fqcn.py` & `antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/fqcn.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/parsing.py` & `antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/parsing.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/docs_parsing/routing.py` & `antsibull_docs-2.9.0/src/antsibull_docs/docs_parsing/routing.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/jinja2/__init__.py` & `antsibull_docs-2.9.0/src/antsibull_docs/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/jinja2/environment.py` & `antsibull_docs-2.9.0/src/antsibull_docs/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/jinja2/filters.py` & `antsibull_docs-2.9.0/src/antsibull_docs/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/jinja2/tests.py` & `antsibull_docs-2.9.0/src/antsibull_docs/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/markup/_counter.py` & `antsibull_docs-2.9.0/src/antsibull_docs/markup/_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/markup/htmlify.py` & `antsibull_docs-2.9.0/src/antsibull_docs/markup/htmlify.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/markup/rstify.py` & `antsibull_docs-2.9.0/src/antsibull_docs/markup/rstify.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/markup/semantic_helper.py` & `antsibull_docs-2.9.0/src/antsibull_docs/markup/semantic_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/ansible_doc.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/app_context.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/app_context.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/collection_config.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/collection_config.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/collection_links.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/collection_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/__init__.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/ansible_doc.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/base.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/base.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/callback.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/callback.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/module.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/module.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/plugin.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/plugin.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/positional.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/positional.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/schemas/docs/role.py` & `antsibull_docs-2.9.0/src/antsibull_docs/schemas/docs/role.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/utils/collection_name_transformer.py` & `antsibull_docs-2.9.0/src/antsibull_docs/utils/collection_name_transformer.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/utils/get_pkg_data.py` & `antsibull_docs-2.9.0/src/antsibull_docs/utils/get_pkg_data.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/vendored/ansible.py` & `antsibull_docs-2.9.0/src/antsibull_docs/vendored/ansible.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/write_docs/__init__.py` & `antsibull_docs-2.9.0/src/antsibull_docs/write_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/write_docs/collections.py` & `antsibull_docs-2.9.0/src/antsibull_docs/write_docs/collections.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/write_docs/hierarchy.py` & `antsibull_docs-2.9.0/src/antsibull_docs/write_docs/hierarchy.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/write_docs/indexes.py` & `antsibull_docs-2.9.0/src/antsibull_docs/write_docs/indexes.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/write_docs/plugin_stubs.py` & `antsibull_docs-2.9.0/src/antsibull_docs/write_docs/plugin_stubs.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/antsibull_docs/write_docs/plugins.py` & `antsibull_docs-2.9.0/src/antsibull_docs/write_docs/plugins.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/__init__.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/antsibull-minimal.css` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/antsibull-minimal.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/antsibull.sty` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/antsibull.sty`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/assets.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/assets.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default-autodark.css` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default-autodark.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default-dark.css` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default-dark.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/colors-default.css` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/colors-default.css`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/directive_helper.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/directive_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/directives.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/directives.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/nodes.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/nodes.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/roles.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/roles.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/sphinx_helper.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/sphinx_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/antsibull-minimal.scss`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/build.sh` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/default-colors-dark.scss` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/default-colors-dark.scss`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/default-colors-light.scss` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/default-colors-light.scss`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/css/package-lock.json` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/css/package-lock.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/src/sphinx_antsibull_ext/schemas/ansible_links.py` & `antsibull_docs-2.9.0/src/sphinx_antsibull_ext/schemas/ansible_links.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/stubs/rstcheck.pyi` & `antsibull_docs-2.9.0/stubs/rstcheck.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/stubs/rstcheck_core/config.pyi` & `antsibull_docs-2.9.0/stubs/rstcheck_core/config.pyi`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/validate-html.py` & `antsibull_docs-2.9.0/tests/validate-html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-all-others.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-all-others.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-all.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-all.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns.col2-ns2.col.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns.col2-ns2.col.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.col.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.col.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.flatcol.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ansible.builtin-ns2.flatcol.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col1-ns.col2-ns2.col-ns2.flatcol.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col1-ns.col2-ns2.col-ns2.flatcol.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col1-ns2.col-ns2.flatcol.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col1-ns2.col-ns2.flatcol.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns.col2.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns.col2.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-doc-cache-ns2.col.json` & `antsibull_docs-2.9.0/tests/functional/ansible-doc-cache-ns2.col.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible-version.output` & `antsibull_docs-2.9.0/tests/functional/ansible-version.output`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/ansible_doc_caching.py` & `antsibull_docs-2.9.0/tests/functional/ansible_doc_caching.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/build-docs-baseline.sh` & `antsibull_docs-2.9.0/tests/functional/build-docs-baseline.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/build-sphinx-init-baseline.sh` & `antsibull_docs-2.9.0/tests/functional/build-sphinx-init-baseline.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/sanitize-ansible-doc-dump.py` & `antsibull_docs-2.9.0/tests/functional/sanitize-ansible-doc-dump.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/sanitize-ansible-galaxy-list.py` & `antsibull_docs-2.9.0/tests/functional/sanitize-ansible-galaxy-list.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/test_docs_baseline.py` & `antsibull_docs-2.9.0/tests/functional/test_docs_baseline.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/test_docs_linting.py` & `antsibull_docs-2.9.0/tests/functional/test_docs_linting.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/test_sphinx_init_baseline.py` & `antsibull_docs-2.9.0/tests/functional/test_sphinx_init_baseline.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/utils.py` & `antsibull_docs-2.9.0/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/environment_variables.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/index_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/index_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col1/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col1/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/bar_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo4_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns/col2/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns/col2/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_redirect_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/is_bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-default/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/index_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col1/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/bar_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo4_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns/col2/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_redirect_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/is_bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-breadcrumbs/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns/col1/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_redirect_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/is_bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-no-indexes/collections/ns2/flatcol/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/index_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/index_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/bar_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo4_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns/col2/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst/collections/ns2/flatcol/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-simplified-rst-squash-hierarchy/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/build.sh` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/conf.py` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-collections/rst/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/build.sh` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-config/conf.py` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-config/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/build.sh` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-current/conf.py` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-current/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/antsibull-docs.cfg`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/build.sh` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/build.sh`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-sphinx-init-extra/conf.py` & `antsibull_docs-2.9.0/tests/functional/baseline-sphinx-init-extra/conf.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_redirect_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/is_bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-squash-hierarchy/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo2_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_become.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cache.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_callback.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_cliconf.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_connection.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_filter.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_inventory.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_lookup.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_redirect_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_role.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_shell.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_strategy.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/foo_vars.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/index.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/is_bar_test.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/sub.foo3_module.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/baseline-use-html-blobs/collections/ns2/col/docsite/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/plugins/modules/foo4.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns/col2/roles/bar/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/galaxy.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/links.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/docs/docsite/rst/filter_guide.rst`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/become/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cache/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/callback/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/cliconf/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/connection/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/filter/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/inventory/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/lookup/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/modules/sub/foo3.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/shell/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/strategy/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/bar.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/test/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/plugins/vars/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/col/roles/foo/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py` & `antsibull_docs-2.9.0/tests/functional/collections/ansible_collections/ns2/flatcol/plugins/modules/sub/foo2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py` & `antsibull_docs-2.9.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/lookup/bar.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py` & `antsibull_docs-2.9.0/tests/functional/other-collections/ansible_collections/ext/col/plugins/modules/foo.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/test_schema.py` & `antsibull_docs-2.9.0/tests/functional/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_become.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_become.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_become_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_become_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cache.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cache.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cache_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cache_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_callback.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_callback.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_callback_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_callback_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cliconf.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cliconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_cliconf_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_cliconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_connection.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_connection_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_filter.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_filter.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_filter_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_filter_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_httpapi.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_httpapi.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_httpapi_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_httpapi_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_inventory.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_inventory.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_inventory_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_inventory_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_lookup.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_lookup.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_lookup_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_lookup_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_module.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_module.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_module_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_module_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_netconf.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_netconf.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_netconf_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_netconf_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_role.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_role.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_role_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_role_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_shell.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_shell.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_shell_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_shell_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_strategy.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_strategy.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_strategy_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_strategy_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_test.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_test.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_test_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_test_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_vars.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_vars.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/one_vars_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/one_vars_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/ssh_connection.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/ssh_connection.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/functional/schema/good_data/ssh_connection_results.json` & `antsibull_docs-2.9.0/tests/functional/schema/good_data/ssh_connection_results.json`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/units/test_jinja2.py` & `antsibull_docs-2.9.0/tests/units/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/units/markup/test_counter.py` & `antsibull_docs-2.9.0/tests/units/markup/test_counter.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/units/markup/test_markup.py` & `antsibull_docs-2.9.0/tests/units/markup/test_markup.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/tests/units/markup/test_semantic_helper.py` & `antsibull_docs-2.9.0/tests/units/markup/test_semantic_helper.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/.gitignore` & `antsibull_docs-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/README.md` & `antsibull_docs-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-docs -- Ansible Documentation Build Scripts
+[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
 [![Discuss on Matrix at #docs:ansible.com](https://img.shields.io/matrix/docs:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23docs:ansible.com&logo=matrix)](https://matrix.to/#/#docs:ansible.com)
 [![Nox badge](https://github.com/ansible-community/antsibull-docs/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-docs/actions/workflows/nox.yml)
 [![Build docs testing badge](https://github.com/ansible-community/antsibull-docs/workflows/antsibull-docs%20tests/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-docs/actions?query=workflow%3A%22antsibull-docs+tests%22+branch%3Amain)
 [![Build CSS testing badge](https://github.com/ansible-community/antsibull-docs/workflows/Build%20CSS/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-docs/actions?query=workflow%3A%22Build+CSS%22+branch%3Amain)
 [![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-docs)](https://codecov.io/gh/ansible-community/antsibull-docs)
 
 Tooling for building Ansible documentation. This is mainly the `antsibull-docs` command and the [Sphinx extension](https://www.sphinx-doc.org/en/master/), ``sphinx_antsibull_ext``. Please check out the [documentation](https://ansible.readthedocs.io/projects/antsibull-docs/) for more information.
```

### Comparing `antsibull_docs-2.8.0/pyproject.toml` & `antsibull_docs-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "ansible-pygments",
-    "antsibull-core >= 2.1.0, <= 3.0.0a1.post0",
+    "antsibull-core >= 2.1.0, < 4.0.0",
     "antsibull-docs-parser >= 1.0.0, < 2.0.0",
     "asyncio-pool",
     "docutils",
     "jinja2 >= 3.0",
     # Support for Version.major
     "packaging >= 20.0",
     "rstcheck >= 3.0.0, < 7.0.0",
```

### Comparing `antsibull_docs-2.8.0/LICENSES/BSD-2-Clause.txt` & `antsibull_docs-2.9.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs-2.8.0/PKG-INFO` & `antsibull_docs-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: antsibull-docs
-Version: 2.8.0
+Version: 2.9.0
 Summary: Tools for building Ansible documentation
 Project-URL: Documentation, https://ansible.readthedocs.io/projects/antsibull-docs/
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-docs/issues
 Project-URL: Changelog, https://github.com/ansible-community/antsibull-docs/tree/main/CHANGELOG.md
 Author-email: Toshio Kuratomi <a.badger@gmail.com>, Felix Fontein <felix@fontein.de>
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: aiohttp>=3.0.0
 Requires-Dist: ansible-pygments
-Requires-Dist: antsibull-core<=3.0.0a1.post0,>=2.1.0
+Requires-Dist: antsibull-core<4.0.0,>=2.1.0
 Requires-Dist: antsibull-docs-parser<2.0.0,>=1.0.0
 Requires-Dist: asyncio-pool
 Requires-Dist: docutils
 Requires-Dist: jinja2>=3.0
 Requires-Dist: packaging>=20.0
 Requires-Dist: pydantic<3.0.0,>=1.0.0
 Requires-Dist: pyyaml
@@ -70,14 +70,15 @@
 <!--
 Copyright (c) Ansible Project
 GNU General Public License v3.0+ (see LICENSES/GPL-3.0-or-later.txt or https://www.gnu.org/licenses/gpl-3.0.txt)
 SPDX-License-Identifier: GPL-3.0-or-later
 -->
 
 # antsibull-docs -- Ansible Documentation Build Scripts
+[![Discuss on Matrix at #antsibull:ansible.com](https://img.shields.io/matrix/antsibull:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23antsibull:ansible.com&logo=matrix)](https://matrix.to/#/#antsibull:ansible.com)
 [![Discuss on Matrix at #docs:ansible.com](https://img.shields.io/matrix/docs:ansible.com.svg?server_fqdn=ansible-accounts.ems.host&label=Discuss%20on%20Matrix%20at%20%23docs:ansible.com&logo=matrix)](https://matrix.to/#/#docs:ansible.com)
 [![Nox badge](https://github.com/ansible-community/antsibull-docs/actions/workflows/nox.yml/badge.svg)](https://github.com/ansible-community/antsibull-docs/actions/workflows/nox.yml)
 [![Build docs testing badge](https://github.com/ansible-community/antsibull-docs/workflows/antsibull-docs%20tests/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-docs/actions?query=workflow%3A%22antsibull-docs+tests%22+branch%3Amain)
 [![Build CSS testing badge](https://github.com/ansible-community/antsibull-docs/workflows/Build%20CSS/badge.svg?event=push&branch=main)](https://github.com/ansible-community/antsibull-docs/actions?query=workflow%3A%22Build+CSS%22+branch%3Amain)
 [![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-docs)](https://codecov.io/gh/ansible-community/antsibull-docs)
 
 Tooling for building Ansible documentation. This is mainly the `antsibull-docs` command and the [Sphinx extension](https://www.sphinx-doc.org/en/master/), ``sphinx_antsibull_ext``. Please check out the [documentation](https://ansible.readthedocs.io/projects/antsibull-docs/) for more information.
```

