# Comparing `tmp/wikimedia-spicerack-8.4.1.tar.gz` & `tmp/wikimedia_spicerack-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimedia-spicerack-8.4.1.tar", last modified: Wed Mar  6 16:49:15 2024, max compression
+gzip compressed data, was "wikimedia_spicerack-8.5.0.tar", last modified: Mon Apr 15 11:13:48 2024, max compression
```

## Comparing `wikimedia-spicerack-8.4.1.tar` & `wikimedia_spicerack-8.5.0.tar`

### file list

```diff
@@ -1,285 +1,287 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.246647 wikimedia-spicerack-8.4.1/
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-8.4.1/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/.git-blame-ignore-revs
--rw-r--r--   0 riccardo   (501) staff       (20)      337 2023-10-09 09:28:22.000000 wikimedia-spicerack-8.4.1/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-8.4.1/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/.mailmap
--rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)   118387 2024-03-06 16:31:09.000000 wikimedia-spicerack-8.4.1/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-8.4.1/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-8.4.1/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     3310 2024-03-06 16:49:15.246128 wikimedia-spicerack-8.4.1/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2023-05-21 08:23:21.000000 wikimedia-spicerack-8.4.1/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.345133 wikimedia-spicerack-8.4.1/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.346507 wikimedia-spicerack-8.4.1/doc/examples/
--rw-r--r--   0 riccardo   (501) staff       (20)     1947 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/doc/examples/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.377920 wikimedia-spicerack-8.4.1/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.379360 wikimedia-spicerack-8.4.1/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/doc/source/_static/theme_overrides.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.482277 wikimedia-spicerack-8.4.1/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)     1072 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.administrative.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.alerting.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.alertmanager.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.apt.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.confctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.debmonitor.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.dhcp.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.dnsdisc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.elasticsearch_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.ganeti.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.icinga.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.ipmi.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.k8s.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.kafka.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.locking.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.mediawiki.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.mysql.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.mysql_legacy.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.netbox.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.peeringdb.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.puppet.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.redfish.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.redis_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.remote.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.reposync.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.service.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.toolforge.etcdctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.toolforge.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/api/spicerack.typing.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-11 12:43:16.000000 wikimedia-spicerack-8.4.1/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/doc/source/configuration.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/doc/source/development.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/doc/source/docutils.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-8.4.1/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)    13752 2023-11-16 09:37:52.000000 wikimedia-spicerack-8.4.1/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/pyproject.toml
--rw-r--r--   0 riccardo   (501) staff       (20)      565 2024-03-06 16:49:15.270527 wikimedia-spicerack-8.4.1/setup.cfg
--rwxr-xr-x   0 riccardo   (501) staff       (20)     3357 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/setup.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.572766 wikimedia-spicerack-8.4.1/spicerack/
--rw-r--r--   0 riccardo   (501) staff       (20)    30626 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18742 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-11 12:43:16.000000 wikimedia-spicerack-8.4.1/spicerack/_log.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20283 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/_menu.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1800 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/_module_api.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-10-09 10:54:02.000000 wikimedia-spicerack-8.4.1/spicerack/administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12928 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8106 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4435 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/spicerack/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11425 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-8.4.1/spicerack/dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)    15764 2024-02-27 14:20:55.000000 wikimedia-spicerack-8.4.1/spicerack/ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18847 2024-03-06 16:31:09.000000 wikimedia-spicerack-8.4.1/spicerack/k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-8.4.1/spicerack/kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    25468 2023-10-18 12:59:29.000000 wikimedia-spicerack-8.4.1/spicerack/locking.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14896 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/spicerack/mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18146 2024-03-06 16:15:48.000000 wikimedia-spicerack-8.4.1/spicerack/netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27908 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)    36793 2024-01-29 10:28:09.000000 wikimedia-spicerack-8.4.1/spicerack/redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    29219 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23308 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.579421 wikimedia-spicerack-8.4.1/spicerack/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-09-30 09:43:02.000000 wikimedia-spicerack-8.4.1/spicerack/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.609601 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.611489 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/confctl/
--rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/confctl/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/confctl/schema.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.612694 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config/valid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-09-24 11:12:36.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config_bad_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config_empty_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-09-24 11:12:27.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/config_wrong_overrides.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.285680 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.622093 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.683895 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      778 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/lock_args.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
--rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
--rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
--rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.691255 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group1/
--rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.744015 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.753424 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
--rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.796547 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
--rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.797860 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.806892 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
--rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
--rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
--rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
--rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
--rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
--rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
--rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.828022 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2023-09-29 08:51:27.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      311 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/root.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.830489 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/debmonitor/
--rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/debmonitor/config.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.831811 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/discovery/
--rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/discovery/authdns.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.833558 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/elasticsearch/
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/elasticsearch/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.291423 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.836039 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
--rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.845789 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.848300 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/
--rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.881492 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/spicerack_ext/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
--rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/spicerack_extender.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.916556 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/404.json
--rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/bogus.json
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       76 2023-10-09 09:28:22.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/groups.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3059 2023-10-09 09:28:22.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/groups_bulk.json
--rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/info.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/instance.json
--rw-r--r--   0 riccardo   (501) staff       (20)      339 2023-10-09 09:28:22.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/nodes.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3817 2023-10-09 09:28:22.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/nodes_bulk.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.964572 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/
--rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_downtimed.json
--rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_invalid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_missing.json
--rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_valid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.970496 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/kafka/
--rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/kafka/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.973643 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/locking/
--rw-r--r--   0 riccardo   (501) staff       (20)       25 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/locking/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.975008 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/netbox/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/netbox/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.978014 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/peeringdb/
--rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/peeringdb/asn.json
--rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/peeringdb/ixlan.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.979453 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/phabricator/valid.conf
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.980868 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/redis_cluster/
--rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/redis_cluster/cluster.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:14.991440 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/remote/
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/remote/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/remote/config_installer.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.009796 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/reposync/
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/reposync/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.015221 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/service/
--rw-r--r--   0 riccardo   (501) staff       (20)     3943 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/service/service.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.148278 wikimedia-spicerack-8.4.1/spicerack/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    29800 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test__cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-11 12:43:16.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test__log.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-10-09 10:54:02.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13905 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7482 2024-01-26 10:26:17.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18439 2023-10-17 20:12:25.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    19964 2024-02-27 14:20:55.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)    17048 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_init.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    24248 2024-03-06 16:31:09.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23449 2023-10-18 12:59:29.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_locking.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11561 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    19269 2024-03-06 16:15:48.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    47647 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    24937 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    16854 2023-10-16 17:16:03.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.164124 wikimedia-spicerack-8.4.1/spicerack/tests/unit/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/tests/unit/toolforge/test_etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3038 2024-02-21 17:31:26.000000 wikimedia-spicerack-8.4.1/spicerack/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.183424 wikimedia-spicerack-8.4.1/spicerack/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-8.4.1/spicerack/toolforge/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-8.4.1/spicerack/toolforge/etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-10-16 12:11:07.000000 wikimedia-spicerack-8.4.1/spicerack/typing.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2180 2024-01-29 13:05:02.000000 wikimedia-spicerack-8.4.1/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.214794 wikimedia-spicerack-8.4.1/utils/
--rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/utils/check-style.sh
--rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-8.4.1/utils/format-code.sh
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-03-06 16:49:15.241193 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     3310 2024-03-06 16:49:13.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)    10094 2024-03-06 16:49:14.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2024-03-06 16:49:13.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2024-03-06 16:49:13.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/entry_points.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2024-03-06 16:49:13.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      666 2024-03-06 16:49:13.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       10 2024-03-06 16:49:13.000000 wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:48.275227 wikimedia_spicerack-8.5.0/
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia_spicerack-8.5.0/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/.git-blame-ignore-revs
+-rw-r--r--   0 riccardo   (501) staff       (20)      337 2023-10-09 09:28:22.000000 wikimedia_spicerack-8.5.0/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia_spicerack-8.5.0/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/.mailmap
+-rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)   120471 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia_spicerack-8.5.0/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia_spicerack-8.5.0/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     3259 2024-04-15 11:13:48.273974 wikimedia_spicerack-8.5.0/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2023-05-21 08:23:21.000000 wikimedia_spicerack-8.5.0/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.137389 wikimedia_spicerack-8.5.0/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.138821 wikimedia_spicerack-8.5.0/doc/examples/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1947 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/doc/examples/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.270267 wikimedia_spicerack-8.5.0/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.275656 wikimedia_spicerack-8.5.0/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/doc/source/_static/theme_overrides.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.398824 wikimedia_spicerack-8.5.0/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1072 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.administrative.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.alerting.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.alertmanager.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.apt.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.confctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.debmonitor.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.dhcp.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.dnsdisc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.elasticsearch_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.ganeti.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.icinga.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.ipmi.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.k8s.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.kafka.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.locking.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.mediawiki.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.mysql.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.mysql_legacy.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.netbox.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.peeringdb.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.puppet.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.redfish.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.redis_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.remote.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.reposync.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.service.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.toolforge.etcdctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.toolforge.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/api/spicerack.typing.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-11 12:43:16.000000 wikimedia_spicerack-8.5.0/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/doc/source/configuration.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/doc/source/development.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/doc/source/docutils.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia_spicerack-8.5.0/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)    13752 2023-11-16 09:37:52.000000 wikimedia_spicerack-8.5.0/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/pyproject.toml
+-rw-r--r--   0 riccardo   (501) staff       (20)      565 2024-04-15 11:13:48.280147 wikimedia_spicerack-8.5.0/setup.cfg
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     3256 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/setup.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.519765 wikimedia_spicerack-8.5.0/spicerack/
+-rw-r--r--   0 riccardo   (501) staff       (20)    32174 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18742 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-11 12:43:16.000000 wikimedia_spicerack-8.5.0/spicerack/_log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20283 2024-02-21 17:31:26.000000 wikimedia_spicerack-8.5.0/spicerack/_menu.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1800 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/_module_api.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-10-09 10:54:02.000000 wikimedia_spicerack-8.5.0/spicerack/administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    15372 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8106 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4435 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/spicerack/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11425 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia_spicerack-8.5.0/spicerack/dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    29926 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    15764 2024-02-27 14:20:55.000000 wikimedia_spicerack-8.5.0/spicerack/ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18847 2024-04-15 09:37:36.000000 wikimedia_spicerack-8.5.0/spicerack/k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia_spicerack-8.5.0/spicerack/kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    25468 2023-10-18 12:59:29.000000 wikimedia_spicerack-8.5.0/spicerack/locking.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14896 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/spicerack/mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    22764 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28169 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)    36793 2024-01-29 10:28:09.000000 wikimedia_spicerack-8.5.0/spicerack/redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    29219 2024-02-21 17:31:26.000000 wikimedia_spicerack-8.5.0/spicerack/remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23473 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.538092 wikimedia_spicerack-8.5.0/spicerack/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-09-30 09:43:02.000000 wikimedia_spicerack-8.5.0/spicerack/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.549242 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.550305 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/alertmanager/
+-rw-r--r--   0 riccardo   (501) staff       (20)      402 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/alertmanager/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.552864 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/confctl/
+-rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/confctl/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/confctl/schema.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.554067 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config/valid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-09-24 11:12:36.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config_bad_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config_empty_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-09-24 11:12:27.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/config_wrong_overrides.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.038875 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.567607 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.629299 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      778 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/lock_args.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.631786 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.635020 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.637858 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.686925 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.690281 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.698294 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.701180 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2023-09-29 08:51:27.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      311 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/root.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.702805 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/debmonitor/
+-rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/debmonitor/config.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.709102 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/discovery/
+-rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/discovery/authdns.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.713396 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/elasticsearch/
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/elasticsearch/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.059928 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.725418 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
+-rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.730677 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.735309 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/
+-rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.738350 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/spicerack_ext/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.765011 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/404.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/bogus.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       76 2023-10-09 09:28:22.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/groups.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3059 2023-10-09 09:28:22.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/groups_bulk.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/info.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/instance.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      339 2023-10-09 09:28:22.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/nodes.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3817 2023-10-09 09:28:22.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/nodes_bulk.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.903585 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/
+-rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_downtimed.json
+-rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_invalid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_missing.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_valid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.905285 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/kafka/
+-rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/kafka/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.907581 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/locking/
+-rw-r--r--   0 riccardo   (501) staff       (20)       25 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/locking/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.910256 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/netbox/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/netbox/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.917016 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/peeringdb/
+-rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/peeringdb/asn.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/peeringdb/ixlan.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.918238 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/phabricator/valid.conf
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.919939 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/redis_cluster/
+-rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/redis_cluster/cluster.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.923159 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/remote/
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/remote/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/remote/config_installer.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.955198 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/reposync/
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/reposync/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:47.988906 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/service/
+-rw-r--r--   0 riccardo   (501) staff       (20)     3943 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/service/service.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:48.145493 wikimedia_spicerack-8.5.0/spicerack/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    29800 2024-02-21 17:31:26.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test__cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-11 12:43:16.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test__log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-10-09 10:54:02.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3598 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    15228 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7482 2024-01-26 10:26:17.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18439 2023-10-17 20:12:25.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    42985 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    19964 2024-02-27 14:20:55.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    19985 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_init.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20469 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24126 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23449 2023-10-18 12:59:29.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_locking.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11561 2023-10-16 17:16:03.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24205 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    48668 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    44853 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24937 2024-02-21 17:31:26.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    17218 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:48.154485 wikimedia_spicerack-8.5.0/spicerack/tests/unit/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/tests/unit/toolforge/test_etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3038 2024-02-21 17:31:26.000000 wikimedia_spicerack-8.5.0/spicerack/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:48.166742 wikimedia_spicerack-8.5.0/spicerack/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia_spicerack-8.5.0/spicerack/toolforge/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia_spicerack-8.5.0/spicerack/toolforge/etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-10-16 12:11:07.000000 wikimedia_spicerack-8.5.0/spicerack/typing.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2180 2024-01-29 13:05:02.000000 wikimedia_spicerack-8.5.0/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:48.182194 wikimedia_spicerack-8.5.0/utils/
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia_spicerack-8.5.0/utils/check-style.sh
+-rwxr-xr-x   0 riccardo   (501) staff       (20)      444 2024-04-15 10:22:42.000000 wikimedia_spicerack-8.5.0/utils/format-code.sh
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2024-04-15 11:13:48.223934 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     3259 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)    10144 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/entry_points.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      630 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       10 2024-04-15 11:13:46.000000 wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/top_level.txt
```

### Comparing `wikimedia-spicerack-8.4.1/.mailmap` & `wikimedia_spicerack-8.5.0/.mailmap`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/CHANGELOG.rst` & `wikimedia_spicerack-8.5.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,45 @@
 Spicerack Changelog
 -------------------
 
+`v8.5.0`_ (2024-04-15)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Minor improvements
+""""""""""""""""""
+
+* netbox: add functions to get and set the device name.
+* elasticsearch: remove the dependency from elasticsearch-curator making the calls directly via the elasticsearch
+  library (`T345337`_ and `T361647`_).
+* alertmanager: add multi-instance and authentication support (`T360932`_):
+
+  * Add support for multiple alertmanager instances based on a configuration file. One of those instances can be
+    marked as ``default`` which is used when the call to the ``Spicerack.alertmanager()`` or
+    ``Spicerack.alertmanager_hosts()`` API is used without specifying a specific instance or some other API (like
+    ``Service.downtime()``) that does not support multiple instances is used.
+  * Add support for per-instance HTTP basic authentication. The metricsinfra Alertmanager instance will be behind
+    HTTP basic authentication to avoid exposing the read-write API to the entire wikiprod network (via the HTTP
+    proxies). This patch adds support for configuring a username and a password to use on a specific Alertmanager
+    instance.
+
+Bug fixes
+"""""""""
+
+* puppet: make ``PuppetServer.destroy()`` have the same behaviour of ``PuppetMaster.destroy()`` and do not raise an
+  exception if the host certificate is already missing (`T360293`_).
+
+Miscellanea
+"""""""""""
+
+* setup.py: remove dependency elasticsearch-curator not needed anymore and remove upper bound for black linter that
+  was there for incompatibilities with elasticsearch-curator.
+* k8s: Remove use of ``@staticmethod`` in tests.
+* tests: fix typos in tests that were erroneously calling mock methods with the wrong names.
+* utils: remove ``--apply`` from isort's call in format-code, now the default in v5.
+
 `v8.4.1`_ (2024-03-06)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Minor improvements
 """"""""""""""""""
 
 * k8s: add getter for the Batch API.
@@ -2788,16 +2823,20 @@
 .. _`T319401`: https://phabricator.wikimedia.org/T319401
 .. _`T320696`: https://phabricator.wikimedia.org/T320696
 .. _`T325168`: https://phabricator.wikimedia.org/T325168
 .. _`T329773`: https://phabricator.wikimedia.org/T329773
 .. _`T330318`: https://phabricator.wikimedia.org/T330318
 .. _`T335855`: https://phabricator.wikimedia.org/T335855
 .. _`T341973`: https://phabricator.wikimedia.org/T341973
+.. _`T345337`: https://phabricator.wikimedia.org/T345337
 .. _`T346134`: https://phabricator.wikimedia.org/T346134
+.. _`T361647`: https://phabricator.wikimedia.org/T361647
 .. _`T347490`: https://phabricator.wikimedia.org/T347490
+.. _`T360293`: https://phabricator.wikimedia.org/T360293
+.. _`T360932`: https://phabricator.wikimedia.org/T360932
 
 .. _`v0.0.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.1
 .. _`v0.0.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.2
 .. _`v0.0.3`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.3
 .. _`v0.0.4`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.4
 .. _`v0.0.5`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.5
 .. _`v0.0.6`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.6
@@ -2907,7 +2946,8 @@
 .. _`v8.0.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.0.2
 .. _`v8.0.3`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.0.3
 .. _`v8.1.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.1.0
 .. _`v8.2.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.2.0
 .. _`v8.3.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.3.0
 .. _`v8.4.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.4.0
 .. _`v8.4.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.4.1
+.. _`v8.5.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v8.5.0
```

### Comparing `wikimedia-spicerack-8.4.1/LICENSE` & `wikimedia_spicerack-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/PKG-INFO` & `wikimedia_spicerack-8.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 8.4.1
+Version: 8.5.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
@@ -26,15 +26,14 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: conftool>=1.0.1
 Requires-Dist: cumin>=3.0.2
 Requires-Dist: dnspython~=2.0.0
 Requires-Dist: elasticsearch<7.15.0,>=5.0.0
-Requires-Dist: elasticsearch-curator~=5.0
 Requires-Dist: gitpython>=3.1.14
 Requires-Dist: kafka-python>=2.0.1
 Requires-Dist: kubernetes==12.0.*
 Requires-Dist: packaging
 Requires-Dist: pymysql>=0.9.3
 Requires-Dist: pynetbox~=6.6
 Requires-Dist: python-etcd~=0.4.5
@@ -55,15 +54,15 @@
 Requires-Dist: sphinx-autodoc-typehints>=1.9.0; extra == "tests"
 Requires-Dist: Sphinx>=3.4.3; extra == "tests"
 Requires-Dist: types-PyMySQL; extra == "tests"
 Requires-Dist: types-redis; extra == "tests"
 Requires-Dist: types-requests; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Provides-Extra: format
-Requires-Dist: black<=21.12b0; extra == "format"
+Requires-Dist: black; extra == "format"
 Requires-Dist: isort; extra == "format"
 Provides-Extra: prospector
 Requires-Dist: prospector[with_everything]>=1.1.7; extra == "prospector"
 Requires-Dist: pytest>=6.0.2; extra == "prospector"
 Requires-Dist: requests-mock>=1.7.0; extra == "prospector"
 
 Spicerack - Automation framework for the WMF production infrastructure
```

### Comparing `wikimedia-spicerack-8.4.1/doc/Makefile` & `wikimedia_spicerack-8.5.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/examples/config.yaml` & `wikimedia_spicerack-8.5.0/doc/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/source/api/index.rst` & `wikimedia_spicerack-8.5.0/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/source/conf.py` & `wikimedia_spicerack-8.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/source/configuration.rst` & `wikimedia_spicerack-8.5.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/source/development.rst` & `wikimedia_spicerack-8.5.0/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/source/installation.rst` & `wikimedia_spicerack-8.5.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/doc/source/introduction.rst` & `wikimedia_spicerack-8.5.0/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/prospector.yaml` & `wikimedia_spicerack-8.5.0/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/setup.cfg` & `wikimedia_spicerack-8.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/setup.py` & `wikimedia_spicerack-8.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 INSTALL_REQUIRES = [
     "conftool>=1.0.1",
     "cumin>=3.0.2",
     "dnspython~=2.0.0",
     "elasticsearch>=5.0.0,<7.15.0",
-    "elasticsearch-curator~=5.0",
     "gitpython>=3.1.14",
     "kafka-python>=2.0.1",
     "kubernetes==12.0.*",  # frozen to the version available on debian bullseye
     "packaging",
     "pymysql>=0.9.3",
     "pynetbox~=6.6",
     "python-etcd~=0.4.5",
@@ -45,15 +44,15 @@
         "Sphinx>=3.4.3",
         "types-PyMySQL",
         "types-redis",
         "types-requests",
         "types-setuptools",
     ],
     "format": [
-        "black<=21.12b0",  # this is needed so that it doesn't confict with curator
+        "black",
         "isort",
     ],
     "prospector": [
         "prospector[with_everything]>=1.1.7",
         "pytest>=6.0.2",
         "requests-mock>=1.7.0",
     ],
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/__init__.py` & `wikimedia_spicerack-8.5.0/spicerack/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os import getpid
 from pathlib import Path
 from socket import gethostname
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 from git import Repo
 from pkg_resources import DistributionNotFound, get_distribution
+from requests.auth import HTTPBasicAuth
 from wmflib import requests
 from wmflib.actions import ActionsDict
 from wmflib.config import load_ini_config, load_yaml_config
 from wmflib.dns import Dns
 from wmflib.interactive import get_username
 from wmflib.phabricator import Phabricator, create_phabricator
 from wmflib.prometheus import Prometheus, Thanos
@@ -670,38 +671,65 @@
             raise SpicerackError(f"Host {hostname} is not a Physical server, Redfish is not supported.")
 
         netbox_ip = netbox.api.ipam.ip_addresses.get(device=hostname, interface=MANAGEMENT_IFACE_NAME)
 
         # TODO: generalize when support for additional vendors will be added.
         return RedfishDell(hostname, ip_interface(netbox_ip), username, password, dry_run=self._dry_run)
 
-    def alertmanager_hosts(self, target_hosts: TypeHosts, *, verbatim_hosts: bool = False) -> AlertmanagerHosts:
+    def alertmanager_hosts(
+        self, target_hosts: TypeHosts, *, instance_name: str = "", verbatim_hosts: bool = False
+    ) -> AlertmanagerHosts:
         """Get an AlertmanagerHosts instance.
 
         Note:
             To interact with both Icinga and Alertmanager alerts, use
             :py:meth:`spicerack.Spicerack.alerting_hosts` instead.
 
         Arguments:
             target_hosts: the target hosts either as a NodeSet instance or a sequence of strings.
+            instance_name: the Alertmanager instance defined in the alertmanager/config.yaml config file to interact
+                with
             verbatim_hosts: if :py:data:`True` use the hosts passed verbatim as is, if instead :py:data:`False`, the
                 default, consider the given target hosts as FQDNs and extract their hostnames to be used in Icinga.
 
         """
-        return AlertmanagerHosts(target_hosts, verbatim_hosts=verbatim_hosts, dry_run=self._dry_run)
+        return self.alertmanager(instance_name=instance_name).hosts(target_hosts, verbatim_hosts=verbatim_hosts)
 
-    def alertmanager(self) -> Alertmanager:
+    def alertmanager(self, instance_name: str = "") -> Alertmanager:
         """Get an Alertmanager instance.
 
+        Arguments:
+            instance_name: the Alertmanager instance defined in the alertmanager/config.yaml config file to interact
+                with
         Note:
             To interact with Alertmanager alerts attached to an ``instance`` use
             :py:meth:`spicerack.Spicerack.alertmanager_hosts` instead.
 
         """
-        return Alertmanager(dry_run=self._dry_run)
+        configuration = load_yaml_config(self._spicerack_config_dir / "alertmanager" / "config.yaml")
+        if not instance_name:
+            instance_name = configuration.get("default_instance", "")
+        if not instance_name:
+            raise SpicerackError("An alertmanager instance name must be specified when no default is set in config")
+
+        instance = configuration.get("instances", {}).get(instance_name)
+        if not instance:
+            raise SpicerackError(f"No such alertmanager instance '{instance_name}' found in config")
+
+        http_authentication = None
+        if "http_username" in instance and "http_password" in instance:
+            http_authentication = HTTPBasicAuth(username=instance["http_username"], password=instance["http_password"])
+        http_proxies = self.requests_proxies if instance.get("http_use_proxy") else None
+
+        return Alertmanager(
+            alertmanager_urls=instance.get("urls", []),
+            http_authentication=http_authentication,
+            http_proxies=http_proxies,
+            dry_run=self._dry_run,
+        )
 
     def alerting_hosts(self, target_hosts: TypeHosts, *, verbatim_hosts: bool = False) -> AlertingHosts:
         """Get an AlertingHosts instance.
 
         Arguments:
             target_hosts: the target hosts either as a NodeSet instance or a sequence of strings.
             verbatim_hosts: if :py:data:`True` use the hosts passed verbatim as is, if instead :py:data:`False`, the
@@ -714,15 +742,19 @@
         )
 
     def service_catalog(self) -> Catalog:
         """Get a Catalog instance that reflects Puppet's service::catalog hieradata variable."""
         if self._service_catalog is None:
             config = load_yaml_config(self._spicerack_config_dir / "service" / "service.yaml")
             self._service_catalog = Catalog(
-                config, confctl=self.confctl("discovery"), authdns_servers=self.authdns_servers, dry_run=self._dry_run
+                config,
+                alertmanager=self.alertmanager(),
+                confctl=self.confctl("discovery"),
+                authdns_servers=self.authdns_servers,
+                dry_run=self._dry_run,
             )
 
         return self._service_catalog
 
     def peeringdb(self, *, ttl: int = 86400) -> PeeringDB:
         """Get a PeeringDB instance to interact with the PeeringDB API.
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/_cookbook.py` & `wikimedia_spicerack-8.5.0/spicerack/_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/_log.py` & `wikimedia_spicerack-8.5.0/spicerack/_log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/_menu.py` & `wikimedia_spicerack-8.5.0/spicerack/_menu.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/_module_api.py` & `wikimedia_spicerack-8.5.0/spicerack/_module_api.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/administrative.py` & `wikimedia_spicerack-8.5.0/spicerack/administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/alerting.py` & `wikimedia_spicerack-8.5.0/spicerack/alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/alertmanager.py` & `wikimedia_spicerack-8.5.0/spicerack/alertmanager.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,60 +4,75 @@
 from collections.abc import Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from datetime import datetime, timedelta, timezone
 from typing import Optional, Union
 
 from cumin import NodeSet, nodeset_fromlist
 from requests import Response
+from requests.auth import AuthBase
 from requests.exceptions import RequestException
 from wmflib.requests import DEFAULT_RETRY_STATUS_CODES, http_session
 
 from spicerack.administrative import Reason
 from spicerack.exceptions import SpicerackError
 from spicerack.typing import TypeHosts
 
 logger = logging.getLogger(__name__)
 MatchersType = Sequence[dict[str, Union[str, int, float, bool]]]
 PORT_REGEX: str = r"(\..+)?(:[0-9]+)?"
 """The regular expression used to match FQDNs and port numbers in the instance labels."""
-ALERTMANAGER_URLS: tuple[str, str] = (
-    "http://alertmanager-eqiad.wikimedia.org",
-    "http://alertmanager-codfw.wikimedia.org",
-)
-"""All the alertmanager instances to contact."""
 
 
 class Alertmanager:
     """Operate on Alertmanager via its APIs."""
 
     def __init__(
         self,
         *,
+        alertmanager_urls: Sequence[str],
+        http_authentication: Optional[AuthBase] = None,
+        http_proxies: Optional[dict[str, str]] = None,
         dry_run: bool = True,
     ) -> None:
         """Initialize the instance.
 
         When using Alertmanager in high availability (cluster) make sure to pass all hosts in your cluster as
         `alertmanager_urls`.
 
         Arguments:
+            alertmanager_urls: list of Alertmanager instances to connect to.
+            http_authentication: Requests authentication configuration to use to connect to the Alertmanager instances.
+            http_proxies: HTTP proxies in requests format to use to connect to the Alertmanager instances.
             dry_run: whether this is a DRY-RUN.
 
+        Raises:
+            spicerack.alertmanager.AlertmanagerError: if `alertmanager_urls` is empty.
+
         """
+        if not alertmanager_urls:
+            raise AlertmanagerError("At least one alertmanager URL is required.")
+
         # Alertmanager API returns HTTP 500 (Internal Server Error) on some requests with a valid JSON response
         # For example when trying to delete a silence that doesn't exist or has already been deleted or is expired
         # Do not retry on 500 and accept it's first response.
         self._http_session = http_session(
             ".".join((self.__module__, self.__class__.__name__)),
             timeout=2,
             retry_codes=tuple(i for i in DEFAULT_RETRY_STATUS_CODES if i != 500),
         )
-        self._alertmanager_urls = ALERTMANAGER_URLS
+        self._alertmanager_urls = alertmanager_urls
         self._dry_run = dry_run
 
+        self._http_authentication = http_authentication
+        if http_authentication:
+            self._http_session.auth = http_authentication
+        self._http_proxies = http_proxies
+        if http_proxies:
+            self._http_session.proxies = http_proxies
+
     def _api_request(self, method: str, path: str, json: Optional[Mapping] = None) -> Response:
         """Perform an Alertmanager API request on multiple endpoints and return the requests response object.
 
         The request is performed on all configured alertmanager endpoints and returns at the first successful response.
 
         Arguments:
             method: the HTTP method to use for the request.
@@ -179,39 +194,77 @@
                 and "silence" in e.response.json()
                 and "already expired" in e.response.json()
             ):
                 logger.warning("Silence ID %s has been already deleted or is expired", downtime_id)
             else:
                 raise
 
+    def hosts(
+        self,
+        target_hosts: TypeHosts,
+        *,
+        verbatim_hosts: bool = False,
+    ) -> "AlertmanagerHosts":
+        """Returns an AlertmanagerHosts instance for the specified hosts.
+
+        Arguments:
+            target_hosts: the target hosts either as a NodeSet instance or a sequence of strings.
+            verbatim_hosts: if :py:data:`True` use the hosts passed verbatim as is, if instead
+                :py:data:`False`, the default, consider the given target hosts as FQDNs and extract their hostnames to
+                be used in Alertmanager.
+
+        Raises:
+            spicerack.alertmanager.AlertmanagerError: if no target hosts are provided.
+
+        """
+        return AlertmanagerHosts(
+            target_hosts=target_hosts,
+            verbatim_hosts=verbatim_hosts,
+            alertmanager_urls=self._alertmanager_urls,
+            http_authentication=self._http_authentication,
+            http_proxies=self._http_proxies,
+            dry_run=self._dry_run,
+        )
+
 
 class AlertmanagerHosts(Alertmanager):
     """Operate on Alertmanager for a list of hosts via its APIs."""
 
     def __init__(
         self,
         target_hosts: TypeHosts,
         *,
         verbatim_hosts: bool = False,
+        alertmanager_urls: Sequence[str],
+        http_authentication: Optional[AuthBase] = None,
+        http_proxies: Optional[dict[str, str]] = None,
         dry_run: bool = True,
     ) -> None:
         """Initialize the instance.
 
         Arguments:
             target_hosts: the target hosts either as a NodeSet instance or a sequence of strings.
             verbatim_hosts: if :py:data:`True` use the hosts passed verbatim as is, if instead
                 :py:data:`False`, the default, consider the given target hosts as FQDNs and extract their hostnames to
                 be used in Alertmanager.
+            alertmanager_urls: list of Alertmanager instances to connect to.
+            http_authentication: Requests authentication configuration to use to connect to the Alertmanager instances.
+            http_proxies: HTTP proxies in requests format to use to connect to the Alertmanager instances.
             dry_run: whether this is a DRY-RUN.
 
         Raises:
             spicerack.alertmanager.AlertmanagerError: if no target hosts are provided.
 
         """
-        super().__init__(dry_run=dry_run)
+        super().__init__(
+            alertmanager_urls=alertmanager_urls,
+            http_authentication=http_authentication,
+            http_proxies=http_proxies,
+            dry_run=dry_run,
+        )
         if not verbatim_hosts:
             target_hosts = [target_host.split(".")[0] for target_host in target_hosts]
 
         if isinstance(target_hosts, NodeSet):
             self._target_hosts = target_hosts
         else:
             self._target_hosts = nodeset_fromlist(target_hosts)
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/apt.py` & `wikimedia_spicerack-8.5.0/spicerack/apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/confctl.py` & `wikimedia_spicerack-8.5.0/spicerack/confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/cookbook.py` & `wikimedia_spicerack-8.5.0/spicerack/cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/debmonitor.py` & `wikimedia_spicerack-8.5.0/spicerack/debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/decorators.py` & `wikimedia_spicerack-8.5.0/spicerack/decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/dhcp.py` & `wikimedia_spicerack-8.5.0/spicerack/dhcp.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/dnsdisc.py` & `wikimedia_spicerack-8.5.0/spicerack/dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/elasticsearch_cluster.py` & `wikimedia_spicerack-8.5.0/spicerack/elasticsearch_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from collections.abc import Iterable, Iterator, Sequence
 from contextlib import ExitStack, contextmanager
 from datetime import datetime, timedelta
 from math import floor
 from random import shuffle
 from typing import Optional
 
-import curator
 from elasticsearch import ConflictError, Elasticsearch, RequestError, TransportError
 from urllib3.exceptions import HTTPError
 from wmflib.prometheus import Prometheus
 
 from spicerack.administrative import Reason
 from spicerack.decorators import retry
 from spicerack.exceptions import SpicerackCheckError, SpicerackError
@@ -452,48 +451,24 @@
             yield
         finally:
             self._start_replication()
 
     def _stop_replication(self) -> None:
         """Stops cluster replication."""
         logger.info("stop replication - %s", self)
-        self._do_cluster_routing(
-            curator.ClusterRouting(
-                self._elasticsearch,
-                routing_type="allocation",
-                setting="enable",
-                value="primaries",
-                wait_for_completion=False,
+        if not self._dry_run:
+            self._elasticsearch.cluster.put_settings(
+                body={"persistent": {"cluster.routing.allocation.enable": "primaries"}}
             )
-        )
 
     def _start_replication(self) -> None:
         """Starts cluster replication."""
         logger.info("start replication - %s", self)
-        self._do_cluster_routing(
-            curator.ClusterRouting(
-                self._elasticsearch,
-                routing_type="allocation",
-                setting="enable",
-                value="all",
-                wait_for_completion=False,
-            )
-        )
-
-    def _do_cluster_routing(self, cluster_routing: curator.ClusterRouting) -> None:
-        """Performs cluster routing of shards.
-
-        Arguments:
-            cluster_routing: Curator's cluster routing object.
-
-        """
-        if self._dry_run:
-            cluster_routing.do_dry_run()
-        else:
-            cluster_routing.do_action()
+        if not self._dry_run:
+            self._elasticsearch.cluster.put_settings(body={"persistent": {"cluster.routing.allocation.enable": "all"}})
 
     def check_green(self) -> None:
         """Cluster health status.
 
         Raises:
             spicerack.elasticsearch_cluster.ElasticsearchClusterCheckError: This is raised when request times and
             cluster is not green.
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/exceptions.py` & `wikimedia_spicerack-8.5.0/spicerack/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/ganeti.py` & `wikimedia_spicerack-8.5.0/spicerack/ganeti.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/icinga.py` & `wikimedia_spicerack-8.5.0/spicerack/icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/interactive.py` & `wikimedia_spicerack-8.5.0/spicerack/interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/ipmi.py` & `wikimedia_spicerack-8.5.0/spicerack/ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/k8s.py` & `wikimedia_spicerack-8.5.0/spicerack/k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/kafka.py` & `wikimedia_spicerack-8.5.0/spicerack/kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/locking.py` & `wikimedia_spicerack-8.5.0/spicerack/locking.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/mediawiki.py` & `wikimedia_spicerack-8.5.0/spicerack/mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/mysql.py` & `wikimedia_spicerack-8.5.0/spicerack/mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/mysql_legacy.py` & `wikimedia_spicerack-8.5.0/spicerack/mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/netbox.py` & `wikimedia_spicerack-8.5.0/spicerack/netbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -216,14 +216,64 @@
         Returns:
             :py:data:`True` if the server is virtual, :py:data:`False` if physical.
 
         """
         return not hasattr(self._server, "rack")
 
     @property
+    def name(self) -> str:
+        """Get the server name. Set the server name, primary IP DNS name, management IP DNS name.
+
+        Modifying its value can be done only on physical devices.
+
+        Arguments:
+            new: the new name for the host.
+
+        Raises:
+            spicerack.netbox.NetboxError: if trying to set it on a virtual device or there is an issue renaming.
+
+        """
+        return self._server.name
+
+    @name.setter
+    def name(self, new: str) -> None:
+        """Get and set the server name. See the getter docstring for info.
+
+        Arguments:
+            new: the new name for the host.
+
+        Raises:
+            spicerack.netbox.NetboxError: if trying to set it on a virtual device or there is an issue renaming.
+
+        """
+        if self.virtual:
+            raise NetboxError(
+                f"Server {self._server.name} is a virtual machine, chaging the name is only for physical servers."
+            )
+
+        current = self._server.name
+        if current == new:
+            logger.debug("Current name is already %s", current)
+            return
+        if self._dry_run:
+            logger.info("Skipping Netbox name change from %s to %s in DRY-RUN.", current, new)
+            return
+
+        self._server.name = new
+        if self._server.save():
+            logger.debug("Updated Netbox name from %s to %s", current, new)
+        else:
+            # See https://github.com/netbox-community/pynetbox/issues/586
+            raise NetboxError(f"Name change for {current} didn't get applied by Netbox.")
+
+        # Update the FQDNs
+        self.fqdn = new + "." + self.fqdn.split(".", 1)[1]
+        self.mgmt_fqdn = new + "." + self.mgmt_fqdn.split(".", 1)[1]
+
+    @property
     def status(self) -> str:
         """Get and set the server status.
 
         Modifying its value can be done only on physical devices and only between allowed transitions.
 
         The allowed transitions are defined in :py:data:`spicerack.netbox.Netbox.allowed_status_transitions`.
 
@@ -437,31 +487,72 @@
         netbox_switch_iface.save()
         logger.debug(
             "Updated Netbox switchport access vlan from %s to %s for device %s", current, value, self._server.name
         )
 
     @property
     def fqdn(self) -> str:
-        """Return the FQDN of the device.
+        """Get and set the device primary IPs FQDN if one is already set.
+
+        Notes:
+            If the FQDN for any of the primary IPs is not set it will not be updated.
+            This is to prevent setting a IPv6 AAAA record by accident.
+
+        Arguments:
+            value: the new FQDN for the host.
 
         Raises:
             spicerack.netbox.NetboxError: if the server has no FQDN defined in Netbox.
 
         """
         # Until https://phabricator.wikimedia.org/T253173 is fixed we can't use the primary_ip attribute
         for attr_name in ("primary_ip4", "primary_ip6"):
             address = getattr(self._server, attr_name)
             if address is not None and address.dns_name:
                 return address.dns_name
 
         raise NetboxError(f"Server {self._server.name} does not have any primary IP with a DNS name set.")
 
+    @fqdn.setter
+    def fqdn(self, value: str) -> None:
+        """Get and set the device primary IPs FQDN if one is already set.
+
+        Notes:
+            If the FQDN for any of the primary IPs is not set it will not be updated.
+            This is to prevent setting a IPv6 AAAA record by accident.
+
+        Arguments:
+            value: the new FQDN for the host.
+
+        Raises:
+            spicerack.netbox.NetboxError: if trying to set it on a virtual device
+                                          or if the server has no FQDN defined in Netbox.
+
+        """
+        if self.virtual:
+            raise NetboxError(
+                f"Server {self._server.name} is a virtual machine, changing the FQDN is only for physical servers."
+            )
+        for attr_name in ("primary_ip4", "primary_ip6"):
+            address = getattr(self._server, attr_name)
+            if address is not None and address.dns_name:
+                if address.dns_name == value:
+                    logger.debug("Current dns_name is already %s", value)
+                    continue
+                address.dns_name = value
+                if not address.save():
+                    raise NetboxError(f"Spicerack was not able to update the {attr_name} FQDN for {self._server.name}.")
+                logger.debug("Updated %s dns_name to %s", attr_name, value)
+
     @property
     def mgmt_fqdn(self) -> str:
-        """Return the management FQDN of the device.
+        """Get and set the management FQDN of the device.
+
+        Arguments:
+            value: the new FQDN for the host.
 
         Raises:
             spicerack.netbox.NetboxError: for virtual servers or the server has no management FQDN defined in Netbox.
 
         """
         if self.virtual:
             raise NetboxError(f"Server {self._server.name} is a virtual machine, does not have a management address.")
@@ -474,14 +565,43 @@
         #       API call to Netbox or the Netbox API become more efficient.
         if address is not None and address.dns_name:
             self._cached_mgmt_fqdn = address.dns_name
             return self._cached_mgmt_fqdn
 
         raise NetboxError(f"Server {self._server.name} has no management interface with a DNS name set.")
 
+    @mgmt_fqdn.setter
+    def mgmt_fqdn(self, value: str) -> None:
+        """Get and set the management FQDN of the device.
+
+        Arguments:
+            value: the new FQDN for the host.
+
+        Raises:
+            spicerack.netbox.NetboxError: if trying to set it on a virtual device or can't find the management IP.
+
+        """
+        if self.virtual:
+            raise NetboxError(
+                f"Server {self._server.name} is a virtual machine, "
+                "changing the mgmt FQDN is only for physical servers."
+            )
+        address = self._api.ipam.ip_addresses.get(device=self._server.name, interface=MANAGEMENT_IFACE_NAME)
+        # TODO: see the getter TODO
+        if address is not None:
+            if address.dns_name == value:
+                self._cached_mgmt_fqdn = value
+                logger.debug("Current dns_name is already %s", value)
+                return
+            address.dns_name = value
+            if not address.save():
+                raise NetboxError(f"Spicerack was not able to update the mgmt_fqdn for {self._server.name}.")
+            self._cached_mgmt_fqdn = value
+            logger.debug("Updated mgmt FQDN to %s", value)
+
     @property
     def asset_tag_fqdn(self) -> str:
         """Return the management FQDN for the asset tag of the device.
 
         Raises:
             spicerack.netbox.NetboxError: for virtual servers or the server has no management FQDN defined in Netbox.
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/peeringdb.py` & `wikimedia_spicerack-8.5.0/spicerack/peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/puppet.py` & `wikimedia_spicerack-8.5.0/spicerack/puppet.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,21 +409,29 @@
         """
         commands = [f"puppet node {action} {hostname}" for action in ("clean", "deactivate")]
         self.server_host.run_sync(*commands, print_progress_bars=False)
 
     def destroy(self, hostname: str) -> None:
         """Remove the certificate for the given hostname.
 
-        If there is no certificate to remove it doesn't raise exception as the Puppet CA just outputs
-        'Nothing was deleted'.
+        If there is no certificate to remove it doesn't raise exception.
 
         Arguments:
             hostname: the FQDN of the host for which to remove the certificate.
 
+        Raises:
+            spicerack.remote.RemoteExecutionError: if unable to destroy the certificate.
+
         """
+        try:
+            self.get_certificate_metadata(hostname)
+        except PuppetServerCheckError:
+            logger.info("The certificate for %s does not exist, nothing to do.", hostname)
+            return
+
         self.server_host.run_sync(f"puppetserver ca clean --certname {hostname}", print_progress_bars=False)
 
     def verify(self, hostname: str) -> None:
         """Verify that there is a valid certificate signed by the Puppet CA for the given hostname.
 
         Arguments:
             hostname: the FQDN of the host for which to verify the certificate.
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/redfish.py` & `wikimedia_spicerack-8.5.0/spicerack/redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/redis_cluster.py` & `wikimedia_spicerack-8.5.0/spicerack/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/remote.py` & `wikimedia_spicerack-8.5.0/spicerack/remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/reposync.py` & `wikimedia_spicerack-8.5.0/spicerack/reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/service.py` & `wikimedia_spicerack-8.5.0/spicerack/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from copy import deepcopy
 from dataclasses import dataclass, field
 from datetime import timedelta
 from ipaddress import IPv4Address, IPv6Address, ip_address
 from typing import Optional, Union
 
 from spicerack.administrative import Reason
-from spicerack.alertmanager import AlertmanagerHosts, MatchersType
+from spicerack.alertmanager import Alertmanager, AlertmanagerHosts, MatchersType
 from spicerack.confctl import ConftoolEntity
 from spicerack.decorators import retry, set_tries
 from spicerack.dnsdisc import Discovery, DiscoveryError
 from spicerack.exceptions import SpicerackError
 
 logger = logging.getLogger(__name__)
 
@@ -528,27 +528,35 @@
         See how many services are configured::
 
             >>> num_services = len(catalog)
 
     """
 
     def __init__(
-        self, catalog: dict, *, confctl: ConftoolEntity, authdns_servers: dict[str, str], dry_run: bool = True
+        self,
+        catalog: dict,
+        *,
+        alertmanager: Alertmanager,
+        confctl: ConftoolEntity,
+        authdns_servers: dict[str, str],
+        dry_run: bool = True,
     ):
         """Initialize the instance.
 
         Args:
             catalog: the content of Puppet's ``hieradata/common/service.yaml``.
+            alertmanager: the alertmanager instance to interact with.
             confctl: the instance to interact with confctl.
             authdns_servers: a dictionary where keys are the hostnames and values are the IPs of the authoritative
                 nameservers to be used.
             dry_run: whether this is a DRY-RUN.
 
         """
         self._catalog = catalog
+        self._alertmanager = alertmanager
         self._confctl = confctl
         self._authdns_servers = authdns_servers
         self._dry_run = dry_run
 
     def __iter__(self) -> Iterator[Service]:
         """Iterate over the catalog services."""
         return (self.get(name) for name in self._catalog)
@@ -579,17 +587,15 @@
         """
         if name not in self._catalog:
             raise ServiceNotFoundError(f"Service {name} was not found in service::catalog")
 
         params = deepcopy(self._catalog[name])
         params["name"] = name
         params["ip"] = ServiceIPs(data=params["ip"])
-        params["_alertmanager"] = AlertmanagerHosts(
-            [f"{name}:{params['port']}"], verbatim_hosts=True, dry_run=self._dry_run
-        )
+        params["_alertmanager"] = self._alertmanager.hosts([f"{name}:{params['port']}"], verbatim_hosts=True)
         params["_dry_run"] = self._dry_run
         if "discovery" in params:
             discovery = []
             for disc in params["discovery"]:
                 instance = Discovery(
                     conftool=self._confctl,
                     authdns_servers=self._authdns_servers,
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/__init__.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/confctl/schema.yaml` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/confctl/schema.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/lock_args.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/lock_args.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/external_modules/spicerack_extender.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/groups_bulk.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/groups_bulk.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/info.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/info.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/instance.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/instance.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/ganeti/nodes_bulk.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/ganeti/nodes_bulk.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_failed_services.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_services.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/peeringdb/asn.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/peeringdb/asn.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/peeringdb/ixlan.json` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/peeringdb/ixlan.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/fixtures/service/service.yaml` & `wikimedia_spicerack-8.5.0/spicerack/tests/fixtures/service/service.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/sphinx_checker.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test__cookbook.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test__cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test__log.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test__log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_administrative.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_alerting.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_alerting.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         self.reason = Reason("test", "user", "host")
 
         self.mocked_icinga_host = mock.MagicMock(spec_set=RemoteHosts)
         self.mocked_icinga_host.__len__.return_value = 1
         set_mocked_icinga_host_output(self.mocked_icinga_host, "/var/lib/icinga/rw/icinga.cmd")
         self.icinga_hosts = icinga.IcingaHosts(self.mocked_icinga_host, self.hosts)
 
-        self.am_hosts = alertmanager.AlertmanagerHosts(self.hosts)
+        self.am_hosts = alertmanager.AlertmanagerHosts(
+            self.hosts, alertmanager_urls=["https://alertmanager-eqiad.wikimedia.example"]
+        )
         self.requests_mock = requests_mock
 
         self.alerting_hosts = alerting.AlertingHosts(self.am_hosts, self.icinga_hosts)
 
     @mock.patch("spicerack.icinga.IcingaHosts.downtime")
     @mock.patch("spicerack.alertmanager.AlertmanagerHosts.downtime", return_value="foo")
     def test_downtime(self, am_dt, icinga_dt):
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_alertmanager.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_alertmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,41 +2,52 @@
 import logging
 from datetime import datetime, timedelta, timezone
 from unittest import mock
 
 import pytest
 import requests
 from cumin import nodeset
+from requests.auth import HTTPBasicAuth
 
 from spicerack import alertmanager
 from spicerack.administrative import Reason
 
+ALERTMANAGER_URLS: tuple[str, str] = (
+    "http://alertmanager-eqiad.wikimedia.example",
+    "http://alertmanager-codfw.wikimedia.example",
+)
+
 
 class TestAlertmanager:
     """Tests for the Alertmanager class."""
 
     @pytest.fixture(autouse=True)
     def setup_method(self, requests_mock):
         """Initialize the test instance."""
         # pylint: disable=attribute-defined-outside-init
         self.matchers = [
             {"name": "site", "value": "dc1", "isRegex": False},
             {"name": "label1", "value": "value1", "isRegex": False},
         ]
-        self.alertmanager = alertmanager.Alertmanager(dry_run=False)
-        self.am_dry_run = alertmanager.Alertmanager(dry_run=True)
+        self.alertmanager = alertmanager.Alertmanager(alertmanager_urls=ALERTMANAGER_URLS, dry_run=False)
+        self.am_dry_run = alertmanager.Alertmanager(alertmanager_urls=ALERTMANAGER_URLS, dry_run=True)
+        self.am_authenticated = alertmanager.Alertmanager(
+            alertmanager_urls=ALERTMANAGER_URLS,
+            dry_run=False,
+            http_authentication=HTTPBasicAuth("spicerack", "example2"),
+        )
         self.requests_mock = requests_mock
         self.reason = Reason("test", "user", "host")
 
     def test_add_silence_basic(self):
         """It should issue a silence with all the matchers."""
         self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
         response = self.alertmanager.downtime(self.reason, matchers=self.matchers)
         assert response == "foobar"
-        assert self.requests_mock.last_request.hostname == "alertmanager-eqiad.wikimedia.org"
+        assert self.requests_mock.last_request.hostname == "alertmanager-eqiad.wikimedia.example"
         request_json = self.requests_mock.last_request.json()
         assert request_json["matchers"] == self.matchers
         assert request_json["comment"] == "test - user@host"
         assert request_json["createdBy"] == "user@host"
 
     def test_add_silence_no_matchers(self):
         """It should raise an AlertmanagerError if there are no matchers specified."""
@@ -120,30 +131,40 @@
         """It should raise AlertmanagerError when unable to contact the API."""
         self.requests_mock.post("/api/v2/silences", exc=requests.exceptions.ConnectionError)
         with pytest.raises(alertmanager.AlertmanagerError):
             self.alertmanager.downtime(self.reason, matchers=self.matchers)
 
     def test_fallback_on_error(self):
         """It should fallback to the next Alertmanager on error."""
-        ams = alertmanager.ALERTMANAGER_URLS
-        self.requests_mock.post(f"{ams[0]}/api/v2/silences", exc=requests.exceptions.ConnectionError)
-        self.requests_mock.post(f"{ams[1]}/api/v2/silences", json={"silenceID": "foobar"})
+        self.requests_mock.post(f"{ALERTMANAGER_URLS[0]}/api/v2/silences", exc=requests.exceptions.ConnectionError)
+        self.requests_mock.post(f"{ALERTMANAGER_URLS[1]}/api/v2/silences", json={"silenceID": "foobar"})
         assert "foobar" == self.alertmanager.downtime(self.reason, matchers=self.matchers)
-        assert self.requests_mock.last_request.hostname == "alertmanager-codfw.wikimedia.org"
+        assert self.requests_mock.last_request.hostname == "alertmanager-codfw.wikimedia.example"
+
+    def test_uses_http_authentication(self):
+        """It should use the given HTTP authentication configuration."""
+        self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
+        assert "foobar" == self.am_authenticated.downtime(self.reason, matchers=self.matchers)
+        # c3BpY2VyYWNrOmV4YW1wbGUy == base64(spicerack:example2)
+        assert self.requests_mock.last_request.headers["Authorization"] == "Basic c3BpY2VyYWNrOmV4YW1wbGUy"
 
 
 class TestAlertmanagerHosts:
     """Tests for the AlertmanagerHosts class."""
 
     @pytest.fixture(autouse=True)
     def setup_method(self, requests_mock):
         """Initialize the test instance."""
         # pylint: disable=attribute-defined-outside-init
-        self.am_hosts = alertmanager.AlertmanagerHosts(["host1", "host2"], dry_run=False)
-        self.am_hosts_dry_run = alertmanager.AlertmanagerHosts(["host1", "host2"], dry_run=True)
+        self.am_hosts = alertmanager.AlertmanagerHosts(
+            ["host1", "host2"], alertmanager_urls=ALERTMANAGER_URLS, dry_run=False
+        )
+        self.am_hosts_dry_run = alertmanager.AlertmanagerHosts(
+            ["host1", "host2"], alertmanager_urls=ALERTMANAGER_URLS, dry_run=True
+        )
         self.requests_mock = requests_mock
         self.reason = Reason("test", "user", "host")
 
     @pytest.mark.parametrize(
         "hosts, regex",
         (
             (["host1", "host2"], r"^(host1|host2)(\..+)?(:[0-9]+)?$"),
@@ -151,18 +172,18 @@
             (["host1.example.com:1234", "host2"], r"^(host1|host2)(\..+)?(:[0-9]+)?$"),
             (["host1:1234", "host2.example.com:5678"], r"^(host1:1234|host2(\..+)?(:[0-9]+)?)$"),
         ),
     )
     def test_add_silence_basic(self, hosts, regex):
         """It should issue a silence with all defaults."""
         self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
-        am_hosts = alertmanager.AlertmanagerHosts(hosts, dry_run=False)
+        am_hosts = alertmanager.AlertmanagerHosts(hosts, alertmanager_urls=ALERTMANAGER_URLS, dry_run=False)
         response = am_hosts.downtime(self.reason)
         assert response == "foobar"
-        assert self.requests_mock.last_request.hostname == "alertmanager-eqiad.wikimedia.org"
+        assert self.requests_mock.last_request.hostname == "alertmanager-eqiad.wikimedia.example"
         request_json = self.requests_mock.last_request.json()
         assert request_json["matchers"] == [
             {"name": "instance", "value": regex, "isRegex": True},
         ]
         assert request_json["comment"] == "test - user@host"
         assert request_json["createdBy"] == "user@host"
 
@@ -180,15 +201,17 @@
         """It should raise an AlertmanagerError if any of the matchers target the instance property."""
         with pytest.raises(alertmanager.AlertmanagerError, match="Matchers cannot target the instance property"):
             self.am_hosts.downtime(self.reason, matchers=({"name": "instance", "value": "host1001", "isRegex": False},))
 
     def test_add_silence_port_included(self):
         """It should issue a silence with the specific port and not any port in the matcher."""
         self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
-        am_hosts = alertmanager.AlertmanagerHosts(["host1:1234", "host2:5678"], dry_run=False)
+        am_hosts = alertmanager.AlertmanagerHosts(
+            ["host1:1234", "host2:5678"], alertmanager_urls=ALERTMANAGER_URLS, dry_run=False
+        )
         am_hosts.downtime(self.reason)
         request_json = self.requests_mock.last_request.json()
         assert request_json["matchers"] == [
             {"name": "instance", "value": r"^(host1:1234|host2:5678)$", "isRegex": True},
         ]
 
     def test_add_silence_duration(self):
@@ -218,40 +241,45 @@
         assert response == ""
         assert self.requests_mock.call_count == 0
 
     def test_verbatim_hosts(self):
         """It should issue silences for verbatim hosts."""
         self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
         am_hosts = alertmanager.AlertmanagerHosts(
-            ["host1.foo.bar", "host2.bar.baz:1234"], verbatim_hosts=True, dry_run=False
+            ["host1.foo.bar", "host2.bar.baz:1234"],
+            verbatim_hosts=True,
+            alertmanager_urls=ALERTMANAGER_URLS,
+            dry_run=False,
         )
         am_hosts.downtime(self.reason)
         request_json = self.requests_mock.last_request.json()
         assert request_json["matchers"] == [
             {
                 "name": "instance",
                 "value": r"^(host1\.foo\.bar(\..+)?(:[0-9]+)?|host2\.bar\.baz:1234)$",
                 "isRegex": True,
             },
         ]
 
     def test_nodeset_hosts(self):
         """It should expand NodeSet hosts."""
         self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
-        am_hosts = alertmanager.AlertmanagerHosts(nodeset("host[1-2]"), verbatim_hosts=True, dry_run=False)
+        am_hosts = alertmanager.AlertmanagerHosts(
+            nodeset("host[1-2]"), verbatim_hosts=True, alertmanager_urls=ALERTMANAGER_URLS, dry_run=False
+        )
         am_hosts.downtime(self.reason)
         request_json = self.requests_mock.last_request.json()
         assert request_json["matchers"] == [
             {"name": "instance", "value": r"^(host1|host2)(\..+)?(:[0-9]+)?$", "isRegex": True},
         ]
 
     def test_empty_target_hosts(self):
         """It should error with empty hosts."""
         with pytest.raises(alertmanager.AlertmanagerError):
-            alertmanager.AlertmanagerHosts([""])
+            alertmanager.AlertmanagerHosts([""], alertmanager_urls=ALERTMANAGER_URLS)
 
     def test_downtimed(self):
         """It should issue a silence and then delete it."""
         self.requests_mock.post("/api/v2/silences", json={"silenceID": "foobar"})
         self.requests_mock.delete("/api/v2/silence/foobar")
         with self.am_hosts.downtimed(self.reason):
             assert self.requests_mock.call_count == 1
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_apt.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_confctl.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_debmonitor.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_decorators.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_dhcp.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_dnsdisc.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_elasticsearch_cluster.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_elasticsearch_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,25 +327,25 @@
     def test_stopped_replication(self):
         """Check that context manager stops replication and then starts replication on each cluster."""
         self.elasticsearch1.cluster.put_settings = mock.Mock(return_value=True)
         self.elasticsearch2.cluster.put_settings = mock.Mock(return_value=True)
         elasticsearch_clusters = self.default_elasticsearch_clusters()
         with elasticsearch_clusters.stopped_replication():
             self.elasticsearch1.cluster.put_settings.assert_called_with(
-                body={"transient": {"cluster.routing.allocation.enable": "primaries"}}
+                body={"persistent": {"cluster.routing.allocation.enable": "primaries"}}
             )
             self.elasticsearch2.cluster.put_settings.assert_called_with(
-                body={"transient": {"cluster.routing.allocation.enable": "primaries"}}
+                body={"persistent": {"cluster.routing.allocation.enable": "primaries"}}
             )
 
         self.elasticsearch1.cluster.put_settings.assert_called_with(
-            body={"transient": {"cluster.routing.allocation.enable": "all"}}
+            body={"persistent": {"cluster.routing.allocation.enable": "all"}}
         )
         self.elasticsearch2.cluster.put_settings.assert_called_with(
-            body={"transient": {"cluster.routing.allocation.enable": "all"}}
+            body={"persistent": {"cluster.routing.allocation.enable": "all"}}
         )
 
     def test_frozen_writes_write_to_index(self):
         """Test that elasticsearch write to index is called to freeze writes."""
         self.elasticsearch1.index = mock.Mock(return_value=True)
         self.elasticsearch2.index = mock.Mock(return_value=True)
         self.elasticsearch1.delete = mock.Mock(return_value=True)
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_ganeti.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_ganeti.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_icinga.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_interactive.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_ipmi.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_ipmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,15 +411,15 @@
         )
 
     @mock.patch("spicerack.ipmi.run")
     def test_reset_password_dryrun(self, mocked_run):
         """It should not reset the users password."""
         mocked_run.return_value = CompletedProcess((), 0, stdout=USERLIST_OUTPUT.encode())
         self.ipmi_dry_run.reset_password("root", "a" * 16)
-        mocked_run.called_once_with(IPMITOOL_BASE + ["user", "list", "1"], env=ENV, stdout=PIPE, check=True)
+        mocked_run.assert_called_once_with(IPMITOOL_BASE + ["user", "list", "1"], env=ENV, stdout=PIPE, check=True)
 
     @mock.patch("spicerack.ipmi.run")
     def test_reset_password_fail_command(self, mocked_run):
         """It should fail the password reset command."""
         mocked_run.side_effect = [
             CompletedProcess((), 0, stdout=USERLIST_OUTPUT.encode()),
             CompletedProcess((), 0, stdout=b"Fail password reset\n"),
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_k8s.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,22 +130,20 @@
     @pytest.fixture
     def kube(self):
         """Fixture to get a test object."""
         k = k8s.Kubernetes("group", "cluster", dry_run=False)
         k.api = self._api
         return k
 
-    @staticmethod
-    def test_initialize_api():
+    def test_initialize_api(self):
         """Values are passed to the api correctly."""
         k = k8s.Kubernetes("group", "cluster")
         assert k.api.cluster == "cluster"
 
-    @staticmethod
-    def test_initialize_dry_run(kube):
+    def test_initialize_dry_run(self, kube):
         """Dry run is initialized correctly."""
         assert kube.dry_run is False
         assert k8s.Kubernetes("group", "cluster", dry_run=True).dry_run is True
 
     def test_get_node(self, kube):
         """Getting a node works."""
         list_node = mock.MagicMock()
@@ -251,23 +249,21 @@
 
     def test_bad_init(self):
         """A bad initial object will cause an exception."""
         n = self.node_from_test_case("schedulable")
         with pytest.raises(k8s.KubernetesError):
             k8s.KubernetesNode("fqdn", self._api, init_obj=n)
 
-    @staticmethod
     @pytest.mark.parametrize("label,expected", [("schedulable", True), ("unschedulable", False)])
-    def test_is_schedulable(node, expected):
+    def test_is_schedulable(self, node, expected):
         """Is the node schedulable or not."""
         assert node.is_schedulable() is expected
 
-    @staticmethod
     @pytest.mark.parametrize("label,expected", [("schedulable", "node1"), ("unschedulable", "node2")])
-    def test_name(node, expected):
+    def test_name(self, node, expected):
         """Test fetching the node name."""
         assert node.name == expected
 
     @pytest.mark.parametrize("label,has_calls", [("schedulable", True), ("unschedulable", False)])
     def test_cordon(self, node, has_calls):
         """Cordoning a schedulable node works."""
         patch_expected = self.node_from_test_case("schedulable")
@@ -435,20 +431,19 @@
     def test_drain_api_error(self, node):
         """Draining with an api error will raise an exception."""
         self._coreapi.list_pod_for_all_namespaces.side_effect = kubernetes.client.exceptions.ApiException("test")
         with pytest.raises(k8s.KubernetesApiError):
             node.drain()
         self._coreapi.list_pod_for_all_namespaces.assert_called_with(field_selector="spec.nodeName=node2")
 
-    @staticmethod
     @pytest.mark.parametrize(
         "label,expected",
         [("schedulable", []), ("tainted", [V1Taint(effect="NoExecute", key="dedicated", value="kask")])],
     )
-    def test_taints(node, expected):
+    def test_taints(self, node, expected):
         """Test fetching taints."""
         assert node.taints == expected
 
 
 class TestKubernetesPod(KubeTestBase):
     """Unit testing KubernetesPod."""
 
@@ -461,47 +456,42 @@
             ns = "bar"
         else:
             name = _pod.metadata.name
             ns = _pod.metadata.namespace
 
         return k8s.KubernetesPod(ns, name, self._api, dry_run=False, init_obj=_pod)
 
-    @staticmethod
     @pytest.mark.parametrize("label,expected", [("orphaned", None), ("invalid_ref", None), ("daemonset", "DaemonSet")])
-    def test_controller(pod, expected):
+    def test_controller(self, pod, expected):
         """The output of pod.controller."""
         if expected is None:
             assert pod.controller is None
         else:
             assert pod.controller.kind == expected
 
-    @staticmethod
     @pytest.mark.parametrize("label, expected", [("daemonset", True), ("replicaset", False), ("invalid_ref", False)])
-    def test_is_daemonset(pod, expected):
+    def test_is_daemonset(self, pod, expected):
         """Detecting a daemonset."""
         assert pod.is_daemonset() is expected
 
-    @staticmethod
     @pytest.mark.parametrize("label, expected", [("finished", True), ("replicaset", False), ("invalid_ref", False)])
-    def test_is_terminated(pod, expected):
+    def test_is_terminated(self, pod, expected):
         """Detecting a terminated pod."""
         assert pod.is_terminated() is expected
 
-    @staticmethod
     @pytest.mark.parametrize("label, expected", [("mirror", True), ("orphaned", False)])
-    def test_is_mirror(pod, expected):
+    def test_is_mirror(self, pod, expected):
         """Detecting mirror pods."""
         assert pod.is_mirror() is expected
 
-    @staticmethod
     @pytest.mark.parametrize(
         "label,expected",
         [("daemonset", False), ("replicaset", True), ("orphaned", False), ("finished", True), ("mirror", False)],
     )
-    def test_is_evictable(pod, expected):
+    def test_is_evictable(self, pod, expected):
         """Is the pod evictable."""
         assert pod.is_evictable() is expected
 
     @pytest.mark.parametrize("label", ["no data"])
     def test_refresh(self, pod):
         """The requests to the api for the pod."""
         self._coreapi.read_namespaced_pod.assert_called_with("foo", "bar")
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_kafka.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_locking.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_locking.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_mediawiki.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_mysql.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_mysql_legacy.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_netbox.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_netbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         # pylint: disable=attribute-defined-outside-init
         self.mocked_api = mocked_api
         self.netbox = Netbox(NETBOX_URL, NETBOX_TOKEN, dry_run=False)
         self.netbox_dry_run = Netbox(NETBOX_URL, NETBOX_TOKEN, dry_run=True)
 
     def test_netbox_api(self):
         """An instance of Netbox should instantiate the Netbox API and expose it via the api property."""
-        self.mocked_api.called_once_with(NETBOX_URL, token=NETBOX_TOKEN)
+        call = mock.call(NETBOX_URL, token=NETBOX_TOKEN, threading=True)
+        assert self.mocked_api.mock_calls == [call, call]
         assert self.netbox.api == self.mocked_api()
 
     def test_get_server_fail_device(self):
         """It should raise a NetboxAPIError if unable to get the device data from Netbox."""
         self.mocked_api().dcim.devices.get.side_effect = _request_error()
         with pytest.raises(NetboxAPIError, match="Error retrieving Netbox device"):
             self.netbox.get_server("physical")
@@ -205,15 +206,15 @@
         """It should return the value of the current status of the server, as a string."""
         assert isinstance(self.physical_server.status, str)
         assert self.physical_server.status == "active"
 
     def test_status_setter_ok(self):
         """It should set the status of the server to its new value, if it's an allowed transition."""
         self.physical_server.status = "failed"
-        assert self.netbox_host.save.called_once_with()
+        self.netbox_host.save.assert_called_once_with()
 
     def test_status_setter_virtual(self):
         """It should raise a NetboxError if trying to set the status on a virtual machine."""
         with pytest.raises(
             NetboxError,
             match="Server virtual is a virtual machine, its Netbox status is automatically synced from Ganeti",
         ):
@@ -245,33 +246,94 @@
     def test_fqdn_getter_no_dns(self):
         """It should raise a NetboxError if there is no DNS name defined for any primary IP of the device."""
         self.netbox_host.primary_ip4 = None
         self.netbox_host.primary_ip6.dns_name = None
         with pytest.raises(NetboxError, match="Server physical does not have any primary IP with a DNS name set"):
             self.physical_server.fqdn  # pylint: disable=pointless-statement
 
+    def test_fqdn_setter_virtual(self):
+        """It should raise a NetboxError if trying to change the FQDN of a VM."""
+        with pytest.raises(NetboxError, match="changing the FQDN is only for physical servers"):
+            self.virtual_server.fqdn = "foo.wikimedia.org"
+
+    def test_fqdn_setter_ok(self):
+        """It should set the new FQDN as expected."""
+        self.physical_server.fqdn = "foo.wikimedia.org"
+        assert self.netbox_host.save.called_once_with()
+        assert self.physical_server.fqdn == "foo.wikimedia.org"
+
+    def test_fqdn_setter_identical(self):
+        """It shouldn' try to change the v4 FQDN."""
+        self.netbox_host.primary_ip6.dns_name = "foo.example.com"
+        self.physical_server.fqdn = "physical.example.com"
+        self.netbox_host.primary_ip4.save.assert_not_called()
+        self.netbox_host.primary_ip6.save.assert_called_once_with()
+
+    def test_fqdn_setter_v6_only(self):
+        """It should set the new FQDN as expected."""
+        self.netbox_host.primary_ip4.dns_name = ""
+        self.physical_server.fqdn = "foo.wikimedia.org"
+        self.netbox_host.primary_ip6.save.assert_called_once_with()
+        self.netbox_host.primary_ip4.save.assert_not_called()
+        assert self.physical_server.fqdn == "foo.wikimedia.org"
+
+    def test_fqdn_setter_error(self):
+        """It should raise a NetboxError."""
+        self.netbox_host.primary_ip4.save.return_value = False
+        with pytest.raises(NetboxError, match="Spicerack was not able to update the primary_ip4 FQDN for physical."):
+            self.physical_server.fqdn = "new_name"
+
     def test_mgmt_fqdn_getter(self):
         """It should return the management FQDN of the device and cache it."""
         assert self.physical_server.mgmt_fqdn == "physical.mgmt.local"
         assert self.physical_server.mgmt_fqdn == "physical.mgmt.local"
         self.mocked_api.ipam.ip_addresses.get.assert_called_once_with(device="physical", interface="mgmt")
 
-    def test_mgmt_fqdn_getter_no_mgmt(self):
+    def test_mgmt_fqdn_getter_no_mgmt_fqdn(self):
         """It should raise a NetboxError if the management FQDN is not set."""
         self.mgmt_ip.dns_name = ""
         with pytest.raises(NetboxError, match="Server physical has no management interface with a DNS name set"):
             self.physical_server.mgmt_fqdn  # pylint: disable=pointless-statement
 
     def test_mgmt_fqdn_getter_virtual(self):
         """It should raise a NetboxError if trying to get the management FQDN on a virtual machine."""
         with pytest.raises(
             NetboxError, match="Server virtual is a virtual machine, does not have a management address"
         ):
             self.virtual_server.mgmt_fqdn  # pylint: disable=pointless-statement
 
+    def test_mgmt_fqdn_setter_virtual(self):
+        """It should raise a NetboxError if trying to change the FQDN of a VM."""
+        with pytest.raises(NetboxError, match="changing the mgmt FQDN is only for physical servers"):
+            self.virtual_server.mgmt_fqdn = "foo.wikimedia.org"
+
+    def test_mgmt_fqdn_setter_ok(self):
+        """It should set the new mgmt FQDN as expected."""
+        self.physical_server.mgmt_fqdn = "foo.wikimedia.org"
+        assert self.netbox_host.save.called_once_with()
+        assert self.physical_server.mgmt_fqdn == "foo.wikimedia.org"
+
+    def test_mgmt_fqdn_setter_identical(self):
+        """It shouldn't try to change the mgmt FQDN."""
+        self.physical_server.mgmt_fqdn = "physical.mgmt.local"
+        self.mocked_api.ipam.ip_addresses.save.assert_not_called()
+
+    def test_mgmt_fqdn_setter_no_mgmt_int(self):
+        """It should silently exit."""
+        self.mocked_api.ipam.ip_addresses.get.return_value = None
+        self.physical_server.mgmt_fqdn = "foo.mgmt.local"
+        with pytest.raises(NetboxError, match="Server physical has no management interface with a DNS name set."):
+            self.physical_server.mgmt_fqdn  # pylint: disable=pointless-statement
+
+    def test_mgmt_fqdn_setter_error(self):
+        """It should raise a NetboxError."""
+        self.mocked_api.ipam.ip_addresses.get.return_value.save.return_value = False
+        with pytest.raises(NetboxError, match="Spicerack was not able to update the mgmt_fqdn for physical."):
+            self.physical_server.mgmt_fqdn = "foo.mgmt.local"
+
     def test_asset_tag_fqdn_getter(self):
         """It should return the management FQDN of the asset tag of the device."""
         assert self.physical_server.asset_tag_fqdn == "asset1234.mgmt.local"
 
     def test_as_dict_physical(self):
         """It should return the dictionary representation of the physical server."""
         as_dict = self.physical_server.as_dict()
@@ -317,15 +379,15 @@
         """It should raise a NetboxError if trying to get the access vlan on a virtual machine."""
         with pytest.raises(NetboxError, match="Server is a virtual machine, can't return a switch interface."):
             self.virtual_server.access_vlan  # pylint: disable=pointless-statement
 
     def test_access_vlan_setter_ok(self):
         """It should set the access vlan."""
         self.physical_server.access_vlan = "set_test_vlan"
-        assert self.netbox_host.save.called_once_with()
+        self.netbox_host.primary_ip.assigned_object.connected_endpoint.save.assert_called_once_with()
 
     def test_access_vlan_setter_not_found(self):
         """It should raise a NetboxError if trying to set an non active vlan."""
         self.mocked_api.ipam.vlans.get.return_value = None
         with pytest.raises(NetboxError, match="Failed to find an active VLAN with name set_test_vlan"):
             self.physical_server.access_vlan = "set_test_vlan"
 
@@ -345,15 +407,15 @@
         self.netbox_host.primary_ip4 = None
         assert self.physical_server.primary_ip4_address is None
 
     def test_primary_ip4_address_setter_ok(self):
         """It should set the primary IPv4 address (and no CIDR means /32)."""
         self.mocked_api.ipam.ip_addresses.count.return_value = 0
         self.physical_server.primary_ip4_address = "192.0.2.1"
-        assert self.netbox_host.save.called_once_with()
+        self.netbox_host.primary_ip4.save.assert_called_once_with()
         assert self.physical_server.primary_ip4_address == IPv4Interface("192.0.2.1/32")
 
     def test_primary_ip4_address_setter_not_valid(self):
         """It should raise a NetboxError if trying to set the v4 IP to an invalid value."""
         with pytest.raises(NetboxError, match="foo is not a valid IP in the CIDR notation."):
             self.physical_server.primary_ip4_address = "foo"
 
@@ -377,22 +439,56 @@
         self.netbox_host.primary_ip6 = None
         assert self.physical_server.primary_ip6_address is None
 
     def test_primary_ip6_address_setter_ok(self):
         """It should set the primary IPv6 address."""
         self.mocked_api.ipam.ip_addresses.count.return_value = 0
         self.physical_server.primary_ip6_address = "2001:db8::1/32"
-        assert self.netbox_host.save.called_once_with()
+        self.netbox_host.primary_ip6.save.assert_called_once_with()
 
     def test_primary_ip6_address_setter_dry_run(self):
         """It should skip setting the primary IPv6 address."""
         self.mocked_api.ipam.ip_addresses.count.return_value = 0
         physical_server = NetboxServer(api=self.mocked_api, server=self.netbox_host, dry_run=True)
         physical_server.primary_ip6_address = "2001:db8::1/32"
         assert self.physical_server.primary_ip6_address == IPv6Interface("2620:0:861:103:10::1/64")
         self.netbox_host.save.assert_not_called()
 
     def test_primary_ip4_address_getter_no_primary_ip(self):
         """It should raise a NetboxError if it tries to set the address to a device without primary IP."""
         self.netbox_host.primary_ip4 = None
         with pytest.raises(NetboxError, match="No existing primary IPv4 for physical."):
             self.physical_server.primary_ip4_address = "192.0.2.1/32"
+
+    def test_name_getter_ok(self):
+        """It should return the name of the device."""
+        assert self.physical_server.name == "physical"
+
+    def test_name_setter_virtual(self):
+        """It should raise a NetboxError if trying to change the name of a VM."""
+        with pytest.raises(NetboxError, match="chaging the name is only for physical servers"):
+            self.virtual_server.name = "foo"
+
+    def test_name_setter_identical(self):
+        """It should not try to change the name if the old name is the same as the new one."""
+        self.physical_server.name = "physical"
+        self.netbox_host.save.assert_not_called()
+
+    def test_name_setter_dry_run(self):
+        """It should not try to change the name if in dry-run mode."""
+        physical_server = NetboxServer(api=self.mocked_api, server=self.netbox_host, dry_run=True)
+        physical_server.name = "new_name"
+        self.netbox_host.save.assert_not_called()
+        assert self.physical_server.name == "physical"
+
+    def test_name_setter_ok(self):
+        """It should set the new name as expected."""
+        self.physical_server.name = "new_name"
+        assert self.physical_server.name == "new_name"
+        assert self.physical_server.fqdn == "new_name.example.com"
+        assert self.physical_server.mgmt_fqdn == "new_name.mgmt.local"
+
+    def test_name_setter_error(self):
+        """It should raise a NetboxError."""
+        self.netbox_host.save.return_value = False
+        with pytest.raises(NetboxError, match="Name change for physical didn't get applied by Netbox."):
+            self.physical_server.name = "new_name"
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_peeringdb.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_puppet.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_puppet.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     b'"dns_alt_names":["DNS:service.example.com"]}]}'
 )
 PUPPET_SERVER_CA_CERT_METADATA_REQUESTED = (
     b'{"signed": [{"name":"test.example.com","state":"requested","fingerprint":"00:AA",'
     b'"fingerprints":{"default":"00:AA","SHA1":"11:BB","SHA256": "00:AA","SHA512":"22:CC"},'
     b'"dns_alt_names":["DNS:service.example.com"]}]}'
 )
+PUPPET_SERVER_CA_CERT_METADATA_MISSING = b'{"missing": ["test.example.org"]}'
 PUPPET_CA_CERT_METADATA_SIGNED = (
     b'[{"name":"test.example.com","state":"signed","fingerprint":"00:AA",'
     b'"fingerprints":{"default":"00:AA","SHA1":"11:BB","SHA256": "00:AA","SHA512":"22:CC"},'
     b'"dns_alt_names":["DNS:service.example.com"]}]'
 )
 PUPPET_CA_CERT_METADATA_REQUESTED = (
     b'[{"name":"test.example.com","state":"requested","fingerprint":"00:AA",'
@@ -561,21 +562,45 @@
     def test_delete(self):
         """It should delete the host from Puppet master and PuppetDB."""
         self.puppet_server.delete("test.example.com")
         self.mocked_server_host.run_sync.assert_called_once_with(
             "puppet node clean test.example.com", "puppet node deactivate test.example.com", print_progress_bars=False
         )
 
-    def test_destroy(self):
+    def test_destroy_ok(self):
         """It should delete the certificate of the host in the Puppet CA."""
+        results = [
+            (
+                nodeset("puppetserver.example.com"),
+                MsgTreeElem(PUPPET_SERVER_CA_CERT_METADATA_SIGNED, parent=MsgTreeElem()),
+            )
+        ]
+        self.mocked_server_host.run_sync.return_value = iter(results)
+
         self.puppet_server.destroy("test.example.com")
-        self.mocked_server_host.run_sync.assert_called_once_with(
+        self.mocked_server_host.run_sync.assert_called_with(
             "puppetserver ca clean --certname test.example.com", print_progress_bars=False
         )
 
+    def test_destroy_missing(self):
+        """It should not do anything if the certificate of the host in the Puppet CA is alredy missing."""
+        results = [
+            (
+                nodeset("puppetserver.example.com"),
+                MsgTreeElem(PUPPET_SERVER_CA_CERT_METADATA_MISSING, parent=MsgTreeElem()),
+            )
+        ]
+        self.mocked_server_host.run_sync.return_value = iter(results)
+
+        self.puppet_server.destroy("test.example.com")
+
+        for call in self.mocked_server_host.mock_calls:
+            if call.args and "ca clean" in call.args[0]:
+                raise RuntimeError(f"Expected ca clean to not be called, got: {call}")
+
     def test_verify_ok(self):
         """It should verify that the host has a signed certificate in the Puppet CA."""
         results = [
             (
                 nodeset("puppetserver.example.com"),
                 MsgTreeElem(PUPPET_SERVER_CA_CERT_METADATA_SIGNED, parent=MsgTreeElem()),
             )
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_redfish.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_redfish.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,15 @@
 
     @mock.patch("spicerack.redfish.Path.open")
     @mock.patch("spicerack.redfish.Redfish.submit_files")
     def test_submit_upload_file(self, mock_submit_files, mocked_path_open):
         """In dry-run mode should not submit a task and return a dummy location."""
         mock_submit_files.return_value = "/redfish/v1/TaskService/Tasks/JID_1234567890"
         assert self.redfish.upload_file(Path("/foo/test")) == "/redfish/v1/TaskService/Tasks/JID_1234567890"
-        mocked_path_open.called_once_with("rb")
+        mocked_path_open.assert_called_once_with("rb")
 
     @pytest.mark.parametrize("reboot", (True, False))
     @mock.patch("spicerack.redfish.Redfish.submit_files")
     def test_submit_multipush_upload(self, mock_submit_files, reboot):
         """In dry-run mode should not submit a task and return a dummy location."""
         mock_submit_files.return_value = "/redfish/v1/TaskService/Tasks/JID_1234567890"
         data = BytesIO()
@@ -856,36 +856,45 @@
     def test_wait_reboot_since(self, mocked_check_connection, mocked_last_reboot, mocked_sleep, generation):
         """It should return immediately if the host has already rebooted."""
         since = datetime.fromisoformat("2022-01-01T00:00:00-00:00")
         mocked_check_connection.return_value = True
         mocked_last_reboot.return_value = datetime.fromisoformat("2022-01-01T00:05:00-00:00")
         self.redfish._generation = generation  # pylint: disable=protected-access
         self.redfish.wait_reboot_since(since)
-        mocked_check_connection.called_once()
-        mocked_last_reboot.called_once_with(since)
+        mocked_check_connection.assert_called_once()
+        mocked_last_reboot.assert_called_once_with()
+        calls = []
         if generation < 14:
-            mocked_sleep.called_once_with(120)
-        mocked_sleep.called_once_with(30)
+            calls.append(mock.call(120))
+        calls.append(mock.call(30))
+        assert mocked_sleep.mock_calls == calls
 
     @pytest.mark.parametrize("generation", (1, 13, 14))
     @mock.patch("spicerack.redfish.time.sleep")
     @mock.patch("spicerack.redfish.RedfishDell.last_reboot")
     @mock.patch("spicerack.redfish.RedfishDell.check_connection")
     def test_wait_reboot_since_to_early(self, mocked_check_connection, mocked_last_reboot, mocked_sleep, generation):
         """It should raise an error if the reboot time is to early."""
         since = datetime.fromisoformat("2022-01-01T00:05:00-00:00")
         mocked_check_connection.return_value = True
         mocked_last_reboot.return_value = datetime.fromisoformat("2022-01-01T00:00:00-00:00")
         self.redfish._generation = generation  # pylint: disable=protected-access
         with pytest.raises(redfish.RedfishError, match="no new reboot detected"):
             self.redfish.wait_reboot_since(since)
-        mocked_check_connection.called_once()
-        mocked_last_reboot.called_once_with(since)
+        mocked_check_connection.assert_called_with()
+        assert mocked_check_connection.call_count == 240
+        mocked_last_reboot.assert_called_with()
+        assert mocked_last_reboot.call_count == 240
+        calls = []
         if generation < 14:
-            mocked_sleep.called_once_with(120)
+            calls = [mock.call(120), mock.call(10)] * 239 + [mock.call(120)]
+        else:
+            calls = [mock.call(10)] * 239
+
+        assert mocked_sleep.mock_calls == calls
 
     @pytest.mark.parametrize("allow_new", (False, True))
     @mock.patch("wmflib.decorators.time.sleep", return_value=None)
     def test_scp_dump(self, mocked_sleep, allow_new):
         """It should return an instance of DellSCP with the current configuration for the given target."""
         self.requests_mock.post(
             "/redfish/v1/Managers/iDRAC.Embedded.1/Actions/Oem/EID_674_Manager.ExportSystemConfiguration",
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_redis_cluster.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_remote.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_reposync.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/test_service.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/test_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Service Module Tests."""
 from ipaddress import ip_address
 from unittest import mock
 
 import pytest
 from wmflib.config import load_yaml_config
 
-from spicerack import service
+from spicerack import Alertmanager, service
 from spicerack.administrative import Reason
 from spicerack.dnsdisc import DiscoveryError
 from spicerack.tests import get_fixture_path
 
 
 def test_service_discovery_no_records():
     """It should raise a DiscoveryRecordNotFoundError exception if no records are present."""
@@ -24,15 +24,18 @@
     def setup_method(self):
         """Initialize the tests."""
         # pylint: disable=attribute-defined-outside-init
         self.mocked_confctl = mock.MagicMock()
         self.authdns_servers = load_yaml_config(get_fixture_path("discovery", "authdns.yaml"))
 
         catalog = load_yaml_config(get_fixture_path("service", "service.yaml"))
-        self.catalog = service.Catalog(catalog, confctl=self.mocked_confctl, authdns_servers=self.authdns_servers)
+        alertmanager = Alertmanager(alertmanager_urls=("https://alertmanager-eqiad.wikimedia.example",))
+        self.catalog = service.Catalog(
+            catalog, alertmanager=alertmanager, confctl=self.mocked_confctl, authdns_servers=self.authdns_servers
+        )
 
     def test_init(self):
         """It should instantiate a Catalog instance properly."""
         assert isinstance(self.catalog, service.Catalog)
 
     def test_service_names(self):
         """It should return the list of all service names."""
@@ -62,16 +65,21 @@
     def setup_method(self):
         """Initialize the tests."""
         # pylint: disable=attribute-defined-outside-init
         self.mocked_confctl = mock.MagicMock()
         self.authdns_servers = load_yaml_config(get_fixture_path("discovery", "authdns.yaml"))
 
         catalog = load_yaml_config(get_fixture_path("service", "service.yaml"))
+        alertmanager = Alertmanager(alertmanager_urls=("https://alertmanager-eqiad.wikimedia.example",), dry_run=False)
         self.catalog = service.Catalog(
-            catalog, confctl=self.mocked_confctl, authdns_servers=self.authdns_servers, dry_run=False
+            catalog,
+            alertmanager=alertmanager,
+            confctl=self.mocked_confctl,
+            authdns_servers=self.authdns_servers,
+            dry_run=False,
         )
 
         self.service1 = self.catalog.get("service1")
         self.service2 = self.catalog.get("service2")
         self.service3 = self.catalog.get("service3")
         self.service_no_lvs = self.catalog.get("service_no_lvs")
         self.subnets = {"eqiad": ip_address("10.10.0.1"), "codfw": ip_address("10.20.0.1")}
```

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/unit/toolforge/test_etcdctl.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/unit/toolforge/test_etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/tests/vulture_whitelist.py` & `wikimedia_spicerack-8.5.0/spicerack/tests/vulture_whitelist.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/spicerack/toolforge/etcdctl.py` & `wikimedia_spicerack-8.5.0/spicerack/toolforge/etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/tox.ini` & `wikimedia_spicerack-8.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/utils/check-style.sh` & `wikimedia_spicerack-8.5.0/utils/check-style.sh`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/PKG-INFO` & `wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 8.4.1
+Version: 8.5.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
@@ -26,15 +26,14 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: conftool>=1.0.1
 Requires-Dist: cumin>=3.0.2
 Requires-Dist: dnspython~=2.0.0
 Requires-Dist: elasticsearch<7.15.0,>=5.0.0
-Requires-Dist: elasticsearch-curator~=5.0
 Requires-Dist: gitpython>=3.1.14
 Requires-Dist: kafka-python>=2.0.1
 Requires-Dist: kubernetes==12.0.*
 Requires-Dist: packaging
 Requires-Dist: pymysql>=0.9.3
 Requires-Dist: pynetbox~=6.6
 Requires-Dist: python-etcd~=0.4.5
@@ -55,15 +54,15 @@
 Requires-Dist: sphinx-autodoc-typehints>=1.9.0; extra == "tests"
 Requires-Dist: Sphinx>=3.4.3; extra == "tests"
 Requires-Dist: types-PyMySQL; extra == "tests"
 Requires-Dist: types-redis; extra == "tests"
 Requires-Dist: types-requests; extra == "tests"
 Requires-Dist: types-setuptools; extra == "tests"
 Provides-Extra: format
-Requires-Dist: black<=21.12b0; extra == "format"
+Requires-Dist: black; extra == "format"
 Requires-Dist: isort; extra == "format"
 Provides-Extra: prospector
 Requires-Dist: prospector[with_everything]>=1.1.7; extra == "prospector"
 Requires-Dist: pytest>=6.0.2; extra == "prospector"
 Requires-Dist: requests-mock>=1.7.0; extra == "prospector"
 
 Spicerack - Automation framework for the WMF production infrastructure
```

### Comparing `wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/SOURCES.txt` & `wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 spicerack/tests/vulture_whitelist.py
 spicerack/tests/fixtures/config.yaml
 spicerack/tests/fixtures/config_bad_external_modules.yaml
 spicerack/tests/fixtures/config_empty_base_dirs.yaml
 spicerack/tests/fixtures/config_external_modules.yaml
 spicerack/tests/fixtures/config_multiple_base_dirs.yaml
 spicerack/tests/fixtures/config_wrong_overrides.yaml
+spicerack/tests/fixtures/alertmanager/config.yaml
 spicerack/tests/fixtures/confctl/config.yaml
 spicerack/tests/fixtures/confctl/schema.yaml
 spicerack/tests/fixtures/config/valid.yaml
 spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
 spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
 spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
 spicerack/tests/fixtures/cookbook/cookbooks/root.py
```

### Comparing `wikimedia-spicerack-8.4.1/wikimedia_spicerack.egg-info/requires.txt` & `wikimedia_spicerack-8.5.0/wikimedia_spicerack.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 conftool>=1.0.1
 cumin>=3.0.2
 dnspython~=2.0.0
 elasticsearch<7.15.0,>=5.0.0
-elasticsearch-curator~=5.0
 gitpython>=3.1.14
 kafka-python>=2.0.1
 kubernetes==12.0.*
 packaging
 pymysql>=0.9.3
 pynetbox~=6.6
 python-etcd~=0.4.5
 redis<=4.1.3,>=3.5.3
 requests>=2.25.0
 wmflib
 
 [format]
-black<=21.12b0
+black
 isort
 
 [prospector]
 prospector[with_everything]>=1.1.7
 pytest>=6.0.2
 requests-mock>=1.7.0
```

