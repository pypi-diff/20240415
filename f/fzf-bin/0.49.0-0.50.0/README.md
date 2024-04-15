# Comparing `tmp/fzf_bin-0.49.0.tar.gz` & `tmp/fzf_bin-0.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fzf_bin-0.49.0.tar", last modified: Fri Apr  5 07:24:44 2024, max compression
+gzip compressed data, was "fzf_bin-0.50.0.tar", last modified: Mon Apr 15 15:21:04 2024, max compression
```

## Comparing `fzf_bin-0.49.0.tar` & `fzf_bin-0.50.0.tar`

### file list

```diff
@@ -1,109 +1,116 @@
--rw-r--r--   0        0        0     1074 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/LICENSE
--rw-r--r--   0        0        0      469 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/README.md
--rw-r--r--   0        0        0       35 2024-04-05 07:23:28.346023 fzf_bin-0.49.0/fzf/.git
--rw-r--r--   0        0        0       17 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/FUNDING.yml
--rw-r--r--   0        0        0     1031 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
--rw-r--r--   0        0        0      209 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/dependabot.yml
--rw-r--r--   0        0        0     1111 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      296 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/depsreview.yaml
--rw-r--r--   0        0        0     1119 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/linux.yml
--rw-r--r--   0        0        0     1001 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/macos.yml
--rw-r--r--   0        0        0      555 2024-04-05 07:23:28.354023 fzf_bin-0.49.0/fzf/.github/workflows/sponsors.yml
--rw-r--r--   0        0        0      193 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.github/workflows/typos.yml
--rw-r--r--   0        0        0      382 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.github/workflows/winget.yml
--rw-r--r--   0        0        0      104 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.gitignore
--rw-r--r--   0        0        0     2431 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.goreleaser.yml
--rw-r--r--   0        0        0      578 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.rubocop.yml
--rw-r--r--   0        0        0       15 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/.tool-versions
--rw-r--r--   0        0        0    28068 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/ADVANCED.md
--rw-r--r--   0        0        0     1455 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/BUILD.md
--rw-r--r--   0        0        0    73299 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/CHANGELOG.md
--rw-r--r--   0        0        0      509 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/Dockerfile
--rw-r--r--   0        0        0     1085 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/LICENSE
--rw-r--r--   0        0        0     5245 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/Makefile
--rw-r--r--   0        0        0    17711 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/README-VIM.md
--rw-r--r--   0        0        0    35700 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/README.md
--rwxr-xr-x   0        0        0     2419 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/bin/fzf-preview.sh
--rwxr-xr-x   0        0        0     7079 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/bin/fzf-tmux
--rw-r--r--   0        0        0    21398 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/doc/fzf.txt
--rw-r--r--   0        0        0      496 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/go.mod
--rw-r--r--   0        0        0     5203 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/go.sum
--rwxr-xr-x   0        0        0    10184 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/install
--rw-r--r--   0        0        0     1881 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/install.ps1
--rw-r--r--   0        0        0     1159 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/main.go
--rw-r--r--   0        0        0     1992 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/man/man1/fzf-tmux.1
--rw-r--r--   0        0        0    50220 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/man/man1/fzf.1
--rw-r--r--   0        0        0    32550 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/plugin/fzf.vim
--rw-r--r--   0        0        0    16178 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/completion.bash
--rw-r--r--   0        0        0    12037 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/completion.zsh
--rw-r--r--   0        0        0     5357 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/key-bindings.bash
--rw-r--r--   0        0        0     5602 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/key-bindings.fish
--rw-r--r--   0        0        0     3879 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/shell/key-bindings.zsh
--rw-r--r--   0        0        0     1085 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/LICENSE
--rw-r--r--   0        0        0     5422 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/actiontype_string.go
--rw-r--r--   0        0        0    25675 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/algo/algo.go
--rw-r--r--   0        0        0     8849 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/algo/algo_test.go
--rw-r--r--   0        0        0    21779 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/algo/normalize.go
--rw-r--r--   0        0        0     9960 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/ansi.go
--rw-r--r--   0        0        0    11138 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/ansi_test.go
--rw-r--r--   0        0        0     1619 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/cache.go
--rw-r--r--   0        0        0      859 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/cache_test.go
--rw-r--r--   0        0        0     1806 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/chunklist.go
--rw-r--r--   0        0        0     1862 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/chunklist_test.go
--rw-r--r--   0        0        0     1704 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/constants.go
--rw-r--r--   0        0        0    10183 2024-04-05 07:23:28.358023 fzf_bin-0.49.0/fzf/src/core.go
--rw-r--r--   0        0        0     2071 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/history.go
--rw-r--r--   0        0        0     1507 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/history_test.go
--rw-r--r--   0        0        0      957 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/item.go
--rw-r--r--   0        0        0      484 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/item_test.go
--rw-r--r--   0        0        0     5411 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/matcher.go
--rw-r--r--   0        0        0     3302 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/merger.go
--rw-r--r--   0        0        0     1989 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/merger_test.go
--rw-r--r--   0        0        0    65018 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/options.go
--rw-r--r--   0        0        0    14755 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/options_test.go
--rw-r--r--   0        0        0    10565 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/pattern.go
--rw-r--r--   0        0        0     8060 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/pattern_test.go
--rw-r--r--   0        0        0      131 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/protector/protector.go
--rw-r--r--   0        0        0      217 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/protector/protector_openbsd.go
--rw-r--r--   0        0        0     5485 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/reader.go
--rw-r--r--   0        0        0     1279 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/reader_test.go
--rw-r--r--   0        0        0     5998 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result.go
--rw-r--r--   0        0        0      338 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result_others.go
--rw-r--r--   0        0        0     6064 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result_test.go
--rw-r--r--   0        0        0      364 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/result_x86.go
--rw-r--r--   0        0        0     6297 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/server.go
--rw-r--r--   0        0        0   113782 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal.go
--rw-r--r--   0        0        0    27879 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal_test.go
--rw-r--r--   0        0        0     1008 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal_unix.go
--rw-r--r--   0        0        0     1088 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/terminal_windows.go
--rw-r--r--   0        0        0     5651 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tokenizer.go
--rw-r--r--   0        0        0     2858 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tokenizer_test.go
--rw-r--r--   0        0        0     1794 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/dummy.go
--rw-r--r--   0        0        0    24069 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/light.go
--rw-r--r--   0        0        0     2508 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/light_unix.go
--rw-r--r--   0        0        0     4777 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/light_windows.go
--rw-r--r--   0        0        0    18498 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tcell.go
--rw-r--r--   0        0        0    17341 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tcell_test.go
--rw-r--r--   0        0        0      908 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/ttyname_unix.go
--rw-r--r--   0        0        0      164 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/ttyname_windows.go
--rw-r--r--   0        0        0    20523 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tui.go
--rw-r--r--   0        0        0      399 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/tui/tui_test.go
--rw-r--r--   0        0        0      748 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/atomicbool.go
--rw-r--r--   0        0        0      301 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/atomicbool_test.go
--rw-r--r--   0        0        0     4284 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/chars.go
--rw-r--r--   0        0        0      981 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/chars_test.go
--rw-r--r--   0        0        0     1976 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/eventbox.go
--rw-r--r--   0        0        0      899 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/eventbox_test.go
--rw-r--r--   0        0        0      185 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/slab.go
--rw-r--r--   0        0        0     3485 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util.go
--rw-r--r--   0        0        0     4194 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util_test.go
--rw-r--r--   0        0        0     1199 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util_unix.go
--rw-r--r--   0        0        0     2219 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/src/util/util_windows.go
--rw-r--r--   0        0        0     5860 2024-04-05 07:23:28.362023 fzf_bin-0.49.0/fzf/test/fzf.vader
--rwxr-xr-x   0        0        0   125876 2024-04-05 07:23:28.366023 fzf_bin-0.49.0/fzf/test/test_go.rb
--rw-r--r--   0        0        0      216 2024-04-05 07:23:28.366023 fzf_bin-0.49.0/fzf/typos.toml
--rwxr-xr-x   0        0        0     2520 2024-04-05 07:23:28.366023 fzf_bin-0.49.0/fzf/uninstall
--rw-r--r--   0        0        0        0 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/fzf_bin/__init__.py
--rw-r--r--   0        0        0     1392 2024-04-05 07:23:26.410044 fzf_bin-0.49.0/pdm_build.py
--rw-r--r--   0        0        0     1073 2024-04-05 07:24:44.009291 fzf_bin-0.49.0/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/LICENSE
+-rw-r--r--   0        0        0      469 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/README.md
+-rw-r--r--   0        0        0       35 2024-04-15 15:19:49.485752 fzf_bin-0.50.0/fzf/.git
+-rw-r--r--   0        0        0       17 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1162 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml
+-rw-r--r--   0        0        0      209 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/dependabot.yml
+-rw-r--r--   0        0        0     1111 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      296 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/depsreview.yaml
+-rw-r--r--   0        0        0     1119 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/linux.yml
+-rw-r--r--   0        0        0     1001 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/macos.yml
+-rw-r--r--   0        0        0      555 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/sponsors.yml
+-rw-r--r--   0        0        0      193 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/typos.yml
+-rw-r--r--   0        0        0      382 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.github/workflows/winget.yml
+-rw-r--r--   0        0        0      104 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.gitignore
+-rw-r--r--   0        0        0     2431 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.goreleaser.yml
+-rw-r--r--   0        0        0      578 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.rubocop.yml
+-rw-r--r--   0        0        0       15 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/.tool-versions
+-rw-r--r--   0        0        0    28068 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/ADVANCED.md
+-rw-r--r--   0        0        0     1718 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/BUILD.md
+-rw-r--r--   0        0        0    74695 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/CHANGELOG.md
+-rw-r--r--   0        0        0      509 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/Dockerfile
+-rw-r--r--   0        0        0     1085 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/LICENSE
+-rw-r--r--   0        0        0     5275 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/Makefile
+-rw-r--r--   0        0        0    17711 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/README-VIM.md
+-rw-r--r--   0        0        0    35715 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/README.md
+-rwxr-xr-x   0        0        0     2419 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/bin/fzf-preview.sh
+-rwxr-xr-x   0        0        0     7079 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/bin/fzf-tmux
+-rw-r--r--   0        0        0    21398 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/doc/fzf.txt
+-rw-r--r--   0        0        0      496 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/go.mod
+-rw-r--r--   0        0        0     5203 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/go.sum
+-rwxr-xr-x   0        0        0    10184 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/install
+-rw-r--r--   0        0        0     1881 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/install.ps1
+-rw-r--r--   0        0        0     1159 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/main.go
+-rw-r--r--   0        0        0     3630 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/main_test.go
+-rw-r--r--   0        0        0     1992 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/man/man1/fzf-tmux.1
+-rw-r--r--   0        0        0    50569 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/man/man1/fzf.1
+-rw-r--r--   0        0        0    32550 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/plugin/fzf.vim
+-rw-r--r--   0        0        0    16179 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/completion.bash
+-rw-r--r--   0        0        0    12038 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/completion.zsh
+-rw-r--r--   0        0        0     5358 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/key-bindings.bash
+-rw-r--r--   0        0        0     5602 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/key-bindings.fish
+-rw-r--r--   0        0        0     3880 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/shell/key-bindings.zsh
+-rw-r--r--   0        0        0     1085 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/LICENSE
+-rw-r--r--   0        0        0     5422 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/actiontype_string.go
+-rw-r--r--   0        0        0    26654 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/algo/algo.go
+-rw-r--r--   0        0        0     8883 2024-04-15 15:19:49.497753 fzf_bin-0.50.0/fzf/src/algo/algo_test.go
+-rw-r--r--   0        0        0    21779 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/algo/normalize.go
+-rw-r--r--   0        0        0     9960 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/ansi.go
+-rw-r--r--   0        0        0    11138 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/ansi_test.go
+-rw-r--r--   0        0        0     1619 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/cache.go
+-rw-r--r--   0        0        0      859 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/cache_test.go
+-rw-r--r--   0        0        0     1806 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/chunklist.go
+-rw-r--r--   0        0        0     1862 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/chunklist_test.go
+-rw-r--r--   0        0        0     1704 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/constants.go
+-rw-r--r--   0        0        0    10292 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/core.go
+-rw-r--r--   0        0        0     2071 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/history.go
+-rw-r--r--   0        0        0     1507 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/history_test.go
+-rw-r--r--   0        0        0      957 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/item.go
+-rw-r--r--   0        0        0      484 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/item_test.go
+-rw-r--r--   0        0        0     5411 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/matcher.go
+-rw-r--r--   0        0        0     3302 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/merger.go
+-rw-r--r--   0        0        0     1989 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/merger_test.go
+-rw-r--r--   0        0        0    65745 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options.go
+-rw-r--r--   0        0        0      307 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_no_pprof.go
+-rw-r--r--   0        0        0     1628 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_pprof.go
+-rw-r--r--   0        0        0     2069 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_pprof_test.go
+-rw-r--r--   0        0        0    14787 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/options_test.go
+-rw-r--r--   0        0        0    10565 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/pattern.go
+-rw-r--r--   0        0        0     8060 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/pattern_test.go
+-rw-r--r--   0        0        0      131 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/protector/protector.go
+-rw-r--r--   0        0        0      217 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/protector/protector_openbsd.go
+-rw-r--r--   0        0        0     5847 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/reader.go
+-rw-r--r--   0        0        0     1279 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/reader_test.go
+-rw-r--r--   0        0        0     5998 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result.go
+-rw-r--r--   0        0        0      338 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result_others.go
+-rw-r--r--   0        0        0     6064 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result_test.go
+-rw-r--r--   0        0        0      364 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/result_x86.go
+-rw-r--r--   0        0        0     6297 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/server.go
+-rw-r--r--   0        0        0   114080 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal.go
+-rw-r--r--   0        0        0    27879 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal_test.go
+-rw-r--r--   0        0        0     1008 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal_unix.go
+-rw-r--r--   0        0        0     1088 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/terminal_windows.go
+-rw-r--r--   0        0        0     5651 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tokenizer.go
+-rw-r--r--   0        0        0     2858 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tokenizer_test.go
+-rw-r--r--   0        0        0     1794 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/dummy.go
+-rw-r--r--   0        0        0     3467 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/eventtype_string.go
+-rw-r--r--   0        0        0    24618 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/light.go
+-rw-r--r--   0        0        0     2510 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/light_unix.go
+-rw-r--r--   0        0        0     4777 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/light_windows.go
+-rw-r--r--   0        0        0    18570 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tcell.go
+-rw-r--r--   0        0        0    17392 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tcell_test.go
+-rw-r--r--   0        0        0      908 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/ttyname_unix.go
+-rw-r--r--   0        0        0      164 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/ttyname_windows.go
+-rw-r--r--   0        0        0    21117 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tui.go
+-rw-r--r--   0        0        0      399 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/tui/tui_test.go
+-rw-r--r--   0        0        0      850 2024-04-15 15:19:49.501752 fzf_bin-0.50.0/fzf/src/util/atexit.go
+-rw-r--r--   0        0        0      452 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/atexit_test.go
+-rw-r--r--   0        0        0      748 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/atomicbool.go
+-rw-r--r--   0        0        0      301 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/atomicbool_test.go
+-rw-r--r--   0        0        0     4308 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/chars.go
+-rw-r--r--   0        0        0      981 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/chars_test.go
+-rw-r--r--   0        0        0     1976 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/eventbox.go
+-rw-r--r--   0        0        0      899 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/eventbox_test.go
+-rw-r--r--   0        0        0      185 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/slab.go
+-rw-r--r--   0        0        0     3733 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util.go
+-rw-r--r--   0        0        0     4194 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util_test.go
+-rw-r--r--   0        0        0     1199 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util_unix.go
+-rw-r--r--   0        0        0     2219 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/src/util/util_windows.go
+-rw-r--r--   0        0        0     5860 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/test/fzf.vader
+-rwxr-xr-x   0        0        0   126533 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/test/test_go.rb
+-rw-r--r--   0        0        0      216 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/typos.toml
+-rwxr-xr-x   0        0        0     2520 2024-04-15 15:19:49.505752 fzf_bin-0.50.0/fzf/uninstall
+-rw-r--r--   0        0        0        0 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/fzf_bin/__init__.py
+-rw-r--r--   0        0        0     1392 2024-04-15 15:19:48.541748 fzf_bin-0.50.0/pdm_build.py
+-rw-r--r--   0        0        0     1073 2024-04-15 15:21:04.710130 fzf_bin-0.50.0/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 fzf_bin-0.50.0/PKG-INFO
```

### Comparing `fzf_bin-0.49.0/LICENSE` & `fzf_bin-0.50.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml` & `fzf_bin-0.50.0/fzf/.github/ISSUE_TEMPLATE/issue_template.yml`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     attributes:
       label: Checklist
       options:
         - label: I have read through the manual page (`man fzf`)
           required: true
         - label: I have searched through the existing issues
           required: true
+        - label: For bug reports, I have checked if the bug is reproducible in the latest version of fzf
+          required: false
 
   - type: input
     attributes:
       label: Output of `fzf --version`
       placeholder: e.g. 0.48.1 (d579e33)
     validations:
       required: true
```

### Comparing `fzf_bin-0.49.0/fzf/.github/workflows/codeql-analysis.yml` & `fzf_bin-0.50.0/fzf/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/.github/workflows/linux.yml` & `fzf_bin-0.50.0/fzf/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/.github/workflows/macos.yml` & `fzf_bin-0.50.0/fzf/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/.github/workflows/sponsors.yml` & `fzf_bin-0.50.0/fzf/.github/workflows/sponsors.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/.goreleaser.yml` & `fzf_bin-0.50.0/fzf/.goreleaser.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/.rubocop.yml` & `fzf_bin-0.50.0/fzf/.rubocop.yml`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/ADVANCED.md` & `fzf_bin-0.50.0/fzf/ADVANCED.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/BUILD.md` & `fzf_bin-0.50.0/fzf/BUILD.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,31 @@
 # Build fzf binaries and archives for all platforms using goreleaser
 make build
 
 # Publish GitHub release
 make release
 ```
 
-> :warning: Makefile uses git commands to determine the version and the
-> revision information for `fzf --version`. So if you're building fzf from an
+> [!WARNING]
+> Makefile uses git commands to determine the version and the revision
+> information for `fzf --version`. So if you're building fzf from an
 > environment where its git information is not available, you have to manually
 > set `$FZF_VERSION` and `$FZF_REVISION`.
 >
 > e.g. `FZF_VERSION=0.24.0 FZF_REVISION=tarball make`
 
+> [!TIP]
+> To build fzf with profiling options enabled, set `TAGS=pprof`
+>
+> ```sh
+> TAGS=pprof make clean install
+> fzf --profile-cpu /tmp/cpu.pprof --profile-mem /tmp/mem.pprof \
+>     --profile-block /tmp/block.pprof --profile-mutex /tmp/mutex.pprof
+> ```
+
 Third-party libraries used
 --------------------------
 
 - [rivo/uniseg](https://github.com/rivo/uniseg)
     - Licensed under [MIT](https://raw.githubusercontent.com/rivo/uniseg/master/LICENSE.txt)
 - [mattn/go-shellwords](https://github.com/mattn/go-shellwords)
     - Licensed under [MIT](http://mattn.mit-license.org)
```

### Comparing `fzf_bin-0.49.0/fzf/CHANGELOG.md` & `fzf_bin-0.50.0/fzf/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,47 @@
 CHANGELOG
 =========
 
+0.50.0
+------
+- Search performance optimization. You can observe 50%+ improvement in some scenarios.
+  ```
+  $ rg --line-number --no-heading --smart-case . > $DATA
+
+  $ wc < $DATA
+   5520118 26862362 897487793
+
+  $ hyperfine -w 1 -L bin fzf-0.49.0,fzf-7ce6452,fzf-a5447b8,fzf '{bin} --filter "///" < $DATA | head -30'
+  Summary
+    fzf --filter "///" < $DATA | head -30 ran
+      1.16 ± 0.03 times faster than fzf-a5447b8 --filter "///" < $DATA | head -30
+      1.23 ± 0.03 times faster than fzf-7ce6452 --filter "///" < $DATA | head -30
+      1.52 ± 0.03 times faster than fzf-0.49.0 --filter "///" < $DATA | head -30
+  ```
+- Added `jump` and `jump-cancel` events that are triggered when leaving `jump` mode
+  ```sh
+  # Default behavior
+  fzf --bind space:jump
+
+  # Same as jump-accept action
+  fzf --bind space:jump,jump:accept
+
+  # Accept on jump, abort on cancel
+  fzf --bind space:jump,jump:accept,jump-cancel:abort
+
+  # Change header on jump-cancel
+  fzf --bind 'space:change-header(Type jump label)+jump,jump-cancel:change-header:Jump cancelled'
+  ```
+- Added a new environment variable `$FZF_KEY` exported to the child processes. It's the name of the last key pressed.
+  ```sh
+  fzf --bind 'space:jump,jump:accept,jump-cancel:transform:[[ $FZF_KEY =~ ctrl-c ]] && echo abort'
+  ```
+- fzf can be built with profiling options. See [BUILD.md](BUILD.md) for more information.
+- Bug fixes
+
 0.49.0
 ------
 - Ingestion performance improved by around 40% (more or less depending on options)
 - `--info=hidden` and `--info=inline-right` will no longer hide the horizontal separator by default. This gives you more flexibility in customizing the layout.
     ```sh
     fzf --border --info=inline-right
     fzf --border --info=inline-right --separator ═
```

### Comparing `fzf_bin-0.49.0/fzf/LICENSE` & `fzf_bin-0.50.0/fzf/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/Makefile` & `fzf_bin-0.50.0/fzf/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 endif
 
 all: target/$(BINARY)
 
 test: $(SOURCES)
 	[ -z "$$(gofmt -s -d src)" ] || (gofmt -s -d src; exit 1)
 	SHELL=/bin/sh GOOS= $(GO) test -v -tags "$(TAGS)" \
+				github.com/junegunn/fzf \
 				github.com/junegunn/fzf/src \
 				github.com/junegunn/fzf/src/algo \
 				github.com/junegunn/fzf/src/tui \
 				github.com/junegunn/fzf/src/util
 
 bench:
 	cd src && SHELL=/bin/sh GOOS= $(GO) test -v -tags "$(TAGS)" -run=Bench -bench=. -benchmem
```

### Comparing `fzf_bin-0.49.0/fzf/README-VIM.md` & `fzf_bin-0.50.0/fzf/README-VIM.md`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/README.md` & `fzf_bin-0.50.0/fzf/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Sponsors ❤️
 -----------
 
 I would like to thank all the sponsors of this project who make it possible for me to continue to improve fzf.
 
 If you'd like to sponsor this project, please visit https://github.com/sponsors/junegunn.
 
-<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/faruzzy"><img src="https://github.com/faruzzy.png" width="60px" alt="Roland" /></a><a href="https://github.com/mrhenry"><img src="https://github.com/mrhenry.png" width="60px" alt="Mr. Henry" /></a><a href="https://github.com/mauricelam"><img src="https://github.com/mauricelam.png" width="60px" alt="Maurice Lam" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><!-- sponsors -->
+<!-- sponsors --><a href="https://github.com/miyanokomiya"><img src="https://github.com/miyanokomiya.png" width="60px" alt="miyanokomiya" /></a><a href="https://github.com/jonhoo"><img src="https://github.com/jonhoo.png" width="60px" alt="Jon Gjengset" /></a><a href="https://github.com/AceofSpades5757"><img src="https://github.com/AceofSpades5757.png" width="60px" alt="Kyle L. Davis" /></a><a href="https://github.com/Frederick888"><img src="https://github.com/Frederick888.png" width="60px" alt="Frederick Zhang" /></a><a href="https://github.com/moritzdietz"><img src="https://github.com/moritzdietz.png" width="60px" alt="Moritz Dietz" /></a><a href="https://github.com/mikker"><img src="https://github.com/mikker.png" width="60px" alt="Mikkel Malmberg" /></a><a href="https://github.com/pldubouilh"><img src="https://github.com/pldubouilh.png" width="60px" alt="Pierre Dubouilh" /></a><a href="https://github.com/rcorre"><img src="https://github.com/rcorre.png" width="60px" alt="Ryan Roden-Corrent" /></a><a href="https://github.com/blissdev"><img src="https://github.com/blissdev.png" width="60px" alt="Jordan Arentsen" /></a><a href="https://github.com/mislav"><img src="https://github.com/mislav.png" width="60px" alt="Mislav Marohnić" /></a><a href="https://github.com/aexvir"><img src="https://github.com/aexvir.png" width="60px" alt="Alex Viscreanu" /></a><a href="https://github.com/dbalatero"><img src="https://github.com/dbalatero.png" width="60px" alt="David Balatero" /></a><a href="https://github.com/comatory"><img src="https://github.com/comatory.png" width="60px" alt="Ondrej Synacek" /></a><a href="https://github.com/moobar"><img src="https://github.com/moobar.png" width="60px" alt="" /></a><a href="https://github.com/majjoha"><img src="https://github.com/majjoha.png" width="60px" alt="Mathias Jean Johansen" /></a><a href="https://github.com/benelan"><img src="https://github.com/benelan.png" width="60px" alt="Ben Elan" /></a><a href="https://github.com/pawelduda"><img src="https://github.com/pawelduda.png" width="60px" alt="Paweł Duda" /></a><a href="https://github.com/slezica"><img src="https://github.com/slezica.png" width="60px" alt="Santiago Lezica" /></a><a href="https://github.com/pbwn"><img src="https://github.com/pbwn.png" width="60px" alt="" /></a><a href="https://github.com/timgluz"><img src="https://github.com/timgluz.png" width="60px" alt="Timo Sulg" /></a><a href="https://github.com/pyrho"><img src="https://github.com/pyrho.png" width="60px" alt="Damien Rajon" /></a><a href="https://github.com/ArtBIT"><img src="https://github.com/ArtBIT.png" width="60px" alt="ArtBIT" /></a><a href="https://github.com/da-moon"><img src="https://github.com/da-moon.png" width="60px" alt="" /></a><a href="https://github.com/hovissimo"><img src="https://github.com/hovissimo.png" width="60px" alt="Hovis" /></a><a href="https://github.com/dariusjonda"><img src="https://github.com/dariusjonda.png" width="60px" alt="Darius Jonda" /></a><a href="https://github.com/cristiand391"><img src="https://github.com/cristiand391.png" width="60px" alt="Cristian Dominguez" /></a><a href="https://github.com/eliangcs"><img src="https://github.com/eliangcs.png" width="60px" alt="Chang-Hung Liang" /></a><a href="https://github.com/asphaltbuffet"><img src="https://github.com/asphaltbuffet.png" width="60px" alt="Ben Lechlitner" /></a><a href="https://github.com/yash1th"><img src="https://github.com/yash1th.png" width="60px" alt="yash" /></a><a href="https://github.com/looshch"><img src="https://github.com/looshch.png" width="60px" alt="george looshch" /></a><a href="https://github.com/kg8m"><img src="https://github.com/kg8m.png" width="60px" alt="Takumi KAGIYAMA" /></a><a href="https://github.com/polm"><img src="https://github.com/polm.png" width="60px" alt="Paul O'Leary McCann" /></a><a href="https://github.com/rbeeger"><img src="https://github.com/rbeeger.png" width="60px" alt="Robert Beeger" /></a><a href="https://github.com/veebch"><img src="https://github.com/veebch.png" width="60px" alt="VEEB Projects" /></a><a href="https://github.com/khuedoan"><img src="https://github.com/khuedoan.png" width="60px" alt="Khue Doan" /></a><a href="https://github.com/yowayb"><img src="https://github.com/yowayb.png" width="60px" alt="Yoway Buorn" /></a><a href="https://github.com/scalisi"><img src="https://github.com/scalisi.png" width="60px" alt="Josh Scalisi" /></a><a href="https://github.com/alecbcs"><img src="https://github.com/alecbcs.png" width="60px" alt="Alec Scott" /></a><a href="https://github.com/thnxdev"><img src="https://github.com/thnxdev.png" width="60px" alt="thanks.dev" /></a><a href="https://github.com/artursapek"><img src="https://github.com/artursapek.png" width="60px" alt="Artur Sapek" /></a><a href="https://github.com/ramnes"><img src="https://github.com/ramnes.png" width="60px" alt="Guillaume Gelin" /></a><a href="https://github.com/jyc"><img src="https://github.com/jyc.png" width="60px" alt="" /></a><a href="https://github.com/mrcnski"><img src="https://github.com/mrcnski.png" width="60px" alt="Marcin S." /></a><a href="https://github.com/roblevy"><img src="https://github.com/roblevy.png" width="60px" alt="Rob Levy" /></a><a href="https://github.com/glozow"><img src="https://github.com/glozow.png" width="60px" alt="Gloria Zhao" /></a><a href="https://github.com/wjt"><img src="https://github.com/wjt.png" width="60px" alt="Will Thompson" /></a><a href="https://github.com/mauricelam"><img src="https://github.com/mauricelam.png" width="60px" alt="Maurice Lam" /></a><a href="https://github.com/toupeira"><img src="https://github.com/toupeira.png" width="60px" alt="Markus Koller" /></a><a href="https://github.com/rkpatel33"><img src="https://github.com/rkpatel33.png" width="60px" alt="" /></a><a href="https://github.com/jamesob"><img src="https://github.com/jamesob.png" width="60px" alt="James O'Beirne" /></a><a href="https://github.com/joshuatz"><img src="https://github.com/joshuatz.png" width="60px" alt="Joshua Tzucker" /></a><!-- sponsors -->
 
 Table of Contents
 -----------------
 
 <!-- vim-markdown-toc GFM -->
 
 * [Installation](#installation)
```

#### html2text {}

```diff
@@ -22,16 +22,16 @@
 _[_M_o_r_i_t_z_ _D_i_e_t_z_]_[_M_i_k_k_e_l_ _M_a_l_m_b_e_r_g_]_[_P_i_e_r_r_e_ _D_u_b_o_u_i_l_h_]_[_R_y_a_n_ _R_o_d_e_n_-_C_o_r_r_e_n_t_]_[_J_o_r_d_a_n
 _A_r_e_n_t_s_e_n_]_[_M_i_s_l_a_v_ _M_a_r_o_h_n_i_Ä__]_[_A_l_e_x_ _V_i_s_c_r_e_a_n_u_]_[_D_a_v_i_d_ _B_a_l_a_t_e_r_o_]_[_O_n_d_r_e_j_ _S_y_n_a_c_e_k_]
 _[_M_a_t_h_i_a_s_ _J_e_a_n_ _J_o_h_a_n_s_e_n_]_[_B_e_n_ _E_l_a_n_]_[_P_a_w_e_Å__ _D_u_d_a_]_[_S_a_n_t_i_a_g_o_ _L_e_z_i_c_a_]_[_T_i_m_o_ _S_u_l_g_]
 _[_D_a_m_i_e_n_ _R_a_j_o_n_]_[_A_r_t_B_I_T_]_[_H_o_v_i_s_]_[_D_a_r_i_u_s_ _J_o_n_d_a_]_[_C_r_i_s_t_i_a_n_ _D_o_m_i_n_g_u_e_z_]_[_C_h_a_n_g_-_H_u_n_g
 _L_i_a_n_g_]_[_B_e_n_ _L_e_c_h_l_i_t_n_e_r_]_[_y_a_s_h_]_[_g_e_o_r_g_e_ _l_o_o_s_h_c_h_]_[_T_a_k_u_m_i_ _K_A_G_I_Y_A_M_A_]_[_P_a_u_l_ _O_'_L_e_a_r_y
 _M_c_C_a_n_n_]_[_R_o_b_e_r_t_ _B_e_e_g_e_r_]_[_V_E_E_B_ _P_r_o_j_e_c_t_s_]_[_K_h_u_e_ _D_o_a_n_]_[_Y_o_w_a_y_ _B_u_o_r_n_]_[_J_o_s_h_ _S_c_a_l_i_s_i_]
 _[_A_l_e_c_ _S_c_o_t_t_]_[_t_h_a_n_k_s_._d_e_v_]_[_A_r_t_u_r_ _S_a_p_e_k_]_[_G_u_i_l_l_a_u_m_e_ _G_e_l_i_n_]_[_M_a_r_c_i_n_ _S_._]_[_R_o_b_ _L_e_v_y_]
-_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_R_o_l_a_n_d_]_[_M_r_._ _H_e_n_r_y_]_[_M_a_u_r_i_c_e_ _L_a_m_]_[_M_a_r_k_u_s
-_K_o_l_l_e_r_]Table of Contents ----------------- * [Installation](#installation) *
+_[_G_l_o_r_i_a_ _Z_h_a_o_]_[_W_i_l_l_ _T_h_o_m_p_s_o_n_]_[_M_a_u_r_i_c_e_ _L_a_m_]_[_M_a_r_k_u_s_ _K_o_l_l_e_r_]_[_J_a_m_e_s_ _O_'_B_e_i_r_n_e_]_[_J_o_s_h_u_a
+_T_z_u_c_k_e_r_]Table of Contents ----------------- * [Installation](#installation) *
 [Using Homebrew](#using-homebrew) * [Using git](#using-git) * [Using Linux
 package managers](#using-linux-package-managers) * [Windows](#windows) *
 [Setting up shell integration](#setting-up-shell-integration) * [As Vim plugin]
 (#as-vim-plugin) * [Upgrading fzf](#upgrading-fzf) * [Building fzf](#building-
 fzf) * [Usage](#usage) * [Using the finder](#using-the-finder) * [Layout]
 (#layout) * [Search syntax](#search-syntax) * [Environment variables]
 (#environment-variables) * [Options](#options) * [Demo](#demo) * [Examples]
```

### Comparing `fzf_bin-0.49.0/fzf/bin/fzf-preview.sh` & `fzf_bin-0.50.0/fzf/bin/fzf-preview.sh`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/bin/fzf-tmux` & `fzf_bin-0.50.0/fzf/bin/fzf-tmux`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/doc/fzf.txt` & `fzf_bin-0.50.0/fzf/doc/fzf.txt`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/go.sum` & `fzf_bin-0.50.0/fzf/go.sum`

 * *Files 6% similar despite different names*

```diff
@@ -32,22 +32,22 @@
 golang.org/x/sys v0.0.0-20201119102817-f84b799fce68/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20210615035016-665e8c7367d1/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220520151302-bc2c85ada10a/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220722155257-8c9f86f7a55f/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.5.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.6.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.17.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
-golang.org/x/sys v0.18.0 h1:DBdB3niSjOA/O0blCZBqDefyWNYveAYMNF1Wum0DYQ4=
-golang.org/x/sys v0.18.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
+golang.org/x/sys v0.19.0 h1:q5f1RH2jigJ1MoAWp2KTp3gm5zAGFUTarQZ5U386+4o=
+golang.org/x/sys v0.19.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
 golang.org/x/term v0.0.0-20201126162022-7de9c90e9dd1/go.mod h1:bj7SfCRtBDWHUb9snDiAeCFNEtKQo2Wmx5Cou7ajbmo=
 golang.org/x/term v0.0.0-20210927222741-03fcf44c2211/go.mod h1:jbD1KX2456YbFQfuXm/mYQcufACuNUgVhRMnK/tPxf8=
 golang.org/x/term v0.5.0/go.mod h1:jMB1sMXY+tzblOD4FWmEbocvup2/aLOaQEp7JmGp78k=
 golang.org/x/term v0.17.0/go.mod h1:lLRBjIVuehSbZlaOtGMbcMncT+aqLLLmKrsjNrUguwk=
-golang.org/x/term v0.18.0 h1:FcHjZXDMxI8mM3nwhX9HlKop4C0YQvCVCdwYl2wOtE8=
-golang.org/x/term v0.18.0/go.mod h1:ILwASektA3OnRv7amZ1xhE/KTR+u50pbXfZ03+6Nx58=
+golang.org/x/term v0.19.0 h1:+ThwsDv+tYfnJFhF4L8jITxu1tdTWRTZpdsWgEgjL6Q=
+golang.org/x/term v0.19.0/go.mod h1:2CuTdWZ7KHSQwUzKva0cbMg6q2DMI3Mmxp+gKJbskEk=
 golang.org/x/text v0.3.0/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.3/go.mod h1:5Zoc/QRtKVWzQhOtBMvqHzDpF6irO9z98xDceosuGiQ=
 golang.org/x/text v0.3.7/go.mod h1:u+2+/6zg+i71rQMx5EYifcz6MCKuco9NR6JIITiCfzQ=
 golang.org/x/text v0.7.0/go.mod h1:mrYo+phRRbMaCq/xk9113O4dZlRixOauAjOtrjsXDZ8=
 golang.org/x/text v0.14.0 h1:ScX5w1eTa3QqT8oi6+ziP7dTV1S2+ALU0bI+0zXKWiQ=
 golang.org/x/text v0.14.0/go.mod h1:18ZOQIKpY8NJVqYksKHtTdi31H5itFRjB5/qKTNYzSU=
 golang.org/x/tools v0.0.0-20180917221912-90fa682c2a6e/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
```

### Comparing `fzf_bin-0.49.0/fzf/install` & `fzf_bin-0.50.0/fzf/install`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 
 set -u
 
-version=0.49.0
+version=0.50.0
 auto_completion=
 key_bindings=
 update_config=2
 shells="bash zsh fish"
 prefix='~/.fzf'
 prefix_expand=~/.fzf
 fish_dir=${XDG_CONFIG_HOME:-$HOME/.config}/fish
```

### Comparing `fzf_bin-0.49.0/fzf/install.ps1` & `fzf_bin-0.50.0/fzf/install.ps1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-$version="0.49.0"
+$version="0.50.0"
 
 $fzf_base=Split-Path -Parent $MyInvocation.MyCommand.Definition
 
 function check_binary () {
   Write-Host "  - Checking fzf executable ... " -NoNewline
   $output=cmd /c $fzf_base\bin\fzf.exe --version 2>&1
   if (-not $?) {
```

### Comparing `fzf_bin-0.49.0/fzf/main.go` & `fzf_bin-0.50.0/fzf/main.go`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	"fmt"
 	"strings"
 
 	fzf "github.com/junegunn/fzf/src"
 	"github.com/junegunn/fzf/src/protector"
 )
 
-var version string = "0.49"
+var version string = "0.50"
 var revision string = "devel"
 
 //go:embed shell/key-bindings.bash
 var bashKeyBindings []byte
 
 //go:embed shell/completion.bash
 var bashCompletion []byte
```

### Comparing `fzf_bin-0.49.0/fzf/man/man1/fzf-tmux.1` & `fzf_bin-0.50.0/fzf/man/man1/fzf-tmux.1`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf-tmux 1 "Apr 2024" "fzf 0.49.0" "fzf-tmux - open fzf in tmux split pane"
+.TH fzf-tmux 1 "Apr 2024" "fzf 0.50.0" "fzf-tmux - open fzf in tmux split pane"
 
 .SH NAME
 fzf-tmux - open fzf in tmux split pane
 
 .SH SYNOPSIS
 .B fzf-tmux [LAYOUT OPTIONS] [--] [FZF OPTIONS]
```

### Comparing `fzf_bin-0.49.0/fzf/man/man1/fzf.1` & `fzf_bin-0.50.0/fzf/man/man1/fzf.1`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ..
-.TH fzf 1 "Apr 2024" "fzf 0.49.0" "fzf - a command-line fuzzy finder"
+.TH fzf 1 "Apr 2024" "fzf 0.50.0" "fzf - a command-line fuzzy finder"
 
 .SH NAME
 fzf - a command-line fuzzy finder
 
 .SH SYNOPSIS
 fzf [options]
 
@@ -187,15 +187,15 @@
 \fBbackward-word\fR
 .br
 \fBforward-word\fR
 .br
 \fBkill-word\fR
 .TP
 .BI "--jump-labels=" "CHARS"
-Label characters for \fBjump\fR and \fBjump-accept\fR
+Label characters for \fBjump\fR mode.
 .SS Layout
 .TP
 .BI "--height=" "[~]HEIGHT[%]"
 Display fzf window below the cursor with the given height instead of using
 the full screen.
 
 If a negative value is specified, the height is calculated as the terminal
@@ -978,14 +978,16 @@
 .br
 .BR FZF_PREVIEW_LABEL "   Preview label string"
 .br
 .BR FZF_BORDER_LABEL "    Border label string"
 .br
 .BR FZF_ACTION "          The name of the last action performed"
 .br
+.BR FZF_KEY "             The name of the last key pressed"
+.br
 .BR FZF_PORT "            Port number when --listen option is used"
 .br
 
 The following variables are additionally exported to the preview commands.
 
 .BR FZF_PREVIEW_TOP "     Top position of the preview window"
 .br
@@ -1048,51 +1050,51 @@
 .br
 \fIctrl-delete\fR
 .br
 \fIctrl-\\\fR
 .br
 \fIctrl-]\fR
 .br
-\fIctrl-^\fR      (\fIctrl-6\fR)
+\fIctrl-^\fR         (\fIctrl-6\fR)
 .br
-\fIctrl-/\fR      (\fIctrl-_\fR)
+\fIctrl-/\fR         (\fIctrl-_\fR)
 .br
 \fIctrl-alt-[a-z]\fR
 .br
-\fIalt-[*]\fR     (Any case-sensitive single character is allowed)
+\fIalt-[*]\fR        (Any case-sensitive single character is allowed)
 .br
 \fIf[1-12]\fR
 .br
-\fIenter\fR       (\fIreturn\fR \fIctrl-m\fR)
+\fIenter\fR          (\fIreturn\fR \fIctrl-m\fR)
 .br
 \fIspace\fR
 .br
-\fIbspace\fR      (\fIbs\fR)
+\fIbackspace\fR      (\fIbspace\fR \fIbs\fR)
 .br
 \fIalt-up\fR
 .br
 \fIalt-down\fR
 .br
 \fIalt-left\fR
 .br
 \fIalt-right\fR
 .br
 \fIalt-enter\fR
 .br
 \fIalt-space\fR
 .br
-\fIalt-bspace\fR  (\fIalt-bs\fR)
+\fIalt-backspace\fR  (\fIalt-bspace\fR \fIalt-bs\fR)
 .br
 \fItab\fR
 .br
-\fIbtab\fR        (\fIshift-tab\fR)
+\fIshift-tab\fR      (\fIbtab\fR)
 .br
 \fIesc\fR
 .br
-\fIdel\fR
+\fIdelete\fR         (\fIdel\fR)
 .br
 \fIup\fR
 .br
 \fIdown\fR
 .br
 \fIleft\fR
 .br
@@ -1100,17 +1102,17 @@
 .br
 \fIhome\fR
 .br
 \fIend\fR
 .br
 \fIinsert\fR
 .br
-\fIpgup\fR        (\fIpage-up\fR)
+\fIpage-up\fR        (\fIpgup\fR)
 .br
-\fIpgdn\fR        (\fIpage-down\fR)
+\fIpage-down\fR      (\fIpgdn\fR)
 .br
 \fIshift-up\fR
 .br
 \fIshift-down\fR
 .br
 \fIshift-left\fR
 .br
@@ -1156,30 +1158,33 @@
 Triggered only once when fzf finder starts. Since fzf consumes the input stream
 asynchronously, the input list is not available unless you use \fI--sync\fR.
 
 e.g.
      \fB# Move cursor to the last item and select all items
      seq 1000 | fzf --multi --sync --bind start:last+select-all\fR
 .RE
+
 \fIload\fR
 .RS
 Triggered when the input stream is complete and the initial processing of the
 list is complete.
 
 e.g.
      \fB# Change the prompt to "loaded" when the input stream is complete
      (seq 10; sleep 1; seq 11 20) | fzf --prompt 'Loading> ' --bind 'load:change-prompt:Loaded> '\fR
 .RE
+
 \fIresize\fR
 .RS
 Triggered when the terminal size is changed.
 
 e.g.
      \fBfzf --bind 'resize:transform-header:echo Resized: ${FZF_COLUMNS}x${FZF_LINES}'\fR
 .RE
+
 \fIresult\fR
 .RS
 Triggered when the filtering for the current query is complete and the result list is ready.
 
 e.g.
      \fB# Put the cursor on the second item when the query string is empty
      # * Note that you can't use 'change' event in this case because the second position may not be available
@@ -1205,25 +1210,27 @@
      # e.g. lolcat isn't one of the fastest programs, and every cursor movement in
      #      fzf will be noticeably affected by its execution time
      fzf --bind 'focus:transform-preview-label:echo [ {} ] | lolcat -f' --preview 'cat {}'
 
      # Beware not to introduce an infinite loop
      seq 10 | fzf --bind 'focus:up' --cycle\fR
 .RE
+
 \fIone\fR
 .RS
 Triggered when there's only one match. \fBone:accept\fR binding is comparable
 to \fB--select-1\fR option, but the difference is that \fB--select-1\fR is only
 effective before the interactive finder starts but \fBone\fR event is triggered
 by the interactive finder.
 
 e.g.
      \fB# Automatically select the only match
      seq 10 | fzf --bind one:accept\fR
 .RE
+
 \fIzero\fR
 .RS
 Triggered when there's no match. \fBzero:abort\fR binding is comparable to
 \fB--exit-0\fR option, but the difference is that \fB--exit-0\fR is only
 effective before the interactive finder starts but \fBzero\fR event is
 triggered by the interactive finder.
 
@@ -1237,14 +1244,30 @@
 Triggered when the query string is already empty and you try to delete it
 backward.
 
 e.g.
      \fBfzf --bind backward-eof:abort\fR
 .RE
 
+\fIjump\fR
+.RS
+Triggered when successfully jumped to the target item in \fBjump\fR mode.
+
+e.g.
+     \fBfzf --bind space:jump,jump:accept\fR
+.RE
+
+\fIjump-cancel\fR
+.RS
+Triggered when \fBjump\fR mode is cancelled.
+
+e.g.
+     \fBfzf --bind space:jump,jump:accept,jump-cancel:abort\fR
+.RE
+
 .SS AVAILABLE ACTIONS:
 A key or an event can be bound to one or more of the following actions.
 
   \fBACTION:                      DEFAULT BINDINGS (NOTES):
     \fBabort\fR                        \fIctrl-c  ctrl-g  ctrl-q  esc\fR
     \fBaccept\fR                       \fIenter   double-click\fR
     \fBaccept-non-empty\fR             (same as \fBaccept\fR except that it prevents fzf from exiting without selection)
@@ -1279,15 +1302,14 @@
     \fBexecute(...)\fR                 (see below for the details)
     \fBexecute-silent(...)\fR          (see below for the details)
     \fBfirst\fR                        (move to the first match; same as \fBpos(1)\fR)
     \fBforward-char\fR                 \fIctrl-f  right\fR
     \fBforward-word\fR                 \fIalt-f   shift-right\fR
     \fBignore\fR
     \fBjump\fR                         (EasyMotion-like 2-keystroke movement)
-    \fBjump-accept\fR                  (jump and accept)
     \fBkill-line\fR
     \fBkill-word\fR                    \fIalt-d\fR
     \fBlast\fR                         (move to the last match; same as \fBpos(-1)\fR)
     \fBnext-history\fR                 (\fIctrl-n\fR on \fB--history\fR)
     \fBnext-selected\fR                (move to the next selected item)
     \fBpage-down\fR                    \fIpgdn\fR
     \fBpage-up\fR                      \fIpgup\fR
```

### Comparing `fzf_bin-0.49.0/fzf/plugin/fzf.vim` & `fzf_bin-0.50.0/fzf/plugin/fzf.vim`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/shell/completion.bash` & `fzf_bin-0.50.0/fzf/shell/completion.bash`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # /_/   /___/_/ completion.bash
 #
 # - $FZF_TMUX               (default: 0)
 # - $FZF_TMUX_OPTS          (default: empty)
 # - $FZF_COMPLETION_TRIGGER (default: '**')
 # - $FZF_COMPLETION_OPTS    (default: empty)
 
-[[ $- =~ i ]] || return 0
+if [[ $- =~ i ]]; then
 
 
 # To use custom commands instead of find, override _fzf_compgen_{path,dir}
 #
 #   _fzf_compgen_path() {
 #     echo "$1"
 #     command find -L "$1" \
@@ -577,7 +577,9 @@
 }
 
 # Environment variables / Aliases / Hosts / Process
 _fzf_setup_completion 'var'   export unset printenv
 _fzf_setup_completion 'alias' unalias
 _fzf_setup_completion 'host'  telnet
 _fzf_setup_completion 'proc'  kill
+
+fi
```

### Comparing `fzf_bin-0.49.0/fzf/shell/completion.zsh` & `fzf_bin-0.50.0/fzf/shell/completion.zsh`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # /_/   /___/_/ completion.zsh
 #
 # - $FZF_TMUX               (default: 0)
 # - $FZF_TMUX_OPTS          (default: '-d 40%')
 # - $FZF_COMPLETION_TRIGGER (default: '**')
 # - $FZF_COMPLETION_OPTS    (default: empty)
 
-[[ -o interactive ]] || return 0
+if [[ -o interactive ]]; then
 
 
 # Both branches of the following `if` do the same thing -- define
 # __fzf_completion_options such that `eval $__fzf_completion_options` sets
 # all options to the same values they currently have. We'll do just that at
 # the bottom of the file after changing options to what we prefer.
 #
@@ -347,7 +347,9 @@
 bindkey '^I' fzf-completion
 
 } always {
   # Restore the original options.
   eval $__fzf_completion_options
   'unset' '__fzf_completion_options'
 }
+
+fi
```

### Comparing `fzf_bin-0.49.0/fzf/shell/key-bindings.bash` & `fzf_bin-0.50.0/fzf/shell/key-bindings.bash`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # - $FZF_TMUX_OPTS
 # - $FZF_CTRL_T_COMMAND
 # - $FZF_CTRL_T_OPTS
 # - $FZF_CTRL_R_OPTS
 # - $FZF_ALT_C_COMMAND
 # - $FZF_ALT_C_OPTS
 
-[[ $- =~ i ]] || return 0
+if [[ $- =~ i ]]; then
 
 
 # Key bindings
 # ------------
 __fzf_select__() {
   local opts
   opts="--height ${FZF_TMUX_HEIGHT:-40%} --bind=ctrl-z:ignore --reverse --walker=file,dir,follow,hidden --scheme=path ${FZF_DEFAULT_OPTS-} ${FZF_CTRL_T_OPTS-} -m"
@@ -128,7 +128,9 @@
 
 # ALT-C - cd into the selected directory
 if [[ "${FZF_ALT_C_COMMAND-x}" != "" ]]; then
   bind -m emacs-standard '"\ec": " \C-b\C-k \C-u`__fzf_cd__`\e\C-e\er\C-m\C-y\C-h\e \C-y\ey\C-x\C-x\C-d"'
   bind -m vi-command '"\ec": "\C-z\ec\C-z"'
   bind -m vi-insert '"\ec": "\C-z\ec\C-z"'
 fi
+
+fi
```

### Comparing `fzf_bin-0.49.0/fzf/shell/key-bindings.fish` & `fzf_bin-0.50.0/fzf/shell/key-bindings.fish`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/shell/key-bindings.zsh` & `fzf_bin-0.50.0/fzf/shell/key-bindings.zsh`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # - $FZF_TMUX_OPTS
 # - $FZF_CTRL_T_COMMAND
 # - $FZF_CTRL_T_OPTS
 # - $FZF_CTRL_R_OPTS
 # - $FZF_ALT_C_COMMAND
 # - $FZF_ALT_C_OPTS
 
-[[ -o interactive ]] || return 0
+if [[ -o interactive ]]; then
 
 
 # Key bindings
 # ------------
 
 # The code at the top and the bottom of this file is the same as in completion.zsh.
 # Refer to that file for explanation.
@@ -115,7 +115,9 @@
 bindkey -M vicmd '^R' fzf-history-widget
 bindkey -M viins '^R' fzf-history-widget
 
 } always {
   eval $__fzf_key_bindings_options
   'unset' '__fzf_key_bindings_options'
 }
+
+fi
```

### Comparing `fzf_bin-0.49.0/fzf/src/LICENSE` & `fzf_bin-0.50.0/fzf/src/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/actiontype_string.go` & `fzf_bin-0.50.0/fzf/src/actiontype_string.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/algo/algo.go` & `fzf_bin-0.50.0/fzf/src/algo/algo.go`

 * *Files 6% similar despite different names*

```diff
@@ -149,14 +149,20 @@
 	// Extra bonus for word boundary after whitespace character or beginning of the string
 	bonusBoundaryWhite int16 = bonusBoundary + 2
 
 	// Extra bonus for word boundary after slash, colon, semi-colon, and comma
 	bonusBoundaryDelimiter int16 = bonusBoundary + 1
 
 	initialCharClass charClass = charWhite
+
+	// A minor optimization that can give 15%+ performance boost
+	asciiCharClasses [unicode.MaxASCII + 1]charClass
+
+	// A minor optimization that can give yet another 5% performance boost
+	bonusMatrix [charNumber + 1][charNumber + 1]int16
 )
 
 type charClass int
 
 const (
 	charWhite charClass = iota
 	charNonWord
@@ -183,14 +189,35 @@
 		initialCharClass = charDelimiter
 	case "history":
 		bonusBoundaryWhite = bonusBoundary
 		bonusBoundaryDelimiter = bonusBoundary
 	default:
 		return false
 	}
+	for i := 0; i <= unicode.MaxASCII; i++ {
+		char := rune(i)
+		c := charNonWord
+		if char >= 'a' && char <= 'z' {
+			c = charLower
+		} else if char >= 'A' && char <= 'Z' {
+			c = charUpper
+		} else if char >= '0' && char <= '9' {
+			c = charNumber
+		} else if strings.ContainsRune(whiteChars, char) {
+			c = charWhite
+		} else if strings.ContainsRune(delimiterChars, char) {
+			c = charDelimiter
+		}
+		asciiCharClasses[i] = c
+	}
+	for i := 0; i <= int(charNumber); i++ {
+		for j := 0; j <= int(charNumber); j++ {
+			bonusMatrix[i][j] = bonusFor(charClass(i), charClass(j))
+		}
+	}
 	return true
 }
 
 func posArray(withPos bool, len int) *[]int {
 	if withPos {
 		pos := make([]int, 0, len)
 		return &pos
@@ -210,29 +237,14 @@
 	if slab != nil && cap(slab.I32) > offset+size {
 		slice := slab.I32[offset : offset+size]
 		return offset + size, slice
 	}
 	return offset, make([]int32, size)
 }
 
-func charClassOfAscii(char rune) charClass {
-	if char >= 'a' && char <= 'z' {
-		return charLower
-	} else if char >= 'A' && char <= 'Z' {
-		return charUpper
-	} else if char >= '0' && char <= '9' {
-		return charNumber
-	} else if strings.ContainsRune(whiteChars, char) {
-		return charWhite
-	} else if strings.ContainsRune(delimiterChars, char) {
-		return charDelimiter
-	}
-	return charNonWord
-}
-
 func charClassOfNonAscii(char rune) charClass {
 	if unicode.IsLower(char) {
 		return charLower
 	} else if unicode.IsUpper(char) {
 		return charUpper
 	} else if unicode.IsNumber(char) {
 		return charNumber
@@ -244,15 +256,15 @@
 		return charDelimiter
 	}
 	return charNonWord
 }
 
 func charClassOf(char rune) charClass {
 	if char <= unicode.MaxASCII {
-		return charClassOfAscii(char)
+		return asciiCharClasses[char]
 	}
 	return charClassOfNonAscii(char)
 }
 
 func bonusFor(prevClass charClass, class charClass) int16 {
 	if class > charNonWord {
 		switch prevClass {
@@ -283,15 +295,15 @@
 	return 0
 }
 
 func bonusAt(input *util.Chars, idx int) int16 {
 	if idx == 0 {
 		return bonusBoundaryWhite
 	}
-	return bonusFor(charClassOf(input.Get(idx-1)), charClassOf(input.Get(idx)))
+	return bonusMatrix[charClassOf(input.Get(idx-1))][charClassOf(input.Get(idx))]
 }
 
 func normalizeRune(r rune) rune {
 	if r < 0x00C0 || r > 0x2184 {
 		return r
 	}
 
@@ -336,38 +348,53 @@
 		if r >= utf8.RuneSelf {
 			return false
 		}
 	}
 	return true
 }
 
-func asciiFuzzyIndex(input *util.Chars, pattern []rune, caseSensitive bool) int {
+func asciiFuzzyIndex(input *util.Chars, pattern []rune, caseSensitive bool) (int, int) {
 	// Can't determine
 	if !input.IsBytes() {
-		return 0
+		return 0, input.Length()
 	}
 
 	// Not possible
 	if !isAscii(pattern) {
-		return -1
+		return -1, -1
 	}
 
-	firstIdx, idx := 0, 0
+	firstIdx, idx, lastIdx := 0, 0, 0
+	var b byte
 	for pidx := 0; pidx < len(pattern); pidx++ {
-		idx = trySkip(input, caseSensitive, byte(pattern[pidx]), idx)
+		b = byte(pattern[pidx])
+		idx = trySkip(input, caseSensitive, b, idx)
 		if idx < 0 {
-			return -1
+			return -1, -1
 		}
 		if pidx == 0 && idx > 0 {
 			// Step back to find the right bonus point
 			firstIdx = idx - 1
 		}
+		lastIdx = idx
 		idx++
 	}
-	return firstIdx
+
+	// Find the last appearance of the last character of the pattern to limit the search scope
+	bu := b
+	if !caseSensitive && b >= 'a' && b <= 'z' {
+		bu = b - 32
+	}
+	scope := input.Bytes()[lastIdx:]
+	for offset := len(scope) - 1; offset > 0; offset-- {
+		if scope[offset] == b || scope[offset] == bu {
+			return firstIdx, lastIdx + offset + 1
+		}
+	}
+	return firstIdx, lastIdx + 1
 }
 
 func debugV2(T []rune, pattern []rune, F []int32, lastIdx int, H []int16, C []int16) {
 	width := lastIdx - int(F[0]) + 1
 
 	for i, f := range F {
 		I := i * width
@@ -408,108 +435,112 @@
 	// If the input string is too long, consider finding the matching chars in
 	// this phase as well (non-optimal alignment).
 	M := len(pattern)
 	if M == 0 {
 		return Result{0, 0, 0}, posArray(withPos, M)
 	}
 	N := input.Length()
+	if M > N {
+		return Result{-1, -1, 0}, nil
+	}
 
 	// Since O(nm) algorithm can be prohibitively expensive for large input,
 	// we fall back to the greedy algorithm.
 	if slab != nil && N*M > cap(slab.I16) {
 		return FuzzyMatchV1(caseSensitive, normalize, forward, input, pattern, withPos, slab)
 	}
 
 	// Phase 1. Optimized search for ASCII string
-	idx := asciiFuzzyIndex(input, pattern, caseSensitive)
-	if idx < 0 {
+	minIdx, maxIdx := asciiFuzzyIndex(input, pattern, caseSensitive)
+	if minIdx < 0 {
 		return Result{-1, -1, 0}, nil
 	}
+	// fmt.Println(N, maxIdx, idx, maxIdx-idx, input.ToString())
+	N = maxIdx - minIdx
 
 	// Reuse pre-allocated integer slice to avoid unnecessary sweeping of garbages
 	offset16 := 0
 	offset32 := 0
 	offset16, H0 := alloc16(offset16, slab, N)
 	offset16, C0 := alloc16(offset16, slab, N)
 	// Bonus point for each position
 	offset16, B := alloc16(offset16, slab, N)
 	// The first occurrence of each character in the pattern
 	offset32, F := alloc32(offset32, slab, M)
 	// Rune array
 	_, T := alloc32(offset32, slab, N)
-	input.CopyRunes(T)
+	input.CopyRunes(T, minIdx)
 
 	// Phase 2. Calculate bonus for each point
 	maxScore, maxScorePos := int16(0), 0
 	pidx, lastIdx := 0, 0
 	pchar0, pchar, prevH0, prevClass, inGap := pattern[0], pattern[0], int16(0), initialCharClass, false
-	Tsub := T[idx:]
-	H0sub, C0sub, Bsub := H0[idx:][:len(Tsub)], C0[idx:][:len(Tsub)], B[idx:][:len(Tsub)]
-	for off, char := range Tsub {
+	for off, char := range T {
 		var class charClass
 		if char <= unicode.MaxASCII {
-			class = charClassOfAscii(char)
+			class = asciiCharClasses[char]
 			if !caseSensitive && class == charUpper {
 				char += 32
+				T[off] = char
 			}
 		} else {
 			class = charClassOfNonAscii(char)
 			if !caseSensitive && class == charUpper {
 				char = unicode.To(unicode.LowerCase, char)
 			}
 			if normalize {
 				char = normalizeRune(char)
 			}
+			T[off] = char
 		}
 
-		Tsub[off] = char
-		bonus := bonusFor(prevClass, class)
-		Bsub[off] = bonus
+		bonus := bonusMatrix[prevClass][class]
+		B[off] = bonus
 		prevClass = class
 
 		if char == pchar {
 			if pidx < M {
-				F[pidx] = int32(idx + off)
+				F[pidx] = int32(off)
 				pidx++
 				pchar = pattern[util.Min(pidx, M-1)]
 			}
-			lastIdx = idx + off
+			lastIdx = off
 		}
 
 		if char == pchar0 {
 			score := scoreMatch + bonus*bonusFirstCharMultiplier
-			H0sub[off] = score
-			C0sub[off] = 1
+			H0[off] = score
+			C0[off] = 1
 			if M == 1 && (forward && score > maxScore || !forward && score >= maxScore) {
-				maxScore, maxScorePos = score, idx+off
+				maxScore, maxScorePos = score, off
 				if forward && bonus >= bonusBoundary {
 					break
 				}
 			}
 			inGap = false
 		} else {
 			if inGap {
-				H0sub[off] = util.Max16(prevH0+scoreGapExtension, 0)
+				H0[off] = util.Max16(prevH0+scoreGapExtension, 0)
 			} else {
-				H0sub[off] = util.Max16(prevH0+scoreGapStart, 0)
+				H0[off] = util.Max16(prevH0+scoreGapStart, 0)
 			}
-			C0sub[off] = 0
+			C0[off] = 0
 			inGap = true
 		}
-		prevH0 = H0sub[off]
+		prevH0 = H0[off]
 	}
 	if pidx != M {
 		return Result{-1, -1, 0}, nil
 	}
 	if M == 1 {
-		result := Result{maxScorePos, maxScorePos + 1, int(maxScore)}
+		result := Result{minIdx + maxScorePos, minIdx + maxScorePos + 1, int(maxScore)}
 		if !withPos {
 			return result, nil
 		}
-		pos := []int{maxScorePos}
+		pos := []int{minIdx + maxScorePos}
 		return result, &pos
 	}
 
 	// Phase 3. Fill in score matrix (H)
 	// Unlike the original algorithm, we do not allow omission.
 	f0 := int(F[0])
 	width := lastIdx - f0 + 1
@@ -598,28 +629,28 @@
 				s1 = H[I-width+j0-1]
 			}
 			if j > int(F[i]) {
 				s2 = H[I+j0-1]
 			}
 
 			if s > s1 && (s > s2 || s == s2 && preferMatch) {
-				*pos = append(*pos, j)
+				*pos = append(*pos, j+minIdx)
 				if i == 0 {
 					break
 				}
 				i--
 			}
 			preferMatch = C[I+j0] > 1 || I+width+j0+1 < len(C) && C[I+width+j0+1] > 0
 			j--
 		}
 	}
 	// Start offset we return here is only relevant when begin tiebreak is used.
 	// However finding the accurate offset requires backtracking, and we don't
 	// want to pay extra cost for the option that has lost its importance.
-	return Result{j, maxScorePos + 1, int(maxScore)}, pos
+	return Result{minIdx + j, minIdx + maxScorePos + 1, int(maxScore)}, pos
 }
 
 // Implement the same sorting criteria as V2
 func calculateScore(caseSensitive bool, normalize bool, text *util.Chars, pattern []rune, sidx int, eidx int, withPos bool) (int, *[]int) {
 	pidx, score, inGap, consecutive, firstBonus := 0, 0, false, 0, int16(0)
 	pos := posArray(withPos, len(pattern))
 	prevClass := initialCharClass
@@ -641,15 +672,15 @@
 			char = normalizeRune(char)
 		}
 		if char == pattern[pidx] {
 			if withPos {
 				*pos = append(*pos, idx)
 			}
 			score += scoreMatch
-			bonus := bonusFor(prevClass, class)
+			bonus := bonusMatrix[prevClass][class]
 			if consecutive == 0 {
 				firstBonus = bonus
 			} else {
 				// Break consecutive chunk
 				if bonus >= bonusBoundary && bonus > firstBonus {
 					firstBonus = bonus
 				}
@@ -679,15 +710,16 @@
 }
 
 // FuzzyMatchV1 performs fuzzy-match
 func FuzzyMatchV1(caseSensitive bool, normalize bool, forward bool, text *util.Chars, pattern []rune, withPos bool, slab *util.Slab) (Result, *[]int) {
 	if len(pattern) == 0 {
 		return Result{0, 0, 0}, nil
 	}
-	if asciiFuzzyIndex(text, pattern, caseSensitive) < 0 {
+	idx, _ := asciiFuzzyIndex(text, pattern, caseSensitive)
+	if idx < 0 {
 		return Result{-1, -1, 0}, nil
 	}
 
 	pidx := 0
 	sidx := -1
 	eidx := -1
 
@@ -773,15 +805,16 @@
 	lenRunes := text.Length()
 	lenPattern := len(pattern)
 
 	if lenRunes < lenPattern {
 		return Result{-1, -1, 0}, nil
 	}
 
-	if asciiFuzzyIndex(text, pattern, caseSensitive) < 0 {
+	idx, _ := asciiFuzzyIndex(text, pattern, caseSensitive)
+	if idx < 0 {
 		return Result{-1, -1, 0}, nil
 	}
 
 	// For simplicity, only look at the bonus at the first character position
 	pidx := 0
 	bestPos, bonus, bestBonus := -1, int16(0), int16(-1)
 	for index := 0; index < lenRunes; index++ {
```

### Comparing `fzf_bin-0.49.0/fzf/src/algo/algo_test.go` & `fzf_bin-0.50.0/fzf/src/algo/algo_test.go`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 	"sort"
 	"strings"
 	"testing"
 
 	"github.com/junegunn/fzf/src/util"
 )
 
+func init() {
+	Init("default")
+}
+
 func assertMatch(t *testing.T, fun Algo, caseSensitive, forward bool, input, pattern string, sidx int, eidx int, score int) {
 	assertMatch2(t, fun, caseSensitive, false, forward, input, pattern, sidx, eidx, score)
 }
 
 func assertMatch2(t *testing.T, fun Algo, caseSensitive, normalize, forward bool, input, pattern string, sidx int, eidx int, score int) {
 	if !caseSensitive {
 		pattern = strings.ToLower(pattern)
```

### Comparing `fzf_bin-0.49.0/fzf/src/algo/normalize.go` & `fzf_bin-0.50.0/fzf/src/algo/normalize.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/ansi.go` & `fzf_bin-0.50.0/fzf/src/ansi.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/ansi_test.go` & `fzf_bin-0.50.0/fzf/src/ansi_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/cache.go` & `fzf_bin-0.50.0/fzf/src/cache.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/cache_test.go` & `fzf_bin-0.50.0/fzf/src/cache_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/chunklist.go` & `fzf_bin-0.50.0/fzf/src/chunklist.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/chunklist_test.go` & `fzf_bin-0.50.0/fzf/src/chunklist_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/constants.go` & `fzf_bin-0.50.0/fzf/src/constants.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/core.go` & `fzf_bin-0.50.0/fzf/src/core.go`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // Package fzf implements fzf, a command-line fuzzy finder.
 package fzf
 
 import (
 	"fmt"
-	"os"
+	"sync"
 	"time"
 	"unsafe"
 
 	"github.com/junegunn/fzf/src/util"
 )
 
 /*
@@ -25,24 +25,26 @@
 
 func sbytes(data string) []byte {
 	return unsafe.Slice(unsafe.StringData(data), len(data))
 }
 
 // Run starts fzf
 func Run(opts *Options, version string, revision string) {
+	defer util.RunAtExitFuncs()
+
 	sort := opts.Sort > 0
 	sortCriteria = opts.Criteria
 
 	if opts.Version {
 		if len(revision) > 0 {
 			fmt.Printf("%s (%s)\n", version, revision)
 		} else {
 			fmt.Println(version)
 		}
-		os.Exit(exitOk)
+		util.Exit(exitOk)
 	}
 
 	// Event channel
 	eventBox := util.NewEventBox()
 
 	// ANSI code processor
 	ansiProcessor := func(data []byte) (util.Chars, *[]ansiOffset) {
@@ -159,22 +161,25 @@
 
 		pattern := patternBuilder([]rune(*opts.Filter))
 		matcher.sort = pattern.sortable
 
 		found := false
 		if streamingFilter {
 			slab := util.MakeSlab(slab16Size, slab32Size)
+			mutex := sync.Mutex{}
 			reader := NewReader(
 				func(runes []byte) bool {
 					item := Item{}
 					if chunkList.trans(&item, runes) {
+						mutex.Lock()
 						if result, _, _ := pattern.MatchItem(&item, false, slab); result != nil {
 							opts.Printer(item.text.ToString())
 							found = true
 						}
+						mutex.Unlock()
 					}
 					return false
 				}, eventBox, opts.ReadZero, false)
 			reader.ReadSource(opts.WalkerRoot, opts.WalkerOpts, opts.WalkerSkip)
 		} else {
 			eventBox.Unwatch(EvtReadNew)
 			eventBox.WaitFor(EvtReadFin)
@@ -185,17 +190,17 @@
 				pattern: pattern})
 			for i := 0; i < merger.Length(); i++ {
 				opts.Printer(merger.Get(i).item.AsString(opts.Ansi))
 				found = true
 			}
 		}
 		if found {
-			os.Exit(exitOk)
+			util.Exit(exitOk)
 		}
-		os.Exit(exitNoMatch)
+		util.Exit(exitNoMatch)
 	}
 
 	// Synchronous search
 	if opts.Sync {
 		eventBox.Unwatch(EvtReadNew)
 		eventBox.WaitFor(EvtReadFin)
 	}
@@ -266,15 +271,15 @@
 			}
 			for evt, value := range *events {
 				switch evt {
 				case EvtQuit:
 					if reading {
 						reader.terminate()
 					}
-					os.Exit(value.(int))
+					util.Exit(value.(int))
 				case EvtReadNew, EvtReadFin:
 					if evt == EvtReadFin && nextCommand != nil {
 						restart(*nextCommand, nextEnviron)
 						nextCommand = nil
 						nextEnviron = nil
 						break
 					} else {
@@ -368,17 +373,17 @@
 									if len(opts.Expect) > 0 {
 										opts.Printer("")
 									}
 									for i := 0; i < count; i++ {
 										opts.Printer(val.Get(i).item.AsString(opts.Ansi))
 									}
 									if count > 0 {
-										os.Exit(exitOk)
+										util.Exit(exitOk)
 									}
-									os.Exit(exitNoMatch)
+									util.Exit(exitNoMatch)
 								}
 								determine(val.final)
 							}
 						}
 						terminal.UpdateList(val)
 					}
 				}
```

### Comparing `fzf_bin-0.49.0/fzf/src/history.go` & `fzf_bin-0.50.0/fzf/src/history.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/history_test.go` & `fzf_bin-0.50.0/fzf/src/history_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/item.go` & `fzf_bin-0.50.0/fzf/src/item.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/matcher.go` & `fzf_bin-0.50.0/fzf/src/matcher.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/merger.go` & `fzf_bin-0.50.0/fzf/src/merger.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/merger_test.go` & `fzf_bin-0.50.0/fzf/src/merger_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/options.go` & `fzf_bin-0.50.0/fzf/src/options.go`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     --keep-right           Keep the right end of the line visible on overflow
     --scroll-off=LINES     Number of screen lines to keep above or below when
                            scrolling to the top or to the bottom (default: 0)
     --no-hscroll           Disable horizontal scroll
     --hscroll-off=COLS     Number of screen columns to keep to the right of the
                            highlighted substring (default: 10)
     --filepath-word        Make word-wise movements respect path separators
-    --jump-labels=CHARS    Label characters for jump and jump-accept
+    --jump-labels=CHARS    Label characters for jump mode
 
   Layout
     --height=[~]HEIGHT[%]  Display fzf window below the cursor with the given
                            height instead of using fullscreen.
                            A negative value is calcalated as the terminal height
                            minus the given value.
                            If prefixed with '~', fzf will determine the height
@@ -359,14 +359,18 @@
 	ListenAddr   *listenAddress
 	Unsafe       bool
 	ClearOnExit  bool
 	WalkerOpts   walkerOpts
 	WalkerRoot   string
 	WalkerSkip   []string
 	Version      bool
+	CPUProfile   string
+	MEMProfile   string
+	BlockProfile string
+	MutexProfile string
 }
 
 func filterNonEmpty(input []string) []string {
 	output := make([]string, 0, len(input))
 	for _, str := range input {
 		if len(str) > 0 {
 			output = append(output, str)
@@ -450,22 +454,22 @@
 		WalkerRoot:   ".",
 		WalkerSkip:   []string{".git", "node_modules"},
 		Version:      false}
 }
 
 func help(code int) {
 	os.Stdout.WriteString(usage)
-	os.Exit(code)
+	util.Exit(code)
 }
 
 var errorContext = ""
 
 func errorExit(msg string) {
 	os.Stderr.WriteString(errorContext + msg + "\n")
-	os.Exit(exitError)
+	util.Exit(exitError)
 }
 
 func optString(arg string, prefixes ...string) (bool, string) {
 	for _, prefix := range prefixes {
 		if strings.HasPrefix(arg, prefix) {
 			return true, arg[len(prefix):]
 		}
@@ -662,16 +666,16 @@
 			add(tui.Left)
 		case "right":
 			add(tui.Right)
 		case "enter", "return":
 			add(tui.CtrlM)
 		case "space":
 			chords[tui.Key(' ')] = key
-		case "bspace", "bs":
-			add(tui.BSpace)
+		case "backspace", "bspace", "bs":
+			add(tui.Backspace)
 		case "ctrl-space":
 			add(tui.CtrlSpace)
 		case "ctrl-delete":
 			add(tui.CtrlDelete)
 		case "ctrl-^", "ctrl-6":
 			add(tui.CtrlCaret)
 		case "ctrl-/", "ctrl-_":
@@ -694,64 +698,68 @@
 			add(tui.Result)
 		case "resize":
 			add(tui.Resize)
 		case "one":
 			add(tui.One)
 		case "zero":
 			add(tui.Zero)
+		case "jump":
+			add(tui.Jump)
+		case "jump-cancel":
+			add(tui.JumpCancel)
 		case "alt-enter", "alt-return":
 			chords[tui.CtrlAltKey('m')] = key
 		case "alt-space":
 			chords[tui.AltKey(' ')] = key
-		case "alt-bs", "alt-bspace":
-			add(tui.AltBS)
+		case "alt-bs", "alt-bspace", "alt-backspace":
+			add(tui.AltBackspace)
 		case "alt-up":
 			add(tui.AltUp)
 		case "alt-down":
 			add(tui.AltDown)
 		case "alt-left":
 			add(tui.AltLeft)
 		case "alt-right":
 			add(tui.AltRight)
 		case "tab":
 			add(tui.Tab)
 		case "btab", "shift-tab":
-			add(tui.BTab)
+			add(tui.ShiftTab)
 		case "esc":
-			add(tui.ESC)
-		case "del":
-			add(tui.Del)
+			add(tui.Esc)
+		case "delete", "del":
+			add(tui.Delete)
 		case "home":
 			add(tui.Home)
 		case "end":
 			add(tui.End)
 		case "insert":
 			add(tui.Insert)
 		case "pgup", "page-up":
-			add(tui.PgUp)
+			add(tui.PageUp)
 		case "pgdn", "page-down":
-			add(tui.PgDn)
+			add(tui.PageDown)
 		case "alt-shift-up", "shift-alt-up":
-			add(tui.AltSUp)
+			add(tui.AltShiftUp)
 		case "alt-shift-down", "shift-alt-down":
-			add(tui.AltSDown)
+			add(tui.AltShiftDown)
 		case "alt-shift-left", "shift-alt-left":
-			add(tui.AltSLeft)
+			add(tui.AltShiftLeft)
 		case "alt-shift-right", "shift-alt-right":
-			add(tui.AltSRight)
+			add(tui.AltShiftRight)
 		case "shift-up":
-			add(tui.SUp)
+			add(tui.ShiftUp)
 		case "shift-down":
-			add(tui.SDown)
+			add(tui.ShiftDown)
 		case "shift-left":
-			add(tui.SLeft)
+			add(tui.ShiftLeft)
 		case "shift-right":
-			add(tui.SRight)
+			add(tui.ShiftRight)
 		case "shift-delete":
-			add(tui.SDelete)
+			add(tui.ShiftDelete)
 		case "left-click":
 			add(tui.LeftClick)
 		case "right-click":
 			add(tui.RightClick)
 		case "shift-left-click":
 			add(tui.SLeftClick)
 		case "shift-right-click":
@@ -1970,14 +1978,22 @@
 			opts.WalkerOpts = parseWalkerOpts(nextString(allArgs, &i, "walker options required [file][,dir][,follow][,hidden]"))
 		case "--walker-root":
 			opts.WalkerRoot = nextString(allArgs, &i, "directory required")
 		case "--walker-skip":
 			opts.WalkerSkip = filterNonEmpty(strings.Split(nextString(allArgs, &i, "directory names to ignore required"), ","))
 		case "--version":
 			opts.Version = true
+		case "--profile-cpu":
+			opts.CPUProfile = nextString(allArgs, &i, "file path required: cpu")
+		case "--profile-mem":
+			opts.MEMProfile = nextString(allArgs, &i, "file path required: mem")
+		case "--profile-block":
+			opts.BlockProfile = nextString(allArgs, &i, "file path required: block")
+		case "--profile-mutex":
+			opts.MutexProfile = nextString(allArgs, &i, "file path required: mutex")
 		case "--":
 			// Ignored
 		default:
 			if match, value := optString(arg, "--algo="); match {
 				opts.FuzzyAlgo = parseAlgo(value)
 			} else if match, value := optString(arg, "--scheme="); match {
 				opts.Scheme = strings.ToLower(value)
@@ -2239,17 +2255,15 @@
 		theme.CurrentMatch = boldify(theme.CurrentMatch)
 		theme.Prompt = boldify(theme.Prompt)
 		theme.Input = boldify(theme.Input)
 		theme.Cursor = boldify(theme.Cursor)
 		theme.Spinner = boldify(theme.Spinner)
 	}
 
-	if opts.Scheme != "default" {
-		processScheme(opts)
-	}
+	processScheme(opts)
 }
 
 func expectsArbitraryString(opt string) bool {
 	switch opt {
 	case "-q", "--query", "-f", "--filter", "--header", "--prompt":
 		return true
 	}
@@ -2295,10 +2309,15 @@
 		parseOptions(opts, words)
 	}
 
 	// 3. Options from command-line arguments
 	errorContext = ""
 	parseOptions(opts, os.Args[1:])
 
+	if err := opts.initProfiling(); err != nil {
+		errorExit("failed to start pprof profiles: " + err.Error())
+	}
+
 	postProcessOptions(opts)
+
 	return opts
 }
```

### Comparing `fzf_bin-0.49.0/fzf/src/options_test.go` & `fzf_bin-0.50.0/fzf/src/options_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -166,36 +166,36 @@
 	pairs = parseKeyChords("enter,Return,space,tab,btab,esc,up,down,left,right", "")
 	if len(pairs) != 9 {
 		t.Error(9)
 	}
 	check(tui.CtrlM, "Return")
 	checkEvent(tui.Key(' '), "space")
 	check(tui.Tab, "tab")
-	check(tui.BTab, "btab")
-	check(tui.ESC, "esc")
+	check(tui.ShiftTab, "btab")
+	check(tui.Esc, "esc")
 	check(tui.Up, "up")
 	check(tui.Down, "down")
 	check(tui.Left, "left")
 	check(tui.Right, "right")
 
 	pairs = parseKeyChords("Tab,Ctrl-I,PgUp,page-up,pgdn,Page-Down,Home,End,Alt-BS,Alt-BSpace,shift-left,shift-right,btab,shift-tab,return,Enter,bspace", "")
 	if len(pairs) != 11 {
 		t.Error(11)
 	}
 	check(tui.Tab, "Ctrl-I")
-	check(tui.PgUp, "page-up")
-	check(tui.PgDn, "Page-Down")
+	check(tui.PageUp, "page-up")
+	check(tui.PageDown, "Page-Down")
 	check(tui.Home, "Home")
 	check(tui.End, "End")
-	check(tui.AltBS, "Alt-BSpace")
-	check(tui.SLeft, "shift-left")
-	check(tui.SRight, "shift-right")
-	check(tui.BTab, "shift-tab")
+	check(tui.AltBackspace, "Alt-BSpace")
+	check(tui.ShiftLeft, "shift-left")
+	check(tui.ShiftRight, "shift-right")
+	check(tui.ShiftTab, "shift-tab")
 	check(tui.CtrlM, "Enter")
-	check(tui.BSpace, "bspace")
+	check(tui.Backspace, "bspace")
 }
 
 func TestParseKeysWithComma(t *testing.T) {
 	checkN := func(a int, b int) {
 		if a != b {
 			t.Errorf("%d != %d", a, b)
 		}
```

### Comparing `fzf_bin-0.49.0/fzf/src/pattern.go` & `fzf_bin-0.50.0/fzf/src/pattern.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/pattern_test.go` & `fzf_bin-0.50.0/fzf/src/pattern_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/reader.go` & `fzf_bin-0.50.0/fzf/src/reader.go`

 * *Files 8% similar despite different names*

```diff
@@ -169,14 +169,20 @@
 					leftover = []byte{}
 				}
 				if (err == nil || len(slice) > 0) && r.pusher(slice) {
 					atomic.StoreInt32(&r.event, int32(EvtReadNew))
 				}
 			} else {
 				// Could not find the delimiter in the buffer
+				//   NOTE: We can further optimize this by keeping track of the cursor
+				//   position in the slab so that a straddling item that doesn't go
+				//   beyond the boundary of a slab doesn't need to be copied to
+				//   another buffer. However, the performance gain is negligible in
+				//   practice (< 0.1%) and is not
+				//   worth the added complexity.
 				leftover = append(leftover, buf...)
 				break
 			}
 		}
 
 		if err == io.EOF {
 			leftover = append(leftover, buf...)
```

### Comparing `fzf_bin-0.49.0/fzf/src/reader_test.go` & `fzf_bin-0.50.0/fzf/src/reader_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/result.go` & `fzf_bin-0.50.0/fzf/src/result.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/result_test.go` & `fzf_bin-0.50.0/fzf/src/result_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/server.go` & `fzf_bin-0.50.0/fzf/src/server.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/terminal.go` & `fzf_bin-0.50.0/fzf/src/terminal.go`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 	eventChan          chan tui.Event
 	slab               *util.Slab
 	theme              *tui.ColorTheme
 	tui                tui.Renderer
 	executing          *util.AtomicBool
 	termSize           tui.TermSize
 	lastAction         actionType
+	lastKey            string
 	lastFocus          int32
 	areaLines          int
 	areaColumns        int
 	forcePreview       bool
 }
 
 type selectedItem struct {
@@ -404,15 +405,15 @@
 	actPageDown
 	actPosition
 	actHalfPageUp
 	actHalfPageDown
 	actOffsetUp
 	actOffsetDown
 	actJump
-	actJumpAccept
+	actJumpAccept // XXX Deprecated in favor of jump:accept binding
 	actPrintQuery
 	actRefreshPreview
 	actReplaceQuery
 	actToggleSort
 	actShowPreview
 	actHidePreview
 	actTogglePreview
@@ -456,22 +457,15 @@
 	actBecome
 	actResponse
 	actShowHeader
 	actHideHeader
 )
 
 func (a actionType) Name() string {
-	name := ""
-	for i, r := range a.String()[3:] {
-		if i > 0 && r >= 'A' && r <= 'Z' {
-			name += "-"
-		}
-		name += string(r)
-	}
-	return strings.ToLower(name)
+	return util.ToKebabCase(a.String()[3:])
 }
 
 func processExecution(action actionType) bool {
 	switch action {
 	case actTransform,
 		actTransformBorderLabel,
 		actTransformHeader,
@@ -542,55 +536,55 @@
 
 	add(tui.Invalid, actInvalid)
 	add(tui.CtrlA, actBeginningOfLine)
 	add(tui.CtrlB, actBackwardChar)
 	add(tui.CtrlC, actAbort)
 	add(tui.CtrlG, actAbort)
 	add(tui.CtrlQ, actAbort)
-	add(tui.ESC, actAbort)
+	add(tui.Esc, actAbort)
 	add(tui.CtrlD, actDeleteCharEof)
 	add(tui.CtrlE, actEndOfLine)
 	add(tui.CtrlF, actForwardChar)
 	add(tui.CtrlH, actBackwardDeleteChar)
-	add(tui.BSpace, actBackwardDeleteChar)
+	add(tui.Backspace, actBackwardDeleteChar)
 	add(tui.Tab, actToggleDown)
-	add(tui.BTab, actToggleUp)
+	add(tui.ShiftTab, actToggleUp)
 	add(tui.CtrlJ, actDown)
 	add(tui.CtrlK, actUp)
 	add(tui.CtrlL, actClearScreen)
 	add(tui.CtrlM, actAccept)
 	add(tui.CtrlN, actDown)
 	add(tui.CtrlP, actUp)
 	add(tui.CtrlU, actUnixLineDiscard)
 	add(tui.CtrlW, actUnixWordRubout)
 	add(tui.CtrlY, actYank)
 	if !util.IsWindows() {
 		add(tui.CtrlZ, actSigStop)
 	}
 
 	addEvent(tui.AltKey('b'), actBackwardWord)
-	add(tui.SLeft, actBackwardWord)
+	add(tui.ShiftLeft, actBackwardWord)
 	addEvent(tui.AltKey('f'), actForwardWord)
-	add(tui.SRight, actForwardWord)
+	add(tui.ShiftRight, actForwardWord)
 	addEvent(tui.AltKey('d'), actKillWord)
-	add(tui.AltBS, actBackwardKillWord)
+	add(tui.AltBackspace, actBackwardKillWord)
 
 	add(tui.Up, actUp)
 	add(tui.Down, actDown)
 	add(tui.Left, actBackwardChar)
 	add(tui.Right, actForwardChar)
 
 	add(tui.Home, actBeginningOfLine)
 	add(tui.End, actEndOfLine)
-	add(tui.Del, actDeleteChar)
-	add(tui.PgUp, actPageUp)
-	add(tui.PgDn, actPageDown)
+	add(tui.Delete, actDeleteChar)
+	add(tui.PageUp, actPageUp)
+	add(tui.PageDown, actPageDown)
 
-	add(tui.SUp, actPreviewUp)
-	add(tui.SDown, actPreviewDown)
+	add(tui.ShiftUp, actPreviewUp)
+	add(tui.ShiftDown, actPreviewDown)
 
 	add(tui.Mouse, actMouse)
 	add(tui.LeftClick, actClick)
 	add(tui.RightClick, actToggle)
 	add(tui.SLeftClick, actToggle)
 	add(tui.SRightClick, actToggle)
 
@@ -847,14 +841,15 @@
 func (t *Terminal) environ() []string {
 	env := os.Environ()
 	if t.listenPort != nil {
 		env = append(env, fmt.Sprintf("FZF_PORT=%d", *t.listenPort))
 	}
 	env = append(env, "FZF_QUERY="+string(t.input))
 	env = append(env, "FZF_ACTION="+t.lastAction.Name())
+	env = append(env, "FZF_KEY="+t.lastKey)
 	env = append(env, "FZF_PROMPT="+string(t.promptString))
 	env = append(env, "FZF_PREVIEW_LABEL="+t.previewLabelOpts.label)
 	env = append(env, "FZF_BORDER_LABEL="+t.borderLabelOpts.label)
 	env = append(env, fmt.Sprintf("FZF_TOTAL_COUNT=%d", t.count))
 	env = append(env, fmt.Sprintf("FZF_MATCH_COUNT=%d", t.merger.Length()))
 	env = append(env, fmt.Sprintf("FZF_SELECT_COUNT=%d", len(t.selected)))
 	env = append(env, fmt.Sprintf("FZF_LINES=%d", t.areaLines))
@@ -3286,14 +3281,15 @@
 				needBarrier = false
 			}
 		}
 
 		t.mutex.Lock()
 		previousInput := t.input
 		previousCx := t.cx
+		t.lastKey = event.KeyName()
 		events := []util.EventType{}
 		req := func(evts ...util.EventType) {
 			for _, event := range evts {
 				events = append(events, event)
 				if event == reqClose || event == reqQuit {
 					looping = false
 				}
@@ -4104,47 +4100,51 @@
 			return true
 		}
 
 		if t.jumping == jumpDisabled || len(actions) > 0 {
 			// Break out of jump mode if any action is submitted to the server
 			if t.jumping != jumpDisabled {
 				t.jumping = jumpDisabled
+				if acts, prs := t.keymap[tui.JumpCancel.AsEvent()]; prs && !doActions(acts) {
+					continue
+				}
 				req(reqList)
 			}
 			if len(actions) == 0 {
 				actions = t.keymap[event.Comparable()]
 			}
 			if len(actions) == 0 && event.Type == tui.Rune {
 				doAction(&action{t: actChar})
 			} else if !doActions(actions) {
 				continue
 			}
 			t.truncateQuery()
 			queryChanged = string(previousInput) != string(t.input)
 			changed = changed || queryChanged
-			if onChanges, prs := t.keymap[tui.Change.AsEvent()]; queryChanged && prs {
-				if !doActions(onChanges) {
-					continue
-				}
+			if onChanges, prs := t.keymap[tui.Change.AsEvent()]; queryChanged && prs && !doActions(onChanges) {
+				continue
 			}
-			if onEOFs, prs := t.keymap[tui.BackwardEOF.AsEvent()]; beof && prs {
-				if !doActions(onEOFs) {
-					continue
-				}
+			if onEOFs, prs := t.keymap[tui.BackwardEOF.AsEvent()]; beof && prs && !doActions(onEOFs) {
+				continue
 			}
 		} else {
+			jumpEvent := tui.JumpCancel
 			if event.Type == tui.Rune {
 				if idx := strings.IndexRune(t.jumpLabels, event.Char); idx >= 0 && idx < t.maxItems() && idx < t.merger.Length() {
+					jumpEvent = tui.Jump
 					t.cy = idx + t.offset
 					if t.jumping == jumpAcceptEnabled {
 						req(reqClose)
 					}
 				}
 			}
 			t.jumping = jumpDisabled
+			if acts, prs := t.keymap[jumpEvent.AsEvent()]; prs && !doActions(acts) {
+				continue
+			}
 			req(reqList)
 		}
 
 		if queryChanged && t.canPreview() && len(t.previewOpts.command) > 0 {
 			_, _, forceUpdate := hasPreviewFlags(t.previewOpts.command)
 			if forceUpdate {
 				t.version++
```

### Comparing `fzf_bin-0.49.0/fzf/src/terminal_test.go` & `fzf_bin-0.50.0/fzf/src/terminal_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/terminal_unix.go` & `fzf_bin-0.50.0/fzf/src/terminal_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/terminal_windows.go` & `fzf_bin-0.50.0/fzf/src/terminal_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/tokenizer.go` & `fzf_bin-0.50.0/fzf/src/tokenizer.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/tokenizer_test.go` & `fzf_bin-0.50.0/fzf/src/tokenizer_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/tui/dummy.go` & `fzf_bin-0.50.0/fzf/src/tui/dummy.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/tui/light.go` & `fzf_bin-0.50.0/fzf/src/tui/light.go`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 	fullcode := "\x1b[" + code
 	r.stderr(fullcode)
 	return fullcode
 }
 
 func (r *LightRenderer) flush() {
 	if r.queued.Len() > 0 {
-		fmt.Fprint(os.Stderr, "\x1b[?25l"+r.queued.String()+"\x1b[?25h")
+		fmt.Fprint(os.Stderr, "\x1b[?7l\x1b[?25l"+r.queued.String()+"\x1b[?25h\x1b[?7h")
 		r.queued.Reset()
 	}
 }
 
 // Light renderer
 type LightRenderer struct {
 	theme         *ColorTheme
@@ -241,30 +241,30 @@
 	c, ok := r.getch(nonblock)
 	if !nonblock && !ok {
 		r.Close()
 		errorExit("Failed to read " + consoleDevice)
 	}
 
 	retries := 0
-	if c == ESC.Int() || nonblock {
+	if c == Esc.Int() || nonblock {
 		retries = r.escDelay / escPollInterval
 	}
 	buffer = append(buffer, byte(c))
 
 	pc := c
 	for {
 		c, ok = r.getch(true)
 		if !ok {
 			if retries > 0 {
 				retries--
 				time.Sleep(escPollInterval * time.Millisecond)
 				continue
 			}
 			break
-		} else if c == ESC.Int() && pc != c {
+		} else if c == Esc.Int() && pc != c {
 			retries = r.escDelay / escPollInterval
 		} else {
 			retries = 0
 		}
 		buffer = append(buffer, byte(c))
 		pc = c
 
@@ -296,26 +296,26 @@
 	case CtrlC.Byte():
 		return Event{CtrlC, 0, nil}
 	case CtrlG.Byte():
 		return Event{CtrlG, 0, nil}
 	case CtrlQ.Byte():
 		return Event{CtrlQ, 0, nil}
 	case 127:
-		return Event{BSpace, 0, nil}
+		return Event{Backspace, 0, nil}
 	case 0:
 		return Event{CtrlSpace, 0, nil}
 	case 28:
 		return Event{CtrlBackSlash, 0, nil}
 	case 29:
 		return Event{CtrlRightBracket, 0, nil}
 	case 30:
 		return Event{CtrlCaret, 0, nil}
 	case 31:
 		return Event{CtrlSlash, 0, nil}
-	case ESC.Byte():
+	case Esc.Byte():
 		ev := r.escSequence(&sz)
 		// Second chance
 		if ev.Type == Invalid {
 			r.buffer = r.getBytes()
 			ev = r.escSequence(&sz)
 		}
 		return ev
@@ -323,45 +323,45 @@
 
 	// CTRL-A ~ CTRL-Z
 	if r.buffer[0] <= CtrlZ.Byte() {
 		return Event{EventType(r.buffer[0]), 0, nil}
 	}
 	char, rsz := utf8.DecodeRune(r.buffer)
 	if char == utf8.RuneError {
-		return Event{ESC, 0, nil}
+		return Event{Esc, 0, nil}
 	}
 	sz = rsz
 	return Event{Rune, char, nil}
 }
 
 func (r *LightRenderer) escSequence(sz *int) Event {
 	if len(r.buffer) < 2 {
-		return Event{ESC, 0, nil}
+		return Event{Esc, 0, nil}
 	}
 
 	loc := offsetRegexpBegin.FindIndex(r.buffer)
 	if loc != nil && loc[0] == 0 {
 		*sz = loc[1]
 		return Event{Invalid, 0, nil}
 	}
 
 	*sz = 2
 	if r.buffer[1] >= 1 && r.buffer[1] <= 'z'-'a'+1 {
 		return CtrlAltKey(rune(r.buffer[1] + 'a' - 1))
 	}
 	alt := false
-	if len(r.buffer) > 2 && r.buffer[1] == ESC.Byte() {
+	if len(r.buffer) > 2 && r.buffer[1] == Esc.Byte() {
 		r.buffer = r.buffer[1:]
 		alt = true
 	}
 	switch r.buffer[1] {
-	case ESC.Byte():
-		return Event{ESC, 0, nil}
+	case Esc.Byte():
+		return Event{Esc, 0, nil}
 	case 127:
-		return Event{AltBS, 0, nil}
+		return Event{AltBackspace, 0, nil}
 	case '[', 'O':
 		if len(r.buffer) < 3 {
 			return Event{Invalid, 0, nil}
 		}
 		*sz = 3
 		switch r.buffer[2] {
 		case 'D':
@@ -382,15 +382,15 @@
 			return Event{Down, 0, nil}
 		case 'A':
 			if alt {
 				return Event{AltUp, 0, nil}
 			}
 			return Event{Up, 0, nil}
 		case 'Z':
-			return Event{BTab, 0, nil}
+			return Event{ShiftTab, 0, nil}
 		case 'H':
 			return Event{Home, 0, nil}
 		case 'F':
 			return Event{End, 0, nil}
 		case '<':
 			return r.mouseSequence(sz)
 		case 'P':
@@ -430,32 +430,32 @@
 					r.buffer = r.buffer[6:]
 					*sz = 0
 					return r.GetChar()
 				}
 				return Event{Invalid, 0, nil} // INS
 			case '3':
 				if r.buffer[3] == '~' {
-					return Event{Del, 0, nil}
+					return Event{Delete, 0, nil}
 				}
 				if len(r.buffer) == 6 && r.buffer[5] == '~' {
 					*sz = 6
 					switch r.buffer[4] {
 					case '5':
 						return Event{CtrlDelete, 0, nil}
 					case '2':
-						return Event{SDelete, 0, nil}
+						return Event{ShiftDelete, 0, nil}
 					}
 				}
 				return Event{Invalid, 0, nil}
 			case '4':
 				return Event{End, 0, nil}
 			case '5':
-				return Event{PgUp, 0, nil}
+				return Event{PageUp, 0, nil}
 			case '6':
-				return Event{PgDn, 0, nil}
+				return Event{PageDown, 0, nil}
 			case '7':
 				return Event{Home, 0, nil}
 			case '8':
 				return Event{End, 0, nil}
 			case '1':
 				switch r.buffer[3] {
 				case '~':
@@ -485,58 +485,71 @@
 					return Event{Invalid, 0, nil}
 				case ';':
 					if len(r.buffer) < 6 {
 						return Event{Invalid, 0, nil}
 					}
 					*sz = 6
 					switch r.buffer[4] {
-					case '1', '2', '3', '5':
+					case '1', '2', '3', '4', '5':
+						//                   Kitty      iTerm2     WezTerm
+						// SHIFT-ARROW       "\e[1;2D"
+						// ALT-SHIFT-ARROW   "\e[1;4D"  "\e[1;10D" "\e[1;4D"
+						// CTRL-SHIFT-ARROW  "\e[1;6D"             N/A
+						// CMD-SHIFT-ARROW   "\e[1;10D" N/A        N/A ("\e[1;2D")
 						alt := r.buffer[4] == '3'
-						altShift := r.buffer[4] == '1' && r.buffer[5] == '0'
 						char := r.buffer[5]
-						if altShift {
+						altShift := false
+						if r.buffer[4] == '1' && r.buffer[5] == '0' {
+							altShift = true
 							if len(r.buffer) < 7 {
 								return Event{Invalid, 0, nil}
 							}
 							*sz = 7
 							char = r.buffer[6]
+						} else if r.buffer[4] == '4' {
+							altShift = true
+							if len(r.buffer) < 6 {
+								return Event{Invalid, 0, nil}
+							}
+							*sz = 6
+							char = r.buffer[5]
 						}
 						switch char {
 						case 'A':
 							if alt {
 								return Event{AltUp, 0, nil}
 							}
 							if altShift {
-								return Event{AltSUp, 0, nil}
+								return Event{AltShiftUp, 0, nil}
 							}
-							return Event{SUp, 0, nil}
+							return Event{ShiftUp, 0, nil}
 						case 'B':
 							if alt {
 								return Event{AltDown, 0, nil}
 							}
 							if altShift {
-								return Event{AltSDown, 0, nil}
+								return Event{AltShiftDown, 0, nil}
 							}
-							return Event{SDown, 0, nil}
+							return Event{ShiftDown, 0, nil}
 						case 'C':
 							if alt {
 								return Event{AltRight, 0, nil}
 							}
 							if altShift {
-								return Event{AltSRight, 0, nil}
+								return Event{AltShiftRight, 0, nil}
 							}
-							return Event{SRight, 0, nil}
+							return Event{ShiftRight, 0, nil}
 						case 'D':
 							if alt {
 								return Event{AltLeft, 0, nil}
 							}
 							if altShift {
-								return Event{AltSLeft, 0, nil}
+								return Event{AltShiftLeft, 0, nil}
 							}
-							return Event{SLeft, 0, nil}
+							return Event{ShiftLeft, 0, nil}
 						}
 					} // r.buffer[4]
 				} // r.buffer[3]
 			} // r.buffer[2]
 		} // r.buffer[2]
 	} // r.buffer[1]
 	rest := bytes.NewBuffer(r.buffer[1:])
```

### Comparing `fzf_bin-0.49.0/fzf/src/tui/light_unix.go` & `fzf_bin-0.50.0/fzf/src/tui/light_unix.go`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 		tty := ttyname()
 		if len(tty) > 0 {
 			if in, err := os.OpenFile(tty, syscall.O_RDONLY, 0); err == nil {
 				return in
 			}
 		}
 		fmt.Fprintln(os.Stderr, "Failed to open "+consoleDevice)
-		os.Exit(2)
+		util.Exit(2)
 	}
 	return in
 }
 
 func (r *LightRenderer) setupTerminal() {
 	term.MakeRaw(r.fd())
 }
```

### Comparing `fzf_bin-0.49.0/fzf/src/tui/light_windows.go` & `fzf_bin-0.50.0/fzf/src/tui/light_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/tui/tcell.go` & `fzf_bin-0.50.0/fzf/src/tui/tcell.go`

 * *Files 0% similar despite different names*

```diff
@@ -316,24 +316,24 @@
 			return keyfn('f')
 		case tcell.KeyCtrlG:
 			return keyfn('g')
 		case tcell.KeyCtrlH:
 			switch ev.Rune() {
 			case 0:
 				if ctrl {
-					return Event{BSpace, 0, nil}
+					return Event{Backspace, 0, nil}
 				}
 			case rune(tcell.KeyCtrlH):
 				switch {
 				case ctrl:
 					return keyfn('h')
 				case alt:
-					return Event{AltBS, 0, nil}
+					return Event{AltBackspace, 0, nil}
 				case none, shift:
-					return Event{BSpace, 0, nil}
+					return Event{Backspace, 0, nil}
 				}
 			}
 		case tcell.KeyCtrlI:
 			return keyfn('i')
 		case tcell.KeyCtrlJ:
 			return keyfn('j')
 		case tcell.KeyCtrlK:
@@ -378,58 +378,58 @@
 		case tcell.KeyCtrlCarat:
 			return Event{CtrlCaret, 0, nil}
 		case tcell.KeyCtrlUnderscore:
 			return Event{CtrlSlash, 0, nil}
 		// section 3: (Alt)+Backspace2
 		case tcell.KeyBackspace2:
 			if alt {
-				return Event{AltBS, 0, nil}
+				return Event{AltBackspace, 0, nil}
 			}
-			return Event{BSpace, 0, nil}
+			return Event{Backspace, 0, nil}
 
 		// section 4: (Alt+Shift)+Key(Up|Down|Left|Right)
 		case tcell.KeyUp:
 			if altShift {
-				return Event{AltSUp, 0, nil}
+				return Event{AltShiftUp, 0, nil}
 			}
 			if shift {
-				return Event{SUp, 0, nil}
+				return Event{ShiftUp, 0, nil}
 			}
 			if alt {
 				return Event{AltUp, 0, nil}
 			}
 			return Event{Up, 0, nil}
 		case tcell.KeyDown:
 			if altShift {
-				return Event{AltSDown, 0, nil}
+				return Event{AltShiftDown, 0, nil}
 			}
 			if shift {
-				return Event{SDown, 0, nil}
+				return Event{ShiftDown, 0, nil}
 			}
 			if alt {
 				return Event{AltDown, 0, nil}
 			}
 			return Event{Down, 0, nil}
 		case tcell.KeyLeft:
 			if altShift {
-				return Event{AltSLeft, 0, nil}
+				return Event{AltShiftLeft, 0, nil}
 			}
 			if shift {
-				return Event{SLeft, 0, nil}
+				return Event{ShiftLeft, 0, nil}
 			}
 			if alt {
 				return Event{AltLeft, 0, nil}
 			}
 			return Event{Left, 0, nil}
 		case tcell.KeyRight:
 			if altShift {
-				return Event{AltSRight, 0, nil}
+				return Event{AltShiftRight, 0, nil}
 			}
 			if shift {
-				return Event{SRight, 0, nil}
+				return Event{ShiftRight, 0, nil}
 			}
 			if alt {
 				return Event{AltRight, 0, nil}
 			}
 			return Event{Right, 0, nil}
 
 		// section 5: (Insert|Home|Delete|End|PgUp|PgDn|BackTab|F1-F12)
@@ -438,25 +438,25 @@
 		case tcell.KeyHome:
 			return Event{Home, 0, nil}
 		case tcell.KeyDelete:
 			if ctrl {
 				return Event{CtrlDelete, 0, nil}
 			}
 			if shift {
-				return Event{SDelete, 0, nil}
+				return Event{ShiftDelete, 0, nil}
 			}
-			return Event{Del, 0, nil}
+			return Event{Delete, 0, nil}
 		case tcell.KeyEnd:
 			return Event{End, 0, nil}
 		case tcell.KeyPgUp:
-			return Event{PgUp, 0, nil}
+			return Event{PageUp, 0, nil}
 		case tcell.KeyPgDn:
-			return Event{PgDn, 0, nil}
+			return Event{PageDown, 0, nil}
 		case tcell.KeyBacktab:
-			return Event{BTab, 0, nil}
+			return Event{ShiftTab, 0, nil}
 		case tcell.KeyF1:
 			return Event{F1, 0, nil}
 		case tcell.KeyF2:
 			return Event{F2, 0, nil}
 		case tcell.KeyF3:
 			return Event{F3, 0, nil}
 		case tcell.KeyF4:
@@ -494,15 +494,15 @@
 				return AltKey(r)
 			default:
 				return Event{Rune, r, nil}
 			}
 
 		// section 7: Esc
 		case tcell.KeyEsc:
-			return Event{ESC, 0, nil}
+			return Event{Esc, 0, nil}
 		}
 	}
 
 	// section 8: Invalid
 	return Event{Invalid, 0, nil}
 }
```

### Comparing `fzf_bin-0.49.0/fzf/src/tui/tcell_test.go` & `fzf_bin-0.50.0/fzf/src/tui/tcell_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -98,40 +98,40 @@
 		{giveKey{tcell.KeyRS, rune(tcell.KeyRS), tcell.ModShift | tcell.ModCtrl}, wantKey{CtrlCaret, 0, nil}},               // actual Ctrl+Shift+6 (i.e. Ctrl+^) keystroke
 		{giveKey{tcell.KeyCtrlUnderscore, rune(tcell.KeyCtrlUnderscore), tcell.ModShift | tcell.ModCtrl}, wantKey{CtrlSlash, 0, nil}},
 
 		// section 3: (Alt)+Backspace2
 		// KeyBackspace2 is alias for KeyDEL = 0x7F (ASCII) (allegedly unused by Windows)
 		// KeyDelete = 0x2E (VK_DELETE constant in Windows)
 		// KeyBackspace is alias for KeyBS = 0x08 (ASCII) (implicit alias with KeyCtrlH)
-		{giveKey{tcell.KeyBackspace2, 0, tcell.ModNone}, wantKey{BSpace, 0, nil}}, // fabricated
-		{giveKey{tcell.KeyBackspace2, 0, tcell.ModAlt}, wantKey{AltBS, 0, nil}},   // fabricated
-		{giveKey{tcell.KeyDEL, 0, tcell.ModNone}, wantKey{BSpace, 0, nil}},        // fabricated, unhandled
-		{giveKey{tcell.KeyDelete, 0, tcell.ModNone}, wantKey{Del, 0, nil}},
-		{giveKey{tcell.KeyDelete, 0, tcell.ModAlt}, wantKey{Del, 0, nil}},
+		{giveKey{tcell.KeyBackspace2, 0, tcell.ModNone}, wantKey{Backspace, 0, nil}},   // fabricated
+		{giveKey{tcell.KeyBackspace2, 0, tcell.ModAlt}, wantKey{AltBackspace, 0, nil}}, // fabricated
+		{giveKey{tcell.KeyDEL, 0, tcell.ModNone}, wantKey{Backspace, 0, nil}},          // fabricated, unhandled
+		{giveKey{tcell.KeyDelete, 0, tcell.ModNone}, wantKey{Delete, 0, nil}},
+		{giveKey{tcell.KeyDelete, 0, tcell.ModAlt}, wantKey{Delete, 0, nil}},
 		{giveKey{tcell.KeyBackspace, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},                                                  // fabricated, unhandled
 		{giveKey{tcell.KeyBS, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},                                                         // fabricated, unhandled
 		{giveKey{tcell.KeyCtrlH, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},                                                      // fabricated, unhandled
-		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModNone}, wantKey{BSpace, 0, nil}},                                    // actual "Backspace" keystroke
-		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModAlt}, wantKey{AltBS, 0, nil}},                                      // actual "Alt+Backspace" keystroke
-		{giveKey{tcell.KeyDEL, rune(tcell.KeyDEL), tcell.ModCtrl}, wantKey{BSpace, 0, nil}},                                        // actual "Ctrl+Backspace" keystroke
-		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModShift}, wantKey{BSpace, 0, nil}},                                   // actual "Shift+Backspace" keystroke
-		{giveKey{tcell.KeyCtrlH, 0, tcell.ModCtrl | tcell.ModAlt}, wantKey{BSpace, 0, nil}},                                        // actual "Ctrl+Alt+Backspace" keystroke
-		{giveKey{tcell.KeyCtrlH, 0, tcell.ModCtrl | tcell.ModShift}, wantKey{BSpace, 0, nil}},                                      // actual "Ctrl+Shift+Backspace" keystroke
-		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModShift | tcell.ModAlt}, wantKey{AltBS, 0, nil}},                     // actual "Shift+Alt+Backspace" keystroke
-		{giveKey{tcell.KeyCtrlH, 0, tcell.ModCtrl | tcell.ModAlt | tcell.ModShift}, wantKey{BSpace, 0, nil}},                       // actual "Ctrl+Shift+Alt+Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModNone}, wantKey{Backspace, 0, nil}},                                 // actual "Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModAlt}, wantKey{AltBackspace, 0, nil}},                               // actual "Alt+Backspace" keystroke
+		{giveKey{tcell.KeyDEL, rune(tcell.KeyDEL), tcell.ModCtrl}, wantKey{Backspace, 0, nil}},                                     // actual "Ctrl+Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModShift}, wantKey{Backspace, 0, nil}},                                // actual "Shift+Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, 0, tcell.ModCtrl | tcell.ModAlt}, wantKey{Backspace, 0, nil}},                                     // actual "Ctrl+Alt+Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, 0, tcell.ModCtrl | tcell.ModShift}, wantKey{Backspace, 0, nil}},                                   // actual "Ctrl+Shift+Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModShift | tcell.ModAlt}, wantKey{AltBackspace, 0, nil}},              // actual "Shift+Alt+Backspace" keystroke
+		{giveKey{tcell.KeyCtrlH, 0, tcell.ModCtrl | tcell.ModAlt | tcell.ModShift}, wantKey{Backspace, 0, nil}},                    // actual "Ctrl+Shift+Alt+Backspace" keystroke
 		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModCtrl}, wantKey{CtrlH, 0, nil}},                                     // actual "Ctrl+H" keystroke
 		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModCtrl | tcell.ModAlt}, wantKey{CtrlAlt, 'h', nil}},                  // fabricated "Ctrl+Alt+H" keystroke
 		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModCtrl | tcell.ModShift}, wantKey{CtrlH, 0, nil}},                    // actual "Ctrl+Shift+H" keystroke
 		{giveKey{tcell.KeyCtrlH, rune(tcell.KeyCtrlH), tcell.ModCtrl | tcell.ModAlt | tcell.ModShift}, wantKey{CtrlAlt, 'h', nil}}, // fabricated "Ctrl+Shift+Alt+H" keystroke
 
 		// section 4: (Alt+Shift)+Key(Up|Down|Left|Right)
 		{giveKey{tcell.KeyUp, 0, tcell.ModNone}, wantKey{Up, 0, nil}},
 		{giveKey{tcell.KeyDown, 0, tcell.ModAlt}, wantKey{AltDown, 0, nil}},
-		{giveKey{tcell.KeyLeft, 0, tcell.ModShift}, wantKey{SLeft, 0, nil}},
-		{giveKey{tcell.KeyRight, 0, tcell.ModShift | tcell.ModAlt}, wantKey{AltSRight, 0, nil}},
+		{giveKey{tcell.KeyLeft, 0, tcell.ModShift}, wantKey{ShiftLeft, 0, nil}},
+		{giveKey{tcell.KeyRight, 0, tcell.ModShift | tcell.ModAlt}, wantKey{AltShiftRight, 0, nil}},
 		{giveKey{tcell.KeyUpLeft, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},    // fabricated, unhandled
 		{giveKey{tcell.KeyUpRight, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},   // fabricated, unhandled
 		{giveKey{tcell.KeyDownLeft, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},  // fabricated, unhandled
 		{giveKey{tcell.KeyDownRight, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}}, // fabricated, unhandled
 		{giveKey{tcell.KeyCenter, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},    // fabricated, unhandled
 		// section 5: (Insert|Home|Delete|End|PgUp|PgDn|BackTab|F1-F12)
 		{giveKey{tcell.KeyInsert, 0, tcell.ModNone}, wantKey{Insert, 0, nil}},
@@ -157,19 +157,19 @@
 
 		{giveKey{tcell.KeyRune, '{', tcell.ModCtrl | tcell.ModAlt}, wantKey{Rune, '{', nil}}, // DE: Ctrl+Alt+7 = "{"
 		{giveKey{tcell.KeyRune, '@', tcell.ModCtrl | tcell.ModAlt}, wantKey{Rune, '@', nil}}, // DE: Ctrl+Alt+q = "@"
 		{giveKey{tcell.KeyRune, 'µ', tcell.ModCtrl | tcell.ModAlt}, wantKey{Rune, 'µ', nil}}, // DE: Ctrl+Alt+m = "µ"
 
 		// section 7: Esc
 		// KeyEsc and KeyEscape are aliases for KeyESC
-		{giveKey{tcell.KeyEsc, rune(tcell.KeyEsc), tcell.ModNone}, wantKey{ESC, 0, nil}},               // fabricated
-		{giveKey{tcell.KeyESC, rune(tcell.KeyESC), tcell.ModNone}, wantKey{ESC, 0, nil}},               // unhandled
-		{giveKey{tcell.KeyEscape, rune(tcell.KeyEscape), tcell.ModNone}, wantKey{ESC, 0, nil}},         // fabricated, unhandled
-		{giveKey{tcell.KeyESC, rune(tcell.KeyESC), tcell.ModCtrl}, wantKey{ESC, 0, nil}},               // actual Ctrl+[ keystroke
-		{giveKey{tcell.KeyCtrlLeftSq, rune(tcell.KeyCtrlLeftSq), tcell.ModCtrl}, wantKey{ESC, 0, nil}}, // fabricated, unhandled
+		{giveKey{tcell.KeyEsc, rune(tcell.KeyEsc), tcell.ModNone}, wantKey{Esc, 0, nil}},               // fabricated
+		{giveKey{tcell.KeyESC, rune(tcell.KeyESC), tcell.ModNone}, wantKey{Esc, 0, nil}},               // unhandled
+		{giveKey{tcell.KeyEscape, rune(tcell.KeyEscape), tcell.ModNone}, wantKey{Esc, 0, nil}},         // fabricated, unhandled
+		{giveKey{tcell.KeyESC, rune(tcell.KeyESC), tcell.ModCtrl}, wantKey{Esc, 0, nil}},               // actual Ctrl+[ keystroke
+		{giveKey{tcell.KeyCtrlLeftSq, rune(tcell.KeyCtrlLeftSq), tcell.ModCtrl}, wantKey{Esc, 0, nil}}, // fabricated, unhandled
 
 		// section 8: Invalid
 		{giveKey{tcell.KeyRune, 'a', tcell.ModMeta}, wantKey{Rune, 'a', nil}}, // fabricated
 		{giveKey{tcell.KeyF24, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},
 		{giveKey{tcell.KeyHelp, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},   // fabricated, unhandled
 		{giveKey{tcell.KeyExit, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},   // fabricated, unhandled
 		{giveKey{tcell.KeyClear, 0, tcell.ModNone}, wantKey{Invalid, 0, nil}},  // unhandled, actual keystroke Numpad_5 with Numlock OFF
@@ -255,28 +255,28 @@
 33					Invalid
 34					Resize
 35					Mouse
 36					DoubleClick
 37					LeftClick
 38					RightClick
 39					BTab
-40					BSpace
+40					Backspace
 41					Del
 42					PgUp
 43					PgDn
 44					Up
 45					Down
 46					Left
 47					Right
 48					Home
 49					End
 50					Insert
 51					SUp
 52					SDown
-53					SLeft
+53					ShiftLeft
 54					SRight
 55					F1
 56					F2
 57					F3
 58					F4
 59					F5
 60					F6
@@ -284,23 +284,23 @@
 62					F8
 63					F9
 64					F10
 65					F11
 66					F12
 67					Change
 68					BackwardEOF
-69					AltBS
+69					AltBackspace
 70					AltUp
 71					AltDown
 72					AltLeft
 73					AltRight
 74					AltSUp
 75					AltSDown
-76					AltSLeft
-77					AltSRight
+76					AltShiftLeft
+77					AltShiftRight
 78					Alt
 79					CtrlAlt
 ..
 127	3		  KeyDEL	KeyBackspace2
 ..
 256	6					KeyRune
 257	4					KeyUp
```

### Comparing `fzf_bin-0.49.0/fzf/src/tui/ttyname_unix.go` & `fzf_bin-0.50.0/fzf/src/tui/ttyname_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/tui/tui.go` & `fzf_bin-0.50.0/fzf/src/tui/tui.go`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 import (
 	"fmt"
 	"os"
 	"strconv"
 	"time"
 
+	"github.com/junegunn/fzf/src/util"
 	"github.com/rivo/uniseg"
 )
 
 // Types of user action
+//
+//go:generate stringer -type=EventType
 type EventType int
 
 const (
 	Rune EventType = iota
 
 	CtrlA
 	CtrlB
@@ -37,96 +40,100 @@
 	CtrlT
 	CtrlU
 	CtrlV
 	CtrlW
 	CtrlX
 	CtrlY
 	CtrlZ
-	ESC
+	Esc
 	CtrlSpace
 	CtrlDelete
 
 	// https://apple.stackexchange.com/questions/24261/how-do-i-send-c-that-is-control-slash-to-the-terminal
 	CtrlBackSlash
 	CtrlRightBracket
 	CtrlCaret
 	CtrlSlash
 
-	Invalid
-	Resize
-	Mouse
-	DoubleClick
-	LeftClick
-	RightClick
-	SLeftClick
-	SRightClick
-	ScrollUp
-	ScrollDown
-	SScrollUp
-	SScrollDown
-	PreviewScrollUp
-	PreviewScrollDown
+	ShiftTab
+	Backspace
 
-	BTab
-	BSpace
-
-	Del
-	PgUp
-	PgDn
+	Delete
+	PageUp
+	PageDown
 
 	Up
 	Down
 	Left
 	Right
 	Home
 	End
 	Insert
 
-	SUp
-	SDown
-	SLeft
-	SRight
-	SDelete
+	ShiftUp
+	ShiftDown
+	ShiftLeft
+	ShiftRight
+	ShiftDelete
 
 	F1
 	F2
 	F3
 	F4
 	F5
 	F6
 	F7
 	F8
 	F9
 	F10
 	F11
 	F12
 
-	Change
-	BackwardEOF
-	Start
-	Load
-	Focus
-	One
-	Zero
-	Result
-
-	AltBS
+	AltBackspace
 
 	AltUp
 	AltDown
 	AltLeft
 	AltRight
 
-	AltSUp
-	AltSDown
-	AltSLeft
-	AltSRight
+	AltShiftUp
+	AltShiftDown
+	AltShiftLeft
+	AltShiftRight
 
 	Alt
 	CtrlAlt
+
+	Invalid
+
+	Mouse
+	DoubleClick
+	LeftClick
+	RightClick
+	SLeftClick
+	SRightClick
+	ScrollUp
+	ScrollDown
+	SScrollUp
+	SScrollDown
+	PreviewScrollUp
+	PreviewScrollDown
+
+	// Events
+	Resize
+	Change
+	BackwardEOF
+	Start
+	Load
+	Focus
+	One
+	Zero
+	Result
+	Jump
+	JumpCancel
 )
 
 func (t EventType) AsEvent() Event {
 	return Event{t, 0, nil}
 }
 
 func (t EventType) Int() int {
@@ -138,14 +145,39 @@
 }
 
 func (e Event) Comparable() Event {
 	// Ignore MouseEvent pointer
 	return Event{e.Type, e.Char, nil}
 }
 
+func (e Event) KeyName() string {
+	if e.Type >= Invalid {
+		return ""
+	}
+
+	switch e.Type {
+	case Rune:
+		return string(e.Char)
+	case Alt:
+		return "alt-" + string(e.Char)
+	case CtrlAlt:
+		return "ctrl-alt-" + string(e.Char)
+	case CtrlBackSlash:
+		return "ctrl-\\"
+	case CtrlRightBracket:
+		return "ctrl-]"
+	case CtrlCaret:
+		return "ctrl-^"
+	case CtrlSlash:
+		return "ctrl-/"
+	}
+
+	return util.ToKebabCase(e.Type.String())
+}
+
 func Key(r rune) Event {
 	return Event{Rune, r, nil}
 }
 
 func AltKey(r rune) Event {
 	return Event{Alt, r, nil}
 }
@@ -642,15 +674,15 @@
 		Separator:        ColorAttr{colDefault, AttrUndefined},
 		Scrollbar:        ColorAttr{colDefault, AttrUndefined},
 	}
 }
 
 func errorExit(message string) {
 	fmt.Fprintln(os.Stderr, message)
-	os.Exit(2)
+	util.Exit(2)
 }
 
 func init() {
 	Default16 = &ColorTheme{
 		Colored:          true,
 		Input:            ColorAttr{colDefault, AttrUndefined},
 		Fg:               ColorAttr{colDefault, AttrUndefined},
```

### Comparing `fzf_bin-0.49.0/fzf/src/util/atomicbool.go` & `fzf_bin-0.50.0/fzf/src/util/atomicbool.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/util/chars.go` & `fzf_bin-0.50.0/fzf/src/util/chars.go`

 * *Files 2% similar despite different names*

```diff
@@ -174,20 +174,20 @@
 	runes := make([]rune, len(bytes))
 	for idx, b := range bytes {
 		runes[idx] = rune(b)
 	}
 	return runes
 }
 
-func (chars *Chars) CopyRunes(dest []rune) {
+func (chars *Chars) CopyRunes(dest []rune, from int) {
 	if runes := chars.optionalRunes(); runes != nil {
-		copy(dest, runes)
+		copy(dest, runes[from:])
 		return
 	}
-	for idx, b := range chars.slice[:len(dest)] {
+	for idx, b := range chars.slice[from:][:len(dest)] {
 		dest[idx] = rune(b)
 	}
 }
 
 func (chars *Chars) Prepend(prefix string) {
 	if runes := chars.optionalRunes(); runes != nil {
 		runes = append([]rune(prefix), runes...)
```

### Comparing `fzf_bin-0.49.0/fzf/src/util/chars_test.go` & `fzf_bin-0.50.0/fzf/src/util/chars_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/util/eventbox.go` & `fzf_bin-0.50.0/fzf/src/util/eventbox.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/util/eventbox_test.go` & `fzf_bin-0.50.0/fzf/src/util/eventbox_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/util/util.go` & `fzf_bin-0.50.0/fzf/src/util/util.go`

 * *Files 3% similar despite different names*

```diff
@@ -172,7 +172,19 @@
 			if rest == 0 {
 				break
 			}
 		}
 	}
 	return output
 }
+
+// ToKebabCase converts the given CamelCase string to kebab-case
+func ToKebabCase(s string) string {
+	name := ""
+	for i, r := range s {
+		if i > 0 && r >= 'A' && r <= 'Z' {
+			name += "-"
+		}
+		name += string(r)
+	}
+	return strings.ToLower(name)
+}
```

### Comparing `fzf_bin-0.49.0/fzf/src/util/util_test.go` & `fzf_bin-0.50.0/fzf/src/util/util_test.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/util/util_unix.go` & `fzf_bin-0.50.0/fzf/src/util/util_unix.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/src/util/util_windows.go` & `fzf_bin-0.50.0/fzf/src/util/util_windows.go`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/test/fzf.vader` & `fzf_bin-0.50.0/fzf/test/fzf.vader`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/fzf/test/test_go.rb` & `fzf_bin-0.50.0/fzf/test/test_go.rb`

 * *Files 0% similar despite different names*

```diff
@@ -1464,14 +1464,27 @@
     tmux.until { |lines| assert_equal '  1000/1000 (0)', lines[-2] }
     tmux.send_keys 'C-j'
     tmux.until { |lines| assert_equal '5 5', lines[-7] }
     tmux.send_keys '3'
     assert_equal '3', readonce.chomp
   end
 
+  def test_jump_events
+    tmux.send_keys "seq 1000 | #{fzf("--multi --jump-labels 12345 --bind 'ctrl-j:jump,jump:preview(echo jumped to {}),jump-cancel:preview(echo jump cancelled at {})'")}", :Enter
+    tmux.until { |lines| assert_equal '  1000/1000 (0)', lines[-2] }
+    tmux.send_keys 'C-j'
+    tmux.until { |lines| assert_includes lines[-7], '5 5' }
+    tmux.send_keys '3'
+    tmux.until { |lines| assert(lines.any? { _1.include?('jumped to 3') }) }
+    tmux.send_keys 'C-j'
+    tmux.until { |lines| assert_includes lines[-7], '5 5' }
+    tmux.send_keys 'C-c'
+    tmux.until { |lines| assert(lines.any? { _1.include?('jump cancelled at 3') }) }
+  end
+
   def test_pointer
     tmux.send_keys "seq 10 | #{fzf("--pointer '>>'")}", :Enter
     # Assert that specified pointer is displayed
     tmux.until { |lines| assert_equal '>> 1', lines[-3] }
   end
 
   def test_pointer_with_jump
```

### Comparing `fzf_bin-0.49.0/fzf/uninstall` & `fzf_bin-0.50.0/fzf/uninstall`

 * *Files identical despite different names*

### Comparing `fzf_bin-0.49.0/pdm_build.py` & `fzf_bin-0.50.0/pdm_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "fzf"
-VERSION = "0.49.0"
+VERSION = "0.50.0"
 
 
 def is_windows():
     if "GOOS" in os.environ:
         return os.environ["GOOS"] == "windows"
     return sys.platform == "win32"
```

### Comparing `fzf_bin-0.49.0/pyproject.toml` & `fzf_bin-0.50.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fzf-bin"
 description = "fzf - 🌸 A command-line fuzzy finder"
-version = "0.49.0"
+version = "0.50.0"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `fzf_bin-0.49.0/PKG-INFO` & `fzf_bin-0.50.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fzf-bin
-Version: 0.49.0
+Version: 0.50.0
 Summary: fzf - 🌸 A command-line fuzzy finder
-Keywords: fzf tui fuzzy finder
+Keywords: fzf,tui,fuzzy finder
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: User Interfaces
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

