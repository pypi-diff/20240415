# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.13a1712973417.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.13a1713148341.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.13a1712973417.tar", last modified: Sat Apr 13 01:59:39 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.13a1713148341.tar", last modified: Mon Apr 15 02:34:13 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417.tar` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.466457 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-13 01:59:39.466457 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.454456 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     3665 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.458456 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.462456 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      828 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    10044 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8426 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    14132 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)     9732 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)     9915 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.462456 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1539 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    31109 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     1250 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27642 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.466457 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      479 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1530 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    22569 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15129 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    14032 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    16572 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    25981 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    16828 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    13649 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    19232 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    17062 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    19599 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:59:39.466457 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-13 01:59:39.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-13 01:59:39.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:59:39.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-13 01:59:39.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 01:59:39.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      897 2024-04-13 01:59:33.000000 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:59:39.466457 pulumi_kubernetes_the_hard_way-0.0.13a1712973417/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.649146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     3729 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.649146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.653146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      856 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    13961 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8426 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    14583 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    13499 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)     9915 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1539 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    31109 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     1250 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27642 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      479 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1530 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    22569 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15129 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    14032 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    16572 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    25981 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    16828 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    13649 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    19232 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    17062 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    19599 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 02:34:13.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      898 2024-04-15 02:34:06.000000 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:34:13.657146 pulumi_kubernetes_the_hard_way-0.0.13a1713148341/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.13a1712973417
+Version: 0.0.13a1713148341
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
 Requires-Dist: pulumi-command<1.0.0,>=0.9.2
-Requires-Dist: pulumi-kubernetes<5.0.0,>=4.9.1
+Requires-Dist: pulumi-kubernetes<5.0.0,>=4.10.0
 Requires-Dist: pulumi-random<5.0.0,>=4.16.0
 Requires-Dist: pulumi-tls<6.0.0,>=5.0.2
 Requires-Dist: semver>=2.8.1
 
 # Pulumi Kubernetes the Hard Way
 
 This is a Pulumi implementation of Kelsey Hightower's [Kubernetes the Hard Way](https://github.com/kelseyhightower/kubernetes-the-hard-way). It attempts to provide a set of building blocks to build a kubernetes cluster from scratch.
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/README.md` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
   "classes": {
    "kubernetes-the-hard-way:remote:CniPluginsInstall": "CniPluginsInstall",
    "kubernetes-the-hard-way:remote:ContainerdInstall": "ContainerdInstall",
    "kubernetes-the-hard-way:remote:CrictlInstall": "CrictlInstall",
    "kubernetes-the-hard-way:remote:Download": "Download",
    "kubernetes-the-hard-way:remote:EtcdConfiguration": "EtcdConfiguration",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
+   "kubernetes-the-hard-way:remote:EtcdService": "EtcdService",
    "kubernetes-the-hard-way:remote:File": "File",
    "kubernetes-the-hard-way:remote:KubeApiServerInstall": "KubeApiServerInstall",
    "kubernetes-the-hard-way:remote:KubeControllerManagerInstall": "KubeControllerManagerInstall",
    "kubernetes-the-hard-way:remote:KubeProxyInstall": "KubeProxyInstall",
    "kubernetes-the-hard-way:remote:KubeSchedulerInstall": "KubeSchedulerInstall",
    "kubernetes-the-hard-way:remote:KubectlInstall": "KubectlInstall",
    "kubernetes-the-hard-way:remote:KubeletInstall": "KubeletInstall",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ._enums import *
 from .cni_plugins_install import *
 from .containerd_install import *
 from .crictl_install import *
 from .download import *
 from .etcd_configuration import *
 from .etcd_install import *
+from .etcd_service import *
 from .file import *
 from .kube_api_server_install import *
 from .kube_controller_manager_install import *
 from .kube_proxy_install import *
 from .kube_scheduler_install import *
 from .kubectl_install import *
 from .kubelet_install import *
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 from .. import tools as _tools
 from .file import File
 import pulumi_command
 
 __all__ = ['EtcdConfigurationArgs', 'EtcdConfiguration']
 
 @pulumi.input_type
@@ -42,14 +43,16 @@
         pulumi.set(__self__, "etcd_path", etcd_path)
         pulumi.set(__self__, "internal_ip", internal_ip)
         pulumi.set(__self__, "key_pem", key_pem)
         if configuration_directory is None:
             configuration_directory = '/etc/etcd'
         if configuration_directory is not None:
             pulumi.set(__self__, "configuration_directory", configuration_directory)
+        if data_directory is None:
+            data_directory = '/var/lib/etcd'
         if data_directory is not None:
             pulumi.set(__self__, "data_directory", data_directory)
 
     @property
     @pulumi.getter(name="caPem")
     def ca_pem(self) -> pulumi.Input[str]:
         """
@@ -225,14 +228,16 @@
             __props__.__dict__["cert_pem"] = cert_pem
             if configuration_directory is None:
                 configuration_directory = '/etc/etcd'
             __props__.__dict__["configuration_directory"] = configuration_directory
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
+            if data_directory is None:
+                data_directory = '/var/lib/etcd'
             __props__.__dict__["data_directory"] = data_directory
             if etcd_path is None and not opts.urn:
                 raise TypeError("Missing required property 'etcd_path'")
             __props__.__dict__["etcd_path"] = etcd_path
             if internal_ip is None and not opts.urn:
                 raise TypeError("Missing required property 'internal_ip'")
             __props__.__dict__["internal_ip"] = internal_ip
@@ -240,14 +245,15 @@
                 raise TypeError("Missing required property 'key_pem'")
             __props__.__dict__["key_pem"] = key_pem
             __props__.__dict__["ca_file"] = None
             __props__.__dict__["cert_file"] = None
             __props__.__dict__["configuration_mkdir"] = None
             __props__.__dict__["data_mkdir"] = None
             __props__.__dict__["key_file"] = None
+            __props__.__dict__["value"] = None
         super(EtcdConfiguration, __self__).__init__(
             'kubernetes-the-hard-way:remote:EtcdConfiguration',
             resource_name,
             __props__,
             opts,
             remote=True)
 
@@ -281,15 +287,15 @@
         """
         The PEM encoded certificate data.
         """
         return pulumi.get(self, "cert_pem")
 
     @property
     @pulumi.getter(name="configurationDirectory")
-    def configuration_directory(self) -> pulumi.Output[Optional[str]]:
+    def configuration_directory(self) -> pulumi.Output[str]:
         """
         The directory to store etcd configuration.
         """
         return pulumi.get(self, "configuration_directory")
 
     @property
     @pulumi.getter(name="configurationMkdir")
@@ -305,15 +311,15 @@
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter(name="dataDirectory")
-    def data_directory(self) -> pulumi.Output[Optional[str]]:
+    def data_directory(self) -> pulumi.Output[str]:
         """
         The directory etcd will store its data.
         """
         return pulumi.get(self, "data_directory")
 
     @property
     @pulumi.getter(name="dataMkdir")
@@ -351,7 +357,15 @@
     @pulumi.getter(name="keyPem")
     def key_pem(self) -> pulumi.Output[str]:
         """
         The PEM encoded key data.
         """
         return pulumi.get(self, "key_pem")
 
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Output['outputs.EtcdConfigurationProps']:
+        """
+        A bag of properties to be consumed by other resources.
+        """
+        return pulumi.get(self, "value")
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,20 +7,136 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 
 __all__ = [
+    'EtcdConfigurationProps',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
+class EtcdConfigurationProps(dict):
+    """
+    Props for resources that consume etcd configuration.
+    """
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "caFilePath":
+            suggest = "ca_file_path"
+        elif key == "certFilePath":
+            suggest = "cert_file_path"
+        elif key == "dataDirectory":
+            suggest = "data_directory"
+        elif key == "etcdPath":
+            suggest = "etcd_path"
+        elif key == "internalIp":
+            suggest = "internal_ip"
+        elif key == "keyFilePath":
+            suggest = "key_file_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in EtcdConfigurationProps. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        EtcdConfigurationProps.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        EtcdConfigurationProps.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ca_file_path: str,
+                 cert_file_path: str,
+                 data_directory: str,
+                 etcd_path: str,
+                 internal_ip: str,
+                 key_file_path: str,
+                 name: str):
+        """
+        Props for resources that consume etcd configuration.
+        :param str ca_file_path: Path to the certificate authority file on the remote system.
+        :param str cert_file_path: Path to the certificate file on the remote system.
+        :param str data_directory: Etcd's data directory.
+        :param str etcd_path: Path to the etcd binary.
+        :param str internal_ip: Internal IP of the etcd node.
+        :param str key_file_path: Path to the private key file on the remote system.
+        :param str name: Name of the etcd node.
+        """
+        pulumi.set(__self__, "ca_file_path", ca_file_path)
+        pulumi.set(__self__, "cert_file_path", cert_file_path)
+        pulumi.set(__self__, "data_directory", data_directory)
+        pulumi.set(__self__, "etcd_path", etcd_path)
+        pulumi.set(__self__, "internal_ip", internal_ip)
+        pulumi.set(__self__, "key_file_path", key_file_path)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter(name="caFilePath")
+    def ca_file_path(self) -> str:
+        """
+        Path to the certificate authority file on the remote system.
+        """
+        return pulumi.get(self, "ca_file_path")
+
+    @property
+    @pulumi.getter(name="certFilePath")
+    def cert_file_path(self) -> str:
+        """
+        Path to the certificate file on the remote system.
+        """
+        return pulumi.get(self, "cert_file_path")
+
+    @property
+    @pulumi.getter(name="dataDirectory")
+    def data_directory(self) -> str:
+        """
+        Etcd's data directory.
+        """
+        return pulumi.get(self, "data_directory")
+
+    @property
+    @pulumi.getter(name="etcdPath")
+    def etcd_path(self) -> str:
+        """
+        Path to the etcd binary.
+        """
+        return pulumi.get(self, "etcd_path")
+
+    @property
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> str:
+        """
+        Internal IP of the etcd node.
+        """
+        return pulumi.get(self, "internal_ip")
+
+    @property
+    @pulumi.getter(name="keyFilePath")
+    def key_file_path(self) -> str:
+        """
+        Path to the private key file on the remote system.
+        """
+        return pulumi.get(self, "key_file_path")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Name of the etcd node.
+        """
+        return pulumi.get(self, "name")
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

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.13a1712973417
+Version: 0.0.13a1713148341
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
 Requires-Dist: pulumi-command<1.0.0,>=0.9.2
-Requires-Dist: pulumi-kubernetes<5.0.0,>=4.9.1
+Requires-Dist: pulumi-kubernetes<5.0.0,>=4.10.0
 Requires-Dist: pulumi-random<5.0.0,>=4.16.0
 Requires-Dist: pulumi-tls<6.0.0,>=5.0.2
 Requires-Dist: semver>=2.8.1
 
 # Pulumi Kubernetes the Hard Way
 
 This is a Pulumi implementation of Kelsey Hightower's [Kubernetes the Hard Way](https://github.com/kelseyhightower/kubernetes-the-hard-way). It attempts to provide a set of building blocks to build a kubernetes cluster from scratch.
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
 pulumi_kubernetes_the_hard_way/remote/containerd_install.py
 pulumi_kubernetes_the_hard_way/remote/crictl_install.py
 pulumi_kubernetes_the_hard_way/remote/download.py
 pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+pulumi_kubernetes_the_hard_way/remote/etcd_service.py
 pulumi_kubernetes_the_hard_way/remote/file.py
 pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
 pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
 pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
 pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.13a1712973417/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.13a1713148341/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
-  dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.9.2,<1.0.0", "pulumi-kubernetes>=4.9.1,<5.0.0", "pulumi-random>=4.16.0,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
+  dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.9.2,<1.0.0", "pulumi-kubernetes>=4.10.0,<5.0.0", "pulumi-random>=4.16.0,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.13a1712973417"
+  version = "0.0.13a1713148341"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

