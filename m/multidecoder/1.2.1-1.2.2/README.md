# Comparing `tmp/multidecoder-1.2.1.tar.gz` & `tmp/multidecoder-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidecoder-1.2.1.tar", last modified: Fri Feb 23 22:16:37 2024, max compression
+gzip compressed data, was "multidecoder-1.2.2.tar", last modified: Mon Apr 15 17:31:57 2024, max compression
```

## Comparing `multidecoder-1.2.1.tar` & `multidecoder-1.2.2.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.399981 multidecoder-1.2.1/
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-02-23 22:15:53.000000 multidecoder-1.2.1/.git-blame-ignore-revs
--rw-r--r--   0 vsts      (1001) docker     (127)     2097 2024-02-23 22:15:53.000000 multidecoder-1.2.1/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.371980 multidecoder-1.2.1/.vscode/
--rw-r--r--   0 vsts      (1001) docker     (127)      616 2024-02-23 22:15:53.000000 multidecoder-1.2.1/.vscode/settings.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-02-23 22:15:53.000000 multidecoder-1.2.1/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-02-23 22:15:53.000000 multidecoder-1.2.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-02-23 22:16:37.399981 multidecoder-1.2.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-02-23 22:15:53.000000 multidecoder-1.2.1/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.371980 multidecoder-1.2.1/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-02-23 22:15:53.000000 multidecoder-1.2.1/pipelines/azure-tests.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-02-23 22:15:53.000000 multidecoder-1.2.1/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)      658 2024-02-23 22:15:53.000000 multidecoder-1.2.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-02-23 22:16:37.399981 multidecoder-1.2.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-02-23 22:15:53.000000 multidecoder-1.2.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.367980 multidecoder-1.2.1/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.375980 multidecoder-1.2.1/src/multidecoder/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1641 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.375980 multidecoder-1.2.1/src/multidecoder/decoders/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4389 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/base64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/chr.py
--rw-r--r--   0 vsts      (1001) docker     (127)      548 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/codec.py
--rw-r--r--   0 vsts      (1001) docker     (127)      955 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/concat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/filename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/javascript.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11393 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/network.py
--rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/path.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1158 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/replace.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6321 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/shell.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/vba.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/decoders/xml.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21889 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/domains.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/hit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/json_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keyword.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.379980 multidecoder-1.2.1/src/multidecoder/keywords/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.395981 multidecoder-1.2.1/src/multidecoder/keywords/api/
--rw-r--r--   0 vsts      (1001) docker     (127)     4040 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.advapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       23 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.apphelp
--rw-r--r--   0 vsts      (1001) docker     (127)     1212 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.atl
--rw-r--r--   0 vsts      (1001) docker     (127)      243 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.atl80
--rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.atl90
--rw-r--r--   0 vsts      (1001) docker     (127)      429 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.au3zip
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.avicap32
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.cabinet
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.clbcatq
--rw-r--r--   0 vsts      (1001) docker     (127)       56 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.cmdial32
--rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.comctl32
--rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.credui
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.cryptbase
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.cryptdll
--rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.cscapi
--rw-r--r--   0 vsts      (1001) docker     (127)      610 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.dbghelp
--rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.devmgr
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.dnsapi
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.drprov
--rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.dsound
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.dsuiext
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.esent
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.fveapi
--rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.fwpuclnt
--rw-r--r--   0 vsts      (1001) docker     (127)     1913 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.gdi32
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.gina
--rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.icmp
--rw-r--r--   0 vsts      (1001) docker     (127)     1254 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.imagehlp
--rw-r--r--   0 vsts      (1001) docker     (127)     1005 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.iphlpapi
--rw-r--r--   0 vsts      (1001) docker     (127)    19404 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.kernel32
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.kernelbase
--rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.libeay32
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.lsasrv
--rw-r--r--   0 vsts      (1001) docker     (127)      265 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mapi32
--rw-r--r--   0 vsts      (1001) docker     (127)     1968 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mfc42
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mpr
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mprapi
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msacm32
--rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msasn1
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mscoree
--rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msi
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msimg32
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mspdb80
--rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mssign32
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msutb
--rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msvbvm60
--rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msvcrt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.msvfw32
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mswsock
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.mydocs
--rw-r--r--   0 vsts      (1001) docker     (127)      525 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.nddeapi
--rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.netapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       20 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.netplwiz
--rw-r--r--   0 vsts      (1001) docker     (127)     4660 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.ntdll
--rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.ntdsapi
--rw-r--r--   0 vsts      (1001) docker     (127)     1137 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.ntoskrnl
--rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.ntshrui
--rw-r--r--   0 vsts      (1001) docker     (127)     1599 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.odbc32
--rw-r--r--   0 vsts      (1001) docker     (127)      970 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.odbccp32
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.odbctrac
--rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.ole32
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.oleaut32
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.oledlg
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.onex
--rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.packet
--rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.pdh
--rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.powrprof
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.psapi
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.pstorec
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.query
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.rasapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.rastapi
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.riched20
--rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.rpcrt4
--rw-r--r--   0 vsts      (1001) docker     (127)       99 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.scarddlg
--rw-r--r--   0 vsts      (1001) docker     (127)     1561 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.scecli
--rw-r--r--   0 vsts      (1001) docker     (127)      729 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.se
--rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.secur32
--rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.sensapi
--rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.setupapi
--rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.sfc
--rw-r--r--   0 vsts      (1001) docker     (127)     3672 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.shell32
--rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.shimgvw
--rw-r--r--   0 vsts      (1001) docker     (127)      544 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.shlwapi
--rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.shsvcs
--rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.ssleay32
--rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.unknown
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.urlmon
--rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.user32
--rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.userenv
--rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.usp10
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.version
--rw-r--r--   0 vsts      (1001) docker     (127)      312 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winhttp
--rw-r--r--   0 vsts      (1001) docker     (127)      928 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wininet
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winmm
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winscard
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winshfhc
--rw-r--r--   0 vsts      (1001) docker     (127)     1994 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winsock
--rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winspool
--rw-r--r--   0 vsts      (1001) docker     (127)     3887 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.winsta
--rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wintrust
--rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wlanapi
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wldap32
--rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wship6
--rw-r--r--   0 vsts      (1001) docker     (127)      754 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wsnmp32
--rw-r--r--   0 vsts      (1001) docker     (127)      490 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/api/api.wtsapi32
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/archive
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/av.name
--rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/cryptography
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/debugger.device.name
--rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/enable_content
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/environment.windows
--rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/event
--rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/guid
--rw-r--r--   0 vsts      (1001) docker     (127)     1091 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/key
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/network.protocol
--rw-r--r--   0 vsts      (1001) docker     (127)      532 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/network.string
--rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/oid
--rw-r--r--   0 vsts      (1001) docker     (127)     2674 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/os_name
--rw-r--r--   0 vsts      (1001) docker     (127)     1476 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/powershell.cmdlet
--rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/privilege
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/ransomware.string
--rw-r--r--   0 vsts      (1001) docker     (127)      263 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/sandbox.id
--rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/security_identifier
--rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/user_agent
--rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/vba.name
--rw-r--r--   0 vsts      (1001) docker     (127)     2164 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords/windows.registry
--rw-r--r--   0 vsts      (1001) docker     (127)    22786 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/keywords_to_review.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/node.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1938 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/query.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2440 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/string_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-02-23 22:15:53.000000 multidecoder-1.2.1/src/multidecoder/xor_helper.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.399981 multidecoder-1.2.1/src/multidecoder.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-23 22:16:10.000000 multidecoder-1.2.1/src/multidecoder.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-23 22:16:37.000000 multidecoder-1.2.1/src/multidecoder.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.395981 multidecoder-1.2.1/stubs/
--rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-02-23 22:15:53.000000 multidecoder-1.2.1/stubs/pefile.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.395981 multidecoder-1.2.1/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/requirements.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-23 22:16:37.399981 multidecoder-1.2.1/tests/test_decoders/
--rw-r--r--   0 vsts      (1001) docker     (127)     2953 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_base64.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_chr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2149 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_concat.py
--rw-r--r--   0 vsts      (1001) docker     (127)      564 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_encoding.py
--rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_filename.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_hex.py
--rw-r--r--   0 vsts      (1001) docker     (127)      305 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_javascript.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8138 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_network.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1014 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_path.py
--rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_replace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10397 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_shell.py
--rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_vba.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_decoders/test_xml.py
--rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      914 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)      809 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tests/test_xor_helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-02-23 22:15:53.000000 multidecoder-1.2.1/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.597282 multidecoder-1.2.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-15 17:31:18.000000 multidecoder-1.2.2/.git-blame-ignore-revs
+-rw-r--r--   0 vsts      (1001) docker     (127)     2097 2024-04-15 17:31:18.000000 multidecoder-1.2.2/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.561282 multidecoder-1.2.2/.vscode/
+-rw-r--r--   0 vsts      (1001) docker     (127)      616 2024-04-15 17:31:18.000000 multidecoder-1.2.2/.vscode/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-04-15 17:31:18.000000 multidecoder-1.2.2/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-15 17:31:18.000000 multidecoder-1.2.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-15 17:31:57.597282 multidecoder-1.2.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-04-15 17:31:18.000000 multidecoder-1.2.2/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.561282 multidecoder-1.2.2/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-15 17:31:18.000000 multidecoder-1.2.2/pipelines/azure-tests.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1255 2024-04-15 17:31:18.000000 multidecoder-1.2.2/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)      658 2024-04-15 17:31:18.000000 multidecoder-1.2.2/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      929 2024-04-15 17:31:57.601282 multidecoder-1.2.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-04-15 17:31:18.000000 multidecoder-1.2.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.557282 multidecoder-1.2.2/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.565282 multidecoder-1.2.2/src/multidecoder/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1641 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      411 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.569282 multidecoder-1.2.2/src/multidecoder/decoders/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4389 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/base64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      569 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/chr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      548 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      955 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/concat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      591 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/filename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1613 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12211 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      550 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1147 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/replace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6227 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/shell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1597 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/vba.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/decoders/xml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21889 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/domains.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/hit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1211 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/json_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1181 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keyword.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.573282 multidecoder-1.2.2/src/multidecoder/keywords/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.593282 multidecoder-1.2.2/src/multidecoder/keywords/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4040 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.advapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       23 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.apphelp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1212 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.atl
+-rw-r--r--   0 vsts      (1001) docker     (127)      243 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.atl80
+-rw-r--r--   0 vsts      (1001) docker     (127)      229 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.atl90
+-rw-r--r--   0 vsts      (1001) docker     (127)      429 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.au3zip
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.avicap32
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.cabinet
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.clbcatq
+-rw-r--r--   0 vsts      (1001) docker     (127)       56 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.cmdial32
+-rw-r--r--   0 vsts      (1001) docker     (127)      177 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.comctl32
+-rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.credui
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.cryptbase
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.cryptdll
+-rw-r--r--   0 vsts      (1001) docker     (127)       24 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.cscapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      610 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.dbghelp
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.devmgr
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.dnsapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.drprov
+-rw-r--r--   0 vsts      (1001) docker     (127)      225 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.dsound
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.dsuiext
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.esent
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.fveapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      127 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.fwpuclnt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1913 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.gdi32
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.gina
+-rw-r--r--   0 vsts      (1001) docker     (127)      100 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.icmp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1254 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.imagehlp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1005 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.iphlpapi
+-rw-r--r--   0 vsts      (1001) docker     (127)    19404 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.kernel32
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.kernelbase
+-rw-r--r--   0 vsts      (1001) docker     (127)     2218 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.libeay32
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.lsasrv
+-rw-r--r--   0 vsts      (1001) docker     (127)      265 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)     1968 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mfc42
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mpr
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mprapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msacm32
+-rw-r--r--   0 vsts      (1001) docker     (127)       81 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msasn1
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mscoree
+-rw-r--r--   0 vsts      (1001) docker     (127)     4043 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msi
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msimg32
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mspdb80
+-rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mssign32
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msutb
+-rw-r--r--   0 vsts      (1001) docker     (127)     1527 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msvbvm60
+-rw-r--r--   0 vsts      (1001) docker     (127)     3448 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msvcrt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.msvfw32
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mswsock
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.mydocs
+-rw-r--r--   0 vsts      (1001) docker     (127)      525 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.nddeapi
+-rw-r--r--   0 vsts      (1001) docker     (127)     1276 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.netapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       20 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.netplwiz
+-rw-r--r--   0 vsts      (1001) docker     (127)     4660 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.ntdll
+-rw-r--r--   0 vsts      (1001) docker     (127)      197 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.ntdsapi
+-rw-r--r--   0 vsts      (1001) docker     (127)     1137 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.ntoskrnl
+-rw-r--r--   0 vsts      (1001) docker     (127)       43 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.ntshrui
+-rw-r--r--   0 vsts      (1001) docker     (127)     1599 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.odbc32
+-rw-r--r--   0 vsts      (1001) docker     (127)      970 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.odbccp32
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.odbctrac
+-rw-r--r--   0 vsts      (1001) docker     (127)      829 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.ole32
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.oleaut32
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.oledlg
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.onex
+-rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.packet
+-rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.pdh
+-rw-r--r--   0 vsts      (1001) docker     (127)     2236 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.powrprof
+-rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.psapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.pstorec
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.query
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.rasapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.rastapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.riched20
+-rw-r--r--   0 vsts      (1001) docker     (127)     1207 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.rpcrt4
+-rw-r--r--   0 vsts      (1001) docker     (127)       99 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.scarddlg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1561 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.scecli
+-rw-r--r--   0 vsts      (1001) docker     (127)      729 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.se
+-rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.secur32
+-rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.sensapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      239 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.setupapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      123 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.sfc
+-rw-r--r--   0 vsts      (1001) docker     (127)     3672 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.shell32
+-rw-r--r--   0 vsts      (1001) docker     (127)       15 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.shimgvw
+-rw-r--r--   0 vsts      (1001) docker     (127)      544 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.shlwapi
+-rw-r--r--   0 vsts      (1001) docker     (127)       26 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.shsvcs
+-rw-r--r--   0 vsts      (1001) docker     (127)     1328 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.ssleay32
+-rw-r--r--   0 vsts      (1001) docker     (127)       86 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.unknown
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.urlmon
+-rw-r--r--   0 vsts      (1001) docker     (127)     1564 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.user32
+-rw-r--r--   0 vsts      (1001) docker     (127)      309 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.userenv
+-rw-r--r--   0 vsts      (1001) docker     (127)      114 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.usp10
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.version
+-rw-r--r--   0 vsts      (1001) docker     (127)      312 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winhttp
+-rw-r--r--   0 vsts      (1001) docker     (127)      928 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wininet
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winmm
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winscard
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winshfhc
+-rw-r--r--   0 vsts      (1001) docker     (127)     1994 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winsock
+-rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winspool
+-rw-r--r--   0 vsts      (1001) docker     (127)     3887 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.winsta
+-rw-r--r--   0 vsts      (1001) docker     (127)       14 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wintrust
+-rw-r--r--   0 vsts      (1001) docker     (127)       55 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wlanapi
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wldap32
+-rw-r--r--   0 vsts      (1001) docker     (127)      266 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wship6
+-rw-r--r--   0 vsts      (1001) docker     (127)      754 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wsnmp32
+-rw-r--r--   0 vsts      (1001) docker     (127)      490 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/api/api.wtsapi32
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/archive
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/av.name
+-rw-r--r--   0 vsts      (1001) docker     (127)      503 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/cryptography
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/debugger.device.name
+-rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/enable_content
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/environment.windows
+-rw-r--r--   0 vsts      (1001) docker     (127)      634 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/event
+-rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/guid
+-rw-r--r--   0 vsts      (1001) docker     (127)     1091 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/key
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/network.protocol
+-rw-r--r--   0 vsts      (1001) docker     (127)      532 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/network.string
+-rw-r--r--   0 vsts      (1001) docker     (127)     1812 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/oid
+-rw-r--r--   0 vsts      (1001) docker     (127)     2674 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/os_name
+-rw-r--r--   0 vsts      (1001) docker     (127)     1476 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/powershell.cmdlet
+-rw-r--r--   0 vsts      (1001) docker     (127)      873 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/privilege
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/ransomware.string
+-rw-r--r--   0 vsts      (1001) docker     (127)      263 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/sandbox.id
+-rw-r--r--   0 vsts      (1001) docker     (127)      902 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/security_identifier
+-rw-r--r--   0 vsts      (1001) docker     (127)      151 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/user_agent
+-rw-r--r--   0 vsts      (1001) docker     (127)       53 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/vba.name
+-rw-r--r--   0 vsts      (1001) docker     (127)     2164 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords/windows.registry
+-rw-r--r--   0 vsts      (1001) docker     (127)    22786 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/keywords_to_review.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     2950 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3777 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1938 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/query.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2440 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      465 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/string_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-15 17:31:18.000000 multidecoder-1.2.2/src/multidecoder/xor_helper.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.597282 multidecoder-1.2.2/src/multidecoder.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2739 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7266 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       60 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-15 17:31:30.000000 multidecoder-1.2.2/src/multidecoder.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-15 17:31:57.000000 multidecoder-1.2.2/src/multidecoder.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.593282 multidecoder-1.2.2/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-15 17:31:18.000000 multidecoder-1.2.2/stubs/pefile.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.593282 multidecoder-1.2.2/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/requirements.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 17:31:57.597282 multidecoder-1.2.2/tests/test_decoders/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2953 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_base64.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_chr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2149 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_concat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      564 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      396 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_filename.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1644 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_hex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      305 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_javascript.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10449 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_network.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1014 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_path.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_replace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10165 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_shell.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_vba.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_decoders/test_xml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      892 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      914 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      809 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tests/test_xor_helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-04-15 17:31:18.000000 multidecoder-1.2.2/tox.ini
```

### Comparing `multidecoder-1.2.1/.gitignore` & `multidecoder-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/.vscode/settings.json` & `multidecoder-1.2.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/LICENSE.md` & `multidecoder-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/PKG-INFO` & `multidecoder-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 1.2.1
+Version: 1.2.2
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidecoder Version: 1.2.1 Summary: A context
+Metadata-Version: 2.1 Name: multidecoder Version: 1.2.2 Summary: A context
 preserving IOC extraction library Home-page: https://github.com/
 CybercentreCanada/Multidecoder Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca License: MIT Project-URL: Bug Tracker,
 https://github.com/CybercentreCanada/Multidecoder/issues Keywords:
 malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
```

### Comparing `multidecoder-1.2.1/README.md` & `multidecoder-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/pipelines/azure-tests.yaml` & `multidecoder-1.2.2/pipelines/azure-tests.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/pipelines/publish.yaml` & `multidecoder-1.2.2/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/pyproject.toml` & `multidecoder-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/setup.cfg` & `multidecoder-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/__main__.py` & `multidecoder-1.2.2/src/multidecoder/__main__.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/base64.py` & `multidecoder-1.2.2/src/multidecoder/decoders/base64.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/chr.py` & `multidecoder-1.2.2/src/multidecoder/decoders/chr.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/codec.py` & `multidecoder-1.2.2/src/multidecoder/decoders/codec.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/concat.py` & `multidecoder-1.2.2/src/multidecoder/decoders/concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/filename.py` & `multidecoder-1.2.2/src/multidecoder/decoders/filename.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/hex.py` & `multidecoder-1.2.2/src/multidecoder/decoders/hex.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/network.py` & `multidecoder-1.2.2/src/multidecoder/decoders/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 # #-/ is the same with # and /
 # #-& is #-/ but stopped before '
 URL_RE = (
     rb"(?i)(?:ftp|https?)://"  # scheme
     rb"(?:[\w!$-.:;=~@]{,2000}@)?"  # userinfo
     rb"(?:(?!%5B)[%A-Z0-9.-]{4,253}|(?:\[|%5B)[%0-9A-F:]{3,117}(?:\]|%5D))"  # host
     rb"(?::[0-6]?[0-9]{0,4})?"  # port
-    rb"(?:[/?#](?:[\w!#-/:;=@?~]{,2000}[\w!#-&(*+\-/:;=@?~])?)?"  # path, query and fragment
-    # The final char class stops urls from ending in ' ) , or .
+    rb"(?:[/?#](?:[\w!#-/:;=@?~]{,2000}[\w!#-&(*+\-/:=@?~])?)?"  # path, query and fragment
+    # The final char class stops urls from ending in ' ) , . or ;
     # to prevent trailing characters from being included in the url.
 )
 
 
 # Regex validators
 def is_domain(domain: bytes) -> bool:
     """Validates a potential domain.
@@ -113,30 +113,54 @@
     """Find email addresses in data"""
     return [match_to_hit(EMAIL_TYPE, match) for match in re.finditer(EMAIL_RE, data) if is_domain(match.group(1))]
 
 
 @decoder
 def find_ips(data: bytes) -> list[Node]:
     """Find ip addresses in data"""
-    return [parse_ip(match.group()).shift(match.start()) for match in re.finditer(IP_RE, data) if is_ip(match.group())]
+    out = []
+    for match in re.finditer(IP_RE, data):
+        ip = match.group()
+        if not is_ip(ip):
+            continue
+        start, end = match.span()
+        if data[start - 3 : start] == b"<t>" and data[end : end + 4] == b"</t>":
+            continue  # xml section numbering
+        if data[start - 8 : start - 1] == b"Version" and data[start - 1 : start] in (b"\0", b"="):
+            continue  # version number, not an ip address
+        out.append(parse_ip(match.group()).shift(match.start()))
+    return out
 
 
 @decoder
 def find_urls(data: bytes) -> list[Node]:
     """Find URLs in data"""
-    return [
-        Node(
-            URL_TYPE,
-            *normalize_percent_encoding(match.group()),
-            *match.span(),
-            children=parse_url(match.group()),
+    # Todo: blunt hack to approximate context
+    # need to do actual context aware search
+    contexts = {
+        ord("'"): ord("'"),
+        ord("("): ord(")"),
+    }
+    out = []
+    for match in re.finditer(URL_RE, data):
+        group = match.group()
+        prev = data[match.start() - 1]
+        if match.start() != 0 and prev in contexts:
+            group = group[: group.find(contexts[prev])]
+        if not is_url(group):
+            continue
+        out.append(
+            Node(
+                URL_TYPE,
+                *normalize_percent_encoding(group),
+                *match.span(),
+                children=parse_url(group),
+            )
         )
-        for match in re.finditer(URL_RE, data)
-        if is_url(match.group())
-    ]
+    return out
 
 
 def parse_ip(ip: bytes) -> Node:
     """Parses an IPv4 address.
 
     Args:
         ip: The IPv4 address as a utf-8 encoded string of a represetation accepted by socket.inet_aton.
```

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/path.py` & `multidecoder-1.2.2/src/multidecoder/decoders/path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/pe_file.py` & `multidecoder-1.2.2/src/multidecoder/decoders/pe_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 from __future__ import annotations
 
+import struct
+
 import pefile
 import regex as re
 
 from multidecoder.node import Node
 from multidecoder.registry import decoder
 
-EXEDOS_RE = rb"(?s)This program cannot be run in DOS mode"
-EXEHEADER_RE = rb"(?s)MZ.{32,1024}PE\000\000"
+E_ELFANEW_OFFSET = 0x3C
 
 
 @decoder
 def find_pe_files(data: bytes) -> list[Node]:
-    """
-    Searches for any PE files within data
-
-    Args:
-        data: The data to search
-    Returns:
-        A list of found PE files
-    """
+    """Searches for any PE files within data."""
     pe_files: list[Node] = []
-    offset = 0
-    while offset < len(data):
-        match = re.search(EXEHEADER_RE, data)
-        if not match:
-            return pe_files
-        pe_data = data[offset:]
-        if not re.search(EXEDOS_RE, pe_data):
-            return pe_files
+    # Regex is faster here than anything with str.find
+    # because for str.find the loop has to be implemented in python
+    for match in re.finditer(b"MZ", data):
+        mz_offset = match.start()
+        (e_elfanew,) = struct.unpack_from("<I", data, mz_offset + E_ELFANEW_OFFSET)
+        pe_offset = mz_offset + e_elfanew
+        if data[pe_offset : pe_offset + 4] != b"PE\0\0":
+            continue
         try:
-            pe = pefile.PE(data=pe_data)
+            pe = pefile.PE(data=data[mz_offset:])
             size = max(section.PointerToRawData + section.SizeOfRawData for section in pe.sections)
             if size == 0:
-                return pe_files
-            end = offset + size
-            pe_files.append(Node("pe_file", data[offset:end], "", offset, end))
-            offset = end
-        except Exception:
+                continue
+            end = mz_offset + size
+            pe_files.append(Node("pe_file", data[mz_offset:end], "", mz_offset, end))
+        except pefile.PEFormatError:
             return pe_files
     return pe_files
```

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/replace.py` & `multidecoder-1.2.2/src/multidecoder/decoders/replace.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/shell.py` & `multidecoder-1.2.2/src/multidecoder/decoders/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import binascii
 
 import regex as re
 
 from multidecoder.decoders.base64 import pad_base64
-from multidecoder.decoders.concat import DOUBLE_QUOTE_ESCAPES
 from multidecoder.node import Node
 from multidecoder.registry import decoder
 
-CMD_RE = b"(?i)\\bc\\^?m\\^?d(?:" + DOUBLE_QUOTE_ESCAPES + rb'|[^)\x00])*'
+CMD_RE = rb"(?i)\bc\^?m\^?d\^?\b[^)\x00]*"
 POWERSHELL_INDICATOR_RE = (
     rb'(?i)(?:^|/c|/k|/r|[\s;,=&\'"])?\b(\^?p\^?(?:o\^?w\^?e\^?r\^?s\^?h\^?e\^?l\^?l|w\^?s\^?h))\b'
 )
 SH_RE = rb'"(\s*(?:sh|bash|zsh|csh)[^"]+)"'
 ENC_RE = (
     rb"(?i)\s\^?(?:-|/)\^?e\^?(?:c|n\^?(?:c\^?(?:o\^?(?:d\^?(?:e\^?(?:d\^?(?:c\^?(?:o\^?(?:m"
     rb"\^?(?:m\^?(?:a\^?(?:n\^?d?)?)?)?)?)?)?)?)?)?)?)?)?[\s^]+[\"\']?[a-z0-9+/^]{4,}=?\^?=?\^?[\'\"]?"
```

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/vba.py` & `multidecoder-1.2.2/src/multidecoder/decoders/vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/decoders/xml.py` & `multidecoder-1.2.2/src/multidecoder/decoders/xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/domains.py` & `multidecoder-1.2.2/src/multidecoder/domains.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/hit.py` & `multidecoder-1.2.2/src/multidecoder/hit.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/json_conversion.py` & `multidecoder-1.2.2/src/multidecoder/json_conversion.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keyword.py` & `multidecoder-1.2.2/src/multidecoder/keyword.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.advapi32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.advapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.atl` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.atl`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.dbghelp` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.dbghelp`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.gdi32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.gdi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.imagehlp` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.imagehlp`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.iphlpapi` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.iphlpapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.kernel32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.kernel32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.libeay32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.libeay32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.mfc42` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.mfc42`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.msi` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.msi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.mssign32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.mssign32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.msvbvm60` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.msvbvm60`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.msvcrt` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.msvcrt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.nddeapi` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.nddeapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.netapi32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.netapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.ntdll` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.ntdll`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.ntoskrnl` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.ntoskrnl`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.odbc32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.odbc32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.odbccp32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.odbccp32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.ole32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.ole32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.oleaut32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.oleaut32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.packet` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.packet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.powrprof` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.powrprof`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.rpcrt4` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.rpcrt4`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.scecli` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.scecli`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.se` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.se`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.shell32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.shell32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.shlwapi` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.shlwapi`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.ssleay32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.ssleay32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.urlmon` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.urlmon`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.user32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.user32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.wininet` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.wininet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.winsock` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.winsock`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.winsta` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.winsta`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/api/api.wsnmp32` & `multidecoder-1.2.2/src/multidecoder/keywords/api/api.wsnmp32`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/event` & `multidecoder-1.2.2/src/multidecoder/keywords/event`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/guid` & `multidecoder-1.2.2/src/multidecoder/keywords/guid`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/key` & `multidecoder-1.2.2/src/multidecoder/keywords/key`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/network.string` & `multidecoder-1.2.2/src/multidecoder/keywords/network.string`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/oid` & `multidecoder-1.2.2/src/multidecoder/keywords/oid`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/os_name` & `multidecoder-1.2.2/src/multidecoder/keywords/os_name`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/powershell.cmdlet` & `multidecoder-1.2.2/src/multidecoder/keywords/powershell.cmdlet`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/privilege` & `multidecoder-1.2.2/src/multidecoder/keywords/privilege`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/ransomware.string` & `multidecoder-1.2.2/src/multidecoder/keywords/ransomware.string`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/security_identifier` & `multidecoder-1.2.2/src/multidecoder/keywords/security_identifier`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords/windows.registry` & `multidecoder-1.2.2/src/multidecoder/keywords/windows.registry`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/keywords_to_review.txt` & `multidecoder-1.2.2/src/multidecoder/keywords_to_review.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/multidecoder.py` & `multidecoder-1.2.2/src/multidecoder/multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/node.py` & `multidecoder-1.2.2/src/multidecoder/node.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/query.py` & `multidecoder-1.2.2/src/multidecoder/query.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/registry.py` & `multidecoder-1.2.2/src/multidecoder/registry.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder/xor_helper.py` & `multidecoder-1.2.2/src/multidecoder/xor_helper.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/src/multidecoder.egg-info/PKG-INFO` & `multidecoder-1.2.2/src/multidecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 1.2.1
+Version: 1.2.2
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: multidecoder Version: 1.2.1 Summary: A context
+Metadata-Version: 2.1 Name: multidecoder Version: 1.2.2 Summary: A context
 preserving IOC extraction library Home-page: https://github.com/
 CybercentreCanada/Multidecoder Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca License: MIT Project-URL: Bug Tracker,
 https://github.com/CybercentreCanada/Multidecoder/issues Keywords:
 malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
```

### Comparing `multidecoder-1.2.1/src/multidecoder.egg-info/SOURCES.txt` & `multidecoder-1.2.2/src/multidecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_base64.py` & `multidecoder-1.2.2/tests/test_decoders/test_base64.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_chr.py` & `multidecoder-1.2.2/tests/test_decoders/test_chr.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_concat.py` & `multidecoder-1.2.2/tests/test_decoders/test_concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_encoding.py` & `multidecoder-1.2.2/tests/test_decoders/test_encoding.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_hex.py` & `multidecoder-1.2.2/tests/test_decoders/test_hex.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_network.py` & `multidecoder-1.2.2/tests/test_decoders/test_network.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import pytest
 from multidecoder.decoders.network import (
     DOMAIN_RE,
     EMAIL_RE,
     IP_RE,
     URL_RE,
+    find_urls,
     # find_domains,
+    find_ips,
     is_domain,
     is_url,
     parse_ip,
 )
 from multidecoder.node import Node
 
 # IP --------------------------------------------
@@ -73,14 +75,22 @@
     assert re.search(IP_RE, data).group() == ip
 
 
 def test_parse_ip():
     assert parse_ip(b"8.8.8.8") == Node("network.ip", b"8.8.8.8", "", 0, 7)
 
 
+@pytest.mark.parametrize(
+    "data",
+    [b"<si><t>1.1.1.4</t></si>", b"ProductVersion\x004.0.0.0\x00", b"FileVersion\x004.0.0.0\x00", b"Version=4.0.0.0"],
+)
+def test_find_ips_false_positives(data):
+    assert find_ips(data) == []
+
+
 # Domain ----------------------------------------
 
 
 @pytest.mark.parametrize(
     "domain",
     [
         b"www.google.com",  # normal domain
@@ -217,15 +227,16 @@
         b"http://%31%32%37%2E%30%2E%30%2E%31",
         b"http://[%3A%3A%31]",
         # Full percent encoded IPv6 to test length constraints.
         b"http://[%30%30%30%30%3a%30%30%30%30%3a%30%30%30%30%3a%30%30%30%30%3a"
         b"%30%30%30%30%3a%30%30%30%30%3a%30%30%30%30%3a%30%30%30%31]",
         # Browser dependent, none of these work in Firefox.
         b"http://%5B%3A%3A1%5D",  # this works in Edge, but not Chrome.
-        b"http://%5B%3A%3A1]",  # This works in Chrome and Edge, the colons have to be percent encoded.
+        b"http://%5B%3A%3A1]",  # This works in Chrome and Edge.
+        b"http://%5B::1]",  # The colons used to have to be percent encoded in edge and chrome, but not anymore.
         b"http://[::1%5D",  # You wouldn't think this would work, but it still does on Chrome and Edge.
         b"http://[::1%5D/path",  # Even handles the rest of the url just fine.
     ],
 )
 def test_URL_RE_matches(url):
     """Test that URL_RE matches expected URLs"""
     assert re.match(URL_RE, url).span() == (0, len(url))
@@ -239,16 +250,77 @@
         (b"full sentence with a url https://example.com/.", b"https://example.com/"),
         (
             b"part of a phrase with a url https://example.com/, still works",
             b"https://example.com/",
         ),
         (b"barefunction(https://example.com) works", b"https://example.com"),
         (b'in a string content "https://example.com"works.', b"https://example.com"),
+        (b"'https://example.com/'; ", b"https://example.com/"),
     ],
 )
 def test_URL_RE_context(data, url):
     """Test that URL_RE correctly matches URLs in context"""
     assert re.search(URL_RE, data).group() == url
 
 
 def test_is_url():
     assert is_url(b"https://some.domain.com")
+
+
+@pytest.mark.parametrize(
+    ("data", "urls"),
+    [
+        (
+            b" https://example.com/path'),.;still_url ",
+            [
+                Node(
+                    "network.url",
+                    b"https://example.com/path'),.;still_url",
+                    "",
+                    1,
+                    39,
+                    children=[
+                        Node("network.url.scheme", b"https", "", 0, 5),
+                        Node("network.domain", b"example.com", "", 8, 19),
+                        Node("network.url.path", b"/path'),.;still_url", "", 19, 38),
+                    ],
+                )
+            ],
+        ),
+        (
+            b"'https://example.com/path'after_the_url",
+            [
+                Node(
+                    "network.url",
+                    b"https://example.com/path",
+                    "",
+                    1,
+                    39,
+                    children=[
+                        Node("network.url.scheme", b"https", "", 0, 5),
+                        Node("network.domain", b"example.com", "", 8, 19),
+                        Node("network.url.path", b"/path", "", 19, 24),
+                    ],
+                )
+            ],
+        ),
+        (
+            b"https://example.com/path'still_the_url'",
+            [
+                Node(
+                    "network.url",
+                    b"https://example.com/path'still_the_url",
+                    "",
+                    0,
+                    38,
+                    children=[
+                        Node("network.url.scheme", b"https", "", 0, 5),
+                        Node("network.domain", b"example.com", "", 8, 19),
+                        Node("network.url.path", b"/path'still_the_url", "", 19, 38),
+                    ],
+                )
+            ],
+        ),
+    ],
+)
+def test_find_url(data, urls):
+    assert find_urls(data) == urls
```

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_path.py` & `multidecoder-1.2.2/tests/test_decoders/test_path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_replace.py` & `multidecoder-1.2.2/tests/test_decoders/test_replace.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_shell.py` & `multidecoder-1.2.2/tests/test_decoders/test_shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pytest
 import regex as re
 from multidecoder.decoders.shell import (
     CMD_RE,
     find_cmd_strings,
     find_powershell_strings,
     get_cmd_command,
     get_powershell_command,
@@ -9,32 +10,36 @@
 )
 from multidecoder.node import Node
 
 test = b"SET.NAME(a , cmd /c m^sh^t^a h^tt^p^:/^/some.url/x.html)"
 
 
 # CMD_RE
-def test_cmd_re_empty():
-    assert not re.search(CMD_RE, b"")
-
-
-def test_cmd_re_command():
-    assert re.match(CMD_RE, b"cmd arguments")
-
-
-def test_cmd_re_mixed_case():
-    assert re.match(CMD_RE, b"CmD ArgUmenTs")
-
-
-def test_cmd_re_carets():
-    assert re.match(CMD_RE, b"c^m^d c^omman^d")
+@pytest.mark.parametrize(
+    "data",
+    [
+        b"",
+        b"CmDF",
+    ],
+)
+def test_cmd_re_not_match(data: bytes):
+    assert not re.search(CMD_RE, data)
 
 
-def test_cmd_re_quotes():
-    assert re.match(CMD_RE, b'cmd /c ""echo bee""')
+@pytest.mark.parametrize(
+    "data",
+    [
+        b"cmd arguments",
+        b"CmD ArgUmenTs",
+        b"c^m^d c^omman^d",
+        b'cmd /c ""echo bee""',
+    ],
+)
+def test_cmd_re_match(data: bytes):
+    assert re.match(CMD_RE, data)
 
 
 def test_cmd_re_null():
     match = re.match(CMD_RE, b"cmd.exe\x00somethingelse")
     assert match
     assert match.span() == (0, 7)
 
@@ -42,44 +47,29 @@
 def test_cmd_re_ex1():
     match = re.search(CMD_RE, test)
     assert match
     assert test[match.start() : match.end()] == b"cmd /c m^sh^t^a h^tt^p^:/^/some.url/x.html"
 
 
 # strip_carets
-def test_strip_carets_empty():
-    assert strip_carets(b"") == b""
-
-
-def test_strip_carets_no_caret():
-    assert strip_carets(b"test") == b"test"
-
-
-def test_strip_carets_caret():
-    assert strip_carets(b"^") == b""
-
-
-def test_strip_carets_escape_caret():
-    assert strip_carets(b"^^") == b"^"
-
-
-def test_strip_carets_trailing_caret():
-    assert strip_carets(b"test^") == b"test"
-
-
-def test_strip_carets_in_strnig():
-    assert strip_carets(b'"^"') == b'"^"'
-
-
-def test_strip_carets_line_continuation():
-    assert strip_carets(b"start^\r\nend") == b"startend"
-
-
-def test_strip_carets_unclosed_string():
-    assert strip_carets(b'"test"" ^') == b'"test"" ^'
+@pytest.mark.parametrize(
+    ("data", "expected"),
+    [
+        (b"", b""),
+        (b"test", b"test"),
+        (b"^", b""),
+        (b"^^", b"^"),
+        (b"test^", b"test"),
+        (b'"^"', b'"^"'),
+        (b"start^\r\nend", b"startend"),
+        (b'"test"" ^', b'"test"" ^'),
+    ],
+)
+def test_strip_carets(data: bytes, expected: bytes):
+    assert strip_carets(data) == expected
 
 
 # find_cmd_strings
 def test_find_cmd_strings():
     assert find_cmd_strings(test) == [
         Node(
             type_="shell.cmd",
```

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_vba.py` & `multidecoder-1.2.2/tests/test_decoders/test_vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_decoders/test_xml.py` & `multidecoder-1.2.2/tests/test_decoders/test_xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_multidecoder.py` & `multidecoder-1.2.2/tests/test_multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_node.py` & `multidecoder-1.2.2/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `multidecoder-1.2.1/tests/test_xor_helper.py` & `multidecoder-1.2.2/tests/test_xor_helper.py`

 * *Files identical despite different names*

