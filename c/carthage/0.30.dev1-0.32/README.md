# Comparing `tmp/carthage-0.30.dev1.tar.gz` & `tmp/carthage-0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carthage-0.30.dev1.tar", last modified: Tue Nov 28 17:23:52 2023, max compression
+gzip compressed data, was "carthage-0.32.tar", last modified: Mon Apr 15 21:08:26 2024, max compression
```

## Comparing `carthage-0.30.dev1.tar` & `carthage-0.32.tar`

### file list

```diff
@@ -1,225 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.873961 carthage-0.30.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    42976 2023-11-28 17:23:43.000000 carthage-0.30.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-28 17:23:43.000000 carthage-0.30.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-11-28 17:23:52.873961 carthage-0.30.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-11-28 17:23:43.000000 carthage-0.30.dev1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.841961 carthage-0.30.dev1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1248 2023-11-28 17:23:43.000000 carthage-0.30.dev1/bin/btrfs-rmrf
--rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2023-11-28 17:23:43.000000 carthage-0.30.dev1/bin/carthage
--rwxr-xr-x   0 runner    (1001) docker     (127)     1109 2023-11-28 17:23:43.000000 carthage-0.30.dev1/bin/carthage-console
--rwxr-xr-x   0 runner    (1001) docker     (127)     8282 2023-11-28 17:23:43.000000 carthage-0.30.dev1/bin/carthage-runner
--rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2023-11-28 17:23:43.000000 carthage-0.30.dev1/bin/carthage-vault-tool
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.849961 carthage-0.30.dev1/carthage/
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/cloud_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.849961 carthage-0.30.dev1/carthage/config/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/config/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/config/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/console.py
--rw-r--r--   0 runner    (1001) docker     (127)    13899 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/debian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.849961 carthage-0.30.dev1/carthage/dependency_injection/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/dependency_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67336 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/dependency_injection/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/dependency_injection/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9396 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.853961 carthage-0.30.dev1/carthage/entanglement/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/entanglement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10564 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/entanglement/instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/entanglement/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.853961 carthage-0.30.dev1/carthage/extra_packages/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/extra_packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/extra_packages/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/extra_packages/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.853961 carthage-0.30.dev1/carthage/extra_packages/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/extra_packages/resources/reprepro_distributions
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    22296 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    18480 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    36898 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.853961 carthage-0.30.dev1/carthage/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)    24595 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13854 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    32141 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/modeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.853961 carthage-0.30.dev1/carthage/network/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43746 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/mac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/network/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/pki.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.853961 carthage-0.30.dev1/carthage/podman/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/podman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33282 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/podman/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/podman/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/podman/modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/80-net-setup-link.rules
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/ansible-chroot-helper
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/class/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/class/DEFAULT.var
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/debconf/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/debconf/IPMI
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/debconf/SERIAL
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/disk_config/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/disk_config/DEFAULT
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/disk_config/LVM
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/files/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/files/etc/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/CLOUD_INIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/CLOUD_INIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/files/etc/pam.d/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/files/etc/pam.d/su/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/files/etc/pam.d/su/OPENROOT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/files/etc/resolv.conf/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/files/etc/resolv.conf/DEFAULT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       76 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/hooks/extrbase.CONTAINER2VM
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/hooks/repository.DEFAULT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/package_config/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/package_config/CLOUD_INIT
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/package_config/DEFAULT
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/package_config/GROW
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/package_config/IPMI
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/package_config/LVM
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.837961 carthage-0.30.dev1/carthage/resources/fai/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/scripts/CLOUD_INIT/
--rwxr-xr-x   0 runner    (1001) docker     (127)      251 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/scripts/CLOUD_INIT/10-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/scripts/GRUB_EFI/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/scripts/GRUB_EFI/10-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.857961 carthage-0.30.dev1/carthage/resources/fai/scripts/OPENROOT/
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/scripts/OPENROOT/10-setup
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/scripts/OPENROOT/20-setup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.861961 carthage-0.30.dev1/carthage/resources/fai/scripts/SERIAL/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/fai/scripts/SERIAL/20-SERIAL
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/hadron-xorg-modes
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/runner_console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.861961 carthage-0.30.dev1/carthage/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/bond-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/bond-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/bridge-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/bridge-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/default-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/network-base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/physical-link.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.861961 carthage-0.30.dev1/carthage/resources/templates/skeletons/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.861961 carthage-0.30.dev1/carthage/resources/templates/skeletons/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/skeletons/layout/carthage_plugin.py.mako
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/skeletons/layout/carthage_plugin.yml.mako
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/skeletons/layout/layout.py.mako
--rw-r--r--   0 runner    (1001) docker     (127)      548 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/skeletons/prototype.mako
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/vlan-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/vlan-network.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/vm-config.mako
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/vm-console.mako
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/templates/xfrm-netdev.mako
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/resources/test_ansible.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/runner_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    33781 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/setup_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/sonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/system_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/tb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.861961 carthage-0.30.dev1/carthage/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vault/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.865961 carthage-0.30.dev1/carthage/vmware/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/config_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17559 2023-11-28 17:23:43.000000 carthage-0.30.dev1/carthage/vmware/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/carthage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-11-28 17:23:52.000000 carthage-0.30.dev1/carthage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2023-11-28 17:23:52.000000 carthage-0.30.dev1/carthage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 17:23:52.000000 carthage-0.30.dev1/carthage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-28 17:23:52.000000 carthage-0.30.dev1/carthage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-28 17:23:52.000000 carthage-0.30.dev1/carthage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-11-28 17:23:43.000000 carthage-0.30.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 17:23:52.873961 carthage-0.30.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/carthage_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/inner_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/inner_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/machine_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/override-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/base_test.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/resources/dynamic_container/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/dynamic_container/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/inventory.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/local_playbook.yml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/test_ansible.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.841961 carthage-0.30.dev1/tests/resources/test_ansible_role/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/resources/test_ansible_role/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/test_ansible_role/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/test_playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/resources/true_container/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/resources/true_container/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/template-2.expected
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/templates/template-2.mako
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/templates/test.mako
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/templates/test_hash.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_carthage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19988 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_dependency_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_pki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 17:23:52.869961 carthage-0.30.dev1/tests/test_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_plugin/carthage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_plugin/carthage_plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_podman.py
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_setup_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-11-28 17:23:43.000000 carthage-0.30.dev1/tests/test_vmware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/
+-rw-r--r--   0 runner    (1001) docker     (127)    42976 2024-04-15 21:08:21.000000 carthage-0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 21:08:21.000000 carthage-0.32/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 21:08:26.754113 carthage-0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-15 21:08:21.000000 carthage-0.32/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.726113 carthage-0.32/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1248 2024-04-15 21:08:21.000000 carthage-0.32/bin/btrfs-rmrf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2758 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1109 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage-console
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8449 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage-runner
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2359 2024-04-15 21:08:21.000000 carthage-0.32/bin/carthage-vault-tool
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.730113 carthage-0.32/carthage/
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-15 21:08:21.000000 carthage-0.32/carthage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28784 2024-04-15 21:08:21.000000 carthage-0.32/carthage/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-15 21:08:21.000000 carthage-0.32/carthage/become_privileged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9396 2024-04-15 21:08:21.000000 carthage-0.32/carthage/carthage_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-15 21:08:21.000000 carthage-0.32/carthage/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-15 21:08:21.000000 carthage-0.32/carthage/cloud_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-15 21:08:21.000000 carthage-0.32/carthage/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-15 21:08:21.000000 carthage-0.32/carthage/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13899 2024-04-15 21:08:21.000000 carthage-0.32/carthage/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-15 21:08:21.000000 carthage-0.32/carthage/debian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/dependency_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dependency_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68732 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dependency_injection/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dependency_injection/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37395 2024-04-15 21:08:21.000000 carthage-0.32/carthage/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-15 21:08:21.000000 carthage-0.32/carthage/deployment_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-04-15 21:08:21.000000 carthage-0.32/carthage/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/entanglement/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-15 21:08:21.000000 carthage-0.32/carthage/entanglement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10564 2024-04-15 21:08:21.000000 carthage-0.32/carthage/entanglement/instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-15 21:08:21.000000 carthage-0.32/carthage/entanglement/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-15 21:08:21.000000 carthage-0.32/carthage/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/extra_packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.734113 carthage-0.32/carthage/extra_packages/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-15 21:08:21.000000 carthage-0.32/carthage/extra_packages/resources/reprepro_distributions
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 21:08:21.000000 carthage-0.32/carthage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-04-15 21:08:21.000000 carthage-0.32/carthage/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18480 2024-04-15 21:08:21.000000 carthage-0.32/carthage/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-15 21:08:21.000000 carthage-0.32/carthage/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42053 2024-04-15 21:08:21.000000 carthage-0.32/carthage/machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25507 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-15 21:08:21.000000 carthage-0.32/carthage/modeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44037 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/mac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-15 21:08:21.000000 carthage-0.32/carthage/network/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-15 21:08:21.000000 carthage-0.32/carthage/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-15 21:08:21.000000 carthage-0.32/carthage/pki.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-15 21:08:21.000000 carthage-0.32/carthage/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33518 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-15 21:08:21.000000 carthage-0.32/carthage/podman/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-15 21:08:21.000000 carthage-0.32/carthage/ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-04-15 21:08:21.000000 carthage-0.32/carthage/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-15 21:08:21.000000 carthage-0.32/carthage/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/80-net-setup-link.rules
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/ansible-chroot-helper
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/class/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/class/DEFAULT.var
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/debconf/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/debconf/IPMI
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/debconf/SERIAL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/disk_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/disk_config/DEFAULT
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/disk_config/LVM
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.718113 carthage-0.32/carthage/resources/fai/files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/files/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.718113 carthage-0.32/carthage/resources/fai/files/etc/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.718113 carthage-0.32/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.738113 carthage-0.32/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/cloud/cloud.cfg.d/20_use_netplan.cfg/CLOUD_INIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/cloud/ds-identify.cfg/CLOUD_INIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/files/etc/pam.d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/files/etc/pam.d/su/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/pam.d/su/OPENROOT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/files/etc/resolv.conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/files/etc/resolv.conf/DEFAULT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       76 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/hooks/extrbase.CONTAINER2VM
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/hooks/repository.DEFAULT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/package_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/CLOUD_INIT
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/DEFAULT
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/GROW
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/IPMI
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/package_config/LVM
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/carthage/resources/fai/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/CLOUD_INIT/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      251 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/CLOUD_INIT/10-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/GRUB_EFI/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/GRUB_EFI/10-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/OPENROOT/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/OPENROOT/10-setup
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/OPENROOT/20-setup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.742113 carthage-0.32/carthage/resources/fai/scripts/SERIAL/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/fai/scripts/SERIAL/20-SERIAL
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/hadron-xorg-modes
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/runner_console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bond-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bond-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bridge-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/bridge-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/default-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/gre-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/gre-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/network-base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/physical-link.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/resources/templates/skeletons/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/resources/templates/skeletons/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/layout/carthage_plugin.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/layout/carthage_plugin.yml.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/layout/layout.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/skeletons/prototype.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vlan-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vlan-network.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vm-config.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/vm-console.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/templates/xfrm-netdev.mako
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 21:08:21.000000 carthage-0.32/carthage/resources/test_ansible.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-15 21:08:21.000000 carthage-0.32/carthage/runner_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33781 2024-04-15 21:08:21.000000 carthage-0.32/carthage/setup_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:08:21.000000 carthage-0.32/carthage/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-15 21:08:21.000000 carthage-0.32/carthage/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-15 21:08:21.000000 carthage-0.32/carthage/sonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-15 21:08:21.000000 carthage-0.32/carthage/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-15 21:08:21.000000 carthage-0.32/carthage/system_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-15 21:08:21.000000 carthage-0.32/carthage/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-15 21:08:21.000000 carthage-0.32/carthage/tb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-04-15 21:08:21.000000 carthage-0.32/carthage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.746113 carthage-0.32/carthage/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vault/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.750113 carthage-0.32/carthage/vmware/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/config_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17559 2024-04-15 21:08:21.000000 carthage-0.32/carthage/vmware/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/carthage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 21:08:26.000000 carthage-0.32/carthage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-15 21:08:21.000000 carthage-0.32/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:08:26.754113 carthage-0.32/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-15 21:08:21.000000 carthage-0.32/tests/carthage_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-15 21:08:21.000000 carthage-0.32/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-15 21:08:21.000000 carthage-0.32/tests/inner_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 21:08:21.000000 carthage-0.32/tests/inner_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-15 21:08:21.000000 carthage-0.32/tests/machine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 21:08:21.000000 carthage-0.32/tests/override-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/base_test.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/dynamic_container/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/dynamic_container/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/inventory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/local_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/test_ansible.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.722113 carthage-0.32/tests/resources/test_ansible_role/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/test_ansible_role/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/test_ansible_role/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/test_playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/resources/true_container/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 21:08:21.000000 carthage-0.32/tests/resources/true_container/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 21:08:21.000000 carthage-0.32/tests/template-2.expected
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:08:21.000000 carthage-0.32/tests/templates/template-2.mako
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-15 21:08:21.000000 carthage-0.32/tests/templates/test.mako
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 21:08:21.000000 carthage-0.32/tests/templates/test_hash.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_become.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_carthage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20584 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_dependency_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9896 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_pki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:08:26.754113 carthage-0.32/tests/test_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_plugin/carthage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_plugin/carthage_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_podman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_setup_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-15 21:08:21.000000 carthage-0.32/tests/test_vmware.py
```

### Comparing `carthage-0.30.dev1/LICENSE` & `carthage-0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/PKG-INFO` & `carthage-0.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carthage
-Version: 0.30.dev1
+Version: 0.32
 Summary: A powerful Infrastructure as Code (IAC) framework
 Author-email: Sam Hartman <sam.hartman@hadronindustries.com>
 License: LGPL-3
 Project-URL: Homepage, https://github.com/hadron/carthage
 Project-URL: Documentation, https://carthage.readthedocs.io
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `carthage-0.30.dev1/README.rst` & `carthage-0.32/README.rst`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/bin/btrfs-rmrf` & `carthage-0.32/bin/btrfs-rmrf`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/bin/carthage` & `carthage-0.32/bin/carthage`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pathlib import Path
 
 if Path(__file__).parents[1].joinpath('carthage').exists():
     sys.path.insert(0, str(Path(__file__).parents[1].absolute()))
 
 from carthage.skeleton import *
 from carthage.utils import carthage_main_setup, carthage_main_argparser, carthage_main_run
-from carthage import deployment
+from carthage import carthage_deployment
 
 
 def new(args):
     dir = Path(args.name)
     if dir.is_absolute():
         raise ValueError('Specify a plugin name, not a directory path')
     if dir.exists():
@@ -56,21 +56,21 @@
                         help='Do not include LGPL-3 license block',
                         action='store_true',
                         )
     new_parser.add_argument('--git',
                         help='Create a git repository for the output',
                         action='store_true',
                         )
-    deployment.setup_deployment_commands(command_action)
+    carthage_deployment.setup_deployment_commands(command_action)
     args = carthage_main_setup(parser, ignore_import_errors=True)
     match args.cmd:
         case 'generate_requirements':
-            carthage_main_run(deployment.gen_requirements_command, args)
+            carthage_main_run(carthage_deployment.gen_requirements_command, args)
         case 'install_dependencies':
-            carthage_main_run(deployment.install_carthage_dependencies_command, args)
+            carthage_main_run(carthage_deployment.install_carthage_dependencies_command, args)
         case 'new':
             new(args)
     
 
 if __name__ == '__main__':
     main()
```

### Comparing `carthage-0.30.dev1/bin/carthage-console` & `carthage-0.32/bin/carthage-console`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/bin/carthage-runner` & `carthage-0.32/bin/carthage-runner`

 * *Files 3% similar despite different names*

```diff
@@ -211,15 +211,22 @@
 carthage.runner_commands.enable_runner_commands(ainjector)
 
 subcommands = loop.run_until_complete(
     console.setup_subcommands(ainjector, subparser_action))
 
 
 if args.help:
-    parser.print_help()
+    if len(unknown) >= 1:
+        cmd = unknown[0]
+    else:
+        cmd = ""
+    if cmd in subcommands:
+        subcommands[cmd].subparser.print_help()
+    else:
+        parser.print_help()
     sys.exit(2)
 args = parser.parse_args()
 
 if args.start is not None:
     args.actions.append('start')
 if args.stop is not None:
     args.actions.append('stop')
```

### Comparing `carthage-0.30.dev1/bin/carthage-vault-tool` & `carthage-0.32/bin/carthage-vault-tool`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/__init__.py` & `carthage-0.32/carthage/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,31 +29,41 @@
 
 
 from .kvstore import KvStore, KvConsistency,AssignmentsExhausted, persistent_seed_path
 
 __all__ += ['persistent_seed_path']
 
 
+from . import deployment
+from .deployment import  (
+    find_deployables, DeployableFinder,
+    find_orphan_deployables,
+    run_deployment, run_deployment_destroy, find_deployable, destroy_policy, DeletionPolicy)
+__all__ += ['find_deployable', 'find_deployables', 'DeployableFinder',
+            'find_orphan_deployables',
+            'run_deployment', 'run_deployment_destroy',
+            'destroy_policy', 'DeletionPolicy']
+
 
 from .network import Network, NetworkConfig, MacStore, V4Config, V4Pool
 
 __all__ += ['Network', 'NetworkConfig', 'MacStore', 'V4Config', 'V4Pool']
 
 
 
-from .machine import Machine, AbstractMachineModel, MachineCustomization, ContainerCustomization, FilesystemCustomization, customization_task, BareMetalMachine
+from .machine import ssh_jump_host, Machine, AbstractMachineModel, MachineCustomization, ContainerCustomization, FilesystemCustomization, customization_task, BareMetalMachine
 import carthage.ssh  # ssh import must come after machine
 from .ssh import RsyncPath
 import carthage.pki
 from . import ansible
 from . import cloud_init
 from .files import rsync_git_tree, git_tree_hash
 
 
-__all__ += ['Machine', 'rsync_git_tree',
+__all__ += ['ssh_jump_host', 'Machine', 'rsync_git_tree',
             'git_tree_hash',
             'RsyncPath',
             'AbstractMachineModel', 'MachineCustomization',
             'ContainerCustomization', 'FilesystemCustomization',
             'customization_task',
             'BareMetalMachine']
 
@@ -89,32 +99,36 @@
 from . import plugins
 
 __all__ += ['CarthagePlugin']
 
 base_injector = carthage.dependency_injection.Injector()
 base_injector.claim("base injector")
 carthage.config.inject_config(base_injector)
+base_injector.add_provider(deployment.MachineDeployableFinder)
 base_injector.add_provider(ssh.SshKey)
 base_injector.add_provider(ssh.AuthorizedKeysFile)
 base_injector.add_provider(asyncio.get_event_loop(), close=False)
 base_injector.add_provider(KvStore)
 base_injector.add_provider(MacStore)
 base_injector.add_provider(ansible.AnsibleConfig)
 base_injector.add_provider(carthage.network.external_network)
 base_injector.add_provider(carthage.network.BridgeNetwork, allow_multiple=True)
 
 base_injector.add_provider(InjectionKey(carthage.ssh.SshAgent), carthage.ssh.ssh_agent)
 base_injector.add_provider(carthage.pki.PkiManager)
 base_injector(carthage.cloud_init.enable_cloud_init_plugins)
 
-
 __all__ += ['base_injector']
 
 base_injector(plugins.load_plugin_from_package, sys.modules[__name__])
 
+# Things that need to import after base_injector is defined
+from . import deployment_commands
+base_injector(deployment_commands.register)
+
 @atexit.register
 def __done():
     asyncio.run(dependency_injection.shutdown_injector(base_injector))
     import sys
     sys.last_traceback = None
     sys.last_value = None
     import gc
```

### Comparing `carthage-0.30.dev1/carthage/ansible.py` & `carthage-0.32/carthage/ansible.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019, 2020, 2021, 2022, Hadron Industries, Inc.
+# Copyright (C) 2019, 2020, 2021, 2022, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -158,15 +158,21 @@
                     var_dict.update(await self.ainjector(p.host_vars, m))
                 except BaseException:
                     logger.exception(f"Error getting variables for {machine_name} from {p.name} plugin:")
                     raise
             if 'ansible_host' not in var_dict:
                 try:
                     var_dict['ansible_host'] = m.ip_address
-                except BaseException:
+                except Exception:
+                    pass
+            if 'ansible_ssh_common_args' not in var_dict:
+                try:
+                    if ssh_options := m.ssh_options:
+                        var_dict['ansible_ssh_common_args'] = " ".join(ssh_options)
+                except Exception:
                     pass
             hosts_dict[machine_name] = var_dict
             groups = []
             for p in self.group_plugins:
                 try:
                     groups += await self.ainjector(p.groups_for, m)
                 except BaseException:
@@ -409,24 +415,31 @@
         inventory=InjectionKey(AnsibleInventory, _optional=True),
         origin=InjectionKey(ansible_origin, _optional=True),
         log=InjectionKey(ansible_log, _optional=True),
         )
 async def run_play(hosts, play,
                    *, raise_on_failure=True,
                    gather_facts=False,
+                   base_vars=None,
                    vars=None, inventory=None,
                    log=None,
                    origin=None,
                    ainjector):
     '''
     Run a single Ansible play, specified as a python dictionary.
     The typical usage of this function is for cases where code wants to use an Ansible module to access some resource, especially when the results need to be programatically examined.  As an example, this can be used to examine the output of Ansible modules that gather facts.
 
     **If you are considering loading a YAML file, parsing it, and calling this function, you are almost certainly better served by :func:`run_playbook`.**
+    :param vars: Run through :func:`resolve_deferred` to produce a dictionary of variables.  Can be a function, an InjectionKey, or a dict.
+
+    :param base_vars: A dictionary of variables to set.  Unlike *vars* this must be a dictionary mapping strings to variable values or None.  *vars* is typically left to the user writing a Carthage layout, where as *base_vars* is used by higher-level constructs like :func:`ansible_role_task` to set variables related to privilege escalation from a customization or Machine.  Variables in *vars* override variables in *base_vars*.
+    
 '''
+    if base_vars is None:
+        base_vars = {}
     async with contextlib.AsyncExitStack() as stack:
         if origin and not isinstance(origin, NetworkNamespaceOrigin):
             root_path = await stack.enter_async_context(origin.filesystem_access())
             ansible_dir = stack.enter_context(tempfile.TemporaryDirectory(dir=root_path, prefix="ansible-"))
         else:
             ansible_dir = stack.enter_context(tempfile.TemporaryDirectory())
             root_path = "/"
@@ -436,18 +449,19 @@
             if isinstance(play, dict):
                 play = [play]
             pb = [{
                 'hosts': ":".join([h.name for h in hosts]),
                 'remote_user': 'root',
                 'gather_facts': gather_facts,
                 'tasks': play}]
-            if callable(vars):
-                vars = await ainjector(vars)
+            vars = await resolve_deferred(ainjector, item=vars, args={})
             if vars:
-                pb[0]['vars'] = vars
+                base_vars.update(vars)
+            if base_vars:
+                pb[0]['vars'] = base_vars
             f.write(yaml.dump(pb, default_flow_style=False))
         if inventory is None:
             with open(os.path.join(ansible_dir,
                                    "inventory.txt"), "wt") as f:
                 f.write("[hosts]\n")
                 for h in hosts:
                     if not h.running and hasattr(h, 'ansible_not_running_context'):
@@ -581,15 +595,15 @@
                 t.update(t['task'])
                 del t['task']
                 t['duration'] = SimpleNamespace(**t['duration'])
                 if t['name'] in self.tasks:
                     raise ValueError(f"{t['name']} duplicated")
                 if len(t['hosts']) == 1:
                     for v in t['hosts'].values():
-                        t.update(v)
+                        t.update({k:v[k] for k in v if k != 'name'})
                 self.tasks[t['name']] = SimpleNamespace(**t)
 
     @property
     def success(self):
         return (self.unreachable == 0) and (self.failures == 0)
 
     def __repr__(self):
@@ -608,31 +622,44 @@
         return res
 
 
 __all__ += ['AnsibleResult']
 
 
 def _handle_host_origin(host, origin):
+    base_vars = {}
+    runas_user = getattr(host, 'runas_user', None)
     if not isinstance(host, Machine) and hasattr(host, 'host'):
         host = host.host
+        if runas_user is None:
+            runas_user = host.runas_user
+    if runas_user != host.ssh_login_user:
+        base_vars['ansible_become_user'] = runas_user
+        base_vars['ansible_become'] = True
     if not origin:
-        return host, {}
+        return host, {}, base_vars
     if isinstance(host, Container) and not host.running:
-        return localhost_machine, dict(origin=dependency_quote(host))
-    return host, dict(origin=dependency_quote(host))
+        return localhost_machine, dict(origin=dependency_quote(host)), base_vars
+    return host, dict(origin=dependency_quote(host)), base_vars
 
 
 class ansible_playbook_task(setup_tasks.TaskWrapper):
 
     extra_attributes = frozenset({'dir', 'playbook'})
 
     def __init__(self, playbook, origin=False, **kwargs):
         async def func(inst):
-            host, extra_args = _handle_host_origin(inst, origin)
-            return await inst.ainjector(run_playbook, host, self.dir.joinpath(self.playbook), **extra_args)
+            host, extra_args, base_vars = _handle_host_origin(inst, origin)
+            args = []
+            if base_vars:
+                for k,v in base_vars.items():
+                    args.append(shlex.join(f'-e{k}={v}'))
+                    
+            return await inst.ainjector(run_playbook, host, self.dir.joinpath(self.playbook),  extra_args=args,
+                                        **extra_args)
         super().__init__(
             func=func,
             description=f'Run {playbook} playbook',
             **kwargs)
         self.playbook = playbook
         self.dir = None
 
@@ -649,39 +676,40 @@
 
 
 def ansible_role_task(roles, vars=None,
                       before=None, order=None, origin=False):
     '''
     A :func:`setup_task` to apply one or more ansible roles to a machine.
 
-    :param roles: A single role (as a string) or list of roles to include.  Roles can also be a list of dictionaries containing argumens to *import_role*.
+    :param roles: A single role (as a string) or list of roles to include.  Roles can also be a list of dictionaries containing arguments to *import_role*.
 
     :param vars: An optional dictionary of ansible variable assignments.
     :param origin: If True, use host as origin from which to run ansible.
 
     '''
     @setup_tasks.setup_task(f'Apply {roles} ansible roles',
                             before=before, order=order)
     @inject(ainjector=AsyncInjector)
     async def apply_roles(self, ainjector):
-        host, extra_args = _handle_host_origin(self, origin)
+        host, extra_args, base_vars = _handle_host_origin(self, origin)
         play = []
         for r in roles:
             if isinstance(r, dict):
                 r_dict = r
             else:
                 r_dict = dict(name=r)
             play.append(dict(
                 import_role=r_dict))
 
         return await ainjector(
             run_play,
             hosts=[host],
             play=play,
             vars=vars,
+            base_vars=base_vars,
             **extra_args
         )
     if isinstance(roles, (str, dict)):
         roles = [roles]
     return apply_roles
```

### Comparing `carthage-0.30.dev1/carthage/carthage_plugin.yml` & `carthage-0.32/carthage/carthage_plugin.yml`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/cloud_init.py` & `carthage-0.32/carthage/cloud_init.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/config/__init__.py` & `carthage-0.32/carthage/config/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/config/base.py` & `carthage-0.32/carthage/config/base.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/config/layout.py` & `carthage-0.32/carthage/config/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,15 @@
             for p in d['plugins']:
                 if (not ':' in p) and (p == '..' or p == '.' or '/' in p):
                     p = base_path.joinpath(p)
                 enable_plugin(p, ignore_import_errors=ignore_import_errors)
             del d['plugins']
         if 'include' in d:
             for include in d['include']:
+                include = injector(ConfigPath, include)
                 include = base_path.joinpath(include)
                 with include.open("rt") as include_file:
                     self.load_yaml(include_file, ignore_import_errors=ignore_import_errors)
             del d['include']
         try: self._load(d, injector, self._schema, "")
         except KeyError:
             if not ignore_import_errors: raise
```

### Comparing `carthage-0.30.dev1/carthage/config/schema.py` & `carthage-0.32/carthage/config/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
 import sys
 from ipaddress import IPv6Address, IPv4Address, IPv4Network, IPv6Network
 from pathlib import Path
+import types
 from ..dependency_injection import inject, Injectable, InjectionKey, Injector, partial_with_dependencies, InjectorClosed, InjectionFailed, injection_failed_unlogged
 
 
 def config_key(k):
     return InjectionKey("config/" + k)
 
 
@@ -114,14 +115,16 @@
         '''
         Represents an item in a configuration schema
 '''
 
         __slots__ = ('name', 'type', 'default', 'key')
 
         def __init__(self, name, type_, default):
+            if isinstance(type_, types.GenericAlias):
+                type_ = type_.__origin__
             assert isinstance(type_, type), f'{name} config key must be declared with a type not {type_}'
             if type_ is bool:
                 from .types import ConfigBool
                 type_ = ConfigBool
             elif type_ is str:
                 from .types import ConfigString
                 type_ = ConfigString
```

### Comparing `carthage-0.30.dev1/carthage/config/types.py` & `carthage-0.32/carthage/config/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,34 +29,42 @@
 
     '''A string that substitutes
 
     * ``{key}`` with the result of that config key
 
     * ``{plugin:selector}`` with the lookup of *selector* using the *plugin* :ref:`.ConfigLookupPlugin`
 
-    Backslash scapes the next character always; ``${var}`` is reserved for :ref:`ConfigPath` use.
+    * ``${var}`` the environment variable *var*
+
+    * ``${var-default}`` The environment variable *var* else *default*
+    
+
+    Backslash scapes the next character always;
 
     '''
 
     @classmethod
     def parse(cls, s, config, injector):
         def tok(i, awaiting_brace):
             # takes an iterator to consume input characters
             lastch = None
             for c in i:
+                if lastch == '$' and c != '{':
+                    yield '$'
                 if lastch == '\\':
                     yield c
                 elif c == '\\':
                     # one backslash always eats itself.
                     pass
+                elif c == '$':
+                    # hold to see if next character is {
+                    pass
                 elif c == '{':
-                    if lastch == "$":
-                        yield '{'
-                        yield from tok(i, True)
-                        yield "}"
+                    if lastch == '$':
+                        yield from iter(cls.subst_var("".join(tok(i, True))))
                     else:
                         yield from iter(cls.subst(
                             "".join(tok(i, True)),
                             config=config,
                             injector=injector
                         ))
                 elif c == '}':
@@ -70,36 +78,48 @@
 
             if awaiting_brace:
                 raise ValueError(f"Missing right brace in `{s}'")
 
         return "".join(tok(iter(s), False))
 
     @staticmethod
+    def subst_var(s):
+        '''When parse encounters ${foo} in a pattern, it calls subst_var(foo); we handle environment substitutions like:
+
+        * ``foo``: look up ``foo in environment``
+
+        * ``foo-bar`` look up ``foo`` in environment; if not found return ``bar``
+
+        '''
+        var, sep, default = s.partition('-')
+        return os.environ.get(var, default)
+    
+    @staticmethod
     def subst(s, *, config, injector):
         plugin, sep, selector = s.partition(':')
         if sep == '':
-            return getattr_path(config, s)
+            return str(getattr_path(config, ConfigString.parse(s,config, injector)))
         else:
             try:
                 plugin = injector.get_instance(InjectionKey(ConfigLookupPlugin, name=plugin))
             except KeyError:
                 raise KeyError(f'Config lookup plugin {plugin} not found') from None
-            return plugin(selector)
+            return plugin(ConfigString.parse(selector,config,injector))
 
     def __new__(cls, s, *, injector):
         config = injector(ConfigLayout)
-        return str.__new__(str, cls.parse(os.path.expandvars(s), config, injector))
+        return str.__new__(str, cls.parse(s, config, injector))
 
 
 @inject(
     injector=Injector)
 class ConfigPath(ConfigString):
 
     def __new__(cls, s, *, injector):
-        return super().__new__(ConfigString, os.path.expanduser(s),
+        return super().__new__(ConfigString, os.path.expanduser(str(s)),
                                injector=injector)
 
 
 class ConfigBool:
 
     "A type that can be subtyped to be injectable used instead of bool"
```

### Comparing `carthage-0.30.dev1/carthage/console.py` & `carthage-0.32/carthage/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             except Exception as e:
                 print(f'[{num}]-> exception')
                 traceback.print_exc()
 
         if isinstance(obj, collections.abc.Coroutine):
             self.history_num += 1
             num = self.history_num
-            future = asyncio.ensure_future(obj, loop=self.loop)
+            future = asyncio.run_coroutine_threadsafe(obj, loop=self.loop)
             future.add_done_callback(future_callback)
             print(f'[{num}]: async {obj.__name__}')
             self.history[num] = future
             self.loop.call_soon_threadsafe(CarthageConsole.noop)
         else:
             self.orig_displayhook(obj)
 
@@ -208,14 +208,21 @@
             else:
                 with injection_failed_unlogged():
                     try:
                         v = await ainjector.get_instance_async(k)
                     except InjectionFailed:
                         continue
 
+            # Unfortunately depending on when commands are registered
+            # by plugins, they are likely registered before the layout
+            # ainjector is established. Explicitly override the
+            # ainjector in the command so that it can access layout
+            # objects.
+            v.injector = ainjector.injector
+            v.ainjector = ainjector
             if await v.should_register():
                 v.register(subparser_action)
             subcommands[v.name] = v
         return subcommands
 
     def runsource(self, source, filename):
         if self.subcommands:
@@ -226,14 +233,17 @@
                 except argparse.ArgumentError as e:
                     print(e)
                     return
                 if args.cmd == 'help':
                     self.subcommands_parser.print_help()
                     return
                 subcommand = self.subcommands[args.cmd]
+                if args.help:
+                    subcommand.subparser.print_help()
+                    return
                 future = asyncio.run_coroutine_threadsafe(self.ainjector(subcommand.run, args), loop=self.loop)
                 try: future.result()  #concurrent not asyncio future
                 except Exception as e:
                     traceback.print_exception(e)
                 return
         return super().runsource(source, filename)
 
@@ -283,17 +293,19 @@
 
     async def should_register(self):
         ''' Returns True if this command should be registered.  For example, start_machine might wish to confirm that the layout has Machines before registering.  This function should bd work even if for example there is no CarthageLayout.
 '''
         return True
 
     def register(self, subparser_action):
-        parser = subparser_action.add_parser(
-            self.name, **self.subparser_kwargs)
-        self.setup_subparser(parser)
+        self.subparser = subparser_action.add_parser(
+            self.name, add_help=False,
+            **self.subparser_kwargs)
+        self.setup_subparser(self.subparser)
+        self.subparser.add_argument('--help', action='store_true', help='Print Usage')
 
     @classmethod
     def default_class_injection_key(cls):
         return InjectionKey(CarthageRunnerCommand, name=cls.name)
 
 
 __all__ += ['CarthageRunnerCommand']
```

### Comparing `carthage-0.30.dev1/carthage/container.py` & `carthage-0.32/carthage/container.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/debian.py` & `carthage-0.32/carthage/debian.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/dependency_injection/__init__.py` & `carthage-0.32/carthage/dependency_injection/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/dependency_injection/base.py` & `carthage-0.32/carthage/dependency_injection/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,17 @@
 
         '''
         def filter_for_constraints(k):
             return all(map(lambda c: c in k.constraints, constraints))
         if isinstance(predicate, list):
             constraints = predicate
             predicate = filter_for_constraints
+        if isinstance(stop_at, AsyncInjector):
+            stop_at = stop_at.injector
+        assert isinstance(stop_at, (Injector, type(None)))
         if stop_at == self:
             result = {}  # stop here
         elif stop_at and not self.parent_injector:
             raise ValueError(f'{stop_at} was not in the parent chain')
         elif self.parent_injector:
             result = {k: True for k in self.parent_injector.filter(target, predicate, stop_at=stop_at)}
         else:  # no stop_at; ended chain
@@ -435,15 +438,15 @@
         for k in self.filter(target, predicate, stop_at=stop_at):
             if ready is not None:
                 k = InjectionKey(k, _ready=ready)
             res = self.get_instance(k)
             if res is not None:
                 yield k, res
 
-    def inspect(self, *,key_filter=None, include_parent:bool = False):
+    def inspect(self, *, key_filter=None, include_parent:bool = False):
         '''
         Inspect the contents of this injector.
         This is a generator yielding key, :class:`~InjectedDependencyInspector` pairs for each dependency provided by the injector.
 
         :param key_filter: A function that takes a key and returns true if  the inspector should inspect the dependency for this key.
 
         :param include_parent: By default only this injector is  covered; if True, then the inspection recurses into the parent.
@@ -695,16 +698,22 @@
                     dependency = cls._injection_dependencies[k]
                     if isinstance(provider, Injectable) and not provider.satisfies_injection_key(dependency):
                         raise UnsatisfactoryDependency(dependency, provider)
                     sub_injector.add_provider(dependency, provider, close=False)
             for k, d in (cls._injection_dependencies.items()) if dks else []:
                 if d is None:
                     continue
-                injector.get_instance(d, placement=kwarg_place(k),
+                try:
+                    injector.get_instance(d, placement=kwarg_place(k),
                                       loop=_loop, futures=futures)
+                except KeyError as e:
+                    if _instantiation_context:
+                        raise InjectionFailed(current_instantiation()) from e
+                    else:
+                        raise
             if futures:
                 fut = asyncio.ensure_future(callback(futures))
                 if current_instantiation():
                     fut.set_name(f'{current_instantiation()}')
                 else:
                     fut.set_name(f'Instantiate {cls} for {self}')
                 return fut
@@ -1192,22 +1201,22 @@
         self._async_ready_state = ReadyState.READY
         return self
 
     async def async_resolve(self):
         '''Returns None or an object that should replace *self* in providing dependencies.'''
         return None
 
-    async def async_become_ready(self, cycle_set=None):
+    async def async_become_ready(self, cycle_set=None, dependency_key=None):
 
         '''
         Interface point to request that a dependency be fully ready (:meth:`async_ready` is called exactly once).  This function manages tracking to make sure that async_ready is called once, and waits for that call if needed.
         This method also makes sure that dependencies registered with :func:`.inject` are made ready before :meth:`async_ready` is called.
         Subclasses should not override this method but instead should override :meth:`async_ready`.
         '''
-        with AsyncBecomeReadyContext(self):
+        with AsyncBecomeReadyContext(self, dependency_key=dependency_key):
             if self._async_ready_state == ReadyState.NOT_READY:
                 raise RuntimeError("Resolution should have already happened")
             elif self._async_ready_state == ReadyState.RESOLVED:
                 self._ready_future = asyncio.ensure_future(_handle_async_deps(self, cycle_set))
                 self._ready_future.set_name(f'Async dependencies for {self}')
                 self._async_ready_state = ReadyState.READY_PENDING
                 try:
@@ -1322,14 +1331,22 @@
                 k = InjectionKey(k, _ready=ready)
             results.append(self.get_instance_async(k))
             result_keys.append(k)
         results = await asyncio.gather(*results)
         zipped = zip(result_keys, results)
         return [z for z in zipped if z[1] is not None]
 
+async def _handle_1_dep(val, cycle_set, dependency_key):
+    with AsyncBecomeReadyContext(val, dependency_key) as context:
+        try: await val.async_become_ready(cycle_set=cycle_set, dependency_key=dependency_key)
+        except Exception as e:
+            tb_utils.filter_before_here(e)
+            failed_instantiation(context, e)
+            raise InjectionFailed(context) from e
+
 
 async def _handle_async_deps(obj, cycle_set):
     if cycle_set is None:
         cycle_set = set()
     futures = []
     try:
         repr = repr(obj)
@@ -1339,36 +1356,49 @@
         if dep is None:
             continue
         if dep.ready is False:
             continue
         val = getattr(obj, attr, None)
         if val is None:
             continue
-        if not isinstance(val, AsyncInjectable):
+        if is_obj_ready(val):
             continue
         if id(val) in cycle_set:
             import warnings
             warnings.warn(f'{obj}.async_become_ready: @inject({attr}={dep}) produced dependency cycle with {val}')
             continue
         cycle_set.add(id(val))
-        future = asyncio.ensure_future(val.async_become_ready(cycle_set=cycle_set))
+        future = asyncio.ensure_future(_handle_1_dep(val, cycle_set=cycle_set, dependency_key=dep))
         future.set_name(f'Dependency become ready for {dep} of {repr}')
         futures.append(future)
 
     gather = asyncio.gather(*futures)
-    await gather
+    try: await gather
+    except Exception as e:
+        tb_utils.filter_chatty_modules(e, _chatty_modules, None)
+        raise
     return await obj.async_ready()
 
 
 # Injector cross reference support
 class InjectorXrefMarkerMeta(type):
 
     def __repr__(self):
         return f'injector_xref({self.injectable_key}, {self.target_key})'
 
+    def __hash__(self):
+        try:return hash(self.injectable_key)+hash(self.target_key)
+        except AttributeError:
+            return hash(self.target_key)
+
+    def __eq__(self, other):
+        if not isinstance(other, InjectorXrefMarkerMeta): return NotImplemented
+        if getattr(self, 'injectable_key', None) != getattr(other, 'injectable_key', None): return False
+        if self.target_key != other.target_key: return False
+        return True
 
 class InjectorXrefMarker(AsyncInjectable, metaclass=InjectorXrefMarkerMeta):
 
     # A separate subclass is created for each injector_xref with one
     # class attributes: target_key.  If possible our __new__ entirely
     # resolves to target_key and simply returns that object.  If that
     # requires asynchronous action, then we actually instantiate
```

### Comparing `carthage-0.30.dev1/carthage/dependency_injection/introspection.py` & `carthage-0.32/carthage/dependency_injection/introspection.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from __future__ import annotations
 
 import contextvars
 import dataclasses
 import traceback
 
+from ..utils import memoproperty
+
 _current_instantiation = contextvars.ContextVar('current_instantiation', default=None)
 
 __all__ = []
 
 
 class GetItemSet(set):
 
@@ -248,39 +250,71 @@
 
 
 __all__ += ['current_instantiation']
 
 
 class AsyncBecomeReadyContext(BaseInstantiationContext):
 
-    def __init__(self, obj):
+    def __init__(self, obj, dependency_key):
         super().__init__(obj.injector)
+        if dependency_key is not None:
+            # Setting self.key to None may make the instantiation
+            # failed tracking mechanisms sad; they may expect that key
+            # is always an InjectionKey if present, so check with hasattr before accessing key.
+            self.key = dependency_key
         self.obj = obj
         self.entered = False
 
     @property
     def description(self):
-        return f'{self.obj}.async_become_ready()'
+        return f'bringing {self.obj} to ready'
 
     def __enter__(self):
+        # If the parent context is an instantiation context for
+        # ourself (async_become_ready as part of get_instance_async),
+        # or the parent is already an AsyncBecomeReadyContext for
+        # ourself (_handle_1_dep), we do not need an extra level of
+        # context.
         parent = _current_instantiation.get()
         if isinstance(parent, InstantiationContext) and parent.provider.provider is self.obj:
             return parent
+        elif isinstance(parent,AsyncBecomeReadyContext) and self.obj is parent.obj:
+            return parent
         self.entered = True
-        return super().__enter__()
+        res =  super().__enter__()
+        if self.parent:
+            self.parent.dependency_progress(self.dependency_key, self)
+        return res
 
     def __exit__(self, *args):
         if self.entered:
             super().__exit__(*args)
             self.done()
         return False
 
+    def get_value_no_instantiate(self):
+        return self.obj
+
     def get_dependencies(self):
         return get_dependencies_for(self.obj, self.obj.injector)
 
+    def done(self):
+        super().done()
+        if self.entered and self.parent:
+            self.parent.dependency_final(self.dependency_key, self)
+
+    @memoproperty
+    def dependency_key(self):
+        if hasattr(self, 'key'):
+            return self.key
+        try:
+            return str(self.obj)
+        except Exception:
+            return repr(self.obj)
+    
 
 __all__ += ['AsyncBecomeReadyContext']
 
 
 def get_dependencies_for(obj, injector):
     if not hasattr(obj, '_injection_dependencies'):
         return
@@ -322,20 +356,41 @@
     failure = FailedInstantiation(exception=exception, dependency=dependency)
     all_instantiation_failures[id(injector), key] = failure
     if len(dependency) == 0:
         failed_instantiation_leaves[id(injector), key] = failure
     injector.emit_event(
         key, "dependency_instantiation_failed",
         failure,
+        context=context,
         adl_keys={base.InjectionKey(base.Injector)})
     
 
 __all__ += ['failed_instantiation']
 
 all_instantiation_failures: dict[tuple, FailedInstantiation] = {}
 failed_instantiation_leaves: dict[tuple, FailedInstantiation] = {}
 
 __all__ += ['all_instantiation_failures', 'failed_instantiation_leaves']
 
+def calculate_reverse_dependencies(obj: object, /, injector,
+                                   *, reverse_dependencies: dict[object,set[object]],
+                                   filter=lambda o:True):
+    def visit(dependencies,val, cycle):
+        reverse_dependencies.setdefault(val, set())
+        for dependency in dependencies:
+            try:
+                inner_val = dependency.get_value(ready=False)
+            except KeyError: continue
+            if not filter(inner_val): continue
+            if inner_val in cycle: continue
+            found_dependency = True
+            if inner_val not in reverse_dependencies:
+                reverse_dependencies.setdefault(inner_val, set())
+            reverse_dependencies[inner_val] |= {val}
+            visit(get_dependencies_for(inner_val, dependency.injector), inner_val, cycle=cycle|{inner_val})
+            
+    visit(get_dependencies_for(obj, injector),
+          obj, {obj})
 
+__all__ += ['calculate_reverse_dependencies']
 
 from . import base
```

### Comparing `carthage-0.30.dev1/carthage/deployment.py` & `carthage-0.32/carthage/carthage_deployment.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/dns.py` & `carthage-0.32/carthage/dns.py`

 * *Files 22% similar despite different names*

```diff
@@ -87,16 +87,18 @@
         if not domain: return
         zone = await self.ainjector.get_instance_async(InjectionKey(
             DnsZone, name=domain, addressing='public', _ready=True, _optional=True))
         if zone is None:
             zone = await self.ainjector.get_instance_async(InjectionKey(DnsZone, role='public_zone', _ready=True, _optional=True))
         if zone is None and link.public_dns_name:
             logger.error(f'No public zone found for {name}')
+            return
         elif zone is None:
             logger.debug(f'No public zone found for {name}, but it may not be required')
+            return
             
         if not zone.contains(name):
             logger.error(f'Not setting DNS for {model}: {name} does not fall within {zone.name}')
         else:
             logger.debug(f'{name} is at {str(link.merged_v4_config.public_address)}')
             await zone.update_records((name, 'A', [str(link.merged_v4_config.public_address)]),
                                       ttl=30)
@@ -105,57 +107,101 @@
         super().__init__(**kwargs)
         if attach_to is None:
             attach_to = self.injector
         attach_to.add_event_listener(InjectionKey(NetworkLink), 'public_address', self.public_ip_updated)
 
 
 __all__ += ['PublicDnsManagement']
+class DnsManagement(AsyncInjectable):
+
+    '''
+Update a DNS zone when :class:`NetworkLinks` change IP  address.  This can be attached to an existing injector if *attach_to* is included on construction.  More typically, this can be used as a Carthage modeling mixin.
+    Typical usage in that mode::
+
+        class some_enclave(Enclave, DnsManagement):
+
+            domain = "machines.example.com"
+            add_provider(InjectionKey(DnsZone, name='machines.example.com', addressing='private'), some_dns_zone)
+
+            class some_machine(MachineModel): ...
+
+    Then, when `some_machine` gains an IP address, an `A` record will be created.
+
+    '''
+
+    async def ip_updated(self, target, **kwargs):
+        link = target
+        model = link.machine
+        name = link.dns_name
+        if name is None: name = model.name
+        if not name: return     # dns_name = ''
+        if not link.merged_v4_config.address:
+            logger.debug('%s: no address', name)
+            return
+        logger.debug(f'{name} is at {str(link.merged_v4_config.address)}')
+        await self.ainjector(
+            update_dns_for,
+            private_name=name,
+            private_records=[('A', str(link.merged_v4_config.address))])
+            
+    def __init__(self, attach_to=None, **kwargs):
+        super().__init__(**kwargs)
+        if attach_to is None:
+            attach_to = self.injector
+        attach_to.add_event_listener(InjectionKey(NetworkLink), 'address', self.ip_updated)
+
+
+__all__ += ['DnsManagement']
 
 @inject(ainjector=AsyncInjector)
-async def update_dns_for(name, *,
-                         public_records,
-                         private_records,
+async def update_dns_for(*,
+                         private_name=None,
+                         public_name=None,
+                         public_records=None,
+                         private_records=None,
                          ainjector, ttl=300,
                          ):
     '''
-    Look up the zone for *name*, and update records within it.
+    Look up the zone for *public_name*, and *private_name*and update records within it.
     For public records,  ``InjectionKey(DnsZone, name=domain, addressing='public')`` is used.
 
-    If a public zone is found, then ``InjectionKey(DnsZone, name=domain, addressing='private')`` is used for private records.  If a public zone is not found, then ``InjectionKey(DnsZone, name=domain)`` will also be accepted for private records.
-
-    The zone keys used are dependent on what zones are registered in the injector hierarchy, **not** on what parameters are passed in.  That is, if a public zone exists, and only private records are passed in, private dns will only be updated if an explicit ``addressing='private'`` zone is provided by the injector.
+     ``InjectionKey(DnsZone, name=domain, addressing='private')`` is used for private records.  If that zone is not found, then ``InjectionKey(DnsZone, name=domain)`` will also be accepted for private records.
     
 
     :param records: A sequence of (rrtype, values)
 
     Example Usage::
 
         await ainjector(update_dns_for,
-            "www.foo.com", public_records=[('CNAME', 'foo.com')])
+            public_name="www.foo.com", public_records=[('CNAME', 'foo.com')])
 
     '''
-    head, sep, domain = name.partition('.')
-    public_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=domain, addressing='public', _optional=True))
-    private_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=domain, addressing='private', _optional=True))
-    if (not public_zone) and (not private_zone):
-        private_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=domain, _optional=True))
+    if public_name:
+        public_head, sep, public_domain = public_name.partition('.')
+        public_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=public_domain, addressing='public', _optional=True))
+    else: public_zone = None
+    if private_name:
+        private_head, sep, private_domain = private_name.partition('.')
+        private_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=private_domain, addressing='private', _optional=True))
+        if  (not private_zone):
+            private_zone = await ainjector.get_instance_async(InjectionKey(DnsZone, name=private_domain, _optional=True))
     futures = []
     if public_records and public_zone:
         args = []
         for type, value in public_records:
-            args.append((name, type, value))
+            args.append((public_name, type, value))
         futures.append(asyncio.ensure_future(public_zone.update_records(*args, ttl=ttl)))
     elif public_records:
-        logger.warning(f'No public zone for {name}')
+        logger.warning(f'No public zone for {public_name}')
     if private_zone and private_records:
         args = []
         for type, value in private_records:
-            args.append((name, type, value))
+            args.append((private_name, type, value))
         futures.append(asyncio.ensure_future(private_zone.update_records(*args, ttl=ttl)))
 
     if private_zone is None and public_zone is None:
-        logger.warning(f'No DNS zone for {name}')
+        logger.warning(f'No DNS zone for {public_name or private_name}')
     if futures:
         await asyncio.gather(*futures)
         
 
 __all__ += ['update_dns_for']
```

### Comparing `carthage-0.30.dev1/carthage/entanglement/__init__.py` & `carthage-0.32/carthage/entanglement/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/entanglement/instrumentation.py` & `carthage-0.32/carthage/entanglement/instrumentation.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/entanglement/server.py` & `carthage-0.32/carthage/entanglement/server.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/event.py` & `carthage-0.32/carthage/event.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/extra_packages/plugin.py` & `carthage-0.32/carthage/extra_packages/plugin.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/extra_packages/repo.py` & `carthage-0.32/carthage/extra_packages/repo.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/files.py` & `carthage-0.32/carthage/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         options = dict(_fg=True)
     else: options = dict(_bg=True, _bg_exc=False)
     config = injector(ConfigLayout)
     path = Path(config.checkout_dir) / repo
     os.makedirs(config.checkout_dir, exist_ok=True)
     if path.exists():
         return sh.git("pull", "--rebase",
-                      _cwd=pat,
+                      _cwd=path,
                       **options)
     else:
         return sh.git("clone",
                       url, str(path),
                       **options)
```

### Comparing `carthage-0.30.dev1/carthage/image.py` & `carthage-0.32/carthage/image.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/kvstore.py` & `carthage-0.32/carthage/kvstore.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/local.py` & `carthage-0.32/carthage/local.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/machine.py` & `carthage-0.32/carthage/machine.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import shlex
 import tempfile
 import typing
 from pathlib import Path
 
 from .dependency_injection import *
 from .config import ConfigLayout
-from .ssh import SshKey, SshAgent, RsyncPath
+from .ssh import SshKey, SshAgent, RsyncPath, ssh_user_addr, ssh_handle_jump_host
 from .utils import memoproperty
 from . import sh
 import carthage.ssh
 from .setup_tasks import SetupTaskMixin, setup_task, TaskWrapperBase, TaskInspector
 import logging
 logger = logging.getLogger("carthage")
 
@@ -63,38 +63,86 @@
             ssh_online = machine.machine_running_ssh_online
         self.ssh_online = ssh_online
 
 
 ssh_origin = InjectionKey('ssh-origin')
 ssh_origin_vrf = InjectionKey("ssh-origin-vrf")
 
+#: A :class:`Machine` to use as a jump host.
+ssh_jump_host = InjectionKey('ssh_jump_host')
+
 
 class SshMixin:
-    '''An Item that can be sshed to.  Will look for the ssh_origin
-    injection key.  If found, this should be a container.  The ssh will be
-    launched from within the network namespace of that container in order
-    to reach the appropriate devices.  Requires ip_address to be made
-    available.  Requires an carthage.ssh.SshAgent be injectable.
+    '''
+    An item that accepts ssh connections.
+
+    :attr:`ip_address` represents  the endpoint to connect to in order to manage the resource via ssh.  In early Carthage development, this was always an IP address. More recently, this can be an IP address or hostname.
+
+    The :data:`ssh_origin` injection key is used to look up a :class:`~carthage.container.Container` from which  the ssh should be run.  If *ssh_origin* is provided by the injector hierarchy, then Carthage enters the network namespace of the Container before running ssh. Note that the mount namespace is not typically used, so the host's ssh binary and keys are used.  There is support for using a Linux VRF within the namespace; see :func:`carthage.network.access_ssh_origin` for details.
+
+    If the injector hierarchy provides :data:`ssh_jump_host`, then that is used as a *ProxyJump* host.
+
+    If neither *ssh_origin* nor *ssh_jump_host* are provided then Carthage connects directly to *ip_address*.
+
+    If *ssh_origin* is provided but not *ssh_jump_host*, then Carthage enters the network namespace of *ssh_origin* and connects to *ip_address* within the context of that namespace (possibly within a VRF within that namespace). DNS resolution for the connection to *ip_address* may be performed by the host in the host's network namespace (systemd-resolved'sNSS plugin or similar) or it may be performed in the *ssh_origin* network namespace using the host's nameserver configuration.  It is best if *ip_address* actually is an IP address to avoid this ambiguity.
+
+    If *ssh_jump_host* is provided but not *ssh_origin*, then Carthage first connects to *ssh_jump_host* and tunnels a connection to *ip_address* within the jump host connection. The DNS resolution for the connection to *ip_address* is performed by the jump host; the DNS resolution for the connection to the jump host is performed by the host.
+
+    If both *ssh_origin* and *ssh_jump_host* are provided:  Carthage enters the namespace of *ssh_origin*.  Within that namespace it establishes an ssh connection to *ssh_jump_host*.  Over that connection it tunnels to *ip_address*. DNS resolution for the connection to *ssh_jump_host* is ambiguous; it is best if *ip_address* is an IP address in this case.  DNS resolution to *ip_address* is performed by *ssh_jump_host*.
+
+
     '''
 
     _ssh_online_required = True
 
     @memoproperty
     def ip_address(self):
         '''The IP address or name at which this machine should be managed.'''
         try:
             return self.model.ip_address
         except AttributeError:
             raise NotImplementedError from None
 
     @memoproperty
     def ssh_options(self):
+        jump_host_options = ssh_handle_jump_host(self.ssh_jump_host)
         if hasattr(self.model, 'ssh_options'):
-            return self.model.ssh_options
-        return ('-lroot', )
+            return self.model.ssh_options + jump_host_options
+        return jump_host_options
+
+    @memoproperty
+    def ssh_jump_host(self):
+        '''
+        An :class:`SshMixin` or string to use as a jump host.
+        '''
+        return self.injector.get_instance(InjectionKey(ssh_jump_host, _ready=False, _optional=True))
+
+    @memoproperty
+    def ssh_login_user(self):
+        '''
+        The ssh user to log in as. Defaults to root, can be set either on the machine or the model.
+        '''
+        try:
+            if self.model.ssh_login_user:
+                return self.model.ssh_login_user
+        except AttributeError:
+            pass
+        return 'root'
+
+    @memoproperty
+    def runas_user(self):
+        '''
+        The user to run commands as.  Mechanisms like :class:`carthage.become_privileged.BecomePrivilegedMixin` provide a mechanism to  use a privilege gateway like ``sudo`` so that *runas_user* can differ from :attr:`ssh_login_user`.
+        Can be set on the machine or model.  Defaults to root.
+        '''
+        try:
+            if self.model.runas_user:
+                return self.model.runas_user
+        except AttributeError: pass
+        return 'root'
 
     @memoproperty
     def ssh_online_retries(self):
         if hasattr(self.model, 'ssh_online_retries'):
             assert isinstance(self.model.ssh_online_retries, int), "ssh_online_retries must be `int`"
             return self.model.ssh_online_retries
         return 60
@@ -130,21 +178,21 @@
             ip_address = self.ip_address
             ssh_origin_container.done_future().add_done_callback(self.ssh_recompute)
             return self.injector(access_ssh_origin).bake(
                 "/usr/bin/ssh",
                 *key_options,
                 *options,
                 *self.config_layout.global_ssh_options.split(),
-                ip_address,
+                ssh_user_addr(self),
                 _env=ssh_agent.agent_environ)
         else:
             return sh.ssh.bake(*key_options,
                                *options,
                                *self.config_layout.global_ssh_options.split(),
-                               self.ip_address,
+                               ssh_user_addr(self),
                                _env=ssh_agent.agent_environ)
 
     def rsync(self, *args):
         '''
         Call rsync with given arguments.
         An argument may be a :class:`.RsyncPath` generated by :meth:`rsync_path`.  Such a path encapsulates a host name and a path.  When *rsync* is called, Carthage
         finds the appropriate ssh_origin to select the right namespace for rsync.
@@ -244,14 +292,17 @@
     When :meth:`resolve_networking` is called, if *self.injector* provides :ref:`network_namespace_key`,  then the network_links are reused from the object providing that dependency.  Typical usage is for a :class:`~carthage.oci.OciPod` or similar network namespace in which a :class:`AbstractMachineModel` will be run to provide *network_namespace_key*.
     
 
     '''
 
     network_links: typing.Mapping[str, carthage.network.NetworkLink]
 
+    #: A class of :class:`~carthage.network.TechnologySpecificNetwork` that will be instantiated for the links on this NetworkedModel.
+    network_implementation_class: carthage.network.TechnologySpecificNetwork = None
+
     async def resolve_networking(self, force: bool = False):
         '''
             Adds all :class:`carthage.network.NetworkLink` objects specified in the :class:`carthage.network.NetworkConfig`  to the network_links property.
 
         :param force: if True, resolve the network config even if it has already been resolved once.
 
         '''
@@ -274,15 +325,28 @@
         if network_config is None:
             return
         result = await ainjector(network_config.resolve, self)
 
     async def resolve_model(self, force:bool=False):
         await self.resolve_networking(force=force)
         return await super().resolve_model(force=force)
-    
+
+    async def dynamic_dependencies(self):
+        '''See :func:`carthage.deployment.Deployable.dynamic_dependencies` for documentation.
+        Returns technology specific networks for links where that is possible.
+        '''
+        if not self.network_implementation_class: return []
+        await self.resolve_networking()
+        results = []
+        network_class = self.network_implementation_class
+        for l in self.network_links.values():
+            if l.local_type: continue
+            instance = await l.net.access_by(network_class, ready=False)
+            results.append(instance)
+        return results
 
 class AbstractMachineModel(NetworkedModel):
 
     '''
     Represents properties of a machine that do not involve interacting with an implementation of that machine.  All the *AbstractMachineModels* in a layout can be instantiated to reason about things like network connections, configuration, and what machines will be built without instantiating any of the machines.  Typically if a :class:`Machine` has a model, the model will be made available either by setting the *model* property on the machine, or by providing a dependency for :class:`AbstractModel` in the injector in which the machine is instantiated.
 
     The most common concrete implementation of a machine model is :class:`carthage.modeling.MachineModel`.
@@ -527,47 +591,63 @@
         return await meth()
 
     def _apply_to_filesystem_customization(self, customization):
         '''
         Adapts the customization to this type of machine.  Overridden in machines that can customize a filesystem without booting.
         '''
         customization.customization_context = customization._machine_context()
-        customization.run_command = self.ssh_run_command
+        customization.run_command = self.run_command
 
-    def ssh_run_command(self,
+    def run_command(self,
                         *args,
                         _bg=True,
-                        _bg_exc=False):
+                        _bg_exc=False,
+                    _user=None):
         '''
-            Ssh has really bad quoting; it effectively  removes one level of quoting from the input.
+        This method is the machine-specific part of :meth:`run_command`.  Override in subclasses if there is a better way to run a command than sshing into a machine.  This method is async, although that is not reflected in the signature because this implementation returns an awaitable.
+
+        :param user: The user to run as.  defaults to :attr:`runas_user`.
+        
+        This implementation calls :meth:`ssh`.
+        Ssh has really bad quoting; it effectively  removes one level of quoting from the input.
 This handles quoting and  makes sure each argument is a separate argument on the eventual shell;
-it works like :meth:`carthage.container.Container.container_command` and is used to give a consistent interface by :meth:`FilesystemCustomization.run_command`.
+it works like :meth:`carthage.container.Container.container_command` and is used to give a consistent interface by :meth:`run_command`.
 '''
+        if _user is None:
+            _user = self.runas_user
+        if _user != self.ssh_login_user:
+            raise ValueError(f'{self.__class__.__qualname__} Does not support runas_user different than ssh_login_user; consider BecomePrivilegedMixin or another privilege management solution.')
         return self.ssh(
             shlex.join(args),
             _bg=_bg, _bg_exc=_bg_exc)
 
-    async def sshfs_process_factory(self):
+        
+    async def sshfs_process_factory(self, user):
+        if user != self.ssh_login_user:
+            raise ValueError(f'{self.__class__.__qualname__} cannot set up filesystem access when runas_user != ssh_login_user')
         return sh.sshfs(
             '-o' 'ssh_command=' + " ".join(
                 str(self.ssh).split()[:-1]),
-            f'{self.ip_address}:/',
+            f'{ssh_user_addr(self)}:/',
             self.sshfs_path,
             '-f',
             _bg=True,
             _bg_exc=False)
 
     @contextlib.asynccontextmanager
-    async def filesystem_access(self):
+    async def filesystem_access(self, user=None):
+
         '''
         An asynchronous context manager that makes the filesystem of the *Machine* available on a local path.
 
         :returns: Path at which the filesystem can be accessed while in the context.
 
         '''
+        if user is None:
+            user = self.runas_user
         async with self.machine_running(ssh_online=True):
             self.sshfs_count += 1
             try:
                 # Argument for correctness of locking.  The goal of
                 # sshfs_lock is to make sure that two callers are not both
                 # trying to spin up sshfs at the same time.  The lock is
                 # never held when sshfs_count is < 1, so it will not block
@@ -577,15 +657,15 @@
                 # incrementing sshfs_count, but more difficult to
                 # implement because the lock must be released by time of
                 # yield so other callers can concurrently access the filesystem.
                 async with self.sshfs_lock:
                     if self.sshfs_count == 1:
                         self.sshfs_path = tempfile.mkdtemp(
                             dir=self.config_layout.state_dir, prefix=self.name, suffix="sshfs")
-                        self.sshfs_process = await self.sshfs_process_factory()
+                        self.sshfs_process = await self.sshfs_process_factory(user=user)
                         for x in range(5):
                             alive, *rest = self.sshfs_process.process.is_alive()
                             if not alive:
                                 await self.sshfs_process
                                 raise RuntimeError  # I'd expect that to have happened from an sh exit error already
                             if os.path.exists(os.path.join(
                                     self.sshfs_path, "run")):
@@ -681,15 +761,15 @@
                  "filesystem_access",
                  'model',
                  'name', 'ansible_inventory_name',
                  'machine_running', 'running',
                  'name', 'full_name',
                  'apply_customization'):
             return getattr(self.host, a)
-        raise AttributeError(f"'{self}' has no attribute '{a}'")
+        raise AttributeError(f"'{self!r}' has no attribute '{a}'")
 
     def __repr__(self):
         return f"<{self.__class__.__name__} description:\"{self.description}\" for {self.host.name}>"
 
     #: A description of the customization for inclusion in task logging
     description = ""
 
@@ -874,12 +954,13 @@
             yield dict(size=size)
     if not primary_disk_found:
         yield from default_disk_config
 
 
 __all__ = ['AbstractMachineModel',
            'ssh_origin',
+           'ssh_jump_host',
            'Machine', 'MachineRunning', 'BareMetalMachine',
            'ResolvableModel', 'NetworkedModel',
            'SshMixin', 'BaseCustomization', 'ContainerCustomization',
            'FilesystemCustomization',
            'MachineCustomization']
```

### Comparing `carthage-0.30.dev1/carthage/modeling/__init__.py` & `carthage-0.32/carthage/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/modeling/ansible.py` & `carthage-0.32/carthage/modeling/ansible.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/modeling/base.py` & `carthage-0.32/carthage/modeling/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,19 +90,50 @@
             if isinstance(c, ModelingBase) and hasattr(c, '_callbacks'):
                 for cb in c._callbacks:
                     cb(self)
 
     def __init_subclass__(cls, *args, template=False, **kwargs):
         super().__init_subclass__(*args, **kwargs)
 
+    def __str__(self):
+        keys = []
+        for a in ('__container_propagation_keys__', '__provides_dependencies_for__'):
+            res = getattr(self, a, None)
+            if res:
+                keys = res
+                break
+        if not keys: return super().__str__()
+        keys = list(keys)
+        # We want globally_unique is True to sort before
+        # globally_unique False and then most constraints first.
+        # So that's reversed of globally_unique followed by len(constraints)
+        keys.sort(key=lambda k: (k.globally_unique, len(k.constraints)), reverse=True)
+        result_key = keys[0]
+        if isinstance(result_key.target, type):
+            result = [result_key.target.__name__]
+        else: result = [str(result_key.target)]
+        result += [f"{k}={v}" for k,v in result_key.constraints.items()]
+        if len(result) > 1:
+            return result[0]+":"+(" ".join(result[1:]))
+        else: return result[0]
+        
+    
+        
 
 __all__ += ['InjectableModel']
 
+class ModelContainer(InjectableModel, metaclass=ModelingContainer): pass
 
-class NetworkModel(carthage.Network, InjectableModel, metaclass=ModelingContainer):
+__all__ +=  ['ModelContainer']
+
+
+
+
+
+class NetworkModel(carthage.Network, ModelContainer):
 
     def __init__(self, **kwargs):
         kwargs.update(gather_from_class(self, 'name', 'vlan_id'))
         super().__init__(**kwargs)
         if hasattr(self, 'bridge_name'):
             self.ainjector.add_provider(InjectionKey(carthage.network.BridgeNetwork),
                                         when_needed(carthage.network.BridgeNetwork, bridge_name=self.bridge_name, delete_bridge=False))
@@ -145,15 +176,15 @@
                          ):
     pass
 
 
 __all__ += ['NetworkConfigModel']
 
 
-class ModelGroup(InjectableModel, AsyncInjectable, metaclass=ModelingContainer):
+class ModelGroup(ModelContainer, AsyncInjectable):
 
     async def all_models(self, ready=None):
         models = await self.ainjector.filter_instantiate_async(
             carthage.machine.ResolvableModel, ['name'],
             stop_at=self.injector,
             ready=ready)
         return [m[1] for m in models]
@@ -211,15 +242,15 @@
             await super().generate()
 
     async def async_ready(self):
         await self.resolve_networking()
         return await super().async_ready()
 
 
-class Enclave(ModelGroup, metaclass=ModelingContainer):
+class Enclave(ModelGroup):
 
     domain: str
 
     @classmethod
     def our_key(self):
         return InjectionKey(Enclave, domain=self.domain)
 
@@ -294,31 +325,30 @@
             machine_key = InjectionKey(carthage.machine.Machine, host=self.name, _globally_unique=True)
             self.__transclusions__[machine_key] = frozenset({machine_key})
             self.__transclusion_key__ = self.our_key()
             self.__initial_injections__[machine_key] = (
                 self.machine, dict(
                     close=True, allow_multiple=False,
                 ))
-            self.__container_propagations__[machine_key] = \
-                self.__initial_injections__[machine_key]
+            self.__container_propagations__.add(machine_key)
             globally_unique_key(InjectionKey(
                 carthage.machine.ResolvableModel,
                 name=self.name))(self)
 
 
 class MachineModelMixin:
     pass
 
 
 @inject(
     _not_transcluded=not_transcluded_key)
 @inject_autokwargs(
     config_layout=ConfigLayout,
                    )
-class MachineModel(InjectableModel, carthage.machine.AbstractMachineModel, metaclass=MachineModelType, template=True):
+class MachineModel(ModelContainer, carthage.machine.AbstractMachineModel, metaclass=MachineModelType, template=True):
 
     '''
 
     Represents the aspects of a :class:`~carthage.machine.Machine` that are independent of the implementation of that machine.  Typically includes things like:
 
     * Network configuration (:class:`~carthage.network.NetworkConfig`
 
@@ -474,15 +504,15 @@
 
     async def async_resolve(self):
         return self.prep(await self.ainjector(self.res, name=self.name), self.model)
 
 
 __all__ += ['MachineModel', 'MachineModelMixin']
 
-class ImageRole(InjectableModel, metaclass=RoleType): pass
+class ImageRole(ModelContainer, metaclass=RoleType): pass
 
 __all__ += ['ImageRole']
 
 
 class CarthageLayout(ModelGroup):
 
     '''
@@ -565,15 +595,15 @@
     return tuple(new_bases)
 
 
 __all__ += ['model_bases']
 
 
 @inject(config_layout=ConfigLayout)
-class ModelTasks(InjectableModel, SetupTaskMixin, AsyncInjectable, metaclass=ModelingContainer):
+class ModelTasks(ModelContainer, SetupTaskMixin, AsyncInjectable):
 
     '''
     A grouping of tasks that will be run at generate time in a :class:`CarthageLayout`.  As part of :meth:`ModelGroup.generate`, the layout searches for any :class:`ModelTasks` provided by its injector and instantiates them.  This causes any setup_tasks to be run.
 
     All :class:`ModelTasks` have a name, which forms part of their key.  If there needs to be an ordering between tasks, the tasks can inject a dependency on other ModelTasks.
 
     Example usage::
```

### Comparing `carthage-0.30.dev1/carthage/modeling/decorators.py` & `carthage-0.32/carthage/modeling/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021, 2022, Hadron Industries, Inc.
+# Copyright (C) 2021, 2022, 2023, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -129,19 +129,26 @@
     def handle(self, cls, ns, k, state):
         super().handle(cls, ns, k, state)
         state.extra_keys.extend(self.keys)
 
 
 def provides(*keys):
     '''Indicate that the decorated value provides these InjectionKeys'''
-    keys = list(map(lambda k: InjectionKey(k), keys))
+    keys = list(map(lambda k: InjectionKey(k) if not isinstance(k, InjectionKey) else k, keys))
 
     def wrapper(val):
         try:
-            setattr_default(val, '__provides_dependencies_for__', [])
+            setattr_default(val, '__provides_dependencies_for__', None)
+            if val.__provides_dependencies_for__ is None:
+                if isinstance(val, type):
+                    val.__provides_dependencies_for__ = [
+                        k for b in val.__bases__
+                        for k in getattr(b, '__provides_dependencies_for__', [])]
+                else:
+                    val.__provides_dependencies_for__ = list(getattr(val.__class__, '__provides_dependencies_for__', []))
             val.__provides_dependencies_for__ = keys + val.__provides_dependencies_for__
             return val
         except BaseException:
 
             return ProvidesDecorator(val, *keys)
     return wrapper
 
@@ -211,14 +218,21 @@
         self.flag = flag
 
     def handle(self, cls, ns, k, state):
         super().handle(cls, ns, k, state)
         state.flags &= ~self.flag
 
 
+def no_inject_name(val=None, /):
+    def wrap(v):
+        return FlagClearDecorator(v, NSFlags.instantiate_on_access|NSFlags.inject_by_name)
+    if val is not None:
+        return wrap(val)
+    else: return wrap
+    
 def no_instantiate():
     def wrapper(val):
         return FlagClearDecorator(val, NSFlags.instantiate_on_access)
     return wrapper
 
 
 def no_close():
@@ -259,42 +273,55 @@
 
 '''
     def wrapper(val):
         return MachineMixin(val, name or val.__name__)
     return wrapper
 
 
-class PropagateUpDecorator(ModelingDecoratorWrapper):
-
-    name = "propagate_up"
-    subclass = ModelingContainer
-
-    def handle(self, cls, ns, k, state):
-        super().handle(cls, ns, k, state)
-        state.flags |= NSFlags.propagate_key
-
 
-def propagate_up():
-    '''Indicate that an assignment should have its keys propagated up in
-    a container::
+def propagate_key(key, obj=None):
+    '''Indicate a set of keys that should be propagated up
+    in a container::
 
         class foo(ModelingContainer):
-            @propagate_up()
-            @provides(InjectionKey(Baz, target = 42))
+            @propagate_key(InjectionKey(Baz, target = 42))
             class ourbaz(Baz): ...
 
     When *foo* is included ain a container, then the *Baz* injection
     key will be propagated up to dependencies provided by that
     container.  Since the key was not marked globally unique,
     constraints from *foo.our_key()* will be added to it as it is
     propagated.
 
+    *keys* are also provided by the contained class as if :func:`provides` or :func:`globally_unique` were called.
+
+    Propagating a key up is typically an interface point; rather than propagating all keys related to an object up, propagate the keys that will be understood by the environment.  Examples of usage include:
+
+    * Any :class:`~carthage.machine.AbstractMachineModel` with a *host* constraint is collected to find all the machine models in a layout
+
+    
     '''
     def wrap(val):
-        return PropagateUpDecorator(val)
+        setattr_default(val,'__container_propagation_keys__', None)
+        if val.__container_propagation_keys__ is None:
+            if isinstance(val, type):
+                val.__container_propagation_keys__ = set(
+                    propagation_keys for  b in val.__bases__
+                    for propagation_keys in getattr(b, '__container_propagation_keys__', set()))
+            else: # not type
+                val.__container_propagation_keys = set(getattr(
+                    val.__class__,
+                    '__container_propagation_keys__',
+                    set()))
+        val.__container_propagation_keys__.add(key)
+        return provides(key)(val)
+    if not isinstance(key, InjectionKey):
+        raise TypeError('propagate_key takes an injection key and optional object to apply it to.')
+    if obj is not None:
+        return wrap(obj)
     return wrap
 
 
 def transclude_overrides(
         key: InjectionKey = None):
     '''
     Decorator indicating that the decorated item should be overridden by one from the injector against which the containing layout is eventually instantiated.  When a :class:`InjectableModel` is eventually instantiated, before an overridable key is added to the local injector, it is searched for in the instantiating injector.  If it is found, the  key is not registered.  This has the effect of using the dependency provider in the instantiating injector rather than the one included in the layout.
@@ -376,15 +403,15 @@
         if instance is None:
             return self.value
         machine = instance.injector.get_instance(InjectionKey(carthage.machine.Machine, _ready=False))
         return instance.injector(self.value, apply_to=machine, stamp=self.name)
 
 
 __all__ = ["ModelingDecoratorWrapper", "provides", 'dynamic_name',
-           'injector_access', 'no_instantiate',
+           'injector_access', 'no_inject_name', 'no_instantiate',
            'allow_multiple', 'no_close',
            'globally_unique_key',
            'MachineMixin', 'machine_mixin',
-           'propagate_up',
+           'propagate_key',
            'transclude_overrides',
            'model_mixin_for',
            ]
```

### Comparing `carthage-0.30.dev1/carthage/modeling/example.py` & `carthage-0.32/carthage/modeling/example.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/modeling/implementation.py` & `carthage-0.32/carthage/modeling/implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class NSFlags(enum.Flag):
     close = 1
     allow_multiple = 2
     inject_by_name = 4
     inject_by_class = 8
     instantiate_on_access = 16
-    propagate_key = 32
+    # 32 previously used by propagate_key, but that has been reworked
     dependency_quote = 64
 
 
 classes_to_quote = set()
 
 
 class NsEntry:
@@ -411,16 +411,16 @@
         for k, v in cls.__dict__.items():
             if isinstance(v, modelmethod):
                 cls.namespace_initial[k] = v  # Parsed further in the namespace constructor
 
 
 __all__ += ["ModelingBase"]
 
-not_transcluded_key = InjectionKey('carthage.modeling.not_transcluded', _optional=True)
 #: An injection key to store the set of keys that could have been transcluded but were not so that container propagation does not  transclude
+not_transcluded_key = InjectionKey('carthage.modeling.not_transcluded', _optional=True)
 
 __all__ += ['not_transcluded_key']
 
 
 class InjectableModelType(ModelingBase):
 
     classes_to_inject: typing.Sequence[type] = (NetworkConfig, carthage.console.CarthageRunnerCommand)
@@ -512,15 +512,15 @@
             transclusions[k] = {k}
         to_inject[k] = (v, dict(
             close=close,
             allow_multiple=allow_multiple,
         ))
         if propagate:
             assert issubclass(metaclass, ModelingContainer), "Only ModelingContainers accept propagation"
-            to_propagate[k] = to_inject[k]
+            to_propagate.add(k)
 
     @modelmethod
     def disable_system_dependency(cls, dependency):
         cls.__initial_injections__[dependency.default_instance_injection_key()] = (
             None, dict(close=False, allow_multiple=False))
 
     @modelmethod
@@ -540,101 +540,123 @@
 
     #: Returns the key under which we are registered in the parent.  Our
     # objects will be adapted by adding these constraints to register in
     # the parent as well.
     our_key: typing.Callable[[object], InjectionKey]
 
     def _integrate_containment(target_cls, ns, k, state):
-        def propagate_provider(k_inner, v, options):
-            # There is the provides_dependencies_for (or outer) keys, and there is a
-            # set of inner keys from the providers being injected.  We
-            # want to pick one outer key and also add the inner keys
-            # (plus the constraints from the outer key) into the outer
-            # injector.  We pick one outer key just for simplicity; it
-            # could be made to work with more.
+        def propagate_provider(outer_key, k_inner, v, options, do_global):
+            # There is the set of outer keys by which the container is
+            # known; typically from @provides_dependencies_for or
+            # @globally_unique_key, and there is a set of inner keys
+            # from the providers being injected (from @propagate_key
+            # or add_provider with propagate True).  We want to pick
+            # one outer key and also add the inner keys (plus the
+            # constraints from the outer key) into the outer
+            # injector. This function will be called for each outer
+            # key to propagate the crossproduct of inner and outer
+            # keys.  
+
             globally_unique = k_inner.globally_unique
             if not globally_unique:
                 if k_inner in val.__transclusions__:
                     raise TypeError(f'{k_inner} cannot be transcluded and propagated unless it is globally unique')
                 outer_constraints = outer_key.constraints
                 if set(outer_constraints) & set(k_inner.constraints):
                     return
                 k_new = InjectionKey(k_inner.target, **outer_constraints, **k_inner.constraints)
             else:
+                if not do_global: return
                 k_new = k_inner  # globally unique
             # Must be after we have chosen a globally unique key if there is one.
-            if k_new not in ns.to_inject:
+            if k_new not in ns.to_inject and k_inner not in inner_key_map:
                 inner_key_map[k_inner] = k_new
             if isinstance(v, decorators.injector_access):
                 # Normally injector_access will not actually get a key
                 # in __initial_injections__, but there are important
                 # cases where that happens, like the machine entry on
                 # MachineModel.  In general this situation will come
                 # up if some modeling type wishes to propagate
                 # something that is referenced by an InjectionKey
-                # rather than a value.  One of the biggest reasons to
-                # try and collapse out injector_access is that
-                # injector_access cannot deal with AsyncRequired but
-                # injector_xref can.
+                # rather than a value.  
                 k_inner = v.key
             # In some cases we could make the injector_xref more clear
             # by adding the outer key's constraints to
             # v.injectable_key and use that as the new injectable key,
             # preserving the inner target key.  That generally works
             # so long as the injectable_key is not masked by a key
             # already in the outer injector or by an overlapping
             # constraint.  Also, It just moves the recursion around.
             v = injector_xref(outer_key, k_inner)
             if k_new not in ns.to_inject:
                 ns.to_inject[k_new] = (v, options)
-                ns.to_propagate[k_new] = (v, options)
+                ns.to_propagate.add(k_new)
 
         if not isinstance(state.value, ModelingContainer):
             return
         inner_key_map = {}
         val = state.value
         outer_key = None
+        to_propagate = val.__container_propagations__
+        outer_keys = []
         if hasattr(val, '__provides_dependencies_for__'):
             for outer_key in sorted(
                     val.__provides_dependencies_for__,
                     key=lambda k: k.globally_unique,
                     reverse=True):
-                if isinstance(outer_key.target, ModelingContainer) and len(outer_key.constraints) > 0:
-                    break
-        to_propagate = val.__container_propagations__
-        if to_propagate and (outer_key is None or len(outer_key.constraints) == 0):
+                if outer_key not in ns.to_propagate: continue
+                if  len(outer_key.constraints) > 0:
+                    outer_keys.append(outer_key)
+        if to_propagate and not outer_keys:
             warnings.warn("Cannot propagate because no outer key with constraints found", stacklevel=3)
             return
-        for k, info in to_propagate.items():
-            v, options = info
-            propagate_provider(k, v, options)
+        for k_inner in to_propagate:
+            if k_inner not in val.__initial_injections__:
+                warnings.warn(f'Cannot propagate {k_inner} because it is not provided by {val}')
+                continue
+            v, options = val.__initial_injections__[k_inner]
+            do_global = True
+            for outer_key in outer_keys:
+                propagate_provider(outer_key, k_inner, v, options, do_global)
+                do_global = False
         map_transclusions(ns.transclusions, val, inner_key_map)
 
     def _propagate_filter(target_cls, ns, k, state):
-        if isinstance(state.value, ModelingContainer) or (state.flags & NSFlags.propagate_key):
-            for k, info in ns.keys_for(name=k, state=state):
-                ns.to_propagate[k] = info
-
+        if hasattr(state.value, '__container_propagation_keys__'):
+            propagation_keys = set(state.value.__container_propagation_keys__)
+        else: propagation_keys = set()
+        keys_for = set((x[0] for x in ns.keys_for(name=k, state=state)))
+        propagation_keys &= keys_for
+        # ModelingContainers must propagate even if they have no explicit keys
+        if (not propagation_keys ) and isinstance(state.value, ModelingContainer):
+            propagation_keys = keys_for
+        ns.to_propagate |= propagation_keys
+        
+    # propagate_filter must come before integrate_containment so that
+    # integrate_containment can check whether outer_keys are in
+    # ns.to_propagate. However, filters are processed in reversed
+    # order.
     namespace_filters = [_integrate_containment, _propagate_filter]
 
     @classmethod
     def __prepare__(cls, *args, **kwargs):
         ns = super().__prepare__(*args, **kwargs)
-        ns.to_propagate = {}
+        ns.to_propagate = set()
         ns.setitem('__container_propagations__', ns.to_propagate)
         return ns
 
     def __new__(cls, name, bases, ns, **kwargs):
         to_propagate = ns.to_propagate
         self = super().__new__(cls, name, bases, ns, **kwargs)
-        to_propagate.update( sum([
-            list(b.__container_propagations__.items()) for b in bases if isinstance(b, ModelingContainer)], []))
-        for k in list(to_propagate.keys()):
+        to_propagate |= set(
+            propagations for b in bases
+            for propagations in getattr(b, '__container_propagations__', set()))
+        for k in set(to_propagate): #copy for mutation
             if k not in self.__initial_injections__:
-                del self.__container_propagations[k]
+                self.__container_propagations__.remove(k)
         return self
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         try:
             our_key = self.our_key()
             if not isinstance(our_key, InjectionKey):
@@ -669,25 +691,27 @@
         if dynamic_name:
             # This is gross, but it's not clear how to support
             # decorators ourselves
             if (not close) or allow_multiple:
                 raise TypeError('If using dynamic_name, use decorators to adjust close and allow_multiple')
             ns[fixup_dynamic_name(dynamic_name)] = obj
             return
-        ModelingContainer._integrate_containment(cls, ns, obj.__name__, state)
         # Since we're not able to use ns.__setitem__, do the injection key stuff ourself.
         if not close:
             state.flags &= ~NSFlags.close
         if allow_multiple:
             state.flags |= NSFlags.allow_multiple
+        state.extra_keys = obj.__provides_dependencies_for__
         options = state.injection_options
         for k in obj.__provides_dependencies_for__:
             if k not in ns.to_inject:
                 ns.to_inject[k] = (obj, options)
-                ns.to_propagate[k] = (obj, options)
+        ModelingContainer._propagate_filter(cls, ns, obj.__name__, state)
+        ModelingContainer._integrate_containment(cls, ns, obj.__name__, state)
+
 
 
 __all__ += ['ModelingContainer']
 
 
 def adjust_bases_for_tasks(bases: tuple[type], namespace: dict) -> tuple[type]:
     '''
@@ -753,15 +777,15 @@
         cls.__transclusions__.add((k, k, cls))
     cls.__initial_injections__[k] = (v, dict(
         close=close,
         allow_multiple=allow_multiple,
     ))
     if propagate:
         assert isinstance(cls, ModelingContainer), "Only ModelingContainers accept propagation"
-        cls.__container_propagations__[k] = cls.__initial_injections__[k]
+        cls.__container_propagations__.add(k)
 
 
 def map_transclusions(container_transclusions, contained, inner_key_map):
     '''
     Consider the case when *contained* is added to *container*.  *contained*  provides a dependency *k*, but that dependency permits transclusion.  That means that if *contained* is instantiated in an injector  that already provides *k*, then the instantiating injector's version of *k* is used.
 
     It's an error for *k* not to be globally unique.  Transcluded keys must either be globally unique or not propagated, because transclusion always happens in the scope of the instantiating injector, and the only time when that naming is the same as the inner injector (for objects provided by the inner injector) is for globally unique keys.  However, when *k* is transcluded, there may be extra keys *k_1* that are also suppressed because they are provided by the same object as *k*.  These keys need to be remapped from *contained*'s transclusions to *container*'s transclusions.
```

### Comparing `carthage-0.30.dev1/carthage/modeling/utils.py` & `carthage-0.32/carthage/modeling/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -122,14 +122,16 @@
 
 def key_from_injector_access(*accesses):
     from .decorators import injector_access
     result = []
     for k in accesses:
         if isinstance(k, injector_access):
             k = k.key
+        elif isinstance(k, list):
+            k = [x.key if isinstance(x, injector_access) else x for x in k]
         elif  hasattr(k, '__provides_dependencies_for__'):
             k = k.__provides_dependencies_for__[0]
         result.append(k)
     return result
 
 
 __all__ += ['key_from_injector_access']
```

### Comparing `carthage-0.30.dev1/carthage/network/__init__.py` & `carthage-0.32/carthage/network/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/network/base.py` & `carthage-0.32/carthage/network/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019, 2020, 2021, 2022, 2023, Hadron Industries, Inc.
+# Copyright (C) 2019, 2020, 2021, 2022, 2023, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
@@ -170,30 +170,30 @@
         import carthage.kvstore
         pool = self.injector.get_instance(V4Pool)
         if link:
             return pool.assignment_loop([link])
         pool.new_assignments()
         pool.assignment_loop(self.network_links)
         
-    async def access_by(self, cls: TechnologySpecificNetwork):
+    async def access_by(self, cls: TechnologySpecificNetwork, ready=None):
         '''Request a view of *self* using *cls* as a technology-specific lens.
 
         :return: The instance of *cls* for accessing this network
         '''
         assert issubclass(cls, TechnologySpecificNetwork), \
             "Must request access by a subclass of TechnologySpecificNetwork"
         instance = None
         if (cls not in self.ainjector) and self.vlan_id is not None:
             try:
-                instance = await self.ainjector.get_instance_async(InjectionKey(cls, vlan_id=self.vlan_id))
+                instance = await self.ainjector.get_instance_async(InjectionKey(cls, vlan_id=self.vlan_id, _ready=ready))
                 self.ainjector.add_provider(instance)
             except KeyError:
                 pass
         if not instance:
-            instance = await self.ainjector.get_instance_async(cls)
+            instance = await self.ainjector.get_instance_async(InjectionKey(cls, _ready=ready))
         assert cls in self.ainjector, \
             f"It looks like {cls} was not registered with add_provider with allow_multiple set to True"
         if instance not in self.technology_networks:
             await instance.also_accessed_by(list(self.technology_networks))
             l = [instance]
             for elt in self.technology_networks:
                 await elt.also_accessed_by(l)
@@ -387,18 +387,15 @@
     @inject(ainjector=AsyncInjector)
     async def resolve(self, connection, ainjector) -> dict[str, NetworkLink]:
         '''
         Return a mapping of interfaces to NetworkLinks
         The *network_links* property of *connection* is updated based on the new network links.  That side effect is a bit unclean, but doing the update here allows :meth:`carthage.machine.Machine.resolve_networking` and :meth:`carthage.machine.AbstractMachineModel.resolve_networking` to have less duplicated code.
         '''
         async def resolve1(r: typing.any, i, args, k):
-            if isinstance(r, InjectionKey):
-                r = await ainjector.get_instance_async(r)
-            elif callable(r):
-                r = await ainjector(r, i)
+            r = await resolve_deferred(ainjector, r, {"interface": i})
             if args is not None:
                 args[k] = r
             return r
 
         def handle_other(link, other_args, other_future):
             def callback(future):
                 other_link = None
@@ -482,15 +479,19 @@
                     continue
                 if k == 'member_of':
                     if callable(v) or isinstance(v, InjectionKey):
                         futures.append(asyncio.ensure_future(resolve1(v, i, members_of, i)))
                     else:
                         members_of[i] = v
                     continue
-                if callable(v) or isinstance(v, InjectionKey):
+                if (
+                    callable(v)
+                    or isinstance(v, InjectionKey)
+                    or isinstance(v, list)
+                ):
                     futures.append(asyncio.ensure_future(resolve1(v, i, link_args, k)))
                 else:
                     link_args[k] = v
             d[i] = link_args
 
         await asyncio.gather(*futures)
         del futures
@@ -718,16 +719,21 @@
             if (not optional) and t.__class__ == typing._GenericAlias:
                 continue
             if optional:
                 t = get_type_args(t)
             if k not in args:
                 if not optional:
                     raise TypeError(f'{k} is required')
-            elif (not unresolved) and (not isinstance(args[k], t)):
-                raise TypeError(f'{k} must be a {t} not {args[k]}')
+            elif not unresolved:
+                if hasattr(t, "__instancecheck__"):
+                    if not t.__instancecheck__(args[k]):
+                        raise TypeError(f'{k} must be a {t} not {args[k]}')
+                else:
+                    if not isinstance(args[k], t):
+                        raise TypeError(f'{k} must be a {t} not {args[k]}')
         if subclass:
             subclass.validate_subclass(args, unresolved=unresolved)
 
     def __repr__(self):
         cls = self.__class__
         result = f'<{cls.__name__} '
         try:
```

### Comparing `carthage-0.30.dev1/carthage/network/config.py` & `carthage-0.32/carthage/network/config.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/network/links.py` & `carthage-0.32/carthage/network/links.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-# Copyright (C) 2021, Hadron Industries, Inc.
+# Copyright (C) 2021, 2024, Hadron Industries, Inc.
 # Carthage is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License version 3
 # as published by the Free Software Foundation. It is distributed
 # WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the file
 # LICENSE for details.
 
 from __future__ import annotations
 import dataclasses
 import typing
 import weakref
-from .base import NetworkLink
+from ipaddress import IPv4Address
+from .base import NetworkLink, Network
 from ..dependency_injection import *
 
 
+class GRELink(NetworkLink):
+    local: typing.Union[str,IPv4Address] = dataclasses.field(kw_only=True)
+    remote: typing.Union[str,IPv4Address] = dataclasses.field(kw_only=True)
+    key: str = None
+    local_type = "gre"
+    required  = False
+    routes: list[Network] = dataclasses.field(default_factory=lambda: [])
+
 class BondLink(NetworkLink):
 
     local_type = "bond"
 
 
 class BridgeLink(NetworkLink):
```

### Comparing `carthage-0.30.dev1/carthage/network/mac.py` & `carthage-0.32/carthage/network/mac.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/network/namespace.py` & `carthage-0.32/carthage/network/namespace.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/network/switch.py` & `carthage-0.32/carthage/network/switch.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/oci.py` & `carthage-0.32/carthage/oci.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/pki.py` & `carthage-0.32/carthage/pki.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/plugins.py` & `carthage-0.32/carthage/plugins.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/podman/__init__.py` & `carthage-0.32/carthage/podman/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/podman/base.py` & `carthage-0.32/carthage/podman/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,23 @@
     machine_running_ssh_online = False
     rsync_uses_filesystem_access = True
 
     #: restart containers (no, always, on-failure)
     podman_restart = 'no'
 
     #:Extra options (as a list) to be passed into podman create
-    podman_options = []
+    @memoproperty
+    def podman_options(self):
+        '''Extra options to be passed into podman create as a list
+        '''
+        try:
+            return self.model.podman_options
+        except AttributeError:
+            return []
+        
 
     @memoproperty
     def ssh_options(self):
         if not hasattr(self, 'ssh_port'):
             raise ValueError('Set ssh_port before ssh')
         return (
             *super().ssh_options,
@@ -387,15 +395,15 @@
             async with self.machine_running(ssh_online=False), self.filesystem_access() as path:
                 customization.path = path
                 yield
             return
         customization.customization_context = customization_context()
         customization.run_command = self.container_exec
 
-    def filesystem_access(self):
+    def filesystem_access(self, user='root'):
         return self.container_host.filesystem_access(self.full_name)
 
     def __repr__(self):
         try:
             host = repr(self.container_host)
         except Exception:
             host = "repr failed"
```

### Comparing `carthage-0.30.dev1/carthage/podman/modeling.py` & `carthage-0.32/carthage/podman/modeling.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from carthage import *
 from carthage.dependency_injection import *
 from carthage.oci import OciImage
 
 __all__ = []
 
 
-class PodmanPodModel( carthage.machine.NetworkedModel, InjectableModel, metaclass=carthage.modeling.implementation.ModelingContainer):
+class PodmanPodModel( carthage.machine.NetworkedModel, ModelContainer):
 
     '''A container that can group a number of :class:`MachineModels` representing Podman containers.
 
     * By default, ``machine_implementation_key`` within a :class:`PodmanPodModel` is :class:`PodmanContainer`.
 
     * By default, when added to an enclosing injector, this model does not provide :class:`PodmanPod` in that context, although it does provide :class:`PodmanPod` within its own injector.  An example illustrates::
```

### Comparing `carthage-0.30.dev1/carthage/ports.py` & `carthage-0.32/carthage/ports.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/pytest.py` & `carthage-0.32/carthage/pytest.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/pytest_plugin.py` & `carthage-0.32/carthage/pytest_plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import argparse
 import asyncio
 import json
 import logging
 import pytest
 import yaml
+from dataclasses import replace, is_dataclass
 from. import base_injector, ConfigLayout
 from .dependency_injection import AsyncInjector
 
 
 @pytest.fixture(scope='session')
 def loop():
     ''':returns: Asyncio event loop
@@ -37,15 +38,23 @@
 
     for i in items:
         if isinstance(i, pytest.Function):
             if hasattr(i.function, '__signature__'):
                 del i.keywords._markers['place_as']
                 del i.keywords._markers['usefixtures']
                 del i.keywords._markers['__signature__']
-                i._fixtureinfo.argnames = tuple(i.function.__signature__.parameters.keys())
+                if is_dataclass(i._fixtureinfo) and i._fixtureinfo.__dataclass_params__.frozen:
+                    # _fixtureinfo is a frozen dataset. We can't change attrs of this. 
+                    # use `replace` to generate a new _fixtureinfo object with the updated `argnames`
+                    old = i._fixtureinfo
+                    new = replace(old, argnames=tuple(i.function.__signature__.parameters.keys()))
+                    i._fixtureinfo = new
+                else:
+                    i._fixtureinfo.argnames = tuple(i.function.__signature__.parameters.keys())
+
 
 
 @pytest.fixture()
 def ainjector():
     ainjector = base_injector.claim()(AsyncInjector)
     yield ainjector
     ainjector.close()
```

### Comparing `carthage-0.30.dev1/carthage/resources/ansible-chroot-helper` & `carthage-0.32/carthage/resources/ansible-chroot-helper`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/fai/files/etc/pam.d/su/OPENROOT` & `carthage-0.32/carthage/resources/fai/files/etc/pam.d/su/OPENROOT`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/fai/files/etc/resolv.conf/DEFAULT` & `carthage-0.32/carthage/resources/fai/files/etc/resolv.conf/DEFAULT`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/fai/scripts/GRUB_EFI/10-setup` & `carthage-0.32/carthage/resources/fai/scripts/GRUB_EFI/10-setup`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/runner_console.py` & `carthage-0.32/carthage/resources/runner_console.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/templates/bridge-network.mako` & `carthage-0.32/carthage/resources/templates/bridge-network.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/templates/default-network.mako` & `carthage-0.32/carthage/resources/templates/default-network.mako`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 DHCP=ipv4
 <%nontrivial = True%>\
 %endif
 %if v4_config.address and not v4_config.dhcp:
 Address=${str(v4_config.address)}/${v4_config.network.prefixlen}
 <%nontrivial = True %>
 %endif
+%if v4_config.secondary_addresses:
+<% nontrivial = True %>
+%for address in v4_config.secondary_addresses:
+Address=${str(address.private)}/${v4_config.network.prefixlen}
+%endfor
+<%nontrivial = True %>
+%endif
 %if link.precious:
 KeepConfiguration = dhcp
 %endif
 %if v4_config.domains:
 Domains=${v4_config.domains}
 %endif
 %if v4_config.dns_servers:
```

### Comparing `carthage-0.30.dev1/carthage/resources/templates/skeletons/prototype.mako` & `carthage-0.32/carthage/resources/templates/skeletons/prototype.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/templates/vlan-network.mako` & `carthage-0.32/carthage/resources/templates/vlan-network.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/resources/templates/vm-config.mako` & `carthage-0.32/carthage/resources/templates/vm-config.mako`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/runner_commands.py` & `carthage-0.32/carthage/runner_commands.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/setup_tasks.py` & `carthage-0.32/carthage/setup_tasks.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/sh.py` & `carthage-0.32/carthage/sh.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/skeleton.py` & `carthage-0.32/carthage/skeleton.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/sonic.py` & `carthage-0.32/carthage/sonic.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/system_dependency.py` & `carthage-0.32/carthage/system_dependency.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/systemd.py` & `carthage-0.32/carthage/systemd.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 from .utils import mako_lookup
 from carthage import ConfigLayout, sh
 import logging
 
 logger = logging.getLogger('carthage.network')
 
 local_type_map = dict(
+    gre=dict(
+        netdev="gre-netdev.mako",
+        network="gre-network.mako",
+    ),
     bond=dict(
         netdev="bond-netdev.mako",
         member_network="bond-network.mako"),
     bridge=dict(
         netdev="bridge-netdev.mako",
         member_network="bridge-network.mako",
     ),
```

### Comparing `carthage-0.30.dev1/carthage/tb_utils.py` & `carthage-0.32/carthage/tb_utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/utils.py` & `carthage-0.32/carthage/utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vault/__init__.py` & `carthage-0.32/carthage/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vm.py` & `carthage-0.32/carthage/vm.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/__init__.py` & `carthage-0.32/carthage/vmware/__init__.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/authorization.py` & `carthage-0.32/carthage/vmware/authorization.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/cluster.py` & `carthage-0.32/carthage/vmware/cluster.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/config_spec.py` & `carthage-0.32/carthage/vmware/config_spec.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/connection.py` & `carthage-0.32/carthage/vmware/connection.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/convenience.py` & `carthage-0.32/carthage/vmware/convenience.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/credentials.py` & `carthage-0.32/carthage/vmware/credentials.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/datacenter.py` & `carthage-0.32/carthage/vmware/datacenter.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/datastore.py` & `carthage-0.32/carthage/vmware/datastore.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/folder.py` & `carthage-0.32/carthage/vmware/folder.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/host.py` & `carthage-0.32/carthage/vmware/host.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/image.py` & `carthage-0.32/carthage/vmware/image.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/inventory.py` & `carthage-0.32/carthage/vmware/inventory.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/network.py` & `carthage-0.32/carthage/vmware/network.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/utils.py` & `carthage-0.32/carthage/vmware/utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage/vmware/vm.py` & `carthage-0.32/carthage/vmware/vm.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/carthage.egg-info/PKG-INFO` & `carthage-0.32/carthage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carthage
-Version: 0.30.dev1
+Version: 0.32
 Summary: A powerful Infrastructure as Code (IAC) framework
 Author-email: Sam Hartman <sam.hartman@hadronindustries.com>
 License: LGPL-3
 Project-URL: Homepage, https://github.com/hadron/carthage
 Project-URL: Documentation, https://carthage.readthedocs.io
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `carthage-0.30.dev1/carthage.egg-info/SOURCES.txt` & `carthage-0.32/carthage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 bin/btrfs-rmrf
 bin/carthage
 bin/carthage-console
 bin/carthage-runner
 bin/carthage-vault-tool
 carthage/__init__.py
 carthage/ansible.py
+carthage/become_privileged.py
+carthage/carthage_deployment.py
 carthage/carthage_plugin.yml
 carthage/cloud_init.py
 carthage/console.py
 carthage/container.py
 carthage/debian.py
 carthage/deployment.py
+carthage/deployment_commands.py
 carthage/dns.py
 carthage/event.py
 carthage/files.py
 carthage/image.py
 carthage/kvstore.py
 carthage/local.py
 carthage/machine.py
@@ -104,14 +107,16 @@
 carthage/resources/fai/scripts/OPENROOT/20-setup
 carthage/resources/fai/scripts/SERIAL/20-SERIAL
 carthage/resources/templates/bond-netdev.mako
 carthage/resources/templates/bond-network.mako
 carthage/resources/templates/bridge-netdev.mako
 carthage/resources/templates/bridge-network.mako
 carthage/resources/templates/default-network.mako
+carthage/resources/templates/gre-netdev.mako
+carthage/resources/templates/gre-network.mako
 carthage/resources/templates/network-base.mako
 carthage/resources/templates/physical-link.mako
 carthage/resources/templates/vlan-netdev.mako
 carthage/resources/templates/vlan-network.mako
 carthage/resources/templates/vm-config.mako
 carthage/resources/templates/vm-console.mako
 carthage/resources/templates/xfrm-netdev.mako
@@ -142,18 +147,20 @@
 tests/conftest.py
 tests/inner_conftest.py
 tests/inner_plugin_test.py
 tests/machine_mock.py
 tests/override-config.yml
 tests/template-2.expected
 tests/test_ansible.py
+tests/test_become.py
 tests/test_carthage_plugin.py
 tests/test_config.py
 tests/test_container.py
 tests/test_dependency_injection.py
+tests/test_deployment.py
 tests/test_event.py
 tests/test_image.py
 tests/test_kvstore.py
 tests/test_modeling.py
 tests/test_network.py
 tests/test_pki.py
 tests/test_plugins.py
```

### Comparing `carthage-0.30.dev1/pyproject.toml` & `carthage-0.32/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "carthage"
-version = "0.30.dev1"
+version = "0.32"
 authors = [
     { name = "Sam Hartman", email = "sam.hartman@hadronindustries.com" },
 ]
 description = "A powerful Infrastructure as Code (IAC) framework"
 readme = "README.rst"
 requires-python = ">=3.11"
 license = { text = "LGPL-3" }
```

### Comparing `carthage-0.30.dev1/tests/carthage_test_utils.py` & `carthage-0.32/tests/carthage_test_utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/conftest.py` & `carthage-0.32/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/machine_mock.py` & `carthage-0.32/tests/machine_mock.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_ansible.py` & `carthage-0.32/tests/test_ansible.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_carthage_plugin.py` & `carthage-0.32/tests/test_carthage_plugin.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_config.py` & `carthage-0.32/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_container.py` & `carthage-0.32/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_dependency_injection.py` & `carthage-0.32/tests/test_dependency_injection.py`

 * *Files 4% similar despite different names*

```diff
@@ -642,7 +642,25 @@
         dict(c=foo,d=func),
         bar], args=args)
     assert result == [
         90,
         dict(a=10, b=20),
         dict(c='foo', d=40),
         'bar']
+
+@async_test
+async def test_filter_failure(ainjector):
+    class Plugin(AsyncInjectable):
+
+        @classmethod
+        def default_class_injection_key(cls):
+            return InjectionKey(Plugin, name=cls.name)
+
+    @inject_autokwargs(not_found=InjectionKey('not_found'))
+    class not_found(Plugin):
+        '''This plugin fails to instantiate because it has a missing dependency
+                       '''
+        name = 'not_found'
+
+    ainjector.add_provider(not_found)
+    with pytest.raises(InjectionFailed):
+        await ainjector.filter_instantiate_async(Plugin, ['name'], ready=True)
```

### Comparing `carthage-0.30.dev1/tests/test_event.py` & `carthage-0.32/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_image.py` & `carthage-0.32/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_kvstore.py` & `carthage-0.32/tests/test_kvstore.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_modeling.py` & `carthage-0.32/tests/test_modeling.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 def test_container(injector):
     class Foo(Injectable):
         pass
 
     def extra_container(domain):
         d = domain
 
-        @provides(InjectionKey("included", constraint=20))
+        @provides(InjectionKey(ModelGroup, constraint=20))
         class Baz(ModelGroup):
             domain = d
 
             class server(MachineModel):
                 name = "server"
         return Baz
 
@@ -93,15 +93,15 @@
 
         net_config = injector_access(InjectionKey(NetworkConfig, domain="evil.com"))
 
         class RedEnclave(Enclave):
 
             domain = "evil.com"
 
-            @propagate_up()
+            @propagate_key(InjectionKey(NetworkConfig))
             class nc(NetworkConfig):
                 pass
 
             include_container(extra_container)
 
             @provides("site-network", InjectionKey(Network, name="red"))
             class SiteNetwork(NetworkModel):
@@ -469,19 +469,30 @@
             class a(InjectableModel):
                 pass
             add_provider(InjectionKey("b"), a) #should raise
 
 @async_test
 async def test_model_subclass_propagation(ainjector):
     "Test that if a template includes classes to be propagated, subclasses of the template properly propagate those classes."
+    class FirstLevel(InjectableModel): pass
+    propagate_key(InjectionKey(FirstLevel), FirstLevel)
+    @propagate_key(InjectionKey(FirstLevel, level=2))
+    class SecondLevel(FirstLevel): pass
+    
     class TemplateNetwork(NetworkModel):
-        @propagate_up()
+        @propagate_key(InjectionKey(NetworkConfig))
         class net_config(NetworkConfigModel): pass
 
     class layout(CarthageLayout):
         @provides(InjectionKey(Network, role='public'))
         class public_network(TemplateNetwork):
             name = 'public_network'
+
+        @provides(InjectionKey(ModelContainer, name='container'))
+        class container(ModelContainer):
+            class third(SecondLevel): pass
+                  
     ainjector.add_provider(layout)
     l = await ainjector.get_instance_async(layout)
     nc = await l.ainjector.get_instance_async(InjectionKey(NetworkConfig, role='public'))
+    l3 = await l.ainjector.get_instance_async(InjectionKey(FirstLevel, name='container'))
```

### Comparing `carthage-0.30.dev1/tests/test_pki.py` & `carthage-0.32/tests/test_pki.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_plugins.py` & `carthage-0.32/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_podman.py` & `carthage-0.32/tests/test_podman.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @pytest.fixture(scope='session')
 def enable_podman():
     import carthage.plugins
     base_injector(carthage.plugins.load_plugin, 'carthage.podman')
 
 @pytest.fixture()
 def ainjector(ainjector, enable_podman):
-    ainjector = ainjector.claim("test_setup.py")
+    ainjector = ainjector.claim("test_podman.py")
     config = ainjector.injector(carthage.ConfigLayout)
     config.state_dir = state_dir
     state_dir.mkdir(parents=True, exist_ok=True)
     yield ainjector
     shutil.rmtree(state_dir, ignore_errors=True)
 
 @pytest.fixture()
@@ -343,15 +343,15 @@
 @async_test
 async def test_podman_pod_network(layout_fixture):
     "Test networking in a pod"
     layout = layout_fixture
     try:
         try: await layout.net_pod.container.machine.async_become_ready()
         except InjectionFailed as e:
-            if isinstance(e.__cause__, NotImplementedError):
+            if isinstance(e.__cause__.__cause__, NotImplementedError):
                 pytest.xfail('Podman is too old')
             raise
         async with layout.net_pod.container.machine.machine_running():
             await layout.net_pod.container.machine.container_exec('apt', 'update')
             machine = layout.net_pod.container.machine
             await machine.container_exec('apt', '-y', 'install', 'iproute2')
             result = await machine.container_exec('ip', 'addr', 'show')
```

### Comparing `carthage-0.30.dev1/tests/test_setup_tasks.py` & `carthage-0.32/tests/test_setup_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,28 +166,28 @@
 async def test_order_override(ainjector):
     two_called = False
 
     class c (Stampable):
         @setup_task("one")
         def one(self): pass
 
-        @setup_task("foo", order=9200)
+        @setup_task("foo", order=12000)
         def two(self):
             nonlocal two_called
             two_called = True
 
         @setup_task("three")
         def three(self):
             assert two_called is True
 
         @setup_task("before_two", before=two)
         def before_two(self):
             assert two_called is False
 
-    assert c.one.order < 9200
+    assert c.one.order < 12000
     assert c.before_two.order < c.two.order
     assert c.three.order > c.two.order
     await ainjector(c)
 
 
 @async_test
 async def test_mako_task(ainjector):
```

### Comparing `carthage-0.30.dev1/tests/test_utils.py` & `carthage-0.32/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_vm.py` & `carthage-0.32/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `carthage-0.30.dev1/tests/test_vmware.py` & `carthage-0.32/tests/test_vmware.py`

 * *Files identical despite different names*

