# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.13a1713148341.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.13a1713149286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.13a1713148341.tar", last modified: Mon Apr 15 02:34:13 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.13a1713149286.tar", last modified: Mon Apr 15 02:49:58 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341.tar` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.649146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     3729 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.649146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.653146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      856 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    13961 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8426 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    14583 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    13499 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)     9915 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1539 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    31109 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     1250 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27642 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      479 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1530 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    22569 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15129 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    14032 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    16572 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    25981 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    16828 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    13649 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    19232 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    17062 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    19599 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      898 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.763395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     3789 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.763395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.767395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      882 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    13961 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8426 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    14583 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    13499 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)     9915 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.771395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1539 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    31109 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     1250 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27642 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.771395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      479 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1530 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    22569 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15129 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    14032 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    16572 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    25981 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    16828 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    13649 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    19232 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    17062 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    19599 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 02:49:58.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      898 2024-04-15 02:49:52.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:49:58.775395 pulumi_kubernetes_the_hard_way-0.0.13a1713149286/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.13a1713148341
+Version: 0.0.13a1713149286
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/README.md` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
    "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
    "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
    "kubernetes-the-hard-way:remote:KubectlInstall": "KubectlInstall",
    "kubernetes-the-hard-way:remote:KubeletInstall": "KubeletInstall",
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
+   "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
    "kubernetes-the-hard-way:remote:StaticPod": "StaticPod",
    "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tls",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
 from .kube_proxy_install import *
 from .kube_scheduler_install import *
 from .kubectl_install import *
 from .kubelet_install import *
 from .runc_install import *
+from .start_etcd import *
 from .static_pod import *
 from .systemd_service import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.13a1713148341
+Version: 0.0.13a1713149286
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
 pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
 pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
 pulumi_kubernetes_the_hard_way/remote/outputs.py
 pulumi_kubernetes_the_hard_way/remote/runc_install.py
+pulumi_kubernetes_the_hard_way/remote/start_etcd.py
 pulumi_kubernetes_the_hard_way/remote/static_pod.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.13a1713149286/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.9.2,<1.0.0", "pulumi-kubernetes>=4.10.0,<5.0.0", "pulumi-random>=4.16.0,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.13a1713148341"
+  version = "0.0.13a1713149286"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

