# Comparing `tmp/nkululeko-0.81.1.tar.gz` & `tmp/nkululeko-0.81.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.81.1.tar", last modified: Thu Mar 21 11:07:55 2024, max compression
+gzip compressed data, was "nkululeko-0.81.2.tar", last modified: Mon Apr 15 11:56:11 2024, max compression
```

## Comparing `nkululeko-0.81.1.tar` & `nkululeko-0.81.2.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16317 2024-03-21 11:07:41.000000 nkululeko-0.81.1/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.1/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34397 2024-03-21 11:07:55.734946 nkululeko-0.81.1/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.1/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.1/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.1/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.1/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.1/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.1/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.1/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.1/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.1/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.1/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/crema-d/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3281 2023-06-13 12:24:10.000000 nkululeko-0.81.1/data/crema-d/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.1/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.1/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.1/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.1/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.1/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.1/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.1/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.1/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.1/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.1/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.1/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.1/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.1/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.1/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.1/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3327 2023-08-31 07:30:49.000000 nkululeko-0.81.1/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.1/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.1/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.1/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.1/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.1/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3072 2024-03-13 09:14:20.000000 nkululeko-0.81.1/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.1/meta/demos/demo_best_model.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.726946 nkululeko-0.81.1/meta/demos/multiple_exeriments/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.1/meta/demos/multiple_exeriments/do_experiments.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.1/meta/demos/multiple_exeriments/parse_nkulu.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.1/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.1/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.1/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.730946 nkululeko-0.81.1/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.1/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.1/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.1/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.730946 nkululeko-0.81.1/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.1/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.1/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.1/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.1/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.730946 nkululeko-0.81.1/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.1/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4818 2023-09-26 13:42:48.000000 nkululeko-0.81.1/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.1/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-03-21 11:07:36.000000 nkululeko-0.81.1/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.730946 nkululeko-0.81.1/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.1/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27110 2024-03-18 15:55:42.000000 nkululeko-0.81.1/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.1/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2500 2024-03-14 10:49:21.000000 nkululeko-0.81.1/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.1/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4544 2024-03-21 10:35:41.000000 nkululeko-0.81.1/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29575 2024-03-18 15:37:11.000000 nkululeko-0.81.1/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2250 2024-02-29 11:07:16.000000 nkululeko-0.81.1/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.1/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.730946 nkululeko-0.81.1/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.1/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3192 2024-03-12 12:44:04.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3278 2024-03-12 12:44:04.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3108 2024-03-12 12:44:04.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3078 2024-03-12 12:44:04.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-03-11 08:25:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4149 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3039 2023-12-15 13:29:14.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2771 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4521 2024-02-20 12:42:26.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.1/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21253 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7281 2023-12-19 11:16:14.000000 nkululeko-0.81.1/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.1/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.1/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.1/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.730946 nkululeko-0.81.1/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.1/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.1/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.1/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9337 2024-02-26 18:28:01.000000 nkululeko-0.81.1/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.1/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11638 2024-03-21 10:35:30.000000 nkululeko-0.81.1/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.1/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9716 2024-02-13 14:17:48.000000 nkululeko-0.81.1/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.1/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.1/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.1/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.1/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9097 2024-03-12 12:49:32.000000 nkululeko-0.81.1/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10054 2024-03-21 10:35:22.000000 nkululeko-0.81.1/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      867 2024-03-21 10:56:45.000000 nkululeko-0.81.1/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.1/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.1/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.1/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.1/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.1/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5732 2024-03-11 14:48:46.000000 nkululeko-0.81.1/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.1/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.1/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1876 2023-12-19 11:16:14.000000 nkululeko-0.81.1/nkululeko/predict.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11497 2024-02-13 13:56:24.000000 nkululeko-0.81.1/nkululeko/reporter.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.1/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.1/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.1/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.1/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.1/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2233 2024-03-14 15:08:12.000000 nkululeko-0.81.1/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      574 2024-02-13 13:17:42.000000 nkululeko-0.81.1/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7451 2024-02-26 18:30:48.000000 nkululeko-0.81.1/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.1/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.1/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.1/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.1/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.1/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.1/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1486 2024-03-18 15:18:33.000000 nkululeko-0.81.1/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2695 2024-03-18 15:40:15.000000 nkululeko-0.81.1/nkululeko/test_predictor.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.1/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.1/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2788 2023-12-19 11:26:19.000000 nkululeko-0.81.1/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.1/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34397 2024-03-21 11:07:55.000000 nkululeko-0.81.1/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5124 2024-03-21 11:07:55.000000 nkululeko-0.81.1/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-03-21 11:07:55.000000 nkululeko-0.81.1/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 11:07:55.000000 nkululeko-0.81.1/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-03-21 11:07:55.000000 nkululeko-0.81.1/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.1/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      968 2024-03-21 11:07:55.734946 nkululeko-0.81.1/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.1/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.722946 nkululeko-0.81.1/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-03-21 11:07:55.734946 nkululeko-0.81.1/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.1/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16443 2024-04-15 11:35:17.000000 nkululeko-0.81.2/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.81.2/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34523 2024-04-15 11:56:11.319774 nkululeko-0.81.2/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16870 2024-03-18 08:28:24.000000 nkululeko-0.81.2/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.81.2/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.81.2/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.81.2/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.81.2/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.81.2/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.81.2/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/crema-d/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3281 2023-06-13 12:24:10.000000 nkululeko-0.81.2/data/crema-d/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.81.2/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.81.2/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.81.2/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.81.2/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.81.2/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.81.2/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.81.2/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.81.2/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3327 2023-08-31 07:30:49.000000 nkululeko-0.81.2/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.81.2/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.81.2/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.81.2/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.81.2/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.81.2/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3072 2024-03-13 09:14:20.000000 nkululeko-0.81.2/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.81.2/meta/demos/demo_best_model.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.311774 nkululeko-0.81.2/meta/demos/multiple_exeriments/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1043 2022-04-12 11:25:08.000000 nkululeko-0.81.2/meta/demos/multiple_exeriments/do_experiments.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3871 2022-08-30 17:14:03.000000 nkululeko-0.81.2/meta/demos/multiple_exeriments/parse_nkulu.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.81.2/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.81.2/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.81.2/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.81.2/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.81.2/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.81.2/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.81.2/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.81.2/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.81.2/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.81.2/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.81.2/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4818 2023-09-26 13:42:48.000000 nkululeko-0.81.2/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.81.2/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-04-15 11:55:58.000000 nkululeko-0.81.2/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.315774 nkululeko-0.81.2/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.81.2/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27265 2024-03-27 10:33:18.000000 nkululeko-0.81.2/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3407 2024-02-28 17:49:47.000000 nkululeko-0.81.2/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2500 2024-03-14 10:49:21.000000 nkululeko-0.81.2/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.81.2/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4733 2024-04-15 11:33:44.000000 nkululeko-0.81.2/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    29575 2024-03-18 15:37:11.000000 nkululeko-0.81.2/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2250 2024-02-29 11:07:16.000000 nkululeko-0.81.2/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.81.2/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3192 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3278 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11399 2024-01-24 16:15:03.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3108 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3078 2024-03-12 12:44:04.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3379 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5205 2023-10-20 09:59:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1598 2024-03-11 08:25:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4149 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4140 2023-10-16 17:04:58.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4734 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3039 2023-12-15 13:29:14.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2771 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3656 2023-11-16 12:12:10.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4521 2024-02-20 12:42:26.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3211 2024-02-29 15:42:20.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5072 2024-02-15 14:59:43.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4683 2024-03-14 11:24:49.000000 nkululeko-0.81.2/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1375 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21287 2024-04-15 11:30:05.000000 nkululeko-0.81.2/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7281 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      453 2024-02-28 17:38:08.000000 nkululeko-0.81.2/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.81.2/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.81.2/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.81.2/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9337 2024-02-26 18:28:01.000000 nkululeko-0.81.2/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.81.2/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11638 2024-03-21 10:35:30.000000 nkululeko-0.81.2/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      378 2023-12-23 10:35:03.000000 nkululeko-0.81.2/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9716 2024-02-13 14:17:48.000000 nkululeko-0.81.2/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      645 2023-09-26 13:42:48.000000 nkululeko-0.81.2/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      573 2023-09-07 11:38:13.000000 nkululeko-0.81.2/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      580 2023-09-07 11:38:09.000000 nkululeko-0.81.2/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      392 2023-12-19 13:57:23.000000 nkululeko-0.81.2/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9097 2024-03-12 12:49:32.000000 nkululeko-0.81.2/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10054 2024-03-21 10:35:22.000000 nkululeko-0.81.2/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      867 2024-03-21 10:56:45.000000 nkululeko-0.81.2/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      699 2024-03-21 10:56:18.000000 nkululeko-0.81.2/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      390 2023-09-07 11:38:37.000000 nkululeko-0.81.2/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      397 2023-09-07 11:38:33.000000 nkululeko-0.81.2/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-03-21 10:21:07.000000 nkululeko-0.81.2/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      227 2023-12-14 15:14:23.000000 nkululeko-0.81.2/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5732 2024-03-11 14:48:46.000000 nkululeko-0.81.2/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1966 2024-02-28 17:41:34.000000 nkululeko-0.81.2/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23025 2024-02-01 14:55:26.000000 nkululeko-0.81.2/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1876 2023-12-19 11:16:14.000000 nkululeko-0.81.2/nkululeko/predict.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11497 2024-02-13 13:56:24.000000 nkululeko-0.81.2/nkululeko/reporter.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.81.2/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.81.2/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.81.2/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.81.2/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.81.2/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2233 2024-03-14 15:08:12.000000 nkululeko-0.81.2/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      574 2024-02-13 13:17:42.000000 nkululeko-0.81.2/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7451 2024-02-26 18:30:48.000000 nkululeko-0.81.2/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.81.2/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.81.2/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.81.2/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.81.2/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.81.2/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.81.2/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1486 2024-03-18 15:18:33.000000 nkululeko-0.81.2/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2695 2024-03-18 15:40:15.000000 nkululeko-0.81.2/nkululeko/test_predictor.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.81.2/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.81.2/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2788 2023-12-19 11:26:19.000000 nkululeko-0.81.2/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12330 2024-03-21 11:06:05.000000 nkululeko-0.81.2/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    34523 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5124 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      267 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-04-15 11:56:11.000000 nkululeko-0.81.2/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.81.2/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      968 2024-04-15 11:56:11.319774 nkululeko-0.81.2/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.81.2/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.307774 nkululeko-0.81.2/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-04-15 11:56:11.319774 nkululeko-0.81.2/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.81.2/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.81.1/CHANGELOG.md` & `nkululeko-0.81.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+Version 0.81.2
+--------------
+* added a parselmouth.Praat error if pitch out of range
+* changed file path for demo_predictor
+
 Version 0.81.1
 --------------
 * fixed bugs in demo module 
 * made kernel for SVM/SVR configurable
 
 Version 0.81.0
 --------------
```

### Comparing `nkululeko-0.81.1/LICENSE` & `nkululeko-0.81.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/PKG-INFO` & `nkululeko-0.81.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.1
+Version: 0.81.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -317,14 +317,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.2
+--------------
+* added a parselmouth.Praat error if pitch out of range
+* changed file path for demo_predictor
+
 Version 0.81.1
 --------------
 * fixed bugs in demo module 
 * made kernel for SVM/SVR configurable
 
 Version 0.81.0
 --------------
```

### Comparing `nkululeko-0.81.1/README.md` & `nkululeko-0.81.2/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/aesdd/process_database.py` & `nkululeko-0.81.2/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/androids/process_database.py` & `nkululeko-0.81.2/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/androids_orig/process_database.py` & `nkululeko-0.81.2/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/androids_test/process_database.py` & `nkululeko-0.81.2/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/ased/process_database.py` & `nkululeko-0.81.2/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/asvp-esd/process_database.py` & `nkululeko-0.81.2/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/baved/process_database.py` & `nkululeko-0.81.2/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/cafe/process_database.py` & `nkululeko-0.81.2/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/clac/process_database.py` & `nkululeko-0.81.2/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/cmu-mosei/process_database.py` & `nkululeko-0.81.2/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/crema-d/process_database.py` & `nkululeko-0.81.2/data/crema-d/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/demos/process_database.py` & `nkululeko-0.81.2/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/ekorpus/process_database.py` & `nkululeko-0.81.2/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emns/process_database.py` & `nkululeko-0.81.2/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emofilm/convert_to_16k.py` & `nkululeko-0.81.2/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emofilm/process_database.py` & `nkululeko-0.81.2/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emorynlp/process_database.py` & `nkululeko-0.81.2/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emov-db/process_database.py` & `nkululeko-0.81.2/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emovo/process_database.py` & `nkululeko-0.81.2/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/emozionalmente/create.py` & `nkululeko-0.81.2/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/enterface/process_database.py` & `nkululeko-0.81.2/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/esd/process_database.py` & `nkululeko-0.81.2/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/gerparas/process_database.py` & `nkululeko-0.81.2/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/iemocap/process_database.py` & `nkululeko-0.81.2/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/jl/process_database.py` & `nkululeko-0.81.2/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/jtes/process_database.py` & `nkululeko-0.81.2/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/meld/process_database.py` & `nkululeko-0.81.2/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/mesd/process_database.py` & `nkululeko-0.81.2/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/mess/process_database.py` & `nkululeko-0.81.2/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/mlendsnd/process_database.py` & `nkululeko-0.81.2/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/msp-improv/process_database2.py` & `nkululeko-0.81.2/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/msp-podcast/process_database.py` & `nkululeko-0.81.2/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/oreau2/process_database.py` & `nkululeko-0.81.2/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/portuguese/process_database.py` & `nkululeko-0.81.2/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/ravdess/process_database.py` & `nkululeko-0.81.2/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/ravdess/process_database_speaker.py` & `nkululeko-0.81.2/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/savee/process_database.py` & `nkululeko-0.81.2/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/shemo/process_database.py` & `nkululeko-0.81.2/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/subesco/process_database.py` & `nkululeko-0.81.2/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/tess/process_database.py` & `nkululeko-0.81.2/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/thorsten-emotional/process_database.py` & `nkululeko-0.81.2/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/urdu/process_database.py` & `nkululeko-0.81.2/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/data/vivae/process_database.py` & `nkululeko-0.81.2/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/docs/source/conf.py` & `nkululeko-0.81.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/meta/demos/demo_best_model.py` & `nkululeko-0.81.2/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/meta/demos/multiple_exeriments/do_experiments.py` & `nkululeko-0.81.2/meta/demos/multiple_exeriments/do_experiments.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/meta/demos/multiple_exeriments/parse_nkulu.py` & `nkululeko-0.81.2/meta/demos/multiple_exeriments/parse_nkulu.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/meta/demos/my_experiment.py` & `nkululeko-0.81.2/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/meta/demos/my_experiment_local.py` & `nkululeko-0.81.2/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/meta/demos/plot_faster_anim.py` & `nkululeko-0.81.2/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/aug_train.py` & `nkululeko-0.81.2/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/augment.py` & `nkululeko-0.81.2/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/augmenting/augmenter.py` & `nkululeko-0.81.2/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.81.2/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.81.2/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/augmenting/resampler.py` & `nkululeko-0.81.2/nkululeko/augmenting/resampler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_age.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.81.2/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.81.2/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/cacheddataset.py` & `nkululeko-0.81.2/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/data/dataset.py` & `nkululeko-0.81.2/nkululeko/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,18 @@
                 if got_age2:
                     df["age"] = df_target["age"].astype(int)
                 # copy other column
                 for column in df_target.columns:
                     if column not in [self.target, "age", "speaker", "gender"]:
                         df[column] = df_target[column]
             except audformat.core.errors.BadKeyError:
-                pass
+                if not self.is_labeled:
+                    self.util.error(
+                        f"Giving up: no target ({self.target}) column found"
+                    )
 
         if self.is_labeled:
             # remember the target in case they get labelencoded later
             df["class_label"] = df[self.target]
 
         self.df = df
         self._report_load()
```

### Comparing `nkululeko-0.81.1/nkululeko/data/dataset_csv.py` & `nkululeko-0.81.2/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/demo.py` & `nkululeko-0.81.2/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/demo_feats.py` & `nkululeko-0.81.2/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/demo_predictor.py` & `nkululeko-0.81.2/nkululeko/demo_predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pandas as pd
 import numpy as np
 import audiofile
 import audformat
 import nkululeko.glob_conf as glob_conf
 from nkululeko.utils.util import Util
 
@@ -48,21 +49,24 @@
                             # first line might be "file"
                             if self.file.endswith(".csv") and first:
                                 first = False
                             else:
                                 file_list.append(line)
                 for file_name in file_list:
                     test_folder = glob_conf.config["DATA"]["test_folder"]
-                    file_path = test_folder + file_name.strip()
+                    file_path = os.path.join(test_folder, file_name.strip())
                     sig, sr = audiofile.read(file_path)
                     print(f"predicting file {file_path}")
                     res_dict = self.predict_signal(sig, sr)
-                    df_tmp = pd.DataFrame(res_dict, index=[file_path])
+                    df_tmp = pd.DataFrame(res_dict, index=[file_name.strip()])
                     df_res = pd.concat([df_res, df_tmp], ignore_index=False)
                 df_res = df_res.set_index(df_res.index.rename("file"))
+                # save only filename and prediction (df_tmp) by default
+                # drop other columns
+                # df_res = df_res[["predicted"]]
                 if self.outfile is not None:
                     df_res.to_csv(self.outfile)
                 else:
                     self.util.debug(df_res)
         else:
             while True:
                 signal = self.record_audio(3)
```

### Comparing `nkululeko-0.81.1/nkululeko/experiment.py` & `nkululeko-0.81.2/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/explore.py` & `nkululeko-0.81.2/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/export.py` & `nkululeko-0.81.2/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_audmodel_dim.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/featureset.py` & `nkululeko-0.81.2/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.81.2/nkululeko/feat_extract/feinberg_praat.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,16 +290,16 @@
                 f4_mean,
                 f1_median,
                 f2_median,
                 f3_median,
                 f4_median,
             ) = measureFormants(sound, 75, 300)
             #        file_list.append(wave_file) # make an ID list
-        except statistics.StatisticsError as se:
-            print(f"error on file {wave_file}: {se}")
+        except (statistics.StatisticsError, parselmouth.PraatError) as errors:
+            print(f"error on file {wave_file}: {errors}")
 
         duration_list.append(duration)  # make duration list
         mean_F0_list.append(meanF0)  # make a mean F0 list
         sd_F0_list.append(stdevF0)  # make a sd F0 list
         hnr_list.append(hnr)  # add HNR data
 
         # add raw jitter and shimmer measures
```

### Comparing `nkululeko-0.81.1/nkululeko/feature_extractor.py` & `nkululeko-0.81.2/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/file_checker.py` & `nkululeko-0.81.2/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/filter_data.py` & `nkululeko-0.81.2/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/losses/loss_ccc.py` & `nkululeko-0.81.2/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.81.2/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/modelrunner.py` & `nkululeko-0.81.2/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model.py` & `nkululeko-0.81.2/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_cnn.py` & `nkululeko-0.81.2/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_gmm.py` & `nkululeko-0.81.2/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_knn.py` & `nkululeko-0.81.2/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_knn_reg.py` & `nkululeko-0.81.2/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_mlp.py` & `nkululeko-0.81.2/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.81.2/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_svm.py` & `nkululeko-0.81.2/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/models/model_svr.py` & `nkululeko-0.81.2/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/multidb.py` & `nkululeko-0.81.2/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/nkululeko.py` & `nkululeko-0.81.2/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/plots.py` & `nkululeko-0.81.2/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/predict.py` & `nkululeko-0.81.2/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/reporter.py` & `nkululeko-0.81.2/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/reporting/defines.py` & `nkululeko-0.81.2/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/reporting/latex_writer.py` & `nkululeko-0.81.2/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/reporting/report.py` & `nkululeko-0.81.2/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/reporting/report_item.py` & `nkululeko-0.81.2/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/resample.py` & `nkululeko-0.81.2/nkululeko/resample.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/result.py` & `nkululeko-0.81.2/nkululeko/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/runmanager.py` & `nkululeko-0.81.2/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/scaler.py` & `nkululeko-0.81.2/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/segment.py` & `nkululeko-0.81.2/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.81.2/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.81.2/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/syllable_nuclei.py` & `nkululeko-0.81.2/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/test.py` & `nkululeko-0.81.2/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/test_predictor.py` & `nkululeko-0.81.2/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/utils/files.py` & `nkululeko-0.81.2/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/utils/stats.py` & `nkululeko-0.81.2/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko/utils/util.py` & `nkululeko-0.81.2/nkululeko/utils/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.81.2/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.81.1
+Version: 0.81.2
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -317,14 +317,19 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.81.2
+--------------
+* added a parselmouth.Praat error if pitch out of range
+* changed file path for demo_predictor
+
 Version 0.81.1
 --------------
 * fixed bugs in demo module 
 * made kernel for SVM/SVR configurable
 
 Version 0.81.0
 --------------
```

### Comparing `nkululeko-0.81.1/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.81.2/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/setup.cfg` & `nkululeko-0.81.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.81.1/venv/bin/activate_this.py` & `nkululeko-0.81.2/venv/bin/activate_this.py`

 * *Files identical despite different names*

