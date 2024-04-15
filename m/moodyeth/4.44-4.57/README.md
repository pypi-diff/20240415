# Comparing `tmp/moodyeth-4.44.tar.gz` & `tmp/moodyeth-4.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moodyeth-4.44.tar", last modified: Wed Sep 21 10:27:41 2022, max compression
+gzip compressed data, was "moodyeth-4.57.tar", last modified: Mon Apr 15 07:35:47 2024, max compression
```

## Comparing `moodyeth-4.44.tar` & `moodyeth-4.57.tar`

### file list

```diff
@@ -1,114 +1,124 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.945179 moodyeth-4.44/
--rw-rw-r--   0 root         (0) staff       (20)       44 2020-09-28 19:29:05.000000 moodyeth-4.44/.coveragerc
--rw-rw-r--   0 root         (0) staff       (20)     1284 2021-04-09 10:33:14.000000 moodyeth-4.44/.gitignore
--rw-r--r--   0 root         (0) staff       (20)      245 2022-04-04 16:05:09.000000 moodyeth-4.44/.readthedocs.yaml
--rw-r--r--   0 root         (0) staff       (20)     1462 2022-04-23 04:18:03.000000 moodyeth-4.44/Challenge.md
--rw-rw-r--   0 root         (0) staff       (20)     1068 2020-10-04 16:29:09.000000 moodyeth-4.44/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     3997 2022-09-21 10:27:41.944769 moodyeth-4.44/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     7404 2022-06-03 12:22:33.000000 moodyeth-4.44/README.md
--rw-rw-r--   0 root         (0) staff       (20)     2399 2022-03-30 15:00:28.000000 moodyeth-4.44/README.rst
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.906347 moodyeth-4.44/moody/
--rw-r--r--   0 root         (0) staff       (20)     4019 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.920953 moodyeth-4.44/moody/artifacts/
--rw-r--r--   0 root         (0) staff       (20)       96 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/Proxy.abi
--rw-r--r--   0 root         (0) staff       (20)        0 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/Proxy.bin
--rw-r--r--   0 root         (0) staff       (20)        0 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/Proxy.bin-runtime
--rw-r--r--   0 root         (0) staff       (20)     1921 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/ProxyAdmin.abi
--rw-r--r--   0 root         (0) staff       (20)     5516 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/ProxyAdmin.bin
--rw-r--r--   0 root         (0) staff       (20)     5264 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/ProxyAdmin.bin-runtime
--rw-r--r--   0 root         (0) staff       (20)     6797 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/ProxyAdmin_meta.json
--rw-r--r--   0 root         (0) staff       (20)     1704 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/Proxy_meta.json
--rw-r--r--   0 root         (0) staff       (20)     1718 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy.abi
--rw-r--r--   0 root         (0) staff       (20)     8892 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy.bin
--rw-r--r--   0 root         (0) staff       (20)     5346 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy.bin-runtime
--rw-r--r--   0 root         (0) staff       (20)     9643 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy_meta.json
--rw-r--r--   0 root         (0) staff       (20)     3475 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WETH9.abi
--rw-r--r--   0 root         (0) staff       (20)     4842 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WETH9.bin
--rw-r--r--   0 root         (0) staff       (20)     4092 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WETH9.bin-runtime
--rw-r--r--   0 root         (0) staff       (20)     4062 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WETH9_meta.json
--rw-r--r--   0 root         (0) staff       (20)     3475 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WRSC.abi
--rw-r--r--   0 root         (0) staff       (20)     4838 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WRSC.bin
--rw-r--r--   0 root         (0) staff       (20)     4092 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WRSC.bin-runtime
--rw-r--r--   0 root         (0) staff       (20)     4059 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/artifacts/WRSC_meta.json
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.922483 moodyeth-4.44/moody/buildercompile/
--rw-r--r--   0 root         (0) staff       (20)     3491 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/buildercompile/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     2784 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/buildercompile/remotecompile.py
--rw-r--r--   0 root         (0) staff       (20)     4679 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/buildercompile/transpile.py
--rw-r--r--   0 root         (0) staff       (20)     1899 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/bussen.py
--rw-r--r--   0 root         (0) staff       (20)    12455 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/conf.py
--rw-r--r--   0 root         (0) staff       (20)     7501 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/contracttool.py
--rw-r--r--   0 root         (0) staff       (20)     1651 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/erc20.py
--rw-r--r--   0 root         (0) staff       (20)     3232 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/exceptions.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.924760 moodyeth-4.44/moody/flashbots/
--rw-r--r--   0 root         (0) staff       (20)      874 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/flashbots/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3409 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/flashbots/builder.py
--rw-r--r--   0 root         (0) staff       (20)    15137 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/flashbots/flashbots.py
--rw-r--r--   0 root         (0) staff       (20)     1293 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/flashbots/middleware.py
--rw-r--r--   0 root         (0) staff       (20)     2048 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/flashbots/provider.py
--rw-r--r--   0 root         (0) staff       (20)     1808 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/flashbots/types.py
--rw-r--r--   0 root         (0) staff       (20)    44326 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/libeb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.925577 moodyeth-4.44/moody/m/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.926583 moodyeth-4.44/moody/m/b_send/
--rw-r--r--   0 root         (0) staff       (20)    70174 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/b_send/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    11139 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/b_send/basec.py
--rw-r--r--   0 root         (0) staff       (20)    13491 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/b_send/looper.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.926992 moodyeth-4.44/moody/m/b_send2/
--rw-r--r--   0 root         (0) staff       (20)   207364 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/b_send2/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6461 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/bases.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.927666 moodyeth-4.44/moody/m/beri_coin/
--rw-r--r--   0 root         (0) staff       (20)   210558 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/beri_coin/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.928728 moodyeth-4.44/moody/m/blockhash_store/
--rw-r--r--   0 root         (0) staff       (20)    23748 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/blockhash_store/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.929080 moodyeth-4.44/moody/m/c_token/
--rw-r--r--   0 root         (0) staff       (20)   148598 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/c_token/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.929796 moodyeth-4.44/moody/m/deposit_contract/
--rw-r--r--   0 root         (0) staff       (20)    28275 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/deposit_contract/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.930373 moodyeth-4.44/moody/m/eth2_multi_deposit/
--rw-r--r--   0 root         (0) staff       (20)    10946 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/eth2_multi_deposit/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.931161 moodyeth-4.44/moody/m/kyc/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/kyc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5568 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/kyc/merkletree.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.931589 moodyeth-4.44/moody/m/layer_zero_u_s_d_t/
--rw-r--r--   0 root         (0) staff       (20)   158141 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/layer_zero_u_s_d_t/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.932795 moodyeth-4.44/moody/m/multicall/
--rw-r--r--   0 root         (0) staff       (20)    27579 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/multicall/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1827 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/multicall/execute.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.934344 moodyeth-4.44/moody/m/multicall2/
--rw-r--r--   0 root         (0) staff       (20)    50365 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/multicall2/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1632 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/multicall2/execute.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.934972 moodyeth-4.44/moody/m/oracle/
--rw-r--r--   0 root         (0) staff       (20)    82006 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/oracle/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.935630 moodyeth-4.44/moody/m/pharaohs/
--rw-r--r--   0 root         (0) staff       (20)    83414 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/pharaohs/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.936147 moodyeth-4.44/moody/m/proxy_admin/
--rw-r--r--   0 root         (0) staff       (20)    50025 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/proxy_admin/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.936623 moodyeth-4.44/moody/m/tc20/
--rw-r--r--   0 root         (0) staff       (20)    76307 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/tc20/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.937232 moodyeth-4.44/moody/m/tether_token2/
--rw-r--r--   0 root         (0) staff       (20)   106808 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/tether_token2/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.937762 moodyeth-4.44/moody/m/transparent_upgradeable_proxy/
--rw-r--r--   0 root         (0) staff       (20)    33226 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/transparent_upgradeable_proxy/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1435 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/tx_params.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.939591 moodyeth-4.44/moody/m/verify/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/verify/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5165 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/verify/http.py
--rw-r--r--   0 root         (0) staff       (20)     2004 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/verify/solfla.py
--rw-r--r--   0 root         (0) staff       (20)     4515 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/m/verify/verify.py
--rw-r--r--   0 root         (0) staff       (20)     3835 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/paths.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.941290 moodyeth-4.44/moody/upgrade/
--rw-r--r--   0 root         (0) staff       (20)     2243 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/upgrade/Token.py
--rw-r--r--   0 root         (0) staff       (20)    56358 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/upgrade/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    16745 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/upgrade/deployupgradable.py
--rw-r--r--   0 root         (0) staff       (20)      471 2022-09-21 10:27:30.000000 moodyeth-4.44/moody/upgrade/timelocker.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2022-09-21 10:27:41.944194 moodyeth-4.44/moodyeth.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     3997 2022-09-21 10:27:41.000000 moodyeth-4.44/moodyeth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2346 2022-09-21 10:27:41.000000 moodyeth-4.44/moodyeth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2022-09-21 10:27:41.000000 moodyeth-4.44/moodyeth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2021-06-14 04:24:04.000000 moodyeth-4.44/moodyeth.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)      757 2022-09-21 10:27:41.000000 moodyeth-4.44/moodyeth.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2022-09-21 10:27:41.000000 moodyeth-4.44/moodyeth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2022-09-21 10:27:41.945316 moodyeth-4.44/setup.cfg
--rw-rw-r--   0 root         (0) staff       (20)     3157 2021-11-08 07:48:16.000000 moodyeth-4.44/setup.py
--rw-r--r--   0 root         (0) staff       (20)     2339 2022-06-14 19:25:13.000000 moodyeth-4.44/update
--rw-r--r--   0 root         (0) staff       (20)        5 2022-09-21 10:27:37.000000 moodyeth-4.44/version
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.419847 moodyeth-4.57/
+-rw-rw-r--   0 root         (0) staff       (20)       44 2020-09-28 19:29:05.000000 moodyeth-4.57/.coveragerc
+-rw-rw-r--   0 root         (0) staff       (20)     1303 2024-04-15 07:20:55.000000 moodyeth-4.57/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)      245 2022-04-04 16:05:09.000000 moodyeth-4.57/.readthedocs.yaml
+-rw-r--r--   0 root         (0) staff       (20)     1462 2022-04-23 04:18:03.000000 moodyeth-4.57/Challenge.md
+-rw-rw-r--   0 root         (0) staff       (20)     1068 2020-10-04 16:29:09.000000 moodyeth-4.57/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     3301 2024-04-15 07:35:47.419607 moodyeth-4.57/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6832 2023-08-09 02:48:20.000000 moodyeth-4.57/README.md
+-rw-r--r--   0 root         (0) staff       (20)     7490 2024-04-15 07:35:47.000000 moodyeth-4.57/README.rst
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.362247 moodyeth-4.57/moody/
+-rw-r--r--   0 root         (0) staff       (20)     4523 2024-04-15 07:35:46.000000 moodyeth-4.57/moody/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.375176 moodyeth-4.57/moody/artifacts/
+-rw-r--r--   0 root         (0) staff       (20)       96 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/Proxy.abi
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/Proxy.bin
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/Proxy.bin-runtime
+-rw-r--r--   0 root         (0) staff       (20)     1921 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/ProxyAdmin.abi
+-rw-r--r--   0 root         (0) staff       (20)     5516 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/ProxyAdmin.bin
+-rw-r--r--   0 root         (0) staff       (20)     5264 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/ProxyAdmin.bin-runtime
+-rw-r--r--   0 root         (0) staff       (20)     6797 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/ProxyAdmin_meta.json
+-rw-r--r--   0 root         (0) staff       (20)     1704 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/Proxy_meta.json
+-rw-r--r--   0 root         (0) staff       (20)     1718 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy.abi
+-rw-r--r--   0 root         (0) staff       (20)     8892 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy.bin
+-rw-r--r--   0 root         (0) staff       (20)     5346 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy.bin-runtime
+-rw-r--r--   0 root         (0) staff       (20)     9643 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy_meta.json
+-rw-r--r--   0 root         (0) staff       (20)     3475 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WETH9.abi
+-rw-r--r--   0 root         (0) staff       (20)     4842 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WETH9.bin
+-rw-r--r--   0 root         (0) staff       (20)     4092 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WETH9.bin-runtime
+-rw-r--r--   0 root         (0) staff       (20)     4062 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WETH9_meta.json
+-rw-r--r--   0 root         (0) staff       (20)     3475 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WRSC.abi
+-rw-r--r--   0 root         (0) staff       (20)     4838 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WRSC.bin
+-rw-r--r--   0 root         (0) staff       (20)     4092 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WRSC.bin-runtime
+-rw-r--r--   0 root         (0) staff       (20)     4059 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/artifacts/WRSC_meta.json
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.376347 moodyeth-4.57/moody/buildercompile/
+-rw-r--r--   0 root         (0) staff       (20)     4000 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/buildercompile/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3128 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/buildercompile/remotecompile.py
+-rw-r--r--   0 root         (0) staff       (20)     5008 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/buildercompile/transpile.py
+-rw-r--r--   0 root         (0) staff       (20)     1899 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/bussen.py
+-rw-r--r--   0 root         (0) staff       (20)    12455 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/conf.py
+-rw-r--r--   0 root         (0) staff       (20)     7502 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/contracttool.py
+-rw-r--r--   0 root         (0) staff       (20)     1651 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/erc20.py
+-rw-r--r--   0 root         (0) staff       (20)     3232 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/exceptions.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.378699 moodyeth-4.57/moody/flashbots/
+-rw-r--r--   0 root         (0) staff       (20)      874 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/flashbots/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3409 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/flashbots/builder.py
+-rw-r--r--   0 root         (0) staff       (20)    15137 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/flashbots/flashbots.py
+-rw-r--r--   0 root         (0) staff       (20)     1293 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/flashbots/middleware.py
+-rw-r--r--   0 root         (0) staff       (20)     2048 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/flashbots/provider.py
+-rw-r--r--   0 root         (0) staff       (20)     1808 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/flashbots/types.py
+-rw-r--r--   0 root         (0) staff       (20)    48080 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/libeb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.380145 moodyeth-4.57/moody/m/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.381492 moodyeth-4.57/moody/m/b_send/
+-rw-r--r--   0 root         (0) staff       (20)    70174 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/b_send/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    11139 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/b_send/basec.py
+-rw-r--r--   0 root         (0) staff       (20)    13491 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/b_send/looper.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.381887 moodyeth-4.57/moody/m/b_send2/
+-rw-r--r--   0 root         (0) staff       (20)   207364 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/b_send2/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6461 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/bases.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.382655 moodyeth-4.57/moody/m/beri_coin/
+-rw-r--r--   0 root         (0) staff       (20)   210558 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/beri_coin/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.383406 moodyeth-4.57/moody/m/blockhash_store/
+-rw-r--r--   0 root         (0) staff       (20)    23748 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/blockhash_store/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.383906 moodyeth-4.57/moody/m/c_token/
+-rw-r--r--   0 root         (0) staff       (20)   148598 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/c_token/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.384791 moodyeth-4.57/moody/m/deposit_contract/
+-rw-r--r--   0 root         (0) staff       (20)    28275 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/deposit_contract/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.385317 moodyeth-4.57/moody/m/eth2_multi_deposit/
+-rw-r--r--   0 root         (0) staff       (20)    10946 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/eth2_multi_deposit/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.386045 moodyeth-4.57/moody/m/kyc/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/kyc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5568 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/kyc/merkletree.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.386477 moodyeth-4.57/moody/m/layer_zero_u_s_d_t/
+-rw-r--r--   0 root         (0) staff       (20)   158141 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/layer_zero_u_s_d_t/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.387725 moodyeth-4.57/moody/m/multicall/
+-rw-r--r--   0 root         (0) staff       (20)    27579 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1827 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall/execute.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.388732 moodyeth-4.57/moody/m/multicall2/
+-rw-r--r--   0 root         (0) staff       (20)    50365 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall2/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1632 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall2/execute.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.397497 moodyeth-4.57/moody/m/multicall3/
+-rw-r--r--   0 root         (0) staff       (20)       88 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4917 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/call.py
+-rw-r--r--   0 root         (0) staff       (20)    20737 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/constants.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/eth_retry.py
+-rw-r--r--   0 root         (0) staff       (20)       53 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/exceptions.py
+-rw-r--r--   0 root         (0) staff       (20)      266 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/loggers.py
+-rw-r--r--   0 root         (0) staff       (20)     8310 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/multicall.py
+-rw-r--r--   0 root         (0) staff       (20)     2486 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/signature.py
+-rw-r--r--   0 root         (0) staff       (20)     3164 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/multicall3/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.398404 moodyeth-4.57/moody/m/oracle/
+-rw-r--r--   0 root         (0) staff       (20)    82006 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/oracle/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.399060 moodyeth-4.57/moody/m/pharaohs/
+-rw-r--r--   0 root         (0) staff       (20)    83414 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/pharaohs/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.399967 moodyeth-4.57/moody/m/proxy_admin/
+-rw-r--r--   0 root         (0) staff       (20)    50025 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/proxy_admin/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.400477 moodyeth-4.57/moody/m/tc20/
+-rw-r--r--   0 root         (0) staff       (20)    76307 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/tc20/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.401008 moodyeth-4.57/moody/m/tether_token2/
+-rw-r--r--   0 root         (0) staff       (20)   106808 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/tether_token2/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.401857 moodyeth-4.57/moody/m/transparent_upgradeable_proxy/
+-rw-r--r--   0 root         (0) staff       (20)    33226 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/transparent_upgradeable_proxy/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1435 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/tx_params.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.404767 moodyeth-4.57/moody/m/verify/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/verify/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5165 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/verify/http.py
+-rw-r--r--   0 root         (0) staff       (20)     2004 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/verify/solfla.py
+-rw-r--r--   0 root         (0) staff       (20)     4515 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/m/verify/verify.py
+-rw-r--r--   0 root         (0) staff       (20)     4215 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/paths.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.407655 moodyeth-4.57/moody/upgrade/
+-rw-r--r--   0 root         (0) staff       (20)     2243 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/upgrade/Token.py
+-rw-r--r--   0 root         (0) staff       (20)    56358 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/upgrade/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    16745 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/upgrade/deployupgradable.py
+-rw-r--r--   0 root         (0) staff       (20)      471 2024-04-15 07:35:43.000000 moodyeth-4.57/moody/upgrade/timelocker.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 07:35:47.412189 moodyeth-4.57/moodyeth.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     3301 2024-04-15 07:35:47.000000 moodyeth-4.57/moodyeth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2633 2024-04-15 07:35:47.000000 moodyeth-4.57/moodyeth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-15 07:35:47.000000 moodyeth-4.57/moodyeth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2021-06-14 04:24:04.000000 moodyeth-4.57/moodyeth.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)      757 2024-04-15 07:35:47.000000 moodyeth-4.57/moodyeth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2024-04-15 07:35:47.000000 moodyeth-4.57/moodyeth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       79 2024-04-15 07:35:47.420448 moodyeth-4.57/setup.cfg
+-rw-rw-r--   0 root         (0) staff       (20)     3810 2024-04-15 07:35:42.000000 moodyeth-4.57/setup.py
+-rw-r--r--   0 root         (0) staff       (20)     2485 2024-04-15 07:22:21.000000 moodyeth-4.57/update
+-rw-r--r--   0 root         (0) staff       (20)        5 2024-04-15 07:35:43.000000 moodyeth-4.57/version
```

### Comparing `moodyeth-4.44/.gitignore` & `moodyeth-4.57/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .idea
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
-
+/moodyeth.egg-info/
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `moodyeth-4.44/Challenge.md` & `moodyeth-4.57/Challenge.md`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/LICENSE` & `moodyeth-4.57/LICENSE`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/__init__.py` & `moodyeth-4.57/moody/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 from dataclasses import dataclass
 
 import pkg_resources
 
 if sys.version_info < (3, 5):
     raise EnvironmentError("Python 3.5 or above is required")
 
-__version__ = pkg_resources.get_distribution("moodyeth").version
-
 __pdoc__ = {
     "moody.flashbots.types.FlashbotsBundleTx": False,
     "moody.flashbots.types.FlashbotsBundleRawTx": False,
     "moody.flashbots.types.FlashbotsBundleDictTx": False,
     "moody.flashbots.types.FlashbotsOpts": False,
     "moody.flashbots.types.SignTx": False,
     "moody.flashbots.types.SignedTxAndHash": False,
 }
 
+if sys.version_info >= (3, 8):
+    from typing import TypedDict, Literal, overload, Union  # pylint: disable=no-name-in-module
+else:
+    from typing_extensions import TypedDict, Literal, overload
 
-# __all__ = [
-#    '__version__',
-# ]
-
+__version__ = '4.57'
 
 @dataclass
 class Token:
     address: str = None
     name: str = None
     code_hash: str = None
     token_contract: str = None
@@ -36,29 +35,30 @@
     spender: dict = None
     balance: dict = None
 
 
 @dataclass
 class Config:
     network_name: str
-    rpc_url: str
+    rpc_url: Union[str, list[str]]
     chain_id: int
     symbol: str
     block_explorer: str
     bridge: str = ""
     faucet: str = ""
     gas: int = 6000000
     gasPrice: int = 1059100000
     one: int = 1000000000000000000
     wait_time: int = 6
     # Oracle from Chainlink
     # https://docs.chain.link/docs/vrf-contracts/
     link_token: str = None
     link_vrf_coordinator: str = None
     link_keyhash: str = None
+    reconnect_tries: int = 5
 
 
 @dataclass
 class Key:
     private_key: str
     wallet_address: str
     token: str
@@ -126,14 +126,28 @@
     Gas costs for `SLOAD`, `*CALL`, `BALANCE`, `EXT*` and `SELFDESTRUCT` increased. The compiler assumes cold gas costs for such operations. This is relevant for gas estimation and the optimizer.
     """
     LONDON = "london"
     """
     5 August 2021
     The block’s base fee (EIP-3198 and EIP-1559) can be accessed via the global block.basefee or basefee() in inline assembly.
     """
+    SHANGHAI = "shanghai"
+    """
+    12 Apr 2023
+    Smaller code size and gas savings due to the introduction of push0
+    """
+    DECUN = "decun"
+    """
+    13 Mar 2024
+    The block’s blob base fee (EIP-7516 and EIP-4844) can be accessed via the global 
+    block.blobbasefee
+         or 
+    blobbasefee()
+    in inline assembly.
+    """
 
 
 class DefaultKeys:
     k0 = "000000000000000000000000000000000000000000000000000000000000001e"
 
 
 root_base_path = os.path.join(os.path.dirname(__file__))
@@ -141,8 +155,8 @@
 __all__ = [
     '__version__',
     'Evm',
     'Config',
     'Bolors',
     'DefaultKeys',
     'root_base_path'
-]
+]
```

### Comparing `moodyeth-4.44/moody/artifacts/ProxyAdmin.abi` & `moodyeth-4.57/moody/artifacts/ProxyAdmin.abi`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/ProxyAdmin.bin` & `moodyeth-4.57/moody/artifacts/ProxyAdmin.bin`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/ProxyAdmin.bin-runtime` & `moodyeth-4.57/moody/artifacts/ProxyAdmin.bin-runtime`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/ProxyAdmin_meta.json` & `moodyeth-4.57/moody/artifacts/ProxyAdmin_meta.json`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/Proxy_meta.json` & `moodyeth-4.57/moody/artifacts/Proxy_meta.json`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy.abi` & `moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy.abi`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy.bin` & `moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy.bin`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy.bin-runtime` & `moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy.bin-runtime`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/TransparentUpgradeableProxy_meta.json` & `moodyeth-4.57/moody/artifacts/TransparentUpgradeableProxy_meta.json`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WETH9.abi` & `moodyeth-4.57/moody/artifacts/WETH9.abi`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WETH9.bin` & `moodyeth-4.57/moody/artifacts/WETH9.bin`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WETH9.bin-runtime` & `moodyeth-4.57/moody/artifacts/WETH9.bin-runtime`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WETH9_meta.json` & `moodyeth-4.57/moody/artifacts/WETH9_meta.json`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WRSC.abi` & `moodyeth-4.57/moody/artifacts/WRSC.abi`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WRSC.bin` & `moodyeth-4.57/moody/artifacts/WRSC.bin`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WRSC.bin-runtime` & `moodyeth-4.57/moody/artifacts/WRSC.bin-runtime`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/artifacts/WRSC_meta.json` & `moodyeth-4.57/moody/artifacts/WRSC_meta.json`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/buildercompile/__init__.py` & `moodyeth-4.57/moody/buildercompile/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env python
+"""
+Compiler build for linux system or unix system
+
+"""
 REC = """#!/bin/bash
 if [[ ! -f {TARGET_LOC} ]]; then
     mkdir -p {TARGET_LOC}/vault
 fi
 if [[ ! -f {TARGET_LOC}/build ]]; then
     mkdir -p {TARGET_LOC}/build
 fi
@@ -35,14 +39,26 @@
 
 {LISTP}
 
 
 exit
 """
 
+FORGE_BUILD = """#!/bin/bash
+
+if ! command -v forge &>/dev/null; then
+    echo "forge in command is not install. Please visit: https://github.com/foundry-rs/foundry"
+    curl -L https://foundry.paradigm.xyz | bash
+    exit;
+fi
+echo "generating compiled files into {BUILD} from {SRC} on forge runs"
+forge build --contracts {SRC} --out {BUILD} --optimizer-runs {RUNS} --force
+
+"""
+
 TRANS_LOCAL = """#!/bin/bash
 # -----------------------------------------------
 {PRE_HEAD}
 
 {LISTP}
 
 {FOOTER}
@@ -99,43 +115,51 @@
     --backend "web3" \
     --language "TypeScript"
 
 echo "==> generate abi to typescript --> 🧊"
 """
 
 ITEM_TRANSPILE_GO = """
-
 echo "==> 🚸 compile abi to golang"
-if [[ ! -f {outputfolder}/{classname} ]]; then
-    mkdir -p {outputfolder}/{classname}
+
+if [[ ! -f {outputfolder} ]]; then
+    mkdir -p {outputfolder}
 fi
 
-abigen --abi {target_abi} --pkg {classname} --type {classname} --out {outputfolder}/{classname}/init.go
+abigen --abi "{target_abi}" --pkg {classname} --out "{outputfolder}/init.go"
+
+echo "==> generate abi to golang --> 🚸✅🧊"
 
-echo "==> generate abi to golang --> 🧊"
 """
 
 PRE_HEAD = """
 
-# . ./{path_definitions}
-
-if [[ ! -d factoryabi ]]; then
-  echo "The factory abi module is not found"
-  exit 1;
-fi
-
 if ! command -v abi-gen-uni &>/dev/null; then
     echo "abi-gen-uni could not be found"
     cnpm i -g easy-abi-gen
 fi
 
 if ! command -v abigen &>/dev/null; then
     echo "abigen could not be found, please go check out: https://geth.ethereum.org/downloads/"
     exit 1;
 fi
+
+
+cp -R {FACTORY} {BUILDPATH}/factoryabi 2>/dev/null
+
+if [[ ! -d factoryabi ]]; then
+  echo "The factory abi module is not found"
+  exit 1;
+fi
+
 """
-SUB_FOOTER= """
 
-#rm localpile
-#rm -rf factoryabi
+SUB_FOOTER = """
 
-"""
+echo "Building the forge bin"
+
+rm buildforgebin
+rm localpile
+rm -rf factoryabi
+
+echo "Cleaned up the useless codebase"
+"""
```

### Comparing `moodyeth-4.44/moody/buildercompile/remotecompile.py` & `moodyeth-4.57/moody/buildercompile/remotecompile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from moody.paths import Paths
-from . import REC, ITEM, ITEMLINK
+from . import REC, ITEM, ITEMLINK, FORGE_BUILD
 
 
 def compileItem1(tar: Paths, k0: str, optimzations: int) -> str:
     """
     list the item content
     :param tar:
     :param k0:
@@ -47,14 +47,28 @@
         LISTP="\n".join(compile_list),
         TARGET_LOC=tar.TARGET_LOC,
         COMPRESSED_NAME=tar.COMPRESSED_NAME,
         SOLVER=tar.SOLC_VER,
     )
 
 
+def wrapForgeCompile(tar: Paths) -> str:
+    return FORGE_BUILD.format(
+        SRC=tar.SOURCE_PATH,
+        BUILD=tar.FORGE_BUILD,
+        RUNS=100000
+    )
+
+
+def BuildForgeLinuxBuildCommand(p: Paths) -> None:
+    with open(p.workspaceFilename("buildforgebin"), 'w') as f:
+        f.write(wrapForgeCompile(p))
+        f.close()
+
+
 def BuildRemoteLinuxCommand(p: Paths, optimize: int, list_files: list = None, linked: dict = None) -> None:
     """
     building the remote linux command line
     :param p:
     :param list_files:
     :return:
     """
```

### Comparing `moodyeth-4.44/moody/buildercompile/transpile.py` & `moodyeth-4.57/moody/buildercompile/transpile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
 
 from ..paths import Paths
-from . import ITEM_CP_LOCAL, ITEM_TRANSPILE_GO, TRANS_LOCAL, ITEM_TRANSPILE_PYTHON, ITEM_TRANSPILE_TS, PRE_HEAD, SUB_FOOTER
+from . import ITEM_CP_LOCAL, ITEM_TRANSPILE_GO, TRANS_LOCAL, ITEM_TRANSPILE_PYTHON, ITEM_TRANSPILE_TS, PRE_HEAD, \
+    SUB_FOOTER
 
 REG = r"(.+?)([A-Z])"
 
 
 def snake(match):
     return match.group(1).lower() + "_" + match.group(2).lower()
 
@@ -85,40 +86,45 @@
     )
 
 
 def buildCmdGo2(p: Paths, pathName: str) -> str:
     based_name = os.path.basename(pathName)
     class_name = filter_file_name(based_name).replace('.sol', '')
     return ITEM_TRANSPILE_GO.format(
-        outputfolder=f"{p.BUILDPATH}/codec/gen_go",
+        outputfolder=f"{p.BUILDPATH}/codec/gen_go/{class_name}",
         target_abi=abiPath_v2(p, pathName),
         BUILDPATH=p.BUILDPATH,
         classname=class_name
     )
 
 
 def wrapContentTranspile(tar: Paths, compile_list: list) -> str:
     """
     wrap content
     :param tar: path in string
     :param compile_list: the list in compile
     :return:
     """
-    head_section = PRE_HEAD.format(path_definitions=tar.LOCAL_BASH_INCLUDE)
     contract_list_content = "\n".join(compile_list)
     return TRANS_LOCAL.format(
         TARGET_LOC=tar.TARGET_LOC,
         COMPRESSED_NAME=tar.COMPRESSED_NAME,
         SOLVER=tar.SOLC_VER,
         LISTP=contract_list_content,
-        PRE_HEAD=head_section,
+        PRE_HEAD=wrapHeadTranspile(tar),
         FOOTER=SUB_FOOTER
     )
 
 
+def wrapHeadTranspile(p: Paths) -> str:
+    return PRE_HEAD.format(
+        FACTORY=p.FACTORY_PATH,
+        BUILDPATH=p.BUILDPATH
+    )
+
 def BuildLang(p: Paths, list_class_names: list) -> None:
     """
 
     :param p: path in string
     :param list_class_names: the class name
     :return:
     """
@@ -145,13 +151,20 @@
     """
     k = list()
     # ==================================================
     for v in list_class_names:
         k.append(buildCmdPy2(p, v))
         k.append(buildCmdTs2(p, v))
         k.append(buildCmdGo2(p, v))
+
+        # ==================================================
+
         if p.WEB_DAPP_SRC is not None:
-            k.append(moveTsFiles(p, v))
+            if os.path.isdir(p.WEB_DAPP_SRC):
+                k.append(moveTsFiles(p, v))
+            else:
+                print(f"app path for implementation {p.WEB_DAPP_SRC} is not exist. file move is stopped.")
+
     # ==================================================
     with open(p.workspaceFilename("localpile"), 'w') as f:
         f.write(wrapContentTranspile(p, k))
         f.close()
```

### Comparing `moodyeth-4.44/moody/bussen.py` & `moodyeth-4.57/moody/bussen.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/conf.py` & `moodyeth-4.57/moody/conf.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/contracttool.py` & `moodyeth-4.57/moody/contracttool.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         while True:
             self.update_timestamp()
             self.scheduled_loop_operations()
 
     def switch_node(self):
         original_cfg = self._worker.GetNode()
         original_cfg.rpc_url = random.choice(self._rpcs)
-        while self._worker.switchNetowrk(original_cfg) is False:
+        while self._worker.switch_network(original_cfg) is False:
             self.update_timestamp()
             print(f"{self._t_now} Retried a new node and it is failed again.")
             original_cfg.rpc_url = random.choice(self._rpcs)
 
     def run_looper_service(self):
         self.update_timestamp()
         while True:
```

### Comparing `moodyeth-4.44/moody/erc20.py` & `moodyeth-4.57/moody/erc20.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/exceptions.py` & `moodyeth-4.57/moody/exceptions.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/flashbots/__init__.py` & `moodyeth-4.57/moody/flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/flashbots/builder.py` & `moodyeth-4.57/moody/flashbots/builder.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/flashbots/flashbots.py` & `moodyeth-4.57/moody/flashbots/flashbots.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/flashbots/middleware.py` & `moodyeth-4.57/moody/flashbots/middleware.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/flashbots/provider.py` & `moodyeth-4.57/moody/flashbots/provider.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/flashbots/types.py` & `moodyeth-4.57/moody/flashbots/types.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/libeb.py` & `moodyeth-4.57/moody/libeb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import codecs
+import datetime
 import json
 import os
+import random
 import subprocess
 import time
 from threading import Lock
 from typing import List, Tuple, Optional
 
 import re
 
@@ -17,15 +19,15 @@
 from web3.exceptions import TransactionNotFound, ContractLogicError, InvalidAddress, TimeExhausted
 from web3.logs import DISCARD
 from web3.middleware import geth_poa_middleware
 from web3.types import BlockData
 
 # ========================== Of course
 from . import Bolors, Evm, DefaultKeys, root_base_path, MetaSetting
-from .buildercompile.remotecompile import BuildRemoteLinuxCommand
+from .buildercompile.remotecompile import BuildRemoteLinuxCommand, BuildForgeLinuxBuildCommand
 from .buildercompile.transpile import BuildLang, filter_file_name, BuildLangForge
 from .conf import Config
 from .exceptions import FoundUndeployedLibraries
 from .flashbots import construct_flashbots_middleware, flashbot
 from .paths import Paths
 
 
@@ -143,15 +145,15 @@
 
     def getAddr(self, keyname: str) -> str:
         pass
 
     def isAddress(self, add: str) -> bool:
         pass
 
-    def switchNetowrk(self, _node_config: Config) -> bool:
+    def switch_network(self, _node_config: Config) -> bool:
         pass
 
 
 class BinOp:
     """
     The binary operation for the ops. Taking care the operations for library linking and the related stuffs.
     """
@@ -198,15 +200,15 @@
         for class_name, instruction_line in self.bin_undeploy_lib.items():
             if databank.hasContractName(class_name) is True:
                 print(f"💽 Found support Class {class_name} - deployment address")
                 if databank.isAddress(databank.getAddr(class_name)):
                     self._knifeBinClass(class_name, self._placehd(instruction_line), databank.getAddr(class_name))
                 else:
                     print("🧊 The found library address is not valid - {}, {}".format(class_name,
-                                                                                      databank.getAddr(class_name)))
+                                                                                     databank.getAddr(class_name)))
                     raise FoundUndeployedLibraries
             else:
                 print(
                     "⚠️ Unfound library Error- {}, please make sure you have this library deployed.".format(class_name))
                 raise FoundUndeployedLibraries
 
         self.bin_knifed = self.bin_knifed.splitlines(True)[0]
@@ -246,34 +248,98 @@
         self._abi = None
         self._bin = None
         self._meta = None
         self.combined_data = None
         self._key = None
 
     def setBuildNameSpace(self, path: str) -> "SolWeb3Tool":
+        """
+        the direction path is found in here
+        :param path:
+        :return:
+        """
         self.OUTPUT_BUILD = path
         return self
 
     def setBasePath(self, path: str) -> "SolWeb3Tool":
+        """
+        the path for the base direction
+        :param path:
+        :return:
+        """
         self.WORKSPACE_PATH = path
         return self
 
+    def _justrun(self, cmd_name: str):
+        """
+        the command name is not found in here.
+        :param cmd_name:
+        :return:
+        """
+        exec_path = f"{self.WORKSPACE_PATH}/{cmd_name}"
+
+        if os.path.isfile(exec_path):
+            subprocess.run(["cd", self.WORKSPACE_PATH])
+            list_files = subprocess.run(["sh", cmd_name])
+            print("The run bash code ->: %d" % list_files.returncode)
+        else:
+            print("The execution file is not found.")
+
+    def RunTranspile(self) -> "SolWeb3Tool":
+        """This is the remote command to execute the localpile bash file
+        using remote compile method to compile the sol files
+        all works will be done with the remote server or using the docker"""
+        self._justrun("localpile")
+        return self
+
+    def ForgeGen(self) -> "SolWeb3Tool":
+        """This is the remote command to execute the buildforgebin bash file
+        using remote compile method to compile the sol files
+        all works will be done with the remote server or using the docker"""
+        self._justrun("buildforgebin")
+        return self
+
+    def BuildRemote(self) -> "SolWeb3Tool":
+        """This is the remote command to execute the solc_remote bash file
+        using remote compile method to compile the sol files
+        all works will be done with the remote server or using the docker"""
+        self._justrun("solc_remote")
+        return self
+
     def SplitForgeBuild(self, class_name: str) -> "SolWeb3Tool":
+        """
+        to process the build files for the solidity
+        :param class_name:
+        :return:
+        """
         uncutjson = dict()
-        combinedjson = os.path.join(self.WORKSPACE_PATH, self.OUTPUT_BUILD, "{}.sol".format(class_name),
-                                    "{}.json".format(class_name))
+        combinedjson = os.path.join(
+            self.WORKSPACE_PATH,
+            self.OUTPUT_BUILD,
+            f"{class_name}.sol",
+            f"{class_name}.json")
         try:
             uncutjson = json.load(codecs.open(combinedjson, 'r', 'utf-8-sig'))
         except FileNotFoundError:
-            message_exit("Some of the files from the build json file in forge is not found.", 3)
+            message_exit(f"The build json file in forge are not found for class {class_name}", 3)
 
-        abifile = os.path.join(self.WORKSPACE_PATH, self.OUTPUT_BUILD, "{}.sol".format(class_name),
-                               "{}.abi".format(class_name))
-        binfile = os.path.join(self.WORKSPACE_PATH, self.OUTPUT_BUILD, "{}.sol".format(class_name),
-                               "{}.bin".format(class_name))
+        abifile = os.path.join(
+            self.WORKSPACE_PATH,
+            self.OUTPUT_BUILD,
+            f"{class_name}.sol",
+            f"{class_name}.abi"
+
+        )
+
+        binfile = os.path.join(
+            self.WORKSPACE_PATH,
+            self.OUTPUT_BUILD,
+            f"{class_name}.sol",
+            f"{class_name}.bin"
+        )
 
         if "abi" in uncutjson:
             predum = uncutjson["abi"]
             writeFile(json.dumps(predum, ensure_ascii=False), abifile)
 
         if "bytecode" in uncutjson:
             pr = uncutjson["bytecode"]
@@ -290,24 +356,29 @@
 
     def GetCodeClassFromForgeBuild(self, class_name: str) -> "SolWeb3Tool":
         """
         get the independent files and content from the file system
         :param class_name:
         :return:
         """
-        p2abi = os.path.join(self.WORKSPACE_PATH, self.OUTPUT_BUILD, "{}.sol".format(class_name),
-                             "{}.abi".format(class_name))
-        p1bin = os.path.join(self.WORKSPACE_PATH, self.OUTPUT_BUILD, "{}.sol".format(class_name),
-                             "{}.bin".format(class_name))
+        p2abi = os.path.join(self.WORKSPACE_PATH,
+                             self.OUTPUT_BUILD,
+                             f"{class_name}.sol",
+                             f"{class_name}.abi")
+
+        p1bin = os.path.join(self.WORKSPACE_PATH,
+                             self.OUTPUT_BUILD,
+                             f"{class_name}.sol",
+                             f"{class_name}.bin")
         try:
             self._bin = codecs.open(p1bin, 'r', 'utf-8-sig').read()
             self._abi = json.load(codecs.open(p2abi, 'r', 'utf-8-sig'))
 
         except FileNotFoundError:
-            message_exit("The artifacts files are not found from forge builds.", 3)
+            message_exit(f"The artifacts files are not found from forge builds. {class_name}", 3)
 
         return self
 
     def GetCodeClassFromBuild(self, class_name: str) -> "SolWeb3Tool":
         """
         get the independent files and content from the file system
         :param class_name:
@@ -415,23 +486,14 @@
         get the code and abi from combined.json
         :param path:
         :param classname:
         :return:
         """
         return self.GetCodeTag(self.byClassName(path, classname))
 
-    def CompileBash(self) -> None:
-        """
-        This is the remote command to execute the solc_remote bash file
-        using remote compile method to compile the sol files
-        all works will be done with the remote server or using the docker
-        """
-        list_files = subprocess.run(["{}/solc_remote".format(self.WORKSPACE_PATH)])
-        print("The exit code was: %d" % list_files.returncode)
-
     @property
     def abi(self) -> str:
         return self._abi
 
     @property
     def bin(self) -> str:
         return self._bin
@@ -472,39 +534,71 @@
         self.is_deploy = False
         self.is_internal = False
         self.is_forge = False
         self.is_flashbot_prc = False
         self.deployed_address = False
         self.last_class = ""
         self.list_type = "list_address"
-        ok = self.switchNetowrk(node)
+        ok = self.switch_network(node)
         if not ok:
             exit(88)
 
-    def switchNetowrk(self, _node_config: Config) -> bool:
+    def switch_network(self, _node_config: Config) -> bool:
+        """
+        the job is to make sure the network of the node is working properly or otherwise it will check and find the best node possible to connect with.
+        :param _node_config: the instance of the configuration
+        :return: true or false after double check all the network and connections
+        """
         self.network_cfg = _node_config
-        self.configUrl(_node_config.rpc_url)
-        result = self.w3.isConnected()
-        if not result:
-            print(
-                f"try to connect {self.network_cfg.network_name}  {Bolors.WARNING} {self.network_cfg.rpc_url}: {result} {Bolors.RESET}")
-            return False
-        else:
-            print(
-                f"You are now connected to {Bolors.OK} {self.network_cfg.network_name} {self.network_cfg.rpc_url} {Bolors.RESET}")
-            return True
+        use_single = True
+        c = 0
+        while True:
+            try:
+                if isinstance(_node_config.rpc_url, str):
+                    self.configUrl(_node_config.rpc_url)
+                if isinstance(_node_config.rpc_url, list):
+                    use_single = False
+                    _url = random.choice(_node_config.rpc_url)
+                    self.configUrl(_url)
+            except FileNotFoundError as f:
+                self.error(str(f))
+                continue
+
+            except ValueError as e:
+                self.error(str(e))
+                continue
+
+            if not self.w3.isConnected():
+                mes = f"try to connect {self.network_cfg.network_name} {Bolors.WARNING} {self.network_cfg.rpc_url} {Bolors.RESET} - {c}"
+                self.error(mes)
+                if c > _node_config.reconnect_tries and use_single:
+                    self.error(f"error from {_node_config.reconnect_tries} reached.")
+                    return False
+                c += 1
+                if use_single:
+                    time.sleep(10)
+                else:
+                    time.sleep(4)
+                continue
+            else:
+                d = f"You are now connected to {Bolors.OK} {self.network_cfg.network_name} {self.network_cfg.rpc_url} {Bolors.RESET}"
+                self.error(d)
+                return True
+
+    def error(self, msg: str):
+        t = str(datetime.datetime.now())
+        print(msg + t)
 
     def configUrl(self, url: str) -> None:
         """
         The url can be anything including http, https, ws, ipc, rpc
         :param url: any connection endpoint
         :return:
         """
         self.w3 = web3_provider(url)
-
         if "flastbot" in url:
             self.is_flashbot_prc = True
 
     def withPOA(self) -> "MiliDoS":
         """
         the normal usual term to fix some POA related problems
         :return:
@@ -530,20 +624,43 @@
         connect the existing deployed contract
         :param workspace: the workspace directory
         :param history: the deployed history folder under the deploy_history
         :return:
         """
         self.is_deploy = False
         self.artifact_manager = SolWeb3Tool()
+        self.pathfinder = Paths(workspace)
         if history is False:
-            self.pathfinder = Paths(workspace).setDefaultPath().Network(self.network_cfg.network_name)
+            self.pathfinder.setDefaultPath()
         else:
-            self.pathfinder = Paths(workspace).SetUseHistory(history).Network(self.network_cfg.network_name)
+            self.pathfinder.SetUseHistory(history)
+        self.pathfinder.Network(self.network_cfg.network_name)
+        self.ready_io(True)
+
+    def brew(self, workspace: str, factory: str, history: any = False) -> "MiliDoS":
+        """
+        brew solidity piplines and flow
+        :param workspace:
+        :param factory:
+        :param history:
+        :return:
+        """
+        self.is_deploy = False
+        self.artifact_manager = SolWeb3Tool()
+        self.artifact_manager.setBasePath(workspace)
+        self.pathfinder = Paths(workspace)
+        if history is False:
+            self.pathfinder.setDefaultPath()
+        else:
+            self.pathfinder.SetUseHistory(history)
+        self.pathfinder.Network(self.network_cfg.network_name)
+        self.pathfinder.setFactory(factory)
 
         self.ready_io(True)
+        return self
 
     def SetupContract(self):
         pass
 
     def GetNode(self) -> Config:
         return self.network_cfg
 
@@ -597,35 +714,44 @@
             exit(0)
         self.pathfinder.setSolVersion(ver)
         self.pathfinder.setEvm(self.EVM_VERSION)
         BuildRemoteLinuxCommand(self.pathfinder, self._optimizations, self._sol_list, self._sol_link)
         return self
 
     def useForge(self) -> "MiliDoS":
+        """
+        use the forge
+        :return:
+        """
+        self.is_forge = True
+        BuildForgeLinuxBuildCommand(self.pathfinder)
+        self.artifact_manager.ForgeGen()
         # ==================================================
         if self._sol_list is not None:
             for v in self._sol_list:
                 based_name = os.path.basename(v)
                 class_name = based_name.replace(".sol", "")
                 # class_name_process = filter_file_name(based_name).replace('.sol', '')
                 self.artifact_manager.SplitForgeBuild(class_name)
-        self.is_forge = True
+
         return self
 
     def localTranspile(self, dapp_ts_folder: str = None) -> "MiliDoS":
         """
         :param dapp_ts_folder: the destination is follow by this path {dapp_ts_folder}/src/api/abi/xxx.ts
         if this valuable is None then there will not be any copy files to the destination
         :return: instance of moody
         """
         self.pathfinder.updateTargetDappFolder(dapp_ts_folder)
         if self.is_forge:
             BuildLangForge(self.pathfinder, self._sol_list)
         else:
             BuildLang(self.pathfinder, self._sol_list)
+
+        self.artifact_manager.RunTranspile()
         return self
 
     def get_block(self, block_identifier, full_transactions: bool = False):
         """
         to see the block information
         :param block_identifier:
         :param full_transactions:
```

### Comparing `moodyeth-4.44/moody/m/b_send/__init__.py` & `moodyeth-4.57/moody/m/b_send/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/b_send/basec.py` & `moodyeth-4.57/moody/m/b_send/basec.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/b_send/looper.py` & `moodyeth-4.57/moody/m/b_send/looper.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/b_send2/__init__.py` & `moodyeth-4.57/moody/m/b_send2/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/bases.py` & `moodyeth-4.57/moody/m/bases.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/beri_coin/__init__.py` & `moodyeth-4.57/moody/m/beri_coin/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/blockhash_store/__init__.py` & `moodyeth-4.57/moody/m/blockhash_store/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/c_token/__init__.py` & `moodyeth-4.57/moody/m/c_token/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/deposit_contract/__init__.py` & `moodyeth-4.57/moody/m/deposit_contract/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/eth2_multi_deposit/__init__.py` & `moodyeth-4.57/moody/m/eth2_multi_deposit/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/kyc/merkletree.py` & `moodyeth-4.57/moody/m/kyc/merkletree.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/layer_zero_u_s_d_t/__init__.py` & `moodyeth-4.57/moody/m/layer_zero_u_s_d_t/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/multicall/__init__.py` & `moodyeth-4.57/moody/m/multicall/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/multicall/execute.py` & `moodyeth-4.57/moody/m/multicall/execute.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/multicall2/__init__.py` & `moodyeth-4.57/moody/m/multicall2/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/multicall2/execute.py` & `moodyeth-4.57/moody/m/multicall2/execute.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/oracle/__init__.py` & `moodyeth-4.57/moody/m/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/pharaohs/__init__.py` & `moodyeth-4.57/moody/m/pharaohs/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/proxy_admin/__init__.py` & `moodyeth-4.57/moody/m/proxy_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/tc20/__init__.py` & `moodyeth-4.57/moody/m/tc20/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/tether_token2/__init__.py` & `moodyeth-4.57/moody/m/tether_token2/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/transparent_upgradeable_proxy/__init__.py` & `moodyeth-4.57/moody/m/transparent_upgradeable_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/tx_params.py` & `moodyeth-4.57/moody/m/tx_params.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/verify/http.py` & `moodyeth-4.57/moody/m/verify/http.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/verify/solfla.py` & `moodyeth-4.57/moody/m/verify/solfla.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/m/verify/verify.py` & `moodyeth-4.57/moody/m/verify/verify.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/paths.py` & `moodyeth-4.57/moody/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,25 @@
     TARGET_LOC = "/root/contracts"
     # ---- including the local bash file
     LOCAL_BASH_INCLUDE = "inc"
     COMPRESSED_NAME = "solc-build.tar.gz"
     SOLC_VER = "0.5.15"
     SOLCPATH = "/root/contracts/vault"
     EVM_VERSION = Evm.ISTANBUL
+    # the workspace
     BUILDPATH = ""
+    # the source code including all the transpile factory codes
+    FACTORY_PATH = ""
+    # forge use only
+    SOURCE_PATH = "vault"
+    # forge use only
+    FORGE_BUILD = "build"
+    # addition application to deliver
     WEB_DAPP_SRC = None
+    # sub fix
     SUB_FIX = ""
 
     def __init__(self, root_path_as_workspace):
         self.___workspace = root_path_as_workspace
         self.___current_deployment_path = os.path.join(self.___workspace, self.ACTION_FOLDER)
         self.___network_name = "mainnet"
         self.BUILDPATH = root_path_as_workspace
@@ -59,14 +68,18 @@
     def showCurrentDeployedClass(cls, class_name: str) -> str:
         return cls.NAME_FILE_EXX.format(cls.ACTION_FOLDER, class_name)
 
     def updateTargetDappFolder(self, folderName: str) -> "Paths":
         self.WEB_DAPP_SRC = folderName
         return self
 
+    def setFactory(self, fac: str) -> "Paths":
+        self.FACTORY_PATH = fac
+        return self
+
     def setSolVersion(self, version: str) -> "Paths":
         self.SOLC_VER = version
         return self
 
     def setEvm(self, ver: str) -> "Paths":
         self.EVM_VERSION = ver
         return self
@@ -87,15 +100,16 @@
 
     @property
     def __playerAddrsFilePath(self) -> str:
         return os.path.join(self.___current_deployment_path, "{}.json".format(self.COLLECTION_CONTRACTS))
 
     @property
     def __deploymentPath(self) -> str:
-        return os.path.join(self.___current_deployment_path, self.DEPLOYMENT_FILE_NAME.format(self.___network_name, self.subFix))
+        return os.path.join(self.___current_deployment_path,
+                            self.DEPLOYMENT_FILE_NAME.format(self.___network_name, self.subFix))
 
     @property
     def SaveDeployConfig(self) -> str:
         return self.__deploymentPath
 
     @property
     def SavePlayersList(self) -> str:
```

### Comparing `moodyeth-4.44/moody/upgrade/Token.py` & `moodyeth-4.57/moody/upgrade/Token.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/upgrade/__init__.py` & `moodyeth-4.57/moody/upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moody/upgrade/deployupgradable.py` & `moodyeth-4.57/moody/upgrade/deployupgradable.py`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/moodyeth.egg-info/requires.txt` & `moodyeth-4.57/moodyeth.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `moodyeth-4.44/setup.py` & `moodyeth-4.57/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 #!/usr/bin/env python
 # --------------------------------------------------------------------
 # Copyright (c) TokenChain. All rights reserved.
 # Licensed under the MIT License.
 # See License.txt in the project root for license information.
+#
+#
+#     :copyright: © 2021 by the TokenChain.
+#     :license: MIT License
 # --------------------------------------------------------------------
 
-"""
-    setup
-    =====
-
-    Tron: A Python API for interacting with ETH (EVM)
-
-    :copyright: © 2021 by the TokenChain.
-    :license: MIT License
-"""
-
 import codecs
 import os
 import platform
 
+import pypandoc
 from setuptools import (
     find_packages,
     setup,
 )
+
 _dir = os.path.dirname(__file__)
 py_version = platform.python_version()
 
 
-def find_version():
+def find_version() -> str:
     f = codecs.open('version', 'r', 'utf-8-sig')
-    line = f.readline()
+    new_ver = f.readline().strip().replace("\n", "")
     f.close()
-    return line
+    edit_at_line(new_ver)
+    return new_ver
+
 
-def finedescription():
-    line = ''
-    with open(os.path.join(_dir, 'README.rst')) as f:
-        line = f.read()
-    return line
+def edit_at_line(version: str):
+    file = 'moody/__init__.py'
+    lines = []
+    with open(file, "r") as f:
+        lines = f.readlines()
+        f.close()
+        o = 0
+        for h in lines:
+            if "__version__" in h:
+                lines[o] = f"__version__ = '{version}'"
+                break
+            o += 1
+    if len(lines) > 0:
+        with open(file, "w") as f:
+            f.write("".join(lines))
+            f.close()
+
+
+_dir = os.path.dirname(__file__)
+py_version = platform.python_version()
 
-PACKAGE_VERSION = str(find_version())
-PACKAGE_LONG_DESCRIPTION = str(finedescription())
 EXTRAS_REQUIRE = {
     "tester": [
         "coverage",
         "pep8",
         "pyflakes",
         "pylint",
         "pytest-cov"
@@ -95,35 +106,44 @@
     "mypy-extensions==0.4.3",
     "web3>=5.20.0",
     "eth-utils==1.10.0",
     "eth-uniswap==0.0.2"
 ]
 
 
+def convert_rst():
+    output = pypandoc.convert_file(os.path.join('README.md'), 'rst', format='md', outputfile='README.rst')
+    io = open('README.rst', 'r')
+    package_description = io.read()
+    return 'README.rst'
+
+
 setup(
     name='moodyeth',
-    version=PACKAGE_VERSION,
+    version=find_version(),
     description='A Python API for interacting with Ethereum based networks',
-    long_description=PACKAGE_LONG_DESCRIPTION,
+    long_description=convert_rst(),
     long_description_content_type='text/x-rst',
     keywords='ethereum eth-api eth-api-python eth-base cli sdk pentest',
     url='https://github.com/tokenchain/moodyeth',
     author='Heskemo',
-    author_email='jobhesk@gmail.com',
+    author_email='topdog@onekexx.com',
     license='MIT License',
     zip_safe=False,
-    python_requires='>=3.6,<4',
+    python_requires='>=3.8,<4',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Topic :: Software Development :: Code Generators',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
-    packages=find_packages(exclude=['examples','lab','test']),
+    packages=find_packages(exclude=['examples', 'lab', 'test']),
     include_package_data=True,
     install_requires=install_requires,
     tests_require=EXTRAS_REQUIRE['tester'],
     extras_require=EXTRAS_REQUIRE,
 )
```

### Comparing `moodyeth-4.44/update` & `moodyeth-4.57/update`

 * *Files 18% similar despite different names*

```diff
@@ -21,72 +21,72 @@
     echo "${new// /.}"
   elif [[ "$OSTYPE" == "cygwin" ]]; then
     echo "not correct system - cygwin detected"
     exit
   fi
 }
 
-
-swap_src(){
+swap_src() {
   local DEV_SRC=$HOME/Documents/b95/devmoody/moody
   local DEPLOY_SRC=$HOME/Documents/piplines/moodyeth/moody
   if [[ -d "$DEV_SRC" ]]; then
     echo "now swapping the source code"
     rm -rf moody
     cp -R $DEV_SRC $DEPLOY_SRC
   fi
 }
-gen_doc(){
+gen_doc() {
   sudo rm -rf dist
   rm -rf docs
   python3 -m pdoc --html moody
   mkdir -p docs
 
   if [[ -d html/moody ]]; then
     mv html/moody docs/moody
   fi
-  
+
   if [[ -d html ]]; then
     rm -rf html
   fi
 }
 pub_ver() {
   VERSION=$(cat version)
   increment_version $VERSION >version
   VERSION=$(cat version)
-  
 
-  python3 -m pip install --user --upgrade setuptools wheel
+  python3.11 -m pip install --user --upgrade setuptools wheel
   # python3 -m pip install --upgrade setuptools wheel
-  python3 -m readme_renderer README.rst -o ./html/README.html
-  sudo python3 setup.py clean sdist bdist_wheel
+  # python3.11 -m readme_renderer README.rst -o ./html/README.html
+  sudo python3.11 setup.py clean sdist bdist_wheel
 
   echo "========================================================="
   echo "now uploading the content to pypi"
-  python3 -m twine upload dist/* --verbose
-
+  python3.11 -m twine upload dist/* --verbose
   echo "please update the package by using this command"
   echo "pip3 install moodyeth==$VERSION"
   echo "pip3 install moodyeth==$VERSION --upgrade"
   echo "pi moodyeth==$VERSION"
   echo "pc moodyeth==$VERSION"
   echo "wait 30 seconds until it gets uploaded online..."
+  sudo rm -rf dist
   # echo "ready and install it again.."
   # sudo pip3 install --proxy 127.0.0.1:1087 moodyeth==$VERSION
 }
-
 git_update() {
+  local gitcheck=$(git diff --shortstat)
   git add .
-  #git remote add origin https://gitee.com/jjhoc/moodyeth.git
-  git commit -m "auto patched"
-  #git remote add origin https://gitee.com/jjhoc/b-explorer-settings.git
-  git push
+  echo "Please enter your commit message:"
+  # shellcheck disable=SC2162
+  read name
+  git commit -m "♻️ $name $gitcheck"
+  git push origin
+  git push github
+  echo "♻️ You can open ${GIT_LOC} or git clone ${GIT_LOC}.git to copy to the local"
 }
-
-serv_doc(){
+serv_doc() {
   ran -r docs/moody -p 8080
 }
 swap_src
-gen_doc
+# gen_doc
 pub_ver
-git_update
-#serv_doc
+#git_update
+#serv_doc
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

