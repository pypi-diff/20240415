# Comparing `tmp/peth-1.0.5.tar.gz` & `tmp/peth-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peth-1.0.5.tar", last modified: Sun Mar 31 01:10:36 2024, max compression
+gzip compressed data, was "peth-1.0.6.tar", last modified: Mon Apr 15 09:17:32 2024, max compression
```

## Comparing `peth-1.0.5.tar` & `peth-1.0.6.tar`

### file list

```diff
@@ -1,79 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.124048 peth-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-31 01:10:30.000000 peth-1.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-31 01:10:30.000000 peth-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-31 01:10:30.000000 peth-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-31 01:10:36.124048 peth-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-03-31 01:10:30.000000 peth-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.112048 peth-1.0.5/peth/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-31 01:10:30.000000 peth-1.0.5/peth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-31 01:10:30.000000 peth-1.0.5/peth/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68734 2024-03-31 01:10:30.000000 peth-1.0.5/peth/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.116048 peth-1.0.5/peth/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18740 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/peth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.116048 peth-1.0.5/peth/core/tracer/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/tracer/txtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-31 01:10:30.000000 peth-1.0.5/peth/core/tracer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.116048 peth-1.0.5/peth/eth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.116048 peth-1.0.5/peth/eth/abi/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/abi/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/abi/abifunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/abi/abitype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/abi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.120048 peth-1.0.5/peth/eth/evm/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/forkchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21798 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/evm/vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/sigs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-03-31 01:10:30.000000 peth-1.0.5/peth/eth/web3ex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.120048 peth-1.0.5/peth/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/logos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/slither.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/solc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-03-31 01:10:30.000000 peth-1.0.5/peth/util/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.124048 peth-1.0.5/peth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-31 01:10:36.000000 peth-1.0.5/peth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-31 01:10:36.000000 peth-1.0.5/peth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 01:10:36.000000 peth-1.0.5/peth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-31 01:10:36.000000 peth-1.0.5/peth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 01:10:36.000000 peth-1.0.5/peth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-31 01:10:30.000000 peth-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 01:10:36.124048 peth-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-31 01:10:30.000000 peth-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.120048 peth-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_bytecode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:36.124048 peth-1.0.5/tests/test_evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_evm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    31412 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_evm/evm_test_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_evm/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_evm/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_evm/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_peth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_sigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-31 01:10:30.000000 peth-1.0.5/tests/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.309538 peth-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 09:17:28.000000 peth-1.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-15 09:17:28.000000 peth-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 09:17:28.000000 peth-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-15 09:17:32.305538 peth-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-15 09:17:28.000000 peth-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.285538 peth-1.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.289538 peth-1.0.6/docs/cn/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/buymeacoffee.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_abi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_bytecode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_conf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_dapp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_eth.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_source.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16207 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_tx.md
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_url.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/cmd_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 09:17:28.000000 peth-1.0.6/docs/cn/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.293538 peth-1.0.6/docs/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/buymeacoffee.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_abi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_bytecode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_conf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_dapp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_eth.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_source.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_tx.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_url.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/cmd_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-15 09:17:28.000000 peth-1.0.6/docs/en/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.293538 peth-1.0.6/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   300459 2024-04-15 09:17:28.000000 peth-1.0.6/docs/img/diffasm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-15 09:17:28.000000 peth-1.0.6/docs/img/peth_eth.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.293538 peth-1.0.6/peth/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 09:17:28.000000 peth-1.0.6/peth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-15 09:17:28.000000 peth-1.0.6/peth/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-15 09:17:28.000000 peth-1.0.6/peth/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/peth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/core/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/txtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-15 09:17:28.000000 peth-1.0.6/peth/core/tracer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.297538 peth-1.0.6/peth/data/bytecode/
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/ExecTxWrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/GetBalanceWrapper.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/MockSender.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/bytecode/MockSender.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/chains.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/contracts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/data/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/arb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/avax.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/bsc.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/eth.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/ftm.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/matic.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens/op.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/data/tokens.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/eth/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/abifunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/abitype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/abi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/eth/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/forkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21801 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/evm/vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/sigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-04-15 09:17:28.000000 peth-1.0.6/peth/eth/web3ex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.301538 peth-1.0.6/peth/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/peth/tools/txexpl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/txexpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/txexpl/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-04-15 09:17:28.000000 peth-1.0.6/peth/tools/txexpl/txexpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/peth/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/logos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/slither.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/solc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-15 09:17:28.000000 peth-1.0.6/peth/util/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/peth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 09:17:32.000000 peth-1.0.6/peth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 09:17:28.000000 peth-1.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.285538 peth-1.0.6/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/scripts/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/scripts/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 09:17:28.000000 peth-1.0.6/scripts/tokens/update_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:17:32.309538 peth-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 09:17:28.000000 peth-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_bytecode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:32.305538 peth-1.0.6/tests/test_evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31412 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/evm_test_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_evm/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_peth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_sigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-15 09:17:28.000000 peth-1.0.6/tests/test_tokens.py
```

### Comparing `peth-1.0.5/LICENSE` & `peth-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/PKG-INFO` & `peth-1.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: peth
-Version: 1.0.5
-Summary: An all-in-one Ethereum SDK and command-line tool, written in Python.
-Home-page: https://github.com/lmy375/peth
-Author: Moon
-License: AGPL-3.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Peth
 
 `Peth` is an all-in-one Ethereum SDK and command-line tool, written in Python. It is designed for developers, smart contract auditors, web3 security researchers, and anyone interested in interacting with EVM-compatible chains with ease.
 
 ```
 ➜ peth
 
@@ -121,8 +110,8 @@
 
 # Buy me a coffee
 
 Send any tokens to [0x2aa75a41805E47eCd94fbBaD84eeF6d1BF21a019](https://debank.com/profile/0x2aa75a41805E47eCd94fbBaD84eeF6d1BF21a019)
 
 # License
 
-This project is licensed under the [AGPL v3](./LICENSE) license.
+This project is licensed under the [AGPL v3](./LICENSE) license.
```

### Comparing `peth-1.0.5/README.md` & `peth-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: peth
+Version: 1.0.6
+Summary: An all-in-one Ethereum SDK and command-line tool written in Python.
+Home-page: https://github.com/lmy375/peth
+Author: Moon
+License: AGPL-3.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: web3==6.15.1
+Requires-Dist: py_solc_x==1.1.1
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: requests==2.28.1
+Requires-Dist: uvicorn==0.29.0
+Requires-Dist: fastapi==0.110.0
+
 # Peth
 
 `Peth` is an all-in-one Ethereum SDK and command-line tool, written in Python. It is designed for developers, smart contract auditors, web3 security researchers, and anyone interested in interacting with EVM-compatible chains with ease.
 
 ```
 ➜ peth
 
@@ -110,8 +127,8 @@
 
 # Buy me a coffee
 
 Send any tokens to [0x2aa75a41805E47eCd94fbBaD84eeF6d1BF21a019](https://debank.com/profile/0x2aa75a41805E47eCd94fbBaD84eeF6d1BF21a019)
 
 # License
 
-This project is licensed under the [AGPL v3](./LICENSE) license.
+This project is licensed under the [AGPL v3](./LICENSE) license.
```

### Comparing `peth-1.0.5/peth/__main__.py` & `peth-1.0.6/peth/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 from argparse import ArgumentParser
 
 from peth.console import PethConsole
-from peth.core import config
+from peth.core.config import config
 from peth.core.log import logger
 from peth.core.peth import Peth
 from peth.eth.utils import convert_value_list
 
 
 def get_args():
     parser = ArgumentParser(
         prog="peth", description="A python Ethereum utilities command-line tool."
     )
 
     parser.add_argument(
         "-c",
         "--chain",
-        choices=list(config.chain_config.keys()),
+        choices=list(config.chains.keys()),
         default="eth",
         help="Chain of the contract.",
     )
 
     parser.add_argument(
         "-r",
         "--rpc-call",
@@ -122,16 +122,16 @@
         project.save()
     elif args.cmd:
         c = PethConsole(peth)
         cmd_str = " ".join(args.cmd)
         for cmd in cmd_str.split(";"):
             c.single_command(cmd)
     else:
-        logger.debug("Config file: %s" % config.CHAIN_CONFIG_PATH)
-        logger.debug("Output path: %s" % config.OUTPUT_PATH)
+        logger.debug("Config file: %s" % config.config_path)
+        logger.debug("Root path: %s" % config.root)
 
         # Default: Open console.
         c = PethConsole(peth)
         c.start_console()
 
 
 if __name__ == "__main__":
```

### Comparing `peth-1.0.5/peth/console.py` & `peth-1.0.6/peth/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 from peth.eth.utils import (
     CoinPrice,
     SelectorDatabase,
     convert_value,
     convert_value_list,
     guess_calldata_types,
     guess_single_calldata,
+    keccak256,
     selector_to_sigs,
-    sha3_256,
 )
 from peth.util import diff
 from peth.util.graph import ContractRelationGraph
 from peth.util.logos import random_logo
 
-from .core import config
+from .core.config import config
 from .core.log import logger, logging
 
 
 class PethConsole(cmd.Cmd):
     """
     An interactive command console to use peth tools.
     """
@@ -209,15 +209,15 @@
             print("     Block number:", self.peth.web3.eth.block_number)
         except Exception:
             pass
         print("  RPC:", self.peth.rpc_url)
         print("  API:", self.peth.api_url)
         print("  Address:", self.peth.address_url)
 
-        if arg in config.chain_config:
+        if arg in config.chains:
             old_sender = self.peth.sender
             self.peth = Peth.get_or_create(arg)
             self.peth.sender = old_sender  # Keep the sender value.
             print("Changed:")
             print("  Chain:", self.peth.chain)
             try:
                 print("     Chain ID:", self.peth.web3.eth.chain_id)
@@ -225,31 +225,30 @@
             except Exception:
                 pass
             print("  RPC:", self.peth.rpc_url)
             print("  API:", self.peth.api_url)
             print("  Address:", self.peth.address_url)
 
         else:
-            print("Supported chains: %s" % ", ".join(config.chain_config.keys()))
+            print("Supported chains: %s" % ", ".join(config.chains.keys()))
 
     def do_config(self, arg):
         """
         config: Print current settings.
-        config <key> <value>: Change settings.
+        config raw: Print raw settings.
+        config <section> <key> <value>: Change settings.
         """
-        args = self._parse_args(arg)
+        args = arg.split()
         if len(args) == 0:
             config.print_config()
-            print("\nUse `config key value` to change settings.")
+        elif args[0] == "raw":
+            config.print_ini()
         else:
-            k, v = args
-            if k in config.__dict__:
-                config.__dict__[k] = v
-            else:
-                print("Not valid config key.")
+            assert len(args) == 3
+            config.cfg.set(args[0], args[1], args[2])
 
     def do_sender(self, arg):
         """
         sender <addr> : Set default sender in eth_call.
         """
         print("Current:", self.peth.sender)
         if Web3.isAddress(arg):
@@ -275,15 +274,15 @@
     ##################################################################
     # Chain-independent utility commands.
 
     def do_keccak256(self, arg):
         """
         keccak256 <string> : Calculate Keccak256 hash.
         """
-        print(sha3_256(bytes(arg.strip(), "ascii", "ignore")).hex())
+        print(keccak256(bytes(arg.strip(), "ascii", "ignore")).hex())
 
     def do_int(self, arg):
         """
         int <number> : Print number.
         """
         arg = arg.replace(",", "")
         if re.findall("[xXa-fA-f]", arg):
@@ -296,24 +295,81 @@
         print("Value/1e8  (BTC): %s" % (value / 1e8))
         print("Value/1e9  (GWei): %s" % (value / 1e9))
         print("Value/1e18 (Ether): %s" % (value / 1e18))
         print("Hex: %#x" % value)
         print("Hex(Address): %#0.40x" % value)
         print("Hex(Uint256): %0.64x" % value)
 
-    def do_common_addresses(self, arg):
+    def do_addresses(self, arg):
         """
-        common_addresses: Print some common addresses.
+        addresses: Print some common contract addresses.
         """
 
         print("%-40s %-10s %s" % ("Name", "Chain", "Address"))
-        for name in config.contracts_config:
-            chain, addr = config.contracts_config[name]
+        for name in config.contracts:
+            chain, addr = config.contracts[name]
             print("%-40s %-10s %s" % (name, chain, addr))
 
+    def do_tokens(self, arg):
+        """
+        tokens: Print tokens.
+        tokens <search text>: Find tokens.
+        """
+        tokens = config.tokens[self.peth.chain]
+        if arg:
+            search_text = arg
+        else:
+            search_text = ""
+
+        print(
+            "%-30s %-10s %-45s %8s %15s"
+            % ("Name", "Symbol", "Address", "Decimals", "Price")
+        )
+        for token in tokens:
+            line = "%-30s %-10s %-45s %8s %15s" % (
+                token["name"],
+                token["symbol"],
+                token["address"],
+                token["decimals"],
+                token["price"],
+            )
+            if search_text.lower() in line.lower():
+                print(line)
+
+    def do_portfolio(self, arg):
+        """
+        portfolio <address>: Print balance of common tokens (like debank)
+        """
+        addr = self._parse_args(arg, "address")
+
+        portfolio = self.peth.get_portfolio([addr])
+        infos = portfolio.get(addr.lower(), [])
+
+        total = 0
+        lines = []
+        for asset in infos:
+            total += asset["usd"]
+            line = "%-30s\t%-10s\t%-45s\t%-10s\t%-20s\t%-20s" % (
+                asset["info"]["name"],
+                asset["info"]["symbol"],
+                asset["info"]["address"],
+                asset["info"]["price"],
+                asset["balance"],
+                asset["usd"],
+            )
+            lines.append(line)
+
+        print("Total: $%0.2f" % total)
+        print(
+            "%-30s\t%-10s\t%-45s\t%-10s\t%-20s\t%-20s"
+            % ("Name", "Symbol", "Address", "Price", "Balance", "USD")
+        )
+        for line in lines:
+            print(line)
+
     def do_sh(self, arg):
         """
         Run system shell command.
         """
         os.system(arg)
 
     def do_py(self, arg):
@@ -452,15 +508,15 @@
         print("Key:", repr(password))
         print("Count:", count)
 
         password = password.encode("utf-8")
         for i in range(count):
             if (i % 100000) == 0:
                 print("    %d %% \r" % (100 * i / count), end="")
-            password = sha3_256(password)
+            password = keccak256(password)
 
         pk = HexBytes(password).hex()
 
         print("Private Key:", pk)
         print("Address:", Account.from_key(pk).address)
 
     ##################################################################
@@ -874,30 +930,31 @@
                     gas_price_max = tx.gasPrice
                 if tx.gasPrice < gas_price_min:
                     gas_price_min = tx.gasPrice
 
             gas_used_avg = gas_used_total / tx_cnt
             gas_price_avg = gas_price_total / tx_cnt
 
-            gas_desc = "%d/%d/%d" % (gas_used_avg, gas_used_min, gas_used_max)
+            gas_desc = "%8d < %8d < %8d" % (gas_used_min, gas_used_avg, gas_used_max)
             GWEI = 10**9
-            gas_price_desc = "%d/%d/%d" % (
-                gas_price_avg / GWEI,
+            gas_price_desc = "%0.2f < %0.2f < %0.2f" % (
                 gas_price_min / GWEI,
+                gas_price_avg / GWEI,
                 gas_price_max / GWEI,
             )
+            tx_cnt = "%4d" % tx_cnt
             print(
-                f"\t{tag} - Block {block.number}, {tx_cnt} txns, gas {gas_desc}, {gas_used_rate} used rate, price {gas_price_desc} gwei"
+                f"\t{tag} - Block {block.number}, {tx_cnt} txns, gas {gas_desc}, {gas_used_rate} used, price {gas_price_desc} Gwei"
             )
 
         cur = get_block("latest")
 
         while True:
             print(datetime.now())
-            print_block("latest", cur)
+            print_block("latest ", cur)
 
             while True:
                 pending = get_block("pending")
 
                 if (
                     pending.number and pending.number <= cur.number
                 ):  # Not valid pending.
@@ -1695,17 +1752,17 @@
             chain1,
             addr1,
             chain2,
             addr2,
             similarity,
         )
 
-        if not os.path.isdir(config.DIFF_PATH):
-            os.makedirs(config.DIFF_PATH)
-        output_filename = os.path.join(config.DIFF_PATH, output_filename)
+        if not os.path.isdir(config.diff_path):
+            os.makedirs(config.diff_path)
+        output_filename = os.path.join(config.diff_path, output_filename)
         open(output_filename + ".html", "w").write(buf)
         print("Written to " + output_filename + ".html")
 
     ##################################################################
     # Contract source tools.
 
     def _get_name(self, addr):
@@ -1754,27 +1811,27 @@
             return
 
         self._print_json(info)
 
         abis = info["ABI"]
         try:
             abi_json = json.loads(abis)
-            print(" ", "=== VIEWS ===")
+            print(" ", "=== CALLED ===")
             contract = self.web3.eth.contract(address=addr, abi=abi_json)
 
             others = []
             for item in abi_json:
                 if item["type"] == "fallback":
                     others.append("fallback()")
                     break
 
             for func in contract.all_functions():
                 sig = Signature.from_abi(func.abi)
 
-                if sig.is_view and len(sig.inputs) == 0:
+                if len(sig.inputs) == 0:
                     try:
                         ret = func().call()
                     except Exception as e:
                         print(
                             " ",
                             f"[*] Error in calling {sig}",
                             e,
@@ -1813,16 +1870,16 @@
             graph.print_assets()
             print("=====================")
             print(graph.dump())
             print("=====================")
             print("Open http://relation-graph.com/#/options-tools and paste the json.")
 
     def _check_alias(self, alias):
-        if alias in config.contracts_config:
-            return config.contracts_config[alias]
+        if alias in config.contracts:
+            return config.contracts[alias]
         else:
             return self.peth.chain, alias
 
     def do_diff(self, arg):
         """
         diff <addr1/alias> <addr2/alias>
         diff <chain1> <addr1> <chain2> <addr2>
@@ -1862,15 +1919,15 @@
         """
         args = arg.split()
         addr = args[0]
         assert Web3.isAddress(addr), f"{addr} is not a valid address."
         if len(args) > 1:
             output_dir = args[1]
             if "/" not in output_dir:
-                output_dir = os.path.join(config.OUTPUT_PATH, output_dir)
+                output_dir = os.path.join(config.output_path, output_dir)
         else:
             output_dir = None
 
         ret = self.peth.scan.download_json(addr, output_dir)
         if ret:
             print(f"Downloaded as {ret}")
         else:
@@ -1882,15 +1939,15 @@
         """
         args = arg.split()
         addr = args[0]
         assert Web3.isAddress(addr), f"{addr} is not a valid address."
         if len(args) > 1:
             output_dir = args[1]
             if "/" not in output_dir:
-                output_dir = os.path.join(config.OUTPUT_PATH, output_dir)
+                output_dir = os.path.join(config.output_path, output_dir)
         else:
             output_dir = None
 
         ret = self.peth.scan.download_source(addr, output_dir)
         if ret:
             for i in ret:
                 print(f"Downloaded {i}")
@@ -1942,18 +1999,18 @@
         code_list2 = self._code_to_list(code2)
         s = difflib.SequenceMatcher(None, code_list1, code_list2)
         similarity = s.ratio()
         print("Similarity %0.2f%%" % (similarity * 100))
 
         d = difflib.HtmlDiff()
         buf = d.make_file(code_list1, code_list2)
-        if not os.path.exists(config.DIFF_PATH):
-            os.makedirs(config.DIFF_PATH)
+        if not os.path.exists(config.diff_path):
+            os.makedirs(config.diff_path)
 
-        path = os.path.join(config.DIFF_PATH, "bytecode_diff.html")
+        path = os.path.join(config.diff_path, "bytecode_diff.html")
         open(path, "w").write(buf)
         print("Written to " + path)
 
     def do_url(self, arg):
         """
         url <addr> : Open blockchain explorer of the address.
         url <tx> : Open tx explorer of the tx.
```

### Comparing `peth-1.0.5/peth/core/analysis.py` & `peth-1.0.6/peth/core/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import json
 import os
 
 from web3 import Web3
 
-from peth.core import config
+from peth.core.config import config
 from peth.core.log import logger
 from peth.eth.bytecode import Code
 from peth.eth.sigs import Signature, Signatures
 from peth.eth.utils import ZERO_ADDRESS, selector_to_sigs
 from peth.util.graph import ContractRelationGraph
 from peth.util.markdown import make_attr_table, make_table
 
@@ -81,15 +81,15 @@
             if not self.verified:
                 self.name = "Unverified Contract"
 
             self.analyze_unverified_contract()
             self.analyze_extra()
 
             # Can be slow.
-            if config.ENABLE_SLITHER:
+            if config.enable_slither:
                 self.analyze_slither()
 
         logger.debug("%s %s done.", self.addr, self.name)
 
     def analyze_verified_contract(self):
         info = self.peth.scan.get_contract_info(self.addr, False)
         if info is None:
@@ -154,15 +154,16 @@
                         self.properties[f"{sig.name}[{i}]"] = ret[i]
 
     def analyze_unverified_contract(self):
         addr = self.addr
         if Web3.isAddress(self.implmentation):
             # If this is a proxy, analyze the implmentation code.
             addr = self.implmentation
-        self.selectors, self.hardcoded_addresses = self.peth.analyze_bytecode(addr)
+        self.selectors = self.peth.get_selectors(addr)
+        self.hardcoded_addresses = self.peth.get_hardcoded_addresses(addr)
         logger.debug(
             "%d selectors, %s hardcode addresses",
             len(self.selectors),
             len(self.hardcoded_addresses),
         )
 
     def __collect_view_values(self, contract, sigs, do_check=True):
@@ -544,13 +545,13 @@
                 g.add_relation(analysis.addr, target, name)
         return g
 
     def save(self) -> None:
         time_tag = datetime.datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         filename = "Report_%s_%s.md" % (time_tag, self.addresses[0][:10])
 
-        report_dir = config.REPORT_PATH
+        report_dir = config.report_path
         if not os.path.exists(report_dir):
             os.makedirs(report_dir)
         path = os.path.join(report_dir, filename)
         open(path, "w").write(self.to_markdown())
         logger.info("Report saved as %s.", path)
```

### Comparing `peth-1.0.5/peth/core/tracer/tracer.py` & `peth-1.0.6/peth/core/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/core/tracer/txtrace.py` & `peth-1.0.6/peth/core/tracer/txtrace.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/core/tracer/utils.py` & `peth-1.0.6/peth/core/tracer/utils.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/abi/abi.py` & `peth-1.0.6/peth/eth/abi/abi.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/abi/abifunc.py` & `peth-1.0.6/peth/eth/abi/abifunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,24 +92,29 @@
     @property
     def selector(self) -> bytes:
         return HexBytes(keccak(self.signature.encode())[:4])
 
     def __repr__(self):
         return self.full
 
-    def encode_input(self, args=[]):
-        return HexBytes(self.selector + HexBytes(abi_encode(self.input_types, args)))
+    def encode_input(self, args=[], include_selector=True) -> HexBytes:
+        calldata = HexBytes(abi_encode(self.input_types, args))
+        if include_selector:
+            calldata = HexBytes(self.selector) + calldata
+        return HexBytes(calldata)
 
     def decode_input(self, calldata):
         calldata = HexBytes(calldata)
-        assert calldata[0:4] == self.selector, "select not match"
+        assert (
+            calldata[0:4] == self.selector
+        ), f"selector not match: {calldata[0:4]} {self.selector}"
         calldata = calldata[4:]
         return abi_decode(self.input_types, calldata)
 
-    def encode_output(self, rets=[], auto_tuple=True):
+    def encode_output(self, rets=[], auto_tuple=True) -> HexBytes:
         if auto_tuple and len(self.outputs) == 1:
             rets = [rets]
         return HexBytes(abi_encode(self.output_types, rets))
 
     def decode_output(self, retdata, auto_one=True):
         if len(self.outputs) == 0:
             # If no output type, return the entire bytes.
@@ -146,14 +151,18 @@
         # Skip function name if provided in indexes.
         if indexes[0] == self.name:
             indexes = indexes[1:]
 
         arg, value = get_item_value_by_index(indexes[0], self.inputs, values)
         return arg.extract_value(indexes[1:], value)
 
+    def extract_calldata(self, indexes, calldata):
+        values = self.decode_input(calldata)
+        return self.extract_value(indexes, values)
+
     def map_values(self, values):
         assert len(values) == len(self.inputs), "Value not match arguments size"
 
         r = []
         for arg, value in zip(self.inputs, values):
             r.append(arg.map_values(value))
         return r
```

### Comparing `peth-1.0.5/peth/eth/abi/abitype.py` & `peth-1.0.6/peth/eth/abi/abitype.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         self._is_dynamic = None
 
     @property
     def type_str(self) -> str:
         if self.is_tuple:
             s = "("
-            s += ",".join(str(i.type) for i in self.components)
+            s += ",".join(i.type_str for i in self.components)
             s += ")"
             assert self.type.startswith("tuple")
             s += self.type.strip("tuple")
             return s
         else:
             return self.type
```

### Comparing `peth-1.0.5/peth/eth/abi/utils.py` & `peth-1.0.6/peth/eth/abi/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 def get_item_by_index(index: str, items: list, only_int=False):
     assert type(items) in (tuple, list)
     try:
         # For int index
         i = int(index)
         if i < 0:
             i = len(items) + i
-        assert i < len(items), "tuple index out-of-bound"
+        assert i < len(items), f"tuple index out-of-bound {i} >= {len(items)}"
         return items[i]
     except ValueError:
         if not only_int:
             # For non-int index
             for item in items:
                 if item.name == index:
                     return item
```

### Comparing `peth-1.0.5/peth/eth/bytecode.py` & `peth-1.0.6/peth/eth/bytecode.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/contract.py` & `peth-1.0.6/peth/eth/contract.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/chain.py` & `peth-1.0.6/peth/eth/evm/chain.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/contract.py` & `peth-1.0.6/peth/eth/evm/contract.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/forkchain.py` & `peth-1.0.6/peth/eth/evm/forkchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import atexit
 import os
 import pickle
 
 from web3 import Web3
 
 from peth import Peth
-from peth.core import config
+from peth.core.config import config
 
 
 class ForkChain(object):
 
     def __init__(self, web3, fix_block_number: int = 0) -> None:
         self.web3 = web3
 
@@ -17,19 +17,19 @@
             self.fix_block_number = fix_block_number
         else:
             self.fix_block_number = web3.eth.block_number  # Fix to current.
 
         self.chainid = web3.eth.chain_id
         self.block = web3.eth.get_block(self.fix_block_number - 1)
 
-        if not os.path.exists(config.EVM_OUTPUT_PATH):
-            os.makedirs(config.EVM_OUTPUT_PATH)
+        if not os.path.exists(config.evm_cache_path):
+            os.makedirs(config.evm_cache_path)
 
         self._cache_file_name = os.path.join(
-            config.EVM_OUTPUT_PATH,
+            config.evm_cache_path,
             "fork_%s_%s.pickle" % (self.chainid, self.fix_block_number),
         )
 
         self.addresses = {}
 
         self.balances = {}
         self.nonces = {}
```

### Comparing `peth-1.0.5/peth/eth/evm/inspector.py` & `peth-1.0.6/peth/eth/evm/inspector.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/receipt.py` & `peth-1.0.6/peth/eth/evm/receipt.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/trace.py` & `peth-1.0.6/peth/eth/evm/trace.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/transaction.py` & `peth-1.0.6/peth/eth/evm/transaction.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/evm/utils.py` & `peth-1.0.6/peth/eth/evm/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import rlp
 from web3 import Web3
 
-from ..utils import sha3_256
+from ..utils import keccak256
 
 UINT_256_MAX = 2**256 - 1
 UINT_256_CEILING = 2**256
 UINT_255_MAX = 2**255 - 1
 UINT_255_CEILING = 2**255
 UINT_160_MAX = 2**160 - 1
 
@@ -53,24 +53,24 @@
 def uint_to_address(i: int) -> int:
     return Web3.toChecksumAddress(int.to_bytes(i, 20, "big")).lower()
 
 
 def generate_contract_address(address: str, nonce: int):
     return uint_to_address(
         int.from_bytes(
-            sha3_256(rlp.encode([address_to_bytes(address), nonce]))[12:], "big"
+            keccak256(rlp.encode([address_to_bytes(address), nonce]))[12:], "big"
         )
     )
 
 
 def generate_safe_contract_address(address: str, salt: int, call_data: bytes):
     return uint_to_address(
         int.from_bytes(
-            sha3_256(
+            keccak256(
                 b"\xff"
                 + address_to_bytes(address)
                 + uint_to_data(salt)
-                + sha3_256(call_data)
+                + keccak256(call_data)
             )[12:],
             "big",
         )
     )
```

### Comparing `peth-1.0.5/peth/eth/evm/vm.py` & `peth-1.0.6/peth/eth/evm/vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .exceptions import InvalidHandlerError, InvalidJumpDestination, VMExecutionError
 from .receipt import Receipt
 from .transaction import Transaction
 from .utils import (
     UINT_256_MAX,
     address_to_uint,
     data_to_uint,
-    sha3_256,
+    keccak256,
     to_int256,
     to_uint256,
     uint_to_address,
     uint_to_data,
 )
 
 
@@ -336,15 +336,15 @@
 
     #
     # Sha3
     #
     def _sha3(self):
         offset, size = self._stack_pop_values(2)
         data = self._read_memory(offset, size)
-        hash = sha3_256(data)
+        hash = keccak256(data)
         v = data_to_uint(hash)
         self._stack_push(v)
         self._trace(f"{data.hex()} => {hash.hex()}")
 
     #
     # Environment Information
     #
@@ -445,15 +445,15 @@
         self._trace(f"calldatacopy({data_start}, {size}) => {mem_start}")
 
     def _extcodehash(self):
         v = self._stack_pop()
         addr = uint_to_address(v)
         code = self.chain.get_code(addr)
         if code:
-            v = data_to_uint(sha3_256(code))
+            v = data_to_uint(keccak256(code))
         else:
             v = 0
 
         self._stack_push(v)
         self._trace(f"extcodehash({addr}) => {hex(v)}")
 
     #
```

### Comparing `peth-1.0.5/peth/eth/opcodes.py` & `peth-1.0.6/peth/eth/opcodes.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/scan.py` & `peth-1.0.6/peth/eth/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 import os
 import re
 import time
 
 import requests
 from web3 import Web3
 
-from ..core import config
+from ..core.config import config
 
 
 class ScanAPI(object):
 
     cache = {}
 
     def __init__(self, api_url) -> None:
         """
         Do NOT use this, use get_or_create instead to
         bypass API rate.
         """
         self.api_url = api_url
 
         self._cache_path = os.path.join(
-            config.CACHE_PATH, re.findall("//(.*)?/", api_url)[0]
+            config.contracts_cache_path, re.findall("//(.*)?/", api_url)[0]
         )
         if not os.path.exists(self._cache_path):
             os.makedirs(self._cache_path)
 
         self._source_path = os.path.join(
-            config.OUTPUT_PATH, "source", re.findall("//(.*)?/", self.api_url)[0]
+            config.sources_path, re.findall("//(.*)?/", self.api_url)[0]
         )
 
     @classmethod
     def get_or_create(cls, api_url):
         if api_url not in cls.cache:
             cls.cache[api_url] = cls(api_url)
         return cls.cache[api_url]
 
     @classmethod
     def get_or_create_by_chain(cls, chain):
         assert (
-            chain in config.chain_config.keys()
-        ), f"Invalid chain {chain}. See config.json."
-        return ScanAPI.get_or_create(config.chain_config[chain][1])
+            chain in config.chains.keys()
+        ), f"Invalid chain {chain}. See {config.chains_path}."
+        return ScanAPI.get_or_create(config.chains[chain][1])
 
     @classmethod
     def get_source_by_chain(cls, chain, addr):
         return ScanAPI.get_or_create_by_chain(chain).get_source(addr)
 
     def _cache_get(self, id: str):
         path = os.path.join(self._cache_path, id)
@@ -62,15 +62,15 @@
         try:
             r = requests.get(url)
             d = r.json()
 
             # retry.
             if "Max rate limit reached" in d["result"]:
                 # API request limit.
-                time.sleep(config.SCAN_API_INTERVAL)
+                time.sleep(config.scan_api_interval)
                 return self.get(url)
 
             assert d["status"] == "1", d
             assert type(d["result"]) is list, d["result"]
             return d["result"]
         except Exception as e:
             print("[!] Etherscan API fail.", e, url)
@@ -265,15 +265,15 @@
             },
         }
         return contract_name, version, json_input
 
     def download_json(self, addr, output_dir=None):
         if not output_dir:
             output_dir = os.path.join(
-                config.OUTPUT_PATH, "json", re.findall("//(.*)?/", self.api_url)[0]
+                config.output_path, "json", re.findall("//(.*)?/", self.api_url)[0]
             )
 
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         ret = self.get_standard_json_input(addr)
         if ret:
```

### Comparing `peth-1.0.5/peth/eth/sigs.py` & `peth-1.0.6/peth/eth/sigs.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/eth/utils.py` & `peth-1.0.6/peth/eth/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import atexit
 import json
 import os
 import re
 from typing import Any, Dict, List, Tuple
 
 import requests
+from eth_hash.auto import keccak
 from web3 import Web3
 
-from peth.core import config
+from peth.core.config import config
 from peth.core.log import logger
 
 ZERO_ADDRESS = "0x0000000000000000000000000000000000000000"
+UINT256_MAX = 2**256 - 1
 
-try:
-    from Crypto.Hash import keccak
 
-    def sha3_256(x):
-        return keccak.new(digest_bits=256, data=x).digest()
-
-except ImportError:
-    import sha3 as _sha3
-
-    def sha3_256(x):
-        return _sha3.keccak_256(x).digest()
+def keccak256(x):
+    return keccak(x)
 
 
 def func_selector(func_sig: str):
-    return sha3_256(bytes(func_sig, "ascii", "ignore"))[:4]
+    return keccak256(bytes(func_sig, "ascii", "ignore"))[:4]
 
 
 # from: https://github.com/ethereum/eth-utils/blob/master/eth_utils/abi.py
 def collapse_if_tuple(abi: Dict[str, Any]) -> str:
     """
     Converts a tuple from a dict to a parenthesized list of its types.
     >>> from eth_utils.abi import collapse_if_tuple
@@ -66,28 +60,28 @@
 class SelectorDatabase(object):
 
     single_instance = None
 
     def __init__(self) -> None:
         self.db = {}
 
-        if not os.path.exists(config.SIG_DB_PATH):
+        if not os.path.exists(config.sig_db_path):
             try:
                 logger.info(
-                    "Downloading SelectorDatabase from %s ..." % config.SIG_DB_URL
+                    "Downloading SelectorDatabase from %s ..." % config.sig_db_url
                 )
-                r = requests.get(config.SIG_DB_URL)
+                r = requests.get(config.sig_db_url)
                 self.db = r.json()
                 logger.info("OK")
             except Exception as e:
                 logger.warn("SelectorDatabase init failed. %s" % e)
-            logger.debug("Load sig db from %s" % config.SIG_DB_URL)
+            logger.debug("Load sig db from %s" % config.sig_db_url)
         else:
-            self.db = json.load(open(config.SIG_DB_PATH))
-            logger.debug("Load sig db from %s" % config.SIG_DB_PATH)
+            self.db = json.load(open(config.sig_db_path))
+            logger.debug("Load sig db from %s" % config.sig_db_path)
 
         atexit.register(self.save)
 
     def _normalize_selector(self, selector, with_prefix=False):
         """
         Return hex format.
         """
@@ -206,16 +200,16 @@
         except Exception:
             if only_one:
                 return None
             else:
                 return []
 
     def save(self):
-        json.dump(self.db, open(config.SIG_DB_PATH, "w"))
-        logger.debug("Save sig db to %s" % config.SIG_DB_PATH)
+        json.dump(self.db, open(config.sig_db_path, "w"))
+        logger.debug("Save sig db to %s" % config.sig_db_path)
 
     @classmethod
     def get(cls):
         if SelectorDatabase.single_instance is None:
             # This can be a little slow as it downloads data from github.
             SelectorDatabase.single_instance = SelectorDatabase()
         return SelectorDatabase.single_instance
```

### Comparing `peth-1.0.5/peth/eth/web3ex.py` & `peth-1.0.6/peth/eth/web3ex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import json
+import os
 import time
+from typing import List, Tuple
 
 from eth_account import Account
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 
 from peth.core.log import logger
 from peth.util.solc import compile_with_eth_call
 
+from ..core.config import DATA_DIR
 from . import utils
 from .abi import ABI, ABIFunction
 from .contract import Contract
 from .scan import ScanAPI
 
 
 class Web3Ex(object):
@@ -132,24 +136,25 @@
             sig = utils.selector_to_sigs(selector, True)
             if sig:
                 return ABIFunction(sig)
 
         # No signature found.
         return None
 
-    def eth_call_raw(self, to, data, sender=None, value: int = 0):
+    def eth_call_raw(self, to=None, data=b"", sender=None, value: int = 0):
         if not sender:
             sender = self.sender
 
         tx = {
             "from": sender,
-            "to": to,
             "data": HexBytes(data).hex(),
             "value": hex(value),
         }
+        if to:
+            tx["to"] = to
         return self.rpc_call("eth_call", [tx, "latest"])
 
     def _sig_name_to_func(self, to, sig_or_name):
         if type(sig_or_name) is str:
             if "(" in sig_or_name:
                 func = ABIFunction(sig_or_name)
             else:
@@ -203,71 +208,62 @@
                     "Web3Ex.call_contract Call %s %s %s" % (contract, sig_or_name, e)
                 )
             return None
 
     # Alias
     call = call_contract
 
-    def run_solidity(self, code):
-        """
-        Compile and run the Executor.run() code with Wrapper contract constructor.
-        """
+    def populate_tx(self, tx, sender=None, gas_price_rate=1.2, gas_limit_rate=1.2):
+        if not sender:
+            sender = self.signer.address
 
-        assert (
-            "Executor" in code and "run" in code
-        ), "Executor.run() is not defined in such code."
+        assert sender, "sender not set"
 
-        output = compile_with_eth_call(code)
-        calldata = output["<stdin>:Wrapper"]["bin"]
-        abi = None
-        for abi in output["<stdin>:Executor"]["abi"]:
-            if abi["type"] == "function" and abi["name"] == "run":
-                break
+        if "from" not in tx:
+            tx["from"] = sender
 
-        if abi is None:
-            raise Exception("Executor.run() not found in the code")
+        if "chainId" not in tx:
+            tx["chainId"] = self.web3.eth.chain_id
 
-        func = ABIFunction(abi)
+        if "nonce" not in tx:
+            tx["nonce"] = self.web3.eth.get_transaction_count(sender)
 
-        tx = {"from": self.sender, "data": "0x" + calldata}
+        if "gas" not in tx:
+            gas = self.web3.eth.estimate_gas(tx)
+            tx["gas"] = int(gas * gas_limit_rate)
 
-        # print(tx)
-        r = self.rpc_call("eth_call", [tx, "latest"])
-        # print(r)
-        try:
-            ret = func.decode_output(r)
-            if ret is not None:
-                return ret
-            else:
-                return r
-        except Exception:
-            return r
+        if "gasPrice" not in tx:
+            gas_price = rpc_gas_price_strategy(self.web3)
+            tx["gasPrice"] = int(gas_price * gas_price_rate)
+
+        return tx
+
+    def get_tx_gas_fee(self, tx):
+        if "gas" not in tx or "gasPrice" not in tx:
+            self.populate_tx(tx)
+
+        return int(tx["gasPrice"] * tx["gas"])
 
     def send_transaction(self, data=None, to=None, value=None, dry_run=False, wait=0):
         assert self.signer, "send_transaction: signer not set."
 
-        tx = {"from": self.signer.address}
-
+        tx = {}
         if data:
             tx["data"] = data
 
         if to:
             tx["to"] = Web3.toChecksumAddress(to)
 
         if value:
             tx["value"] = value
 
-        tx["chainId"] = self.web3.eth.chain_id
-        tx["nonce"] = self.web3.eth.get_transaction_count(self.signer.address)
-
-        gas = self.web3.eth.estimate_gas(tx)
-        tx["gas"] = int(gas * 1.2)
+        self.send_tx(self, tx, dry_run, wait)
 
-        gas_price = rpc_gas_price_strategy(self.web3)
-        tx["gasPrice"] = int(gas_price * 1.2)
+    def send_tx(self, tx, dry_run=False, wait=0):
+        self.populate_tx(tx)
         signed_tx = self.signer.sign_transaction(tx)
         if dry_run:
             return tx, signed_tx
 
         current_block = self.web3.eth.block_number
         txid = self.web3.eth.send_raw_transaction(signed_tx.rawTransaction)
         if not wait:
@@ -323,7 +319,110 @@
     def contract(self, address, abi: str | ABI | dict = None):
         if abi is None:
             abi = self.scan.get_abi(address)
         elif self.web3.isAddress(str(abi)):
             abi = self.scan.get_abi(str(abi))
 
         return Contract(self, address, abi)
+
+    def run_solidity(self, code):
+        """
+        Compile and run the Executor.run() code with Wrapper contract constructor.
+        """
+
+        assert (
+            "Executor" in code and "run" in code
+        ), "Executor.run() is not defined in such code."
+
+        output = compile_with_eth_call(code)
+        calldata = output["<stdin>:Wrapper"]["bin"]
+        abi = None
+        for abi in output["<stdin>:Executor"]["abi"]:
+            if abi["type"] == "function" and abi["name"] == "run":
+                break
+
+        if abi is None:
+            raise Exception("Executor.run() not found in the code")
+
+        func = ABIFunction(abi)
+
+        tx = {"from": self.sender, "data": "0x" + calldata}
+
+        # print(tx)
+        r = self.rpc_call("eth_call", [tx, "latest"])
+        # print(r)
+        try:
+            ret = func.decode_output(r)
+            if ret is not None:
+                return ret
+            else:
+                return r
+        except Exception:
+            return r
+
+    def get_token_balances(
+        self, tokens: List[str], users: List[str], min_balance=1
+    ) -> List[Tuple[str, str, int]]:
+        """
+        Check token balances of users.
+            token: ERC20 addresses. address(0) for ETH.
+            users: user addresses.
+            min_balance: Do not return if balance is smaller than min_balance.
+        Returns
+            [(token, user, balance), ]
+        """
+        BYTECODE_PATH = os.path.join(DATA_DIR, "bytecode", "GetBalanceWrapper.json")
+        ABI_PATH = os.path.join(DATA_DIR, "bytecode", "MockSender.json")
+        code = HexBytes(json.load(open(BYTECODE_PATH))["bytecode"])
+        fn = ABI(json.load(open(ABI_PATH))["abi"]).getBalance
+
+        data = fn.encode_input([tokens, users, min_balance], False)
+
+        output = self.eth_call_raw(data=code + data)
+        _, balances = fn.decode_output(output)
+        return balances
+
+    def multicall_raw(
+        self, txs: List[Tuple[str, HexBytes, int]]
+    ) -> List[Tuple[bool, HexBytes]]:
+        """
+        Call multiple transactions.
+            txs: [(to, data, value), ..]
+        Returns:
+            [(status, returndata), ..]
+        """
+        BYTECODE_PATH = os.path.join(DATA_DIR, "bytecode", "ExecTxWrapper.json")
+        ABI_PATH = os.path.join(DATA_DIR, "bytecode", "MockSender.json")
+        code = HexBytes(json.load(open(BYTECODE_PATH))["bytecode"])
+        fn = ABI(json.load(open(ABI_PATH))["abi"]).execTxs
+
+        data = fn.encode_input([txs], False)
+
+        output = self.eth_call_raw(data=code + data)
+        _, balances = fn.decode_output(output)
+        return balances
+
+    def multicall_from(
+        self, txs: List[Tuple[str, HexBytes, int]], sender=None
+    ) -> List[Tuple[bool, HexBytes]]:
+        """
+        Simulate multiple transactions with the same sender using `eth_call override`
+        Ref: https://geth.ethereum.org/docs/interacting-with-geth/rpc/ns-eth#eth-call
+        """
+        BYTECODE_PATH = os.path.join(DATA_DIR, "bytecode", "MockSender.json")
+        ABI_PATH = os.path.join(DATA_DIR, "bytecode", "MockSender.json")
+
+        code = json.load(open(BYTECODE_PATH))["deployedBytecode"]
+        fn = ABI(json.load(open(ABI_PATH))["abi"]).execTxs
+
+        if sender is None:
+            sender = self.sender
+
+        calldata = fn.encode_input([txs])
+
+        tx = {"to": sender, "data": calldata.hex()}
+
+        output = self.rpc_call(
+            "eth_call", [tx, "latest", {sender: {"code": code}}]  # Or pending?
+        )
+        _, results = fn.decode_output(output)
+        return results
```

### Comparing `peth-1.0.5/peth/util/diff.py` & `peth-1.0.6/peth/util/diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 
 from web3 import Web3
 
-from peth.core import config
+from peth.core.config import config
 from peth.core.peth import Peth
 from peth.eth.scan import ScanAPI
 
 from .source import ContractSource
 
 
 def diff_source(src1, src2, output=None):
     src1 = ContractSource(src1)
     src2 = ContractSource(src2)
     if output:
-        output = os.path.join(config.DIFF_PATH, output)
+        output = os.path.join(config.diff_path, output)
     src1.compare(src2, output)
 
 
 def diff_chain_src(chain1, addr1, chain2, addr2, output=None):
     try:
         print("[*] Diff %s-%s  %s-%s" % (chain1, addr1, chain2, addr2))
         src1 = ScanAPI.get_source_by_chain(chain1, addr1)
```

### Comparing `peth-1.0.5/peth/util/graph.py` & `peth-1.0.6/peth/util/graph.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/util/logos.py` & `peth-1.0.6/peth/util/logos.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/util/markdown.py` & `peth-1.0.6/peth/util/markdown.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/util/slither.py` & `peth-1.0.6/peth/util/slither.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     _convert_version,
     _handle_multiple_files,
     _handle_single_file,
 )
 from crytic_compile.platform.exceptions import InvalidCompilation
 from slither.slither import Slither
 
-from peth.core import config
+from peth.core.config import config
 from peth.eth.scan import ScanAPI
 
 
 class Uniscan(Etherscan):
 
     # pylint: disable=too-many-locals,too-many-branches,too-many-statements
     def compile(self, crytic_compile: "CryticCompile", **kwargs: str) -> None:
         """
         target: <network>:<address>
         """
 
         target = self._target
         export_dir = os.path.join(
-            config.OUTPUT_PATH, kwargs.get("etherscan_export_dir", "compile-contracts")
+            config.output_path, kwargs.get("etherscan_export_dir", "compile-contracts")
         )
 
         source_code: str = ""
         result: Dict[str, Union[bool, str, int]] = {}
         contract_name: str = ""
 
         chain, addr = target.split(":")
```

### Comparing `peth-1.0.5/peth/util/solc.py` & `peth-1.0.6/peth/util/solc.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/peth/util/source.py` & `peth-1.0.6/peth/util/source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import difflib
 import os
 
-from peth.core import config
+from peth.core.config import config
 
 _disable_format = False
 
 
 def format_solidity(code):
     global _disable_format
 
     if _disable_format:
         return code
 
-    if not os.path.exists(config.DIFF_PATH):
-        os.makedirs(config.DIFF_PATH)
+    if not os.path.exists(config.diff_path):
+        os.makedirs(config.diff_path)
 
-    path = config.DIFF_TMP_FILE
+    path = os.path.join(config.diff_path, "peth.tmp.sol")
     open(path, "w").write(code)
 
     ret = os.system("npx prettier -w %s >/dev/null" % path)
     if ret != 0:
         print(
             "Run `npm install -g prettier prettier-plugin-solidity` to install solidity formatter to get better diff result."
         )
@@ -90,15 +90,15 @@
         buf = d.make_file(a.splitlines(), b.splitlines())
         open(output_filename + ".html", "w").write(buf)
         print("Written to " + output_filename + ".html")
 
     def compare(self, other, output=None):
 
         if output is None:
-            output = config.DIFF_PATH
+            output = config.diff_path
 
         if not os.path.isdir(output):
             os.makedirs(output)
 
         src_left = dict(self.contracts)
         dst_left = dict(other.contracts)
 
@@ -121,15 +121,15 @@
                 continue
 
             for name2, src2 in to_comp.items():
                 s = difflib.SequenceMatcher(None, src1.splitlines(), src2.splitlines())
                 similarity = s.ratio()
                 filename = "%s_%s_%0.2f" % (name1, name2, similarity)
                 # print(filename)
-                if similarity > config.DIFF_MIN_SIMILARITY:
+                if similarity > config.diff_min_similarity:
                     self.__diff_file(src1, src2, os.path.join(output, filename))
                     src_left[name1] = None
                     dst_left[name2] = None
 
         src_left_names = list(filter(lambda x: src_left[x], src_left))
         dst_left_names = list(filter(lambda x: dst_left[x], dst_left))
         if src_left_names or dst_left_names:
```

### Comparing `peth-1.0.5/peth.egg-info/PKG-INFO` & `peth-1.0.6/peth.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: peth
-Version: 1.0.5
-Summary: An all-in-one Ethereum SDK and command-line tool, written in Python.
+Version: 1.0.6
+Summary: An all-in-one Ethereum SDK and command-line tool written in Python.
 Home-page: https://github.com/lmy375/peth
 Author: Moon
 License: AGPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: web3==6.15.1
+Requires-Dist: py_solc_x==1.1.1
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: requests==2.28.1
+Requires-Dist: uvicorn==0.29.0
+Requires-Dist: fastapi==0.110.0
 
 # Peth
 
 `Peth` is an all-in-one Ethereum SDK and command-line tool, written in Python. It is designed for developers, smart contract auditors, web3 security researchers, and anyone interested in interacting with EVM-compatible chains with ease.
 
 ```
 ➜ peth
```

### Comparing `peth-1.0.5/setup.py` & `peth-1.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 requires = open("requirements.txt").read().splitlines()
-requires = filter(lambda x: not x.startswith("#"), requires)
+requires = list(filter(lambda x: not x.startswith("#"), requires))
 
 setup(
     name="peth",
-    description="An all-in-one Ethereum SDK and command-line tool, written in Python.",
+    description="An all-in-one Ethereum SDK and command-line tool written in Python.",
     url="https://github.com/lmy375/peth",
     author="Moon",
-    version="1.0.5",
-    packages=find_packages(exclude=["tests", "peth/4byte.json"]),
+    version="1.0.6",
+    packages=find_packages(exclude=["tests", "scripts"]),
     python_requires=">=3.8",
     install_requires=requires,
     license="AGPL-3.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
-            "peth = peth.__main__:main",
+            "peth = peth.cli:main",
             "tx-expl-server = peth.tools.txexpl.server.server:main",
         ]
     },
+    include_package_data=True,
 )
```

### Comparing `peth-1.0.5/tests/test_abi.py` & `peth-1.0.6/tests/test_abi.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/tests/test_evm/evm_test_codes.py` & `peth-1.0.6/tests/test_evm/evm_test_codes.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/tests/test_evm/test_chain.py` & `peth-1.0.6/tests/test_evm/test_chain.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/tests/test_evm/test_misc.py` & `peth-1.0.6/tests/test_evm/test_misc.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/tests/test_evm/test_vm.py` & `peth-1.0.6/tests/test_evm/test_vm.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/tests/test_sigs.py` & `peth-1.0.6/tests/test_sigs.py`

 * *Files identical despite different names*

### Comparing `peth-1.0.5/tests/test_source.py` & `peth-1.0.6/tests/test_source.py`

 * *Files identical despite different names*

