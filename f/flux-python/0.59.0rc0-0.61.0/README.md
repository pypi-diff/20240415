# Comparing `tmp/flux-python-0.59.0rc0.tar.gz` & `tmp/flux-python-0.61.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-python-0.59.0rc0.tar", last modified: Wed Mar  6 22:04:34 2024, max compression
+gzip compressed data, was "dist/flux-python-0.61.0.tar", last modified: Mon Apr 15 21:18:37 2024, max compression
```

## Comparing `flux-python-0.59.0rc0.tar` & `flux-python-0.61.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.409738 flux-python-0.59.0rc0/
--rw-r--r--   0 root         (0) root         (0)     7652 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      186 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1167 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/NOTICE.LLNS
--rw-r--r--   0 root         (0) root         (0)     6494 2024-03-06 22:04:34.409738 flux-python-0.59.0rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5310 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.385738 flux-python-0.59.0rc0/flux/
--rw-r--r--   0 root         (0) root         (0)       52 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3565 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/Makefile.am
--rw-r--r--   0 root         (0) root         (0)      668 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.389738 flux-python-0.59.0rc0/flux/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6324 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/alloc.py
--rw-r--r--   0 root         (0) root         (0)    57550 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/base.py
--rw-r--r--   0 root         (0) root         (0)     5340 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/batch.py
--rw-r--r--   0 root         (0) root         (0)     7228 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/bulksubmit.py
--rw-r--r--   0 root         (0) root         (0)    32425 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/fortune.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/run.py
--rw-r--r--   0 root         (0) root         (0)      829 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/cli/submit.py
--rw-r--r--   0 root         (0) root         (0)     2742 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/compat36.py
--rw-r--r--   0 root         (0) root         (0)      754 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.389738 flux-python-0.59.0rc0/flux/constraint/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/constraint/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13588 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/constraint/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.389738 flux-python-0.59.0rc0/flux/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12480 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/core/handle.py
--rw-r--r--   0 root         (0) root         (0)      814 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/core/inner.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/core/trampoline.py
--rw-r--r--   0 root         (0) root         (0)     5167 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/core/watchers.py
--rw-r--r--   0 root         (0) root         (0)      567 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/debugged.py
--rw-r--r--   0 root         (0) root         (0)    15467 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/future.py
--rw-r--r--   0 root         (0) root         (0)     7913 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/hostlist.py
--rw-r--r--   0 root         (0) root         (0)    10040 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/idset.py
--rw-r--r--   0 root         (0) root         (0)     2029 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/importer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.393738 flux-python-0.59.0rc0/flux/job/
--rw-r--r--   0 root         (0) root         (0)     3446 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/JobID.py
--rw-r--r--   0 root         (0) root         (0)    39126 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/Jobspec.py
--rw-r--r--   0 root         (0) root         (0)     1543 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/_wrapper.py
--rw-r--r--   0 root         (0) root         (0)    10156 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/directives.py
--rw-r--r--   0 root         (0) root         (0)     6805 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/event.py
--rw-r--r--   0 root         (0) root         (0)    26007 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.393738 flux-python-0.59.0rc0/flux/job/frobnicator/
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/frobnicator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4929 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/frobnicator/frobnicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.393738 flux-python-0.59.0rc0/flux/job/frobnicator/plugins/
--rw-r--r--   0 root         (0) root         (0)     2632 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/frobnicator/plugins/constraints.py
--rw-r--r--   0 root         (0) root         (0)     3088 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/frobnicator/plugins/defaults.py
--rw-r--r--   0 root         (0) root         (0)    27740 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/info.py
--rw-r--r--   0 root         (0) root         (0)     2449 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/kill.py
--rw-r--r--   0 root         (0) root         (0)     1136 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/kvs.py
--rw-r--r--   0 root         (0) root         (0)     7776 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/kvslookup.py
--rw-r--r--   0 root         (0) root         (0)    10701 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/list.py
--rw-r--r--   0 root         (0) root         (0)    34556 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/output.py
--rw-r--r--   0 root         (0) root         (0)     3841 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/stats.py
--rw-r--r--   0 root         (0) root         (0)     4598 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/submit.py
--rw-r--r--   0 root         (0) root         (0)     1249 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/timeleft.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.393738 flux-python-0.59.0rc0/flux/job/validator/
--rw-r--r--   0 root         (0) root         (0)      452 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/validator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.397738 flux-python-0.59.0rc0/flux/job/validator/plugins/
--rw-r--r--   0 root         (0) root         (0)     1710 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/validator/plugins/feasibility.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/validator/plugins/jobspec.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/validator/plugins/require-instance.py
--rw-r--r--   0 root         (0) root         (0)     7593 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/validator/validator.py
--rw-r--r--   0 root         (0) root         (0)     7096 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/wait.py
--rw-r--r--   0 root         (0) root         (0)    20638 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/job/watcher.py
--rw-r--r--   0 root         (0) root         (0)    31451 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/kvs.py
--rw-r--r--   0 root         (0) root         (0)     2629 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/memoized_property.py
--rw-r--r--   0 root         (0) root         (0)     6705 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/message.py
--rw-r--r--   0 root         (0) root         (0)    11825 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.397738 flux-python-0.59.0rc0/flux/resource/
--rw-r--r--   0 root         (0) root         (0)     8710 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/resource/ResourceSet.py
--rw-r--r--   0 root         (0) root         (0)     2767 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/resource/ResourceSetImplementation.py
--rw-r--r--   0 root         (0) root         (0)     4403 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/resource/Rlist.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/resource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/resource/list.py
--rw-r--r--   0 root         (0) root         (0)     6676 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/resource/status.py
--rw-r--r--   0 root         (0) root         (0)     2578 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/rpc.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.397738 flux-python-0.59.0rc0/flux/uri/
--rw-r--r--   0 root         (0) root         (0)      470 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/uri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.397738 flux-python-0.59.0rc0/flux/uri/resolvers/
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/uri/resolvers/jobid.py
--rw-r--r--   0 root         (0) root         (0)     3601 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/uri/resolvers/lsf.py
--rw-r--r--   0 root         (0) root         (0)     3917 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/uri/resolvers/pid.py
--rw-r--r--   0 root         (0) root         (0)     3357 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/uri/resolvers/slurm.py
--rw-r--r--   0 root         (0) root         (0)     6461 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/uri/uri.py
--rw-r--r--   0 root         (0) root         (0)    45815 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.397738 flux-python-0.59.0rc0/flux/utils/
--rw-r--r--   0 root         (0) root         (0)      201 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.397738 flux-python-0.59.0rc0/flux/utils/parsedatetime/
--rw-r--r--   0 root         (0) root         (0)   105234 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/context.py
--rw-r--r--   0 root         (0) root         (0)       61 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/parsedatetime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.401739 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/
--rw-r--r--   0 root         (0) root         (0)      719 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4611 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/base.py
--rw-r--r--   0 root         (0) root         (0)     3130 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py
--rw-r--r--   0 root         (0) root         (0)      380 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/en_AU.py
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/en_US.py
--rw-r--r--   0 root         (0) root         (0)      959 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/es.py
--rw-r--r--   0 root         (0) root         (0)     6090 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
--rw-r--r--   0 root         (0) root         (0)     4566 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py
--rw-r--r--   0 root         (0) root         (0)     2998 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
--rw-r--r--   0 root         (0) root         (0)     4577 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
--rw-r--r--   0 root         (0) root         (0)      485 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/parsedatetime/warns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.401739 flux-python-0.59.0rc0/flux/utils/tomli/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/tomli/LICENSE
--rw-r--r--   0 root         (0) root         (0)      294 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/tomli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21649 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/tomli/_parser.py
--rw-r--r--   0 root         (0) root         (0)     2813 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/tomli/_re.py
--rw-r--r--   0 root         (0) root         (0)      126 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/tomli/_types.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/utils/tomli/py.typed
--rw-r--r--   0 root         (0) root         (0)    12713 2024-03-06 22:01:29.000000 flux-python-0.59.0rc0/flux/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.409738 flux-python-0.59.0rc0/flux_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6494 2024-03-06 22:04:34.000000 flux-python-0.59.0rc0/flux_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3030 2024-03-06 22:04:34.000000 flux-python-0.59.0rc0/flux_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 22:04:34.000000 flux-python-0.59.0rc0/flux_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 22:01:36.000000 flux-python-0.59.0rc0/flux_python.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-06 22:04:34.000000 flux-python-0.59.0rc0/flux_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-06 22:04:34.000000 flux-python-0.59.0rc0/flux_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-06 22:04:34.409738 flux-python-0.59.0rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    12504 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 22:04:34.409738 flux-python-0.59.0rc0/src/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1637 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/_core_build.py
--rw-r--r--   0 root         (0) root         (0)   130073 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_core_clean.h
--rw-r--r--   0 root         (0) root         (0)    55013 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_core_preproc.h
--rw-r--r--   0 root         (0) root         (0)      876 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/_hostlist_build.py
--rw-r--r--   0 root         (0) root         (0)     4265 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_hostlist_clean.h
--rw-r--r--   0 root         (0) root         (0)     1564 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_hostlist_preproc.h
--rw-r--r--   0 root         (0) root         (0)      961 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/_idset_build.py
--rw-r--r--   0 root         (0) root         (0)     7921 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_idset_clean.h
--rw-r--r--   0 root         (0) root         (0)     3289 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_idset_preproc.h
--rw-r--r--   0 root         (0) root         (0)     1755 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/_rlist_build.py
--rw-r--r--   0 root         (0) root         (0)     1218 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/_security_build.py
--rw-r--r--   0 root         (0) root         (0)     5187 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_security_clean.h
--rw-r--r--   0 root         (0) root         (0)     2078 2024-03-06 22:04:27.000000 flux-python-0.59.0rc0/src/_security_preproc.h
--rw-r--r--   0 root         (0) root         (0)      599 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/callbacks.h
--rwxr-xr-x   0 root         (0) root         (0)     2804 2024-03-06 21:57:45.000000 flux-python-0.59.0rc0/src/make_clean_header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/
+-rw-r--r--   0 root         (0) root         (0)     7652 2024-04-15 21:13:08.000000 flux-python-0.61.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      186 2024-04-15 21:13:08.000000 flux-python-0.61.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-15 21:13:08.000000 flux-python-0.61.0/NOTICE.LLNS
+-rw-r--r--   0 root         (0) root         (0)     6491 2024-04-15 21:18:37.000000 flux-python-0.61.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5310 2024-04-15 21:13:08.000000 flux-python-0.61.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3565 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/Makefile.am
+-rw-r--r--   0 root         (0) root         (0)      668 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6324 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/alloc.py
+-rw-r--r--   0 root         (0) root         (0)    57815 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/base.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/batch.py
+-rw-r--r--   0 root         (0) root         (0)     7228 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/bulksubmit.py
+-rw-r--r--   0 root         (0) root         (0)    32425 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/fortune.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)      829 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/cli/submit.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/compat36.py
+-rw-r--r--   0 root         (0) root         (0)      754 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/constraint/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/constraint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13588 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/constraint/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12495 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/core/handle.py
+-rw-r--r--   0 root         (0) root         (0)      814 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/core/inner.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/core/trampoline.py
+-rw-r--r--   0 root         (0) root         (0)     5167 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/core/watchers.py
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/debugged.py
+-rw-r--r--   0 root         (0) root         (0)    15467 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/future.py
+-rw-r--r--   0 root         (0) root         (0)     7913 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/hostlist.py
+-rw-r--r--   0 root         (0) root         (0)    10040 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/idset.py
+-rw-r--r--   0 root         (0) root         (0)     2029 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/importer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/job/
+-rw-r--r--   0 root         (0) root         (0)     3446 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/JobID.py
+-rw-r--r--   0 root         (0) root         (0)    39126 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/Jobspec.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/directives.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/event.py
+-rw-r--r--   0 root         (0) root         (0)    26007 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/job/frobnicator/
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/frobnicator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4929 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/frobnicator/frobnicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/job/frobnicator/plugins/
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/frobnicator/plugins/constraints.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/frobnicator/plugins/defaults.py
+-rw-r--r--   0 root         (0) root         (0)    27719 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/info.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/kill.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/kvs.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/kvslookup.py
+-rw-r--r--   0 root         (0) root         (0)    10701 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/list.py
+-rw-r--r--   0 root         (0) root         (0)    34556 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/output.py
+-rw-r--r--   0 root         (0) root         (0)     3841 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/stats.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/submit.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/timeleft.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/job/validator/
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/validator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/job/validator/plugins/
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/validator/plugins/feasibility.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/validator/plugins/jobspec.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/validator/plugins/require-instance.py
+-rw-r--r--   0 root         (0) root         (0)     7593 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/validator/validator.py
+-rw-r--r--   0 root         (0) root         (0)     7096 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/wait.py
+-rw-r--r--   0 root         (0) root         (0)    20638 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/job/watcher.py
+-rw-r--r--   0 root         (0) root         (0)    31451 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/kvs.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/memoized_property.py
+-rw-r--r--   0 root         (0) root         (0)     6705 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/message.py
+-rw-r--r--   0 root         (0) root         (0)    11825 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/resource/
+-rw-r--r--   0 root         (0) root         (0)     8710 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/resource/ResourceSet.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/resource/ResourceSetImplementation.py
+-rw-r--r--   0 root         (0) root         (0)     4403 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/resource/Rlist.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/resource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/resource/list.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/resource/status.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/rpc.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/uri/
+-rw-r--r--   0 root         (0) root         (0)      470 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/uri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/uri/resolvers/
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/uri/resolvers/jobid.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/uri/resolvers/lsf.py
+-rw-r--r--   0 root         (0) root         (0)     3917 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/uri/resolvers/pid.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/uri/resolvers/slurm.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/uri/uri.py
+-rw-r--r--   0 root         (0) root         (0)    46047 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/utils/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/utils/parsedatetime/
+-rw-r--r--   0 root         (0) root         (0)   105234 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/context.py
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/parsedatetime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/
+-rw-r--r--   0 root         (0) root         (0)      719 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4611 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/base.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/de_DE.py
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/en_AU.py
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/en_US.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/es.py
+-rw-r--r--   0 root         (0) root         (0)     6090 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
+-rw-r--r--   0 root         (0) root         (0)     4566 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/icu.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
+-rw-r--r--   0 root         (0) root         (0)     4577 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/parsedatetime/warns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux/utils/tomli/
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/tomli/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      294 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/tomli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21649 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/tomli/_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2813 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/tomli/_re.py
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/tomli/_types.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/utils/tomli/py.typed
+-rw-r--r--   0 root         (0) root         (0)    12777 2024-04-15 21:17:02.000000 flux-python-0.61.0/flux/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6491 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3030 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 21:17:09.000000 flux-python-0.61.0/flux_python.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-15 21:18:37.000000 flux-python-0.61.0/flux_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 21:18:37.000000 flux-python-0.61.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    12501 2024-04-15 21:13:08.000000 flux-python-0.61.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 21:18:37.000000 flux-python-0.61.0/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/_core_build.py
+-rw-r--r--   0 root         (0) root         (0)   128959 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_core_clean.h
+-rw-r--r--   0 root         (0) root         (0)    54959 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_core_preproc.h
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/_hostlist_build.py
+-rw-r--r--   0 root         (0) root         (0)     4265 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_hostlist_clean.h
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_hostlist_preproc.h
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/_idset_build.py
+-rw-r--r--   0 root         (0) root         (0)     7921 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_idset_clean.h
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_idset_preproc.h
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/_rlist_build.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/_security_build.py
+-rw-r--r--   0 root         (0) root         (0)     5187 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_security_clean.h
+-rw-r--r--   0 root         (0) root         (0)     2078 2024-04-15 21:18:28.000000 flux-python-0.61.0/src/_security_preproc.h
+-rw-r--r--   0 root         (0) root         (0)      599 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/callbacks.h
+-rwxr-xr-x   0 root         (0) root         (0)     2804 2024-04-15 21:13:08.000000 flux-python-0.61.0/src/make_clean_header.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `flux-python-0.59.0rc0/LICENSE` & `flux-python-0.61.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/NOTICE.LLNS` & `flux-python-0.61.0/NOTICE.LLNS`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/PKG-INFO` & `flux-python-0.61.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.59.0rc0
+Version: 0.61.0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 Keywords: flux,job manager,workload manager,orchestration,hpc
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: C++
```

### Comparing `flux-python-0.59.0rc0/README.md` & `flux-python-0.61.0/README.md`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/Makefile.am` & `flux-python-0.61.0/flux/Makefile.am`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/__init__.py` & `flux-python-0.61.0/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/cli/alloc.py` & `flux-python-0.61.0/flux/cli/alloc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/cli/base.py` & `flux-python-0.61.0/flux/cli/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,20 +625,22 @@
         #  Format each argument in args.command, splitting on the
         #   special "::list::" sentinel to handle the case where
         #   custom input methods return a list (See Xinput.__getattr__)
         #
         self.command = []
         for arg in args.command:
             try:
-                result = arg.format(*inputs, **kwargs).split("::list::")
+                val = self.preserve_mustache(arg)
+                result = val.format(*inputs, **kwargs).split("::list::")
+                newval = self.restore_mustache(result)
             except (IndexError, KeyError):
                 LOGGER.error("Invalid replacement string in command: '%s'", arg)
                 sys.exit(1)
-            if result:
-                self.command.extend(result)
+            if newval:
+                self.command.extend(newval)
 
         #  Format all supported mutable options defined in `mutable_args`
         #  Note: only list and string options are supported.
         #
         self.modified = {}
         for attr in self.mutable_args:
             val = getattr(args, attr)
@@ -865,48 +867,56 @@
             + "multiple times to build a reduced set of propagated limits, "
             + "e.g. --rlimit=-*,core will only propagate RLIMIT_CORE.",
             metavar="RULE",
         )
         parser.add_argument(
             "--input",
             type=str,
-            help="Redirect job stdin from FILENAME, bypassing KVS"
-            if not exclude_io
-            else argparse.SUPPRESS,
+            help=(
+                "Redirect job stdin from FILENAME, bypassing KVS"
+                if not exclude_io
+                else argparse.SUPPRESS
+            ),
             metavar="FILENAME",
         )
         parser.add_argument(
             "--output",
             type=str,
-            help="Redirect job stdout to FILENAME, bypassing KVS"
-            if not exclude_io
-            else argparse.SUPPRESS,
+            help=(
+                "Redirect job stdout to FILENAME, bypassing KVS"
+                if not exclude_io
+                else argparse.SUPPRESS
+            ),
             metavar="FILENAME",
         )
         parser.add_argument(
             "--error",
             type=str,
-            help="Redirect job stderr to FILENAME, bypassing KVS"
-            if not exclude_io
-            else argparse.SUPPRESS,
+            help=(
+                "Redirect job stderr to FILENAME, bypassing KVS"
+                if not exclude_io
+                else argparse.SUPPRESS
+            ),
             metavar="FILENAME",
         )
         parser.add_argument(
             "-u",
             "--unbuffered",
             action="store_true",
             help="Disable buffering of input and output",
         )
         parser.add_argument(
             "-l",
             "--label-io",
             action="store_true",
-            help="Add rank labels to stdout, stderr lines"
-            if not exclude_io
-            else argparse.SUPPRESS,
+            help=(
+                "Add rank labels to stdout, stderr lines"
+                if not exclude_io
+                else argparse.SUPPRESS
+            ),
         )
         parser.add_argument(
             "--cwd", help="Set job working directory", metavar="DIRECTORY"
         )
         parser.add_argument(
             "--flags",
             action="append",
```

### Comparing `flux-python-0.59.0rc0/flux/cli/batch.py` & `flux-python-0.61.0/flux/cli/batch.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/cli/bulksubmit.py` & `flux-python-0.61.0/flux/cli/bulksubmit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/cli/fortune.py` & `flux-python-0.61.0/flux/cli/fortune.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/cli/run.py` & `flux-python-0.61.0/flux/cli/run.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/cli/submit.py` & `flux-python-0.61.0/flux/cli/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/compat36.py` & `flux-python-0.61.0/flux/compat36.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/constants.py` & `flux-python-0.61.0/flux/constants.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/constraint/parser.py` & `flux-python-0.61.0/flux/constraint/parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/core/handle.py` & `flux-python-0.61.0/flux/core/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         if events is None:
             # TODO add mypy type stubs for constants so this passes vermin without
             # comment
             events = FLUX_POLLIN | FLUX_POLLOUT | FLUX_POLLERR  # novm
         return FDWatcher(self, fd_int, events, callback, args=args)
 
     def barrier(self, name, nprocs):
-        self.flux_barrier(name, nprocs)
+        return Future(self.flux_barrier(name, nprocs))
 
     def get_rank(self):
         rank = ffi.new("uint32_t [1]")
         self.flux_get_rank(rank)
         return rank[0]
 
     def attr_get(self, attr_name):
```

### Comparing `flux-python-0.59.0rc0/flux/core/inner.py` & `flux-python-0.61.0/flux/core/inner.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/core/trampoline.py` & `flux-python-0.61.0/flux/core/trampoline.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/core/watchers.py` & `flux-python-0.61.0/flux/core/watchers.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/debugged.py` & `flux-python-0.61.0/flux/debugged.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/future.py` & `flux-python-0.61.0/flux/future.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/hostlist.py` & `flux-python-0.61.0/flux/hostlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/idset.py` & `flux-python-0.61.0/flux/idset.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/importer.py` & `flux-python-0.61.0/flux/importer.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/JobID.py` & `flux-python-0.61.0/flux/job/JobID.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/Jobspec.py` & `flux-python-0.61.0/flux/job/Jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/__init__.py` & `flux-python-0.61.0/flux/job/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/_wrapper.py` & `flux-python-0.61.0/flux/job/_wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/directives.py` & `flux-python-0.61.0/flux/job/directives.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/event.py` & `flux-python-0.61.0/flux/job/event.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/executor.py` & `flux-python-0.61.0/flux/job/executor.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/frobnicator/frobnicator.py` & `flux-python-0.61.0/flux/job/frobnicator/frobnicator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/frobnicator/plugins/constraints.py` & `flux-python-0.61.0/flux/job/frobnicator/plugins/constraints.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/frobnicator/plugins/defaults.py` & `flux-python-0.61.0/flux/job/frobnicator/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/info.py` & `flux-python-0.61.0/flux/job/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,17 +223,17 @@
 class InstanceInfo:
     def __init__(self, uri=None):
         self.initialized = False
         try:
             if not uri or SchedResourceList is None:
                 raise ValueError
             handle = flux.Flux(str(uri))
-            future = handle.rpc("sched.resource-status")
+            future = flux.resource.resource_list(handle)
             self.stats = StatsInfo(handle).update_sync()
-            self.resources = SchedResourceList(future.get())
+            self.resources = future.get()
             self.initialized = True
             return
         except (ValueError, OSError, FileNotFoundError):
             self.stats = EmptyObject()
             self.resources = EmptyObject()
 
     @memoized_property
@@ -827,15 +827,15 @@
         Throws an exception if any format fields do not match the allowed
         list of headings above.
 
         Special case for annotations, which may be arbitrary
         creations of scheduler or user.
         """
         format_list = string.Formatter().parse(fmt)
-        for (_, field, _, _) in format_list:
+        for _, field, _, _ in format_list:
             if field and not field in self.headings:
                 if field.startswith("annotations."):
                     field_heading = field[len("annotations.") :].upper()
                     self.headings[field] = field_heading
                 elif field.startswith("sched.") or field.startswith("user."):
                     field_heading = field.upper()
                     self.headings[field] = field_heading
```

### Comparing `flux-python-0.59.0rc0/flux/job/kill.py` & `flux-python-0.61.0/flux/job/kill.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/kvs.py` & `flux-python-0.61.0/flux/job/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/kvslookup.py` & `flux-python-0.61.0/flux/job/kvslookup.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/list.py` & `flux-python-0.61.0/flux/job/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/output.py` & `flux-python-0.61.0/flux/job/output.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/stats.py` & `flux-python-0.61.0/flux/job/stats.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/submit.py` & `flux-python-0.61.0/flux/job/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/timeleft.py` & `flux-python-0.61.0/flux/job/timeleft.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/validator/plugins/feasibility.py` & `flux-python-0.61.0/flux/job/validator/plugins/feasibility.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/validator/plugins/jobspec.py` & `flux-python-0.61.0/flux/job/validator/plugins/jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/validator/plugins/require-instance.py` & `flux-python-0.61.0/flux/job/validator/plugins/require-instance.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/validator/validator.py` & `flux-python-0.61.0/flux/job/validator/validator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/wait.py` & `flux-python-0.61.0/flux/job/wait.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/job/watcher.py` & `flux-python-0.61.0/flux/job/watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
     @staticmethod
     def _status_to_exitcode(status):
         """Calculate exitcode from job status"""
         if os.WIFEXITED(status):
             status = os.WEXITSTATUS(status)
         elif os.WIFSIGNALED(status):
-            status = 127 + os.WTERMSIG(status)
+            status = 128 + os.WTERMSIG(status)
         return status
 
     def start(self):
         """
         Start JobWatcher progress bar if configured
         """
         if self.show_progress:
```

### Comparing `flux-python-0.59.0rc0/flux/kvs.py` & `flux-python-0.61.0/flux/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/memoized_property.py` & `flux-python-0.61.0/flux/memoized_property.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/message.py` & `flux-python-0.61.0/flux/message.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/progress.py` & `flux-python-0.61.0/flux/progress.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/resource/ResourceSet.py` & `flux-python-0.61.0/flux/resource/ResourceSet.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/resource/ResourceSetImplementation.py` & `flux-python-0.61.0/flux/resource/ResourceSetImplementation.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/resource/Rlist.py` & `flux-python-0.61.0/flux/resource/Rlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/resource/__init__.py` & `flux-python-0.61.0/flux/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/resource/list.py` & `flux-python-0.61.0/flux/resource/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 #
 # This file is part of the Flux resource manager framework.
 # For details, see https://github.com/flux-framework.
 #
 # SPDX-License-Identifier: LGPL-3.0
 ###############################################################
 
+import errno
+import json
+import os
+
+from flux.future import FutureExt
 from flux.idset import IDset
 from flux.memoized_property import memoized_property
 from flux.resource import ResourceSet
-from flux.rpc import RPC
 
 
 class SchedResourceList:
     """
-    Encapsulate response from sched.resource-status query.
+    Encapsulate response from resource.sched-status query.
     The response will contain 3 Rv1 resource sets:
 
     :ivar all:         all resources known to scheduler
     :ivar down:        resources currently unavailable (drained or down)
     :ivar allocated:   resources currently allocated to jobs
 
     From these sets, the "up" and "free" resource sets are
@@ -74,17 +78,39 @@
     def free(self):
         """All resources which are neither down nor allocated."""
         res = self.up - self.allocated
         res.state = "free"
         return res
 
 
-class ResourceListRPC(RPC):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+class ResourceListRPC(FutureExt):
+    def __init__(self, flux_handle, topic, nodeid=0):
+        self.topic = topic
+        super().__init__(self._init_cb, flux_handle=flux_handle)
+
+    def _init_cb(self, future):
+        future.get_flux().rpc(self.topic, nodeid=0).then(self._list_cb)
+
+    def _list_cb(self, future):
+        try:
+            self.fulfill(future.get())
+        except Exception as exc:
+            if exc.errno == errno.ENOSYS:
+                #  Fall back to sched.resource-status:
+                future.get_flux().rpc("sched.resource-status", nodeid=0).then(
+                    self._fallback_cb
+                )
+            else:
+                self.fulfill_error(exc.errno, exc.strerror)
+
+    def _fallback_cb(self, future):
+        try:
+            self.fulfill(json.loads(future.get_str()))
+        except OSError as exc:
+            self.fulfill_error(exc.errno, exc.strerror)
 
     def get(self):
         """Return a SchedResourceList corresponding to the request.
 
         Blocks until the request is fulfilled."""
         return SchedResourceList(super().get())
 
@@ -94,8 +120,9 @@
 
     Args:
         flux_handle (flux.Flux): a Flux handle
 
     Returns:
         ResourceListRPC: a future representing the request.
     """
-    return ResourceListRPC(flux_handle, "sched.resource-status")
+    topic = os.getenv("FLUX_RESOURCE_LIST_RPC") or "resource.sched-status"
+    return ResourceListRPC(flux_handle, topic, nodeid=0)
```

### Comparing `flux-python-0.59.0rc0/flux/resource/status.py` & `flux-python-0.61.0/flux/resource/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,22 +104,29 @@
         # drained: free+drain
         self.drained = IDset()
         # draining: allocated+drain
         self.draining = IDset()
 
         # drain_info: ranks, timestamp, reason tuples for all drained resources
         self.drain_info = []
+        self._drain_lookup = {}
         for drain_ranks, entry in self.rstatus["drain"].items():
             ranks = IDset(drain_ranks)
             if include_ranks is not None:
                 ranks = ranks.intersect(include_ranks)
-            self.drained += ranks - self.allocated
-            self.draining += ranks - self.drained
+            self.drained += ranks
             info = DrainInfo(ranks, entry["timestamp"], entry["reason"])
             self.drain_info.append(info)
+            for rank in ranks:
+                self._drain_lookup[rank] = info
+
+        # create the set of draining ranks as the intersection of
+        #  drained and allocated
+        self.draining = self.drained & self.allocated
+        self.drained -= self.draining
 
         # available: all ranks not excluded or drained/draining
         self.avail = self.all - self.get_idset("exclude", "drained", "draining")
 
     def __getitem__(self, state):
         """
         Allow a ResourceStatus object to be subscriptable for convenience,
@@ -138,15 +145,15 @@
 
     def get_drain_info(self, rank):
         """
         Find and return the DrainInfo object for rank ``rank``
         """
         if rank not in self.all:
             raise ValueError("invalid rank {rank}")
-        return next((i for i in self.drain_info if rank in i.ranks), None)
+        return self._drain_lookup.get(rank)
 
 
 class ResourceStatusRPC:
     """
     A ResourceStatusRPC encapsulates a query to both the resource module
     and scheduler and returns a ResourceStatus object.
     """
```

### Comparing `flux-python-0.59.0rc0/flux/rpc.py` & `flux-python-0.61.0/flux/rpc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/security.py` & `flux-python-0.61.0/flux/security.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/uri/resolvers/jobid.py` & `flux-python-0.61.0/flux/uri/resolvers/jobid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/uri/resolvers/lsf.py` & `flux-python-0.61.0/flux/uri/resolvers/lsf.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/uri/resolvers/pid.py` & `flux-python-0.61.0/flux/uri/resolvers/pid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/uri/resolvers/slurm.py` & `flux-python-0.61.0/flux/uri/resolvers/slurm.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/uri/uri.py` & `flux-python-0.61.0/flux/uri/uri.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/util.py` & `flux-python-0.61.0/flux/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,14 +458,19 @@
                 value = UtilDatetime.fromtimestamp(value)
             except TypeError:
                 if orig_value == "":
                     value = UtilDatetime.fromtimestamp(0.0)
                 else:
                     raise
         elif conv == "D":
+            # the JobInfo class initializes many timestamps to 0.0 if
+            # they are not available.  Treat epoch time as special case
+            # and just return empty string.
+            if not value:
+                return ""
             # As above, but convert to ISO 8601 date time string.
             try:
                 value = datetime.fromtimestamp(value).strftime("%FT%T")
             except TypeError:
                 if orig_value == "":
                     value = ""
                 else:
@@ -611,15 +616,15 @@
 
     def header_format(self):
         """
         Return the header row formatted by the user-provided format spec,
         which will be made "safe" for use with string headings.
         """
         format_list = []
-        for (text, field, spec, _) in self.format_list:
+        for text, field, spec, _ in self.format_list:
             #  Remove number formatting on any spec:
             spec = re.sub(r"(0?\.)?(\d+)?[bcdoxXeEfFgGn%]$", r"\2", spec)
 
             #  Only keep fill, align, and min width of the result.
             #  This strips possible type-specific formatting spec that
             #   will not apply to a heading, but keeps width and alignment.
             match = re.search(r"([<>=^])?(\d+)", spec)
@@ -640,15 +645,15 @@
         """
         Return the format string, ensuring that the string in "prepend"
         is prepended to each format field
         """
         if except_fields is None:
             except_fields = []
         lst = []
-        for (text, field, spec, conv) in self.format_list:
+        for text, field, spec, conv in self.format_list:
             # Skip this field if it is in except_fields
             if field in except_fields:
                 # Preserve any format "prefix" (i.e. the text):
                 lst.append(text)
                 continue
             # If field doesn't have 'prepend' then add it
             if field and not field.startswith(prepend):
@@ -700,15 +705,15 @@
         #
         #  Note: we remove the leading `text` and the format `spec` because
         #  these may make even empty formatted fields non-empty. E.g. a spec
         #  of `:>8` will always make the format result 8 characters wide.
         #
         lst = []
         index = 0
-        for (text, field, _, conv) in self.format_list:
+        for text, field, _, conv in self.format_list:
             if text.endswith("?:"):
                 fmt = self._fmt_tuple("", "0." + field, None, conv)
                 lst.append(dict(fmt=fmt, index=index))
             index = index + 1
 
         # Return immediately if no format fields are collapsible
         if not lst:
```

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/__init__.py` & `flux-python-0.61.0/flux/utils/parsedatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/context.py` & `flux-python-0.61.0/flux/utils/parsedatetime/context.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/base.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/base.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/de_DE.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/es.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/es.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/fr_FR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/icu.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/nl_NL.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/pt_BR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py` & `flux-python-0.61.0/flux/utils/parsedatetime/pdt_locales/ru_RU.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/tomli/LICENSE` & `flux-python-0.61.0/flux/utils/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/tomli/_parser.py` & `flux-python-0.61.0/flux/utils/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/utils/tomli/_re.py` & `flux-python-0.61.0/flux/utils/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/flux/wrapper.py` & `flux-python-0.61.0/flux/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,17 +210,19 @@
 
         if self.is_error(result):
             errnum = calling_object.ffi.errno
             if errnum != 0:
                 raise EnvironmentError(
                     errnum,
                     "{}: {}".format(
-                        errno.errorcode[errnum]
-                        if errnum in errno.errorcode
-                        else "Errno" + str(errnum),
+                        (
+                            errno.errorcode[errnum]
+                            if errnum in errno.errorcode
+                            else "Errno" + str(errnum)
+                        ),
                         os.strerror(errnum),
                     ),
                 )
 
         return result
```

### Comparing `flux-python-0.59.0rc0/flux_python.egg-info/PKG-INFO` & `flux-python-0.61.0/flux_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.59.0rc0
+Version: 0.61.0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 Keywords: flux,job manager,workload manager,orchestration,hpc
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: C++
```

### Comparing `flux-python-0.59.0rc0/flux_python.egg-info/SOURCES.txt` & `flux-python-0.61.0/flux_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/setup.py` & `flux-python-0.61.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from setuptools import find_packages
 from setuptools import setup as _setup
 from distutils.core import setup, Command
 
 # Metadata
 package_name = "flux-python"
-package_version = "0.59.0rc0"
+package_version = "0.61.0"
 package_description = "Python bindings for the flux resource manager API"
 package_url = "https://github.com/flux-framework/flux-python"
 package_keywords = "flux, job manager, workload manager, orchestration, hpc"
 
 try:
     with open("README.md") as filey:
         package_long_description = filey.read()
```

### Comparing `flux-python-0.59.0rc0/src/_core_build.py` & `flux-python-0.61.0/src/_core_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_core_clean.h` & `flux-python-0.61.0/src/_core_clean.h`

 * *Files 2% similar despite different names*

```diff
@@ -1978,17 +1978,17 @@
 
 /* Flux uses semantic versioning: <major>.<minor>.<patch>
  */
 
 /* The VERSION_STRING may include a "-N-hash" suffix from git describe
  * if this snapshot is not tagged.  This is not reflected in VERSION_PATCH.
  */
-#define FLUX_CORE_VERSION_STRING    "0.59.0"
+#define FLUX_CORE_VERSION_STRING    "0.61.0"
 #define FLUX_CORE_VERSION_MAJOR     0
-#define FLUX_CORE_VERSION_MINOR     59
+#define FLUX_CORE_VERSION_MINOR     61
 #define FLUX_CORE_VERSION_PATCH     0
 
 /* The version in 3 bytes, for numeric comparison.
  */
 #define FLUX_CORE_VERSION_HEX       ((FLUX_CORE_VERSION_MAJOR << 16) | \
                                      (FLUX_CORE_VERSION_MINOR << 8) | \
                                      (FLUX_CORE_VERSION_PATCH << 0))
@@ -2885,14 +2885,26 @@
     FLUX_JOB_NOVALIDATE = 8,    // don't validate jobspec (instance owner only)
 };
 
 enum job_event_watch_flags {
     FLUX_JOB_EVENT_WATCH_WAITCREATE = 1, // wait for path to exist
 };
 
+enum job_lookup_flags {
+    /* return special fields as decoded JSON objects instead of strings
+     * - currently works for jobspec and R
+     */
+    FLUX_JOB_LOOKUP_JSON_DECODE = 1,
+    /* get current value of special fields by applying eventlog
+     * updates for those fields
+     * - currently works for jobspec and R
+     */
+    FLUX_JOB_LOOKUP_CURRENT = 2,
+};
+
 enum job_urgency {
     FLUX_JOB_URGENCY_MIN = 0,
     FLUX_JOB_URGENCY_HOLD = FLUX_JOB_URGENCY_MIN,
     FLUX_JOB_URGENCY_DEFAULT = 16,
     FLUX_JOB_URGENCY_MAX = 31,
     FLUX_JOB_URGENCY_EXPEDITE = FLUX_JOB_URGENCY_MAX,
 };
@@ -3336,15 +3348,15 @@
  */
 void flux_cmd_destroy (flux_cmd_t *cmd);
 
 /*
  *  Append formatted string to argv of `cmd`.
  */
 int flux_cmd_argv_appendf (flux_cmd_t *cmd,
-		           const char *fmt, ...)
+                           const char *fmt, ...)
                            __attribute__ ((format (printf, 2, 3)));
 
 /*
  *  Append string to argv of `cmd`.
  */
 int flux_cmd_argv_append (flux_cmd_t *cmd, const char *arg);
 
@@ -3374,18 +3386,18 @@
 char *flux_cmd_stringify (const flux_cmd_t *cmd);
 
 /*
  *  Set a single environment variable (name) to formatted string `fmt`.
  *   If `overwrite` is non-zero then overwrite any existing setting for `name`.
  */
 int flux_cmd_setenvf (flux_cmd_t *cmd,
-		      int overwrite,
+                      int overwrite,
                       const char *name,
-		      const char *fmt,
-		      ...)
+                      const char *fmt,
+                      ...)
                       __attribute__ ((format (printf, 4, 5)));
 
 /*
  *  Unset environment variable `name` in the command object `cmd`.
  *   If `name` is a glob pattern, unset all matching variables.
  */
 void flux_cmd_unsetenv (flux_cmd_t *cmd, const char *name);
@@ -3447,40 +3459,26 @@
  *    option to "false", the output callback will be called whenever any amount
  *    of data is available on the stream.  These options can also be set to
  *    "true" to keep default behavior of line buffering.
  *
  *    - name + "_LINE_BUFFER" - configuring line buffering on channel name
  *    - stdout_LINE_BUFFER - configure line buffering for stdout
  *    - stderr_LINE_BUFFER - configure line buffering for stderr
- *
- *  "STREAM_STOP" option
- *
- *    By default, the 'on_output' callback
- *    can immediately begin receiving stdout/stderr data
- *    once a subprocess has started.  There are circumstances where a
- *    caller may wish to wait and can have the stream stopped by
- *    default and restarted later by flux_subprocess_stream_start().
- *    By setting this option to "true", the output callback will be
- *    stopped by default.  These options can also be set to "false" to
- *    keep default behavior.  Note that these options only apply to
- *    local subprocesses.
- *
- *    - name + "_STREAM_STOP" - configure start/stop on channel name
- *    - stdout_STREAM_STOP - configure start/stop for stdout
- *    - stderr_STREAM_STOP - configure start/stop for stderr
  */
 int flux_cmd_setopt (flux_cmd_t *cmd, const char *var, const char *val);
 const char *flux_cmd_getopt (flux_cmd_t *cmd, const char *var);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_SUBPROCESS_COMMAND_H */
 
+// vi: ts=4 sw=4 expandtab
+
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /*
  *  flux_subprocess_t: A subprocess is an instantiation of a command
  *   as a remote or local process. A subprocess has a state (e.g.
@@ -3559,37 +3557,25 @@
     flux_subprocess_hook_f post_fork;
     void *post_fork_arg;
 } flux_subprocess_hooks_t;
 
 /*
  *  llog-compatible callback
  */
-typedef void (*subprocess_log_f) (void *arg,
-                                  const char *file,
-                                  int line,
-                                  const char *func,
-                                  const char *subsys,
-                                  int level,
-                                  const char *fmt,
-                                  va_list args);
+typedef void (*subprocess_log_f)(void *arg,
+                                 const char *file,
+                                 int line,
+                                 const char *func,
+                                 const char *subsys,
+                                 int level,
+                                 const char *fmt,
+                                 va_list args);
 
 
 /*
- * Convenience Functions:
- */
-
-/*  General output callback that will send output from the subprocess
- *  to stdout or stderr.  Set the `on_stdout` and/or `on_stderr`
- *  callbacks in flux_subprocess_ops_t and this function will output
- *  to stdout/stderr respectively.  You can also set 'on_channel_out'
- *  to this function, which will send all channel output to stdout.
- */
-void flux_standard_output (flux_subprocess_t *p, const char *stream);
-
-/*
  *  Subprocesses:
  */
 
 /*
  *  Asynchronously create a new subprocess described by command object
  *   `cmd`.  flux_local_exec() create a new subprocess locally.
  *   flux_rexec() creates a new subprocess on Flux rank
@@ -3615,54 +3601,48 @@
                                        const flux_cmd_t *cmd,
                                        const flux_subprocess_ops_t *ops,
                                        const flux_subprocess_hooks_t *hooks,
                                        subprocess_log_f log_fn,
                                        void *log_data);
 
 flux_subprocess_t *flux_rexec (flux_t *h,
-		               int rank,
-			       int flags,
+                               int rank,
+                               int flags,
                                const flux_cmd_t *cmd,
                                const flux_subprocess_ops_t *ops);
 
 flux_subprocess_t *flux_rexec_ex (flux_t *h,
                                   const char *service_name,
                                   int rank,
                                   int flags,
                                   const flux_cmd_t *cmd,
                                   const flux_subprocess_ops_t *ops,
                                   subprocess_log_f log_fn,
                                   void *log_data);
 
 
 /* Start / stop a read stream temporarily on local processes.  This
- * may be useful for flow control.  If you desire to have a stream not
- * call 'on_stdout' or 'on_stderr' when the local subprocess has
- * started, see STREAM_STOP configuration above.
- *
- * start and stop return 0 for success, -1 on error
- * status returns > 0 for started, 0 for stopped, -1 on error
- */
-int flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
-int flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
-int flux_subprocess_stream_status (flux_subprocess_t *p, const char *stream);
+ * may be useful for flow control.
+ */
+void flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
+void flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
 
 /*
  *  Write data to "stream" stream of subprocess `p`.  'stream' can be
  *  "stdin" or the name of a stream specified with flux_cmd_add_channel().
  *
  *  Returns the total amount of data successfully buffered or -1 on error
  *  with errno set. Note: this function will not return a short write. If
  *  all `len` bytes cannot fit in the destination buffer, then no bytes
  *  will be written and -1 will be returned with errno=ENOSPC.
  */
 int flux_subprocess_write (flux_subprocess_t *p,
-		           const char *stream,
+                           const char *stream,
                            const char *buf,
-			   size_t len);
+                           size_t len);
 
 /*
  *  Close "stream" stream of subprocess `p` and schedule EOF to be sent.
  *  'stream' can be "stdin" or the name of a stream specified with
  *  flux_cmd_add_channel().
  */
 int flux_subprocess_close (flux_subprocess_t *p, const char *stream);
@@ -3677,15 +3657,15 @@
  *   free returned pointer.  Length of buffer returned can optionally
  *   returned in 'lenp'.  A length of 0 indicates that the subprocess
  *   has closed this stream.
  */
 const char *flux_subprocess_read (flux_subprocess_t *p,
                                   const char *stream,
                                   int len,
-				  int *lenp);
+                                  int *lenp);
 
 /*
  *  Read line unread data from stream `stream`.  'stream' can be
  *   "stdout", "stderr", or the name of a stream specified with
  *   flux_cmd_add_channel().
  *
  *   Returns pointer to buffer on success and NULL on error with errno
@@ -3707,19 +3687,18 @@
 
 /* Determine if the read stream has is closed / received an EOF.  This
  * function can be useful if you are reading lines via
  * flux_subprocess_read_line() or flux_subprocess_read_trimmed_line()
  * in output callbacks.  Those functions will return length 0 when no
  * lines are available, making it difficult to determine if the stream
  * has been closed and there is any non-newline terminated data left
- * available for reading with flux_subprocess_read().  Returns > 0 on
- * closed / eof seen, 0 if not, -1 on error.
+ * available for reading with flux_subprocess_read().
  */
-int flux_subprocess_read_stream_closed (flux_subprocess_t *p,
-                                        const char *stream);
+bool flux_subprocess_read_stream_closed (flux_subprocess_t *p,
+                                         const char *stream);
 
 /* flux_subprocess_getline() is a special case function
  * that behaves identically to flux_subprocess_read_line() but handles
  * several common special cases.  It requires the stream of data to be
  * line buffered (by default on, see LINE_BUFFER under
  * flux_cmd_setopt()).
  *
@@ -3742,21 +3721,19 @@
  *  This call returns a flux_future_t. Use flux_future_then(3) to register
  *   a continuation callback when the kill operation is complete, or
  *   flux_future_wait_for(3) to block until the kill operation is complete.
  */
 flux_future_t *flux_subprocess_kill (flux_subprocess_t *p, int signo);
 
 /*
- *  Add/remove a reference to subprocess object `p`. The subprocess object
- *   is destroyed once the last reference is removed.  These calls
- *   silently do nothing if called within a hook.
- */
-void flux_subprocess_ref (flux_subprocess_t *p);
-void flux_subprocess_unref (flux_subprocess_t *p);
-#define flux_subprocess_destroy(x) flux_subprocess_unref(x)
+ *  Remove a reference to subprocess object `p`. The subprocess object
+ *   is destroyed once the last reference is removed.  This call
+ *   silently deso nothing if called within a hook.
+ */
+void flux_subprocess_destroy (flux_subprocess_t *p);
 
 /*  Return current state value of subprocess.  Note this may differ
  *  than state returned in on_state_change callback, as a subprocess
  *  may have already transitioned past that point (e.g. the callback
  *  received a transition change to RUNNING, but the child subprocess
  *  has already EXITED).
  */
@@ -3803,16 +3780,16 @@
 /*
  *  Set arbitrary context `ctx` with name `name` on subprocess object `p`.
  *
  *  Returns 0 on success
  */
 int flux_subprocess_aux_set (flux_subprocess_t *p,
                              const char *name,
-			     void *ctx,
-			     flux_free_f free);
+                             void *ctx,
+                             flux_free_f free);
 
 /*
  *  Return pointer to any context associated with `p` under `name`. If
  *   no such context exists, then NULL is returned.
  */
 void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
 
@@ -3826,14 +3803,16 @@
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_FLUX_CORE_SUBPROCESS_H */
 
+// vi: ts=4 sw=4 expandtab
+
 #endif /* !_FLUX_CORE_H */
 
 /*
  * vi:tabstop=4 shiftwidth=4 expandtab
  */
 //flux_msg_handler_f
 extern "Python" void message_handler_wrapper(flux_t *, flux_msg_handler_t *, const flux_msg_t *, void *);
```

### Comparing `flux-python-0.59.0rc0/src/_core_preproc.h` & `flux-python-0.61.0/src/_core_preproc.h`

 * *Files 1% similar despite different names*

```diff
@@ -1634,14 +1634,26 @@
     FLUX_JOB_NOVALIDATE = 8,
 };
 
 enum job_event_watch_flags {
     FLUX_JOB_EVENT_WATCH_WAITCREATE = 1,
 };
 
+enum job_lookup_flags {
+
+
+
+    FLUX_JOB_LOOKUP_JSON_DECODE = 1,
+
+
+
+
+    FLUX_JOB_LOOKUP_CURRENT = 2,
+};
+
 enum job_urgency {
     FLUX_JOB_URGENCY_MIN = 0,
     FLUX_JOB_URGENCY_HOLD = FLUX_JOB_URGENCY_MIN,
     FLUX_JOB_URGENCY_DEFAULT = 16,
     FLUX_JOB_URGENCY_MAX = 31,
     FLUX_JOB_URGENCY_EXPEDITE = FLUX_JOB_URGENCY_MAX,
 };
@@ -1688,18 +1700,18 @@
 
 typedef uint64_t flux_jobid_t;
 
 
 
 
 int flux_job_id_parse (const char *s, flux_jobid_t *id);
-# 2955 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 2967 "/__w/flux-python/flux-python/src/_core_clean.h"
 int flux_job_id_encode (flux_jobid_t id, const char *type,
                         char *buf, size_t bufsz);
-# 2966 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 2978 "/__w/flux-python/flux-python/src/_core_clean.h"
 const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
 
 
 
 
 int flux_job_strtostate (const char *s, flux_job_state_t *state);
 
@@ -1805,24 +1817,24 @@
 
 flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
 
 
 
 int flux_job_result_get (flux_future_t *f,
                          const char **json_str);
-# 3097 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3109 "/__w/flux-python/flux-python/src/_core_clean.h"
 int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
-# 3111 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3123 "/__w/flux-python/flux-python/src/_core_clean.h"
 int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
-# 3127 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3139 "/__w/flux-python/flux-python/src/_core_clean.h"
 char *flux_unwrap_string (const char *in,
                           bool verify,
                           uint32_t *userid,
                           flux_error_t *error);
-# 3155 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3167 "/__w/flux-python/flux-python/src/_core_clean.h"
 typedef struct flux_jobspec1 flux_jobspec1_t;
 typedef flux_error_t flux_jobspec1_error_t;
 
 
 
 
 
@@ -1912,27 +1924,27 @@
 
 
 
 
 
 flux_jobspec1_t *flux_jobspec1_decode (const char *s,
                                        flux_jobspec1_error_t *error);
-# 3266 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3278 "/__w/flux-python/flux-python/src/_core_clean.h"
 flux_jobspec1_t *flux_jobspec1_from_command (int argc,
                                              char **argv,
                                              char **env,
                                              int ntasks,
                                              int cores_per_task,
                                              int gpus_per_task,
                                              int nnodes,
                                              double duration);
 
 
 void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
-# 3322 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3334 "/__w/flux-python/flux-python/src/_core_clean.h"
 typedef struct flux_command flux_cmd_t;
 
 
 
 
 flux_cmd_t * flux_cmd_create (int argc, char *argv[], char **env);
 
@@ -1946,15 +1958,15 @@
 
 void flux_cmd_destroy (flux_cmd_t *cmd);
 
 
 
 
 int flux_cmd_argv_appendf (flux_cmd_t *cmd,
-             const char *fmt, ...)
+                           const char *fmt, ...)
                            ;
 
 
 
 
 int flux_cmd_argv_append (flux_cmd_t *cmd, const char *arg);
 
@@ -1984,18 +1996,18 @@
 char *flux_cmd_stringify (const flux_cmd_t *cmd);
 
 
 
 
 
 int flux_cmd_setenvf (flux_cmd_t *cmd,
-        int overwrite,
+                      int overwrite,
                       const char *name,
-        const char *fmt,
-        ...)
+                      const char *fmt,
+                      ...)
                       ;
 
 
 
 
 
 void flux_cmd_unsetenv (flux_cmd_t *cmd, const char *name);
@@ -2008,22 +2020,22 @@
 const char *flux_cmd_getenv (const flux_cmd_t *cmd, const char *name);
 
 
 
 
 int flux_cmd_setcwd (flux_cmd_t *cmd, const char *cwd);
 const char *flux_cmd_getcwd (const flux_cmd_t *cmd);
-# 3418 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3430 "/__w/flux-python/flux-python/src/_core_clean.h"
 int flux_cmd_add_channel (flux_cmd_t *cmd, const char *name);
-# 3471 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3467 "/__w/flux-python/flux-python/src/_core_clean.h"
 int flux_cmd_setopt (flux_cmd_t *cmd, const char *var, const char *val);
 const char *flux_cmd_getopt (flux_cmd_t *cmd, const char *var);
-# 3490 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3488 "/__w/flux-python/flux-python/src/_core_clean.h"
 typedef struct flux_subprocess flux_subprocess_t;
-# 3502 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3500 "/__w/flux-python/flux-python/src/_core_clean.h"
 typedef enum {
     FLUX_SUBPROCESS_INIT,
     FLUX_SUBPROCESS_RUNNING,
     FLUX_SUBPROCESS_EXITED,
     FLUX_SUBPROCESS_FAILED,
     FLUX_SUBPROCESS_STOPPED,
 } flux_subprocess_state_t;
@@ -2080,88 +2092,89 @@
     flux_subprocess_hook_f post_fork;
     void *post_fork_arg;
 } flux_subprocess_hooks_t;
 
 
 
 
-typedef void (*subprocess_log_f) (void *arg,
-                                  const char *file,
-                                  int line,
-                                  const char *func,
-                                  const char *subsys,
-                                  int level,
-                                  const char *fmt,
-                                  va_list args);
-# 3586 "/__w/flux-python/flux-python/src/_core_clean.h"
-void flux_standard_output (flux_subprocess_t *p, const char *stream);
-# 3608 "/__w/flux-python/flux-python/src/_core_clean.h"
+typedef void (*subprocess_log_f)(void *arg,
+                                 const char *file,
+                                 int line,
+                                 const char *func,
+                                 const char *subsys,
+                                 int level,
+                                 const char *fmt,
+                                 va_list args);
+# 3594 "/__w/flux-python/flux-python/src/_core_clean.h"
 flux_subprocess_t *flux_local_exec (flux_reactor_t *r,
                                     int flags,
                                     const flux_cmd_t *cmd,
                                     const flux_subprocess_ops_t *ops);
 
 flux_subprocess_t *flux_local_exec_ex (flux_reactor_t *r,
                                        int flags,
                                        const flux_cmd_t *cmd,
                                        const flux_subprocess_ops_t *ops,
                                        const flux_subprocess_hooks_t *hooks,
                                        subprocess_log_f log_fn,
                                        void *log_data);
 
 flux_subprocess_t *flux_rexec (flux_t *h,
-                 int rank,
-          int flags,
+                               int rank,
+                               int flags,
                                const flux_cmd_t *cmd,
                                const flux_subprocess_ops_t *ops);
 
 flux_subprocess_t *flux_rexec_ex (flux_t *h,
                                   const char *service_name,
                                   int rank,
                                   int flags,
                                   const flux_cmd_t *cmd,
                                   const flux_subprocess_ops_t *ops,
                                   subprocess_log_f log_fn,
                                   void *log_data);
-# 3645 "/__w/flux-python/flux-python/src/_core_clean.h"
-int flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
-int flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
-int flux_subprocess_stream_status (flux_subprocess_t *p, const char *stream);
-# 3658 "/__w/flux-python/flux-python/src/_core_clean.h"
+
+
+
+
+
+void flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
+void flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
+# 3638 "/__w/flux-python/flux-python/src/_core_clean.h"
 int flux_subprocess_write (flux_subprocess_t *p,
-             const char *stream,
+                           const char *stream,
                            const char *buf,
-      size_t len);
+                           size_t len);
 
 
 
 
 
 
 int flux_subprocess_close (flux_subprocess_t *p, const char *stream);
-# 3681 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3661 "/__w/flux-python/flux-python/src/_core_clean.h"
 const char *flux_subprocess_read (flux_subprocess_t *p,
                                   const char *stream,
                                   int len,
-      int *lenp);
-# 3697 "/__w/flux-python/flux-python/src/_core_clean.h"
+                                  int *lenp);
+# 3677 "/__w/flux-python/flux-python/src/_core_clean.h"
 const char *flux_subprocess_read_line (flux_subprocess_t *p,
                                        const char *stream,
                                        int *lenp);
 
 
 
 
 const char *flux_subprocess_read_trimmed_line (flux_subprocess_t *p,
                                                const char *stream,
                                                int *lenp);
-# 3717 "/__w/flux-python/flux-python/src/_core_clean.h"
-int flux_subprocess_read_stream_closed (flux_subprocess_t *p,
-                                        const char *stream);
-# 3736 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3696 "/__w/flux-python/flux-python/src/_core_clean.h"
+bool flux_subprocess_read_stream_closed (flux_subprocess_t *p,
+                                         const char *stream);
+# 3715 "/__w/flux-python/flux-python/src/_core_clean.h"
 const char *flux_subprocess_getline (flux_subprocess_t *p,
                                      const char *stream,
                                      int *lenp);
 
 
 
 
@@ -2171,17 +2184,22 @@
 flux_future_t *flux_subprocess_kill (flux_subprocess_t *p, int signo);
 
 
 
 
 
 
-void flux_subprocess_ref (flux_subprocess_t *p);
-void flux_subprocess_unref (flux_subprocess_t *p);
-# 3763 "/__w/flux-python/flux-python/src/_core_clean.h"
+void flux_subprocess_destroy (flux_subprocess_t *p);
+
+
+
+
+
+
+
 flux_subprocess_state_t flux_subprocess_state (flux_subprocess_t *p);
 
 
 
 const char *flux_subprocess_state_string (flux_subprocess_state_t state);
 
 int flux_subprocess_rank (flux_subprocess_t *p);
@@ -2221,31 +2239,31 @@
 
 
 
 
 
 int flux_subprocess_aux_set (flux_subprocess_t *p,
                              const char *name,
-        void *ctx,
-        flux_free_f free);
+                             void *ctx,
+                             flux_free_f free);
 
 
 
 
 
 void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
 
 
 
 
 
 
 void flux_subprocess_channel_incref (flux_subprocess_t *p, const char *name);
 void flux_subprocess_channel_decref (flux_subprocess_t *p, const char *name);
-# 3839 "/__w/flux-python/flux-python/src/_core_clean.h"
+# 3818 "/__w/flux-python/flux-python/src/_core_clean.h"
 extern "Python" void message_handler_wrapper(flux_t *, flux_msg_handler_t *, const flux_msg_t *, void *);
 
 
 extern "Python" void timeout_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void fd_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void signal_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
```

### Comparing `flux-python-0.59.0rc0/src/_hostlist_build.py` & `flux-python-0.61.0/src/_hostlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_hostlist_clean.h` & `flux-python-0.61.0/src/_hostlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_hostlist_preproc.h` & `flux-python-0.61.0/src/_hostlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_idset_build.py` & `flux-python-0.61.0/src/_idset_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_idset_clean.h` & `flux-python-0.61.0/src/_idset_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_idset_preproc.h` & `flux-python-0.61.0/src/_idset_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_rlist_build.py` & `flux-python-0.61.0/src/_rlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_security_build.py` & `flux-python-0.61.0/src/_security_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_security_clean.h` & `flux-python-0.61.0/src/_security_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/_security_preproc.h` & `flux-python-0.61.0/src/_security_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/callbacks.h` & `flux-python-0.61.0/src/callbacks.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.59.0rc0/src/make_clean_header.py` & `flux-python-0.61.0/src/make_clean_header.py`

 * *Files identical despite different names*

