# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.13a1713149286.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.13a1713150524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.13a1713149286.tar", last modified: Mon Apr 15 02:49:58 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.13a1713150524.tar", last modified: Mon Apr 15 03:11:27 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286.tar` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.763395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     3789 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.763395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.767395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      882 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    13961 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8426 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    14583 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    13499 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)     9915 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.771395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1539 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    31109 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     1250 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27642 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.771395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      479 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1530 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    22569 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15129 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    14032 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    16572 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    25981 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    16828 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    13649 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    19232 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    17062 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    19599 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      898 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.565280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 03:11:27.565280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.557280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     3921 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.557280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.561280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      940 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    15965 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8426 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15536 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)     9915 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.565280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3157 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    31109 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     3101 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27642 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.565280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      479 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1530 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    22569 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15129 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    14032 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    16572 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    25981 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    16828 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    13649 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    19232 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    17062 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    19599 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:11:27.565280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 03:11:27.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-15 03:11:27.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:11:27.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 03:11:27.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 03:11:27.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      898 2024-04-15 03:11:21.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:11:27.565280 pulumi_kubernetes_the_hard_way-0.0.13a1713150524/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.13a1713149286
+Version: 0.0.13a1713150524
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/README.md` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,24 +39,26 @@
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
    "kubernetes-the-hard-way:remote:CniPluginsInstall": "CniPluginsInstall",
    "kubernetes-the-hard-way:remote:ContainerdInstall": "ContainerdInstall",
    "kubernetes-the-hard-way:remote:CrictlInstall": "CrictlInstall",
    "kubernetes-the-hard-way:remote:Download": "Download",
+   "kubernetes-the-hard-way:remote:EtcdCluster": "EtcdCluster",
    "kubernetes-the-hard-way:remote:EtcdConfiguration": "EtcdConfiguration",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:EtcdService": "EtcdService",
    "kubernetes-the-hard-way:remote:File": "File",
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
    "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
    "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
    "kubernetes-the-hard-way:remote:KubectlInstall": "KubectlInstall",
    "kubernetes-the-hard-way:remote:KubeletInstall": "KubeletInstall",
+   "kubernetes-the-hard-way:remote:ProvisionEtcd": "ProvisionEtcd",
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
    "kubernetes-the-hard-way:remote:StaticPod": "StaticPod",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
   }
  },
  {
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 import typing
 # Export this package's modules as members:
 from ._enums import *
 from .cni_plugins_install import *
 from .containerd_install import *
 from .crictl_install import *
 from .download import *
+from .etcd_cluster import *
 from .etcd_configuration import *
 from .etcd_install import *
 from .etcd_service import *
 from .file import *
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
 from .kube_proxy_install import *
 from .kube_scheduler_install import *
 from .kubectl_install import *
 from .kubelet_install import *
+from .provision_etcd import *
 from .runc_install import *
 from .start_etcd import *
 from .static_pod import *
 from .systemd_service import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
+import pulumi_command
 
 __all__ = [
     'EtcdConfigurationPropsArgs',
+    'EtcdNodeArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
 @pulumi.input_type
 class EtcdConfigurationPropsArgs:
@@ -127,14 +129,68 @@
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
+class EtcdNodeArgs:
+    def __init__(__self__, *,
+                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
+                 internal_ip: pulumi.Input[str],
+                 architecture: Optional[pulumi.Input['Architecture']] = None):
+        """
+        Etcd node description.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
+        :param pulumi.Input[str] internal_ip: The internal IP of the node.
+        :param pulumi.Input['Architecture'] architecture: The CPU architecture of the node.
+        """
+        pulumi.set(__self__, "connection", connection)
+        pulumi.set(__self__, "internal_ip", internal_ip)
+        if architecture is not None:
+            pulumi.set(__self__, "architecture", architecture)
+
+    @property
+    @pulumi.getter
+    def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
+        """
+        The parameters with which to connect to the remote host.
+        """
+        return pulumi.get(self, "connection")
+
+    @connection.setter
+    def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
+        pulumi.set(self, "connection", value)
+
+    @property
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> pulumi.Input[str]:
+        """
+        The internal IP of the node.
+        """
+        return pulumi.get(self, "internal_ip")
+
+    @internal_ip.setter
+    def internal_ip(self, value: pulumi.Input[str]):
+        pulumi.set(self, "internal_ip", value)
+
+    @property
+    @pulumi.getter
+    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
+        """
+        The CPU architecture of the node.
+        """
+        return pulumi.get(self, "architecture")
+
+    @architecture.setter
+    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
+        pulumi.set(self, "architecture", value)
+
+
+@pulumi.input_type
 class SystemdInstallSectionArgs:
     def __init__(__self__, *,
                  wanted_by: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#%5BInstall%5D%20Section%20Options
         :param pulumi.Input[Sequence[pulumi.Input[str]]] wanted_by: A symbolic link is created in the .wants/, .requires/, or .upholds/ directory of each of the listed units when this unit is installed by systemctl enable.
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,15 @@
                 raise TypeError("Missing required property 'internal_ip'")
             __props__.__dict__["internal_ip"] = internal_ip
             if key_pem is None and not opts.urn:
                 raise TypeError("Missing required property 'key_pem'")
             __props__.__dict__["key_pem"] = key_pem
             __props__.__dict__["ca_file"] = None
             __props__.__dict__["cert_file"] = None
+            __props__.__dict__["configuration_chmod"] = None
             __props__.__dict__["configuration_mkdir"] = None
             __props__.__dict__["data_mkdir"] = None
             __props__.__dict__["key_file"] = None
             __props__.__dict__["value"] = None
         super(EtcdConfiguration, __self__).__init__(
             'kubernetes-the-hard-way:remote:EtcdConfiguration',
             resource_name,
@@ -286,14 +287,22 @@
     def cert_pem(self) -> pulumi.Output[str]:
         """
         The PEM encoded certificate data.
         """
         return pulumi.get(self, "cert_pem")
 
     @property
+    @pulumi.getter(name="configurationChmod")
+    def configuration_chmod(self) -> pulumi.Output[Optional['_tools.Chmod']]:
+        """
+        The configuration chmod operation.
+        """
+        return pulumi.get(self, "configuration_chmod")
+
+    @property
     @pulumi.getter(name="configurationDirectory")
     def configuration_directory(self) -> pulumi.Output[str]:
         """
         The directory to store etcd configuration.
         """
         return pulumi.get(self, "configuration_directory")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
+import pulumi_command
 
 __all__ = [
     'EtcdConfigurationProps',
+    'EtcdNode',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
 class EtcdConfigurationProps(dict):
@@ -129,14 +131,76 @@
         """
         Name of the etcd node.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
+class EtcdNode(dict):
+    """
+    Etcd node description.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "internalIp":
+            suggest = "internal_ip"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in EtcdNode. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        EtcdNode.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        EtcdNode.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 connection: 'pulumi_command.remote.outputs.Connection',
+                 internal_ip: str,
+                 architecture: Optional['Architecture'] = None):
+        """
+        Etcd node description.
+        :param 'pulumi_command.remote.Connection' connection: The parameters with which to connect to the remote host.
+        :param str internal_ip: The internal IP of the node.
+        :param 'Architecture' architecture: The CPU architecture of the node.
+        """
+        pulumi.set(__self__, "connection", connection)
+        pulumi.set(__self__, "internal_ip", internal_ip)
+        if architecture is not None:
+            pulumi.set(__self__, "architecture", architecture)
+
+    @property
+    @pulumi.getter
+    def connection(self) -> 'pulumi_command.remote.outputs.Connection':
+        """
+        The parameters with which to connect to the remote host.
+        """
+        return pulumi.get(self, "connection")
+
+    @property
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> str:
+        """
+        The internal IP of the node.
+        """
+        return pulumi.get(self, "internal_ip")
+
+    @property
+    @pulumi.getter
+    def architecture(self) -> Optional['Architecture']:
+        """
+        The CPU architecture of the node.
+        """
+        return pulumi.get(self, "architecture")
+
+
+@pulumi.output_type
 class SystemdInstallSection(dict):
     """
     https://www.freedesktop.org/software/systemd/man/latest/systemd.unit.html#%5BInstall%5D%20Section%20Options
     """
     @staticmethod
     def __key_warning(key: str):
         suggest = None
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.13a1713149286
+Version: 0.0.13a1713150524
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,27 @@
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
 pulumi_kubernetes_the_hard_way/remote/containerd_install.py
 pulumi_kubernetes_the_hard_way/remote/crictl_install.py
 pulumi_kubernetes_the_hard_way/remote/download.py
+pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
 pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/etcd_service.py
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
 pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
 pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
+pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
 pulumi_kubernetes_the_hard_way/remote/runc_install.py
 pulumi_kubernetes_the_hard_way/remote/start_etcd.py
 pulumi_kubernetes_the_hard_way/remote/static_pod.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.13a1713150524/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.9.2,<1.0.0", "pulumi-kubernetes>=4.10.0,<5.0.0", "pulumi-random>=4.16.0,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.13a1713149286"
+  version = "0.0.13a1713150524"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

