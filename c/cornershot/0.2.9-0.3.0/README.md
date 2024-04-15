# Comparing `tmp/cornershot-0.2.9.tar.gz` & `tmp/cornershot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornershot-0.2.9.tar", last modified: Tue Feb  9 11:57:37 2021, max compression
+gzip compressed data, was "cornershot-0.3.0.tar", last modified: Mon Apr 15 07:30:18 2024, max compression
```

## Comparing `cornershot-0.2.9.tar` & `cornershot-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 11:57:37.922578 cornershot-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-02-09 11:57:26.000000 cornershot-0.2.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-02-09 11:57:26.000000 cornershot-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14979 2021-02-09 11:57:37.922578 cornershot-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12479 2021-02-09 11:57:26.000000 cornershot-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 11:57:37.922578 cornershot-0.2.9/cornershot/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7550 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/cornershot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 11:57:37.922578 cornershot-0.2.9/cornershot/shots/
--rw-r--r--   0 runner    (1001) docker     (121)     4734 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/shots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/shots/even.py
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/shots/even6.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/shots/rprn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-02-09 11:57:26.000000 cornershot-0.2.9/cornershot/shots/rrp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-09 11:57:37.922578 cornershot-0.2.9/cornershot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14979 2021-02-09 11:57:37.000000 cornershot-0.2.9/cornershot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-02-09 11:57:37.000000 cornershot-0.2.9/cornershot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-09 11:57:37.000000 cornershot-0.2.9/cornershot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-02-09 11:57:37.000000 cornershot-0.2.9/cornershot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-02-09 11:57:37.000000 cornershot-0.2.9/cornershot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-02-09 11:57:37.922578 cornershot-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2021-02-09 11:57:26.000000 cornershot-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:30:18.102000 cornershot-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 07:30:09.000000 cornershot-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 07:30:09.000000 cornershot-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-04-15 07:30:18.102000 cornershot-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-04-15 07:30:09.000000 cornershot-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:30:18.102000 cornershot-0.3.0/cornershot/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/cornershot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:30:18.102000 cornershot-0.3.0/cornershot/shots/
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/shots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/shots/even.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/shots/even6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/shots/rprn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 07:30:09.000000 cornershot-0.3.0/cornershot/shots/rrp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:30:18.102000 cornershot-0.3.0/cornershot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-04-15 07:30:18.000000 cornershot-0.3.0/cornershot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-15 07:30:18.000000 cornershot-0.3.0/cornershot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:30:18.000000 cornershot-0.3.0/cornershot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 07:30:18.000000 cornershot-0.3.0/cornershot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 07:30:18.000000 cornershot-0.3.0/cornershot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-15 07:30:18.106000 cornershot-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-15 07:30:09.000000 cornershot-0.3.0/setup.py
```

### Comparing `cornershot-0.2.9/LICENSE.txt` & `cornershot-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cornershot-0.2.9/PKG-INFO` & `cornershot-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,216 +1,222 @@
 Metadata-Version: 2.1
 Name: cornershot
-Version: 0.2.9
+Version: 0.3.0
 Summary: Library to test network connectivity
 Home-page: https://github.com/zeronetworks/cornershot
 Author: Sagie Dulce, Zero Networks
 Author-email: support@zeronetworks.com
 License: Apache v2
-Description: # What is CornerShot
-        In warfare, CornerShot is a weapon that allows a soldier to look past a corner (and possibly take a shot), without risking exposure.
-        Similarly, the CornerShot package allows one to look at a remote host’s network access without the need to have any special privileges on that host.
-        
-        Using CornerShot, a **source**, with network access to **carrier**, can determine whether there is network access between the **carrier** and **target** for a specific port **p**.
-        
-        For example, let's assume an red team is trying to propagate from a "compromised" source host A, to a target host X, for which host A has no access to. 
-        If they propagate through host B, only then they will discover that there is not network access between host B and X. 
-        
-        By using CornerShot, the team can discover that host C actually has access to target X, so propagation towards target X should go through host C first.   
-        
-        ```
-        +-----+        +-----+          +-----+
-        |     |        |     | filtered |     |
-        |  A  +-------->  B  +----X--->(p) X  |
-        |     |        |     |          |     |
-        +-----+        +-----+          +-(p)-+
-         source      carrier        target
-           +                               ^
-           |                               |
-           |           +-----+             |
-           |           |     |   open      |
-           +---------->+  C  +-------------+
-                       |     |
-                       +-----+
-        
-        
-        ```
-        
-        Similarly to [nmap](https://nmap.org/), CornerShot differentiates between the following state of ports: *open*,*closed*, *filtered* and *unknown* (if it can't be determined).
-        
-        The following demo shows running CornerShot against two carriers hosts 172.0.1.12 & 172.0.1.13, in order to determine if the have network access to 192.168.200.1:
-        
-        ![cornershot demo](./demos/csdemo.gif)  
-        
-        Read more [here](https://zeronetworks.com/blog/adversary-resilience-via-least-privilege-networking-part-1/).
-        
-        # Use Cases
-        
-        ## Single Deployment for Complete Network Visibility
-        The seemingly simple task of identifying if some host B in the network has access to host C may require large deployment of network sensors, device agents or collection of a multitude of firewall rules, router configurations and host policies. 
-        
-        CornerShot can simplify this process by using one (or very few) agents that can query other hosts in the network, to determine their access to remote hosts.  
-          
-        ## Validate BloodHound Paths
-        Security teams that utilize BloodHound to find, and mitigate, privilege escalation paths inside their network, often struggle with millions of logical paths discovered by BloodHound.
-        
-        [ShotHound](https://github.com/zeronetworks/BloodHound-Tools/tree/main/ShotHound) is a tool that integrated CornerShot with BloodHound, in order to discover practical paths that are supported by network access. 
-        
-        # Getting Started
-        CornerShot can be used as a package, or as a standalone module. The only requirements are Python 3 and the impacket package.
-        
-        ## Installation 
-        
-        ```bash
-        pip install cornershot
-        ```
-        
-        ## Standalone Usage
-        
-        Basic usage requires credentials from a valid domain user, a FQDN domain, a carrier IP and target IP.
-        ```bash
-        python -m cornershot <user> <password> <domain> <carrier> <target>
-        ```
-        
-        To scan a range of carriers against a range of targets, subnets or IP ranges may be used in a comma delimited list:
-        ```bash
-        python -m cornershot <user> <password> <domain> 192.168.1.10-192.168.1.20 192.168.5.0/24,192.168.6.0/24
-        ```
-        
-        By default, CornerShot will try to scan the following ports: 135, 445, 3389, 5985, 5986. The user can provide a comma delimited list of ports and port ranges:
-        ```bash
-        python -m cornershot -tp 22,8080,45000-45005 <user> <password> <domain> <carrier> <target>
-        ```  
-        
-        ## As a Package
-        Within code, one needs to instantiate a CornerShot object with the username, password and domain name of a valid domain user. 
-        Adding carriers, target and ports is achieved via the *add_shots* method. Once ready, the *open_fire* method can be called, which performs only the relevant RPC calls based on the required ports.  
-        
-        ```python
-        from cornershot import CornerShot
-        cs = CornerShot("username", "password", "fqdn")
-        cs.add_shots(carriers=["192.168.1.1"],targets=["192.168.1.2","192.168.1.3"])
-        results = cs.open_fire()
-        ```
-        
-        The result of *open_fire* is a dictionary with keys of carriers, each carrier has another set of keys for targets, and finally, each target holds a dictionary of ports and their respective states. 
-        This is an example format of a result: 
-        ```javascript
-        {'carrier_1': 
-        	{'target_1': 
-        		{135: 'unknown', 445: 'filtered', 3389: 'filtered', 5986: 'filtered', 5985: 'filtered'},
-        	'target_2': 
-        		{135: 'unknown', 445: 'open', 5985: 'unknown', 5986: 'filtered', 3389: 'open'}
-        	}, 
-        'carrier_2': 
-        	{'target_1': 
-        		{3389: 'filtered', 135: 'filtered', 5985: 'filtered', 445: 'filtered', 5986: 'unknown'}, 
-        	'target_2': 
-        		{5985: 'filtered', 5986: 'filtered', 445: 'filtered', 135: 'filtered', 3389: 'open'}
-        	}
-        }
-        ```
-        
-        # How CornerShot Works?
-        
-        CornerShot relies on various, well documented, standard Remote Procedure Call (RPC) methods that are used by various Microsoft services. 
-        By using methods that only require an authenticated account in the domain, CornerShot is able to trigger network traffic from a carrier host to a target.
-        
-        CornerShot is able to determine the remote's port state by measuring the time an RPC call took, and using different error codes for each RPC method.
-        
-        ## RPC Methods
-        
-        The reader may be familiar with the ["printer bug"](https://www.slideshare.net/harmj0y/derbycon-the-unintended-risks-of-trusting-active-directory/41), which was discovered by [Lee Christensen](https://twitter.com/tifkin_). While it is called a bug, it is a well documented behaviour of the printing service, which allows any authenticated user to coerce a remote server to authenticate to any machine, using the [RpcRemoteFindFirstPrinterChangeNotificationEx](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/eb66b221-1c1f-4249-b8bc-c5befec2314d) method.     
-          
-        CornerShot utilizes the following RPC methods from several Microsoft protocols (there are many additional methods, which will be implemented in future versions): 
-         - RPRN    : [RpcOpenPrinter](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/989357e2-446e-4872-bb38-1dce21e1313f)
-         - RRP     : [BaseRegSaveKey](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/f022247d-6ef1-4f46-b195-7f60654f4a0d)
-         - EVEN    : [ElfrOpenBELW](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even/4db1601c-7bc2-4d5c-8375-c58a6f8fc7e1)
-         - EVEN6   : [EvtRpcOpenLogHandle](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even6/30a294b1-4e95-468a-a90a-185a5ea63ea0)
-         
-        Implementation of the protocols themselves is achieved via the wonderful [impacket](https://github.com/SecureAuthCorp/impacket) package.
-           
-        ### RpcOpenPrinter
-        This method receives a [printerName](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/24fcd124-035c-4988-a858-3a7d8d6f7b43) as parameter. 
-        The printerName name can be a path to a local file, a remote file or even to a web printer. By supplying a name that conforms with the WEB_PRINT_SERVER format, it is possible to query any remote port.
-        One example of a web print server name which will trigger HTTP traffic to a remote host and port is: "http://<target_ip>:<target_port>/printers/ppp/.printer".
-        ### BaseRegSaveKey
-        To utilize this method, we need a two step approach: first, open a registry key on the remote host - which results with a valid handle, and second, try and save a backup of this handle to a remote file. 
-        The BaseRegSaveKey method receives a file path to which it can save a backup of a registry, which triggers SMB traffic over port 445 (and 135 as backup) to a target.
-        The registry key CornerShot opens is the HKEY_CURRENT_USER, which is open for reading by default on most client hosts.
-        ### ElfrOpenBELW
-        This function tries to backup Windows events into a file path, which can be remote - in such a case the service will try and access the remote host and path.
-        ### EvtRpcOpenLogHandle
-        Similarly to the EVEN method, only this method utilizes a different version of the Windows Events protocol, which is done directly over TCP - no need for SMB port to be open.
-         
-        ## Determining Port State
-        CornerShot estimates the remote ports' state based on timing factors and error messages received by the RPC method or underlying transport.
-        By experimenting with different Windows hosts and various RPC protocols, we came up with 3 different timing thresholds that prove to work in most network environments.
-        These thresholds are best illustrated with the following figure:
-        ```
-                        +                           +                 +     
-                        |                           |                 |
-             unknown    |       open / closed       |     filtered    |  open
-             /          |                           |                 |
-             open       |                           |                 |
-                        |                           |                 |
-          +-------------+------------------+-----------------+--------------+
-          0            0.5                          20                40    Seconds
-                       MIN                        FILTERED           UPPER  
-        ``` 
-        
-        The MIN threshold is 0.5 seconds, responses below this threshold either mean an error in the underlying RPC method or underlying transport, or a response could have been received from the target host.
-        
-        Replies below FILTERED threshold of 20 seconds could indicate either an open or a closed port, depending on the type of error message received for the method. 
-        
-        Replies between the FILTERED and UPPER threshold of 40 seconds indicate a filtered port for all tested methods (so far...). And requests taking more than the UPPER limit indicate a prolonged open TCP connection.
-        
-        ## OS support
-        Executing Corenershot against different OS versions and configurations will yield different results. Not all Windows versions have the same named pipes or behave the same when queried with the same RPC method. 
-        Most Windows OOTB will not expose SMB and other RPC services over the network, however, experience has shown that in large environments these ports tend to be open and accessible for most of the assets.
-        
-        The following table shows default support for various RPC protocols, given that the appropriate ports are accessible to the carrier host and no configuration changes were made to the host: 
-        
-        | OS            | Supported RPC Protocols   | Required Open Carrier Ports  | Possible Target Ports to Scan | 
-        | ------------- |:-------------------------:| --------------------------------:|  ---------------------------------:|
-        | Windows 7     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
-        | Windows 8     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
-        | Windows 10    | EVEN,EVEN6,RPRN           |     445 / 135 & even6 tcp port   |            **ANY**                 |
-        | Server 2008   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        | Server 2012   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        | Server 2016   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        | Server 2019   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        
-        \* If Webclient service is running on a client machine, additional ports can be scanned. Currently CornerShot does not support this option.
-        
-        \** RPRN protocol is supported on server hosts, however opening a remote web printer does not work (which is why we can't scan ANY target port) - until we find a workaround :wink:  
-        
-        # Developers
-        Additional RPC shots, or any other contribution is welcome! 
-        
-        All RPC methods are implemented under */shots*, and inherit from an abstract class named *BaseRPCShot*. 
-        The */example* folder shows how to create a custom RPC shot and use it in code.  
-        
-        # License
-        CornerShot is released under the Apache 2.0 license. For more details see [LICENSE](https://github.com/zeronetworks/cornershot/blob/expansion_doc/LICENSE.txt).
-        
-        # Contact Us
-        We are happy to hear from you! 
-        For bugs, patches, suggestions on this package, please contact us at [support@zeronetworks.com](mailto:support@zeronetworks.com)
-        
-        
 Keywords: cornershot zerotrust ztna zeronetworks network scanner networkscanner
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: impacket==0.9.23
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/zeronetworks/cornershot)](https://github.com/zeronetworks/cornershot/releases/latest)
+![GitHub all releases](https://img.shields.io/github/downloads/zeronetworks/cornershot/total)
+
+# What is CornerShot
+In warfare, CornerShot is a weapon that allows a soldier to look past a corner (and possibly take a shot), without risking exposure.
+Similarly, the CornerShot package allows one to look at a remote host’s network access without the need to have any special privileges on that host.
+
+Using CornerShot, a **source**, with network access to **carrier**, can determine whether there is network access between the **carrier** and **target** for a specific port **p**.
+
+For example, let's assume an red team is trying to propagate from a "compromised" source host A, to a target host X, for which host A has no access to. 
+If they propagate through host B, only then they will discover that there is not network access between host B and X. 
+
+By using CornerShot, the team can discover that host C actually has access to target X, so propagation towards target X should go through host C first.   
+
+```
++-----+        +-----+          +-----+
+|     |        |     | filtered |     |
+|  A  +-------->  B  +----X--->(p) X  |
+|     |        |     |          |     |
++-----+        +-----+          +-(p)-+
+ source      carrier        target
+   +                               ^
+   |                               |
+   |           +-----+             |
+   |           |     |   open      |
+   +---------->+  C  +-------------+
+               |     |
+               +-----+
+
+
+```
+
+Similarly to [nmap](https://nmap.org/), CornerShot differentiates between the following state of ports: *open*,*closed*, *filtered* and *unknown* (if it can't be determined).
+
+The following demo shows running CornerShot against two carriers hosts 172.0.1.12 & 172.0.1.13, in order to determine if the have network access to 192.168.200.1:
+
+![cornershot demo](./demos/csdemo.gif)  
+
+Read more [here](https://zeronetworks.com/blog/adversary-resilience-via-least-privilege-networking-part-1/).
+
+# Use Cases
+
+## Single Deployment for Complete Network Visibility
+The seemingly simple task of identifying if some host B in the network has access to host C may require large deployment of network sensors, device agents or collection of a multitude of firewall rules, router configurations and host policies. 
+
+CornerShot can simplify this process by using one (or very few) agents that can query other hosts in the network, to determine their access to remote hosts.  
+  
+## Validate BloodHound Paths
+Security teams that utilize BloodHound to find, and mitigate, privilege escalation paths inside their network, often struggle with millions of logical paths discovered by BloodHound.
+
+[ShotHound](https://github.com/zeronetworks/BloodHound-Tools/tree/main/ShotHound) is a tool that integrated CornerShot with BloodHound, in order to discover practical paths that are supported by network access. 
+
+# Getting Started
+CornerShot can be used as a package, or as a standalone module. The only requirements are Python 3 and the impacket package.
+
+## Installation 
+
+```bash
+pip install cornershot
+```
+
+## Standalone Usage
+
+Basic usage requires credentials from a valid domain user, a FQDN domain, a carrier IP and target IP.
+```bash
+python -m cornershot <user> <password> <domain> <carrier> <target>
+```
+
+To scan a range of carriers against a range of targets, subnets or IP ranges may be used in a comma delimited list:
+```bash
+python -m cornershot <user> <password> <domain> 192.168.1.10-192.168.1.20 192.168.5.0/24,192.168.6.0/24
+```
+
+By default, CornerShot will try to scan the following ports: 135, 445, 3389, 5985, 5986. The user can provide a comma delimited list of ports and port ranges:
+```bash
+python -m cornershot -tp 22,8080,45000-45005 <user> <password> <domain> <carrier> <target>
+```  
+
+## As a Package
+Within code, one needs to instantiate a CornerShot object with the username, password and domain name of a valid domain user. 
+Adding carriers, target and ports is achieved via the *add_shots* method. Once ready, the *open_fire* method can be called, which performs only the relevant RPC calls based on the required ports.  
+
+```python
+from cornershot import CornerShot
+cs = CornerShot("username", "password", "fqdn")
+cs.add_shots(carriers=["192.168.1.1"],targets=["192.168.1.2","192.168.1.3"])
+results = cs.open_fire()
+```
+
+The result of *open_fire* is a dictionary with keys of carriers, each carrier has another set of keys for targets, and finally, each target holds a dictionary of ports and their respective states. 
+This is an example format of a result: 
+```javascript
+{'carrier_1': 
+	{'target_1': 
+		{135: 'unknown', 445: 'filtered', 3389: 'filtered', 5986: 'filtered', 5985: 'filtered'},
+	'target_2': 
+		{135: 'unknown', 445: 'open', 5985: 'unknown', 5986: 'filtered', 3389: 'open'}
+	}, 
+'carrier_2': 
+	{'target_1': 
+		{3389: 'filtered', 135: 'filtered', 5985: 'filtered', 445: 'filtered', 5986: 'unknown'}, 
+	'target_2': 
+		{5985: 'filtered', 5986: 'filtered', 445: 'filtered', 135: 'filtered', 3389: 'open'}
+	}
+}
+```
+
+# How CornerShot Works?
+
+CornerShot relies on various, well documented, standard Remote Procedure Call (RPC) methods that are used by various Microsoft services. 
+By using methods that only require an authenticated account in the domain, CornerShot is able to trigger network traffic from a carrier host to a target.
+
+CornerShot is able to determine the remote's port state by measuring the time an RPC call took, and using different error codes for each RPC method.
+
+## RPC Methods
+
+The reader may be familiar with the ["printer bug"](https://www.slideshare.net/harmj0y/derbycon-the-unintended-risks-of-trusting-active-directory/41), which was discovered by [Lee Christensen](https://twitter.com/tifkin_). While it is called a bug, it is a well documented behaviour of the printing service, which allows any authenticated user to coerce a remote server to authenticate to any machine, using the [RpcRemoteFindFirstPrinterChangeNotificationEx](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/eb66b221-1c1f-4249-b8bc-c5befec2314d) method.     
+  
+CornerShot utilizes the following RPC methods from several Microsoft protocols (there are many additional methods, which will be implemented in future versions): 
+ - RPRN    : [RpcOpenPrinter](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/989357e2-446e-4872-bb38-1dce21e1313f)
+ - RRP     : [BaseRegSaveKey](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/f022247d-6ef1-4f46-b195-7f60654f4a0d)
+ - EVEN    : [ElfrOpenBELW](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even/4db1601c-7bc2-4d5c-8375-c58a6f8fc7e1)
+ - EVEN6   : [EvtRpcOpenLogHandle](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even6/30a294b1-4e95-468a-a90a-185a5ea63ea0)
+ 
+Implementation of the protocols themselves is achieved via the wonderful [impacket](https://github.com/SecureAuthCorp/impacket) package.
+   
+### RpcOpenPrinter
+This method receives a [printerName](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/24fcd124-035c-4988-a858-3a7d8d6f7b43) as parameter. 
+The printerName name can be a path to a local file, a remote file or even to a web printer. By supplying a name that conforms with the WEB_PRINT_SERVER format, it is possible to query any remote port.
+One example of a web print server name which will trigger HTTP traffic to a remote host and port is: "http://<target_ip>:<target_port>/printers/ppp/.printer".
+### BaseRegSaveKey
+To utilize this method, we need a two step approach: first, open a registry key on the remote host - which results with a valid handle, and second, try and save a backup of this handle to a remote file. 
+The BaseRegSaveKey method receives a file path to which it can save a backup of a registry, which triggers SMB traffic over port 445 (and 135 as backup) to a target.
+The registry key CornerShot opens is the HKEY_CURRENT_USER, which is open for reading by default on most client hosts.
+### ElfrOpenBELW
+This function tries to backup Windows events into a file path, which can be remote - in such a case the service will try and access the remote host and path.
+### EvtRpcOpenLogHandle
+Similarly to the EVEN method, only this method utilizes a different version of the Windows Events protocol, which is done directly over TCP - no need for SMB port to be open.
+ 
+## Determining Port State
+CornerShot estimates the remote ports' state based on timing factors and error messages received by the RPC method or underlying transport.
+By experimenting with different Windows hosts and various RPC protocols, we came up with 3 different timing thresholds that prove to work in most network environments.
+These thresholds are best illustrated with the following figure:
+```
+                +                           +                 +     
+                |                           |                 |
+     unknown    |       open / closed       |     filtered    |  open
+     /          |                           |                 |
+     open       |                           |                 |
+                |                           |                 |
+  +-------------+------------------+-----------------+--------------+
+  0            0.5                          20                40    Seconds
+               MIN                        FILTERED           UPPER  
+``` 
+
+The MIN threshold is 0.5 seconds, responses below this threshold either mean an error in the underlying RPC method or underlying transport, or a response could have been received from the target host.
+
+Replies below FILTERED threshold of 20 seconds could indicate either an open or a closed port, depending on the type of error message received for the method. 
+
+Replies between the FILTERED and UPPER threshold of 40 seconds indicate a filtered port for all tested methods (so far...). And requests taking more than the UPPER limit indicate a prolonged open TCP connection.
+
+## OS support
+Executing Corenershot against different OS versions and configurations will yield different results. Not all Windows versions have the same named pipes or behave the same when queried with the same RPC method. 
+Most Windows OOTB will not expose SMB and other RPC services over the network, however, experience has shown that in large environments these ports tend to be open and accessible for most of the assets.
+
+The following table shows default support for various RPC protocols, given that the appropriate ports are accessible to the carrier host and no configuration changes were made to the host: 
+
+| OS            | Supported RPC Protocols   | Required Open Carrier Ports  | Possible Target Ports to Scan | 
+| ------------- |:-------------------------:| --------------------------------:|  ---------------------------------:|
+| Windows 7     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
+| Windows 8     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
+| Windows 10    | EVEN,EVEN6,RPRN           |     445 / 135 & even6 tcp port   |            **ANY**                 |
+| Server 2008   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+| Server 2012   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+| Server 2016   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+| Server 2019   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+
+\* If Webclient service is running on a client machine, additional ports can be scanned. Currently CornerShot does not support this option.
+
+\** RPRN protocol is supported on server hosts, however opening a remote web printer does not work (which is why we can't scan ANY target port) - until we find a workaround :wink:  
+
+# Developers
+Additional RPC shots, or any other contribution is welcome! 
+
+All RPC methods are implemented under */shots*, and inherit from an abstract class named *BaseRPCShot*. 
+The */example* folder shows how to create a custom RPC shot and use it in code.  
+
+# License
+CornerShot is released under the Apache 2.0 license. For more details see [LICENSE](https://github.com/zeronetworks/cornershot/blob/expansion_doc/LICENSE.txt).
+
+# Contact Us
+We are happy to hear from you! 
+For bugs, patches, suggestions on this package, please contact us at [support@zeronetworks.com](mailto:support@zeronetworks.com)
+
```

### Comparing `cornershot-0.2.9/README.md` & `cornershot-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/zeronetworks/cornershot)](https://github.com/zeronetworks/cornershot/releases/latest)
+![GitHub all releases](https://img.shields.io/github/downloads/zeronetworks/cornershot/total)
+
 # What is CornerShot
 In warfare, CornerShot is a weapon that allows a soldier to look past a corner (and possibly take a shot), without risking exposure.
 Similarly, the CornerShot package allows one to look at a remote host’s network access without the need to have any special privileges on that host.
 
 Using CornerShot, a **source**, with network access to **carrier**, can determine whether there is network access between the **carrier** and **target** for a specific port **p**.
 
 For example, let's assume an red team is trying to propagate from a "compromised" source host A, to a target host X, for which host A has no access to.
```

### Comparing `cornershot-0.2.9/cornershot/__main__.py` & `cornershot-0.3.0/cornershot/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from argparse import ArgumentParser
 import re
 from ipaddress import ip_network, AddressValueError, NetmaskValueError, summarize_address_range, ip_address,collapse_addresses
 from .cornershot import CornerShot
 from . import logger
 import logging
-from json import dumps
+from json import dump, dumps
 
 DEFAULT_NUM_THREADS = 200
 DEFAULT_TARGET_PORTS = [135, 445, 3389, 5985, 5986]
+OUTPUT_FILE_NAME = 'cornershot.json'
 
 INVALID_SUBNET_ERROR_MESSAGE = f"please pick a valid comma delimited list of ip subnet or range such as '192.168.10.0/24,10.9.0.0-10.9.0.255'"
 INVALID_PORTS_ERROR_MESSAGE = f"please pick a valid comma delimited list of port ranges, or list of ports"
 
 
 def parse_args():
     parser = ArgumentParser(prog="CornerShot", prefix_chars="-/", add_help=False, description=f'Corner Shooter')
@@ -21,14 +22,15 @@
     parser.add_argument("password", help="domain password", type=str)
     parser.add_argument("domain", help="the FQDN of the domain.", type=str)
     parser.add_argument("carrier", help="carrier host for cornershot", type=str)
     parser.add_argument("target", help="target for shot", type=str)
     parser.add_argument("-tp", "--tports", dest='tports', default=DEFAULT_TARGET_PORTS, help="comma delimited list of target port ranges to scan for", type=str)
     parser.add_argument("-w", "--workerthreads", dest='threads', help="number of threads to perform shots", default=DEFAULT_NUM_THREADS, type=int)
     parser.add_argument('-v', dest='verbose', action='store_true', help='enable verbose logging')
+    parser.add_argument('-f', '--file', dest='output_to_file', action='store_true', help='write output to file')
 
     args = parser.parse_args()
 
     return args
 
 
 def set_logger(is_verbose):
@@ -97,14 +99,20 @@
                 raise ValueError(INVALID_PORTS_ERROR_MESSAGE)
     else:
         raise ValueError(INVALID_PORTS_ERROR_MESSAGE)
 
     return port_ranges
 
 
+def write_output_to_file(results, filename=OUTPUT_FILE_NAME):
+    with open(filename, 'w', encoding='utf-8') as f:
+        dump(results, f, ensure_ascii=False, indent=4)
+    logger.info(f'Written output to {filename}')
+
+
 if __name__ == '__main__':
     try:
         cs = None
         args = parse_args()
         set_logger(args.verbose)
         logger.info('CornerShot starting...')
 
@@ -117,8 +125,12 @@
     except Exception as err:
         logger.error(f"CornerShot got exception - {err}")
         logger.debug(f"CornerShot unexpected exception!", exc_info=True)
     finally:
         logger.info('CornerShot finished...')
         if cs:
             res = cs.read_results()
-            if res: logger.info(dumps(res,indent=4))
+            if res:
+                if args.output_to_file:
+                    write_output_to_file(res)
+                else:
+                    logger.info(dumps(res,indent=4))
```

### Comparing `cornershot-0.2.9/cornershot/cornershot.py` & `cornershot-0.3.0/cornershot/cornershot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import queue
 import threading
 import time
 from random import uniform,shuffle
 
-from .shots import PORT_UNKNOWN,PORT_FILTERED
+from .shots import PORT_UNKNOWN,PORT_FILTERED,PORT_OPEN
 from .shots.even import EVENShot
 from .shots.even6 import EVEN6Shot
 from .shots.rprn import RPRNShot
 from .shots.rrp import RRPShot
 
 from . import logger
 
@@ -33,14 +33,15 @@
         self.runthreads = True
         self.results = {}
         self.shot_list = []
         self.total_shots = 0
         self.current_tasks = []
         self.skip_scanned = False
         self.already_scanned = []
+        self.batch_scanned_event = None
 
     def _takeashot(self):
         while self.runthreads:
             res = None
             try:
                 bullet = self.bulletQ.get(timeout=0.1)
                 if bullet:
@@ -88,18 +89,17 @@
         for destination in destinations:
             for target in targets:
                 for target_port in target_ports:
                     for cls in self._get_suitable_shots(target_port, destination_ports):
                         self.shot_list.append(cls(self.username, self.password, self.domain, destination, target,target_port=target_port))
 
     def _merge_result(self, dest, target, tport, state):
-        if self.skip_scanned and PORT_UNKNOWN not in state:
-            tp_pair = target + ":" + str(tport)
-            if tp_pair not in self.already_scanned:
-                self.already_scanned.append(tp_pair)
+        if self.skip_scanned and PORT_OPEN in state:
+            if target not in self.already_scanned:
+                self.already_scanned.append(target)
 
         if dest not in self.results:
             self.results[dest] = {}
         if target not in self.results[dest]:
             self.results[dest][target] = {}
         if tport not in self.results[dest][target]:
             self.results[dest][target][tport] = state
@@ -118,77 +118,82 @@
 
         new_tasks = []
         remaining = min(len(self.shot_list),remaining)
         if self.skip_scanned:
             iterated_shots = 0
             for bullet in self.shot_list:
                 if remaining > 0:
-                    trgt = bullet.target + ":" + str(bullet.trgt_port)
-                    if trgt not in self.already_scanned:
+                    if bullet.target not in self.already_scanned:
                         new_tasks.append(bullet)
                     else:
-                        logger.info(f"Skipping {trgt}, already scanned...")
+                        logger.info(f"Skipping {bullet.target}, already scanned...")
                         self.total_shots -= 1
                     iterated_shots += 1
                     remaining -= 1
                 else:
                     break
             self.shot_list = self.shot_list[iterated_shots:]
 
         else:
             new_tasks = self.shot_list[0:remaining ]
-            self.shot_list = self.shot_list[remaining + 1:]
+            self.shot_list = self.shot_list[remaining:]
 
         return new_tasks
 
-
     def _shots_manager(self):
-        remaining = MAX_QUEUE_SIZE
+        remaining = min(self.workers,MAX_QUEUE_SIZE)
+        shuffle(self.shot_list)
         self.total_shots = len(self.shot_list)
+
         while self.runthreads:
             self.current_tasks = self._get_next_tasks(remaining)
 
-            shuffle(self.current_tasks)
-
             remaining = remaining - len(self.current_tasks)
 
             for bt in self.current_tasks:
                 self.bulletQ.put(bt)
 
             while True:
                 try:
                     result = self.resultQ.get(timeout=5)
                     if result:
                         destination, target, target_port, state = result
                         self._merge_result(destination, target, target_port, state)
                     self.resultQ.task_done()
                     remaining += 1
                     self.total_shots -= 1
+                    if self.total_shots % 500 == 0 and self.batch_scanned_event is not None:  # skip if blocking == True
+                        self.batch_scanned_event.set()
                     if self.total_shots < 1:
                         self.runthreads = False
                 except (TimeoutError,queue.Empty):
                     break
 
         self.total_shots = 0
+        self.batch_scanned_event.set() if self.batch_scanned_event is not None else None  # skip if blocking == True
 
     def open_fire(self,blocking=True,skip_scanned=False):
         self.skip_scanned = skip_scanned
+        self.total_shots = len(self.shot_list)
 
-        num_threads = min(self.total_shots,self.workers)
+        self.workers = min(self.total_shots,self.workers)
 
         if self.total_shots > 0:
-            for _ in range(num_threads):
+            for _ in range(self.workers):
                 w = threading.Thread(target=self._takeashot, daemon=True)
                 w.start()
+
         if blocking:
             self._shots_manager()
             return self.results
         else:
             main_thread = threading.Thread(target=self._shots_manager,daemon=True)
             main_thread.start()
+            self.batch_scanned_event = threading.Event()
+            return self.batch_scanned_event
 
     def read_results(self):
         return self.results
 
     def remaining_shots(self):
         return self.total_shots
```

### Comparing `cornershot-0.2.9/cornershot/shots/__init__.py` & `cornershot-0.3.0/cornershot/shots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import asyncio
 from abc import ABCMeta, abstractmethod
 
 from impacket.dcerpc.v5 import transport
 from impacket.dcerpc.v5.rpcrt import DCERPCException
 
 from .. import logger
```

### Comparing `cornershot-0.2.9/cornershot/shots/even.py` & `cornershot-0.3.0/cornershot/shots/even.py`

 * *Files identical despite different names*

### Comparing `cornershot-0.2.9/cornershot/shots/even6.py` & `cornershot-0.3.0/cornershot/shots/even6.py`

 * *Files identical despite different names*

### Comparing `cornershot-0.2.9/cornershot/shots/rprn.py` & `cornershot-0.3.0/cornershot/shots/rprn.py`

 * *Files identical despite different names*

### Comparing `cornershot-0.2.9/cornershot/shots/rrp.py` & `cornershot-0.3.0/cornershot/shots/rrp.py`

 * *Files identical despite different names*

### Comparing `cornershot-0.2.9/cornershot.egg-info/PKG-INFO` & `cornershot-0.3.0/cornershot.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,216 +1,222 @@
 Metadata-Version: 2.1
 Name: cornershot
-Version: 0.2.9
+Version: 0.3.0
 Summary: Library to test network connectivity
 Home-page: https://github.com/zeronetworks/cornershot
 Author: Sagie Dulce, Zero Networks
 Author-email: support@zeronetworks.com
 License: Apache v2
-Description: # What is CornerShot
-        In warfare, CornerShot is a weapon that allows a soldier to look past a corner (and possibly take a shot), without risking exposure.
-        Similarly, the CornerShot package allows one to look at a remote host’s network access without the need to have any special privileges on that host.
-        
-        Using CornerShot, a **source**, with network access to **carrier**, can determine whether there is network access between the **carrier** and **target** for a specific port **p**.
-        
-        For example, let's assume an red team is trying to propagate from a "compromised" source host A, to a target host X, for which host A has no access to. 
-        If they propagate through host B, only then they will discover that there is not network access between host B and X. 
-        
-        By using CornerShot, the team can discover that host C actually has access to target X, so propagation towards target X should go through host C first.   
-        
-        ```
-        +-----+        +-----+          +-----+
-        |     |        |     | filtered |     |
-        |  A  +-------->  B  +----X--->(p) X  |
-        |     |        |     |          |     |
-        +-----+        +-----+          +-(p)-+
-         source      carrier        target
-           +                               ^
-           |                               |
-           |           +-----+             |
-           |           |     |   open      |
-           +---------->+  C  +-------------+
-                       |     |
-                       +-----+
-        
-        
-        ```
-        
-        Similarly to [nmap](https://nmap.org/), CornerShot differentiates between the following state of ports: *open*,*closed*, *filtered* and *unknown* (if it can't be determined).
-        
-        The following demo shows running CornerShot against two carriers hosts 172.0.1.12 & 172.0.1.13, in order to determine if the have network access to 192.168.200.1:
-        
-        ![cornershot demo](./demos/csdemo.gif)  
-        
-        Read more [here](https://zeronetworks.com/blog/adversary-resilience-via-least-privilege-networking-part-1/).
-        
-        # Use Cases
-        
-        ## Single Deployment for Complete Network Visibility
-        The seemingly simple task of identifying if some host B in the network has access to host C may require large deployment of network sensors, device agents or collection of a multitude of firewall rules, router configurations and host policies. 
-        
-        CornerShot can simplify this process by using one (or very few) agents that can query other hosts in the network, to determine their access to remote hosts.  
-          
-        ## Validate BloodHound Paths
-        Security teams that utilize BloodHound to find, and mitigate, privilege escalation paths inside their network, often struggle with millions of logical paths discovered by BloodHound.
-        
-        [ShotHound](https://github.com/zeronetworks/BloodHound-Tools/tree/main/ShotHound) is a tool that integrated CornerShot with BloodHound, in order to discover practical paths that are supported by network access. 
-        
-        # Getting Started
-        CornerShot can be used as a package, or as a standalone module. The only requirements are Python 3 and the impacket package.
-        
-        ## Installation 
-        
-        ```bash
-        pip install cornershot
-        ```
-        
-        ## Standalone Usage
-        
-        Basic usage requires credentials from a valid domain user, a FQDN domain, a carrier IP and target IP.
-        ```bash
-        python -m cornershot <user> <password> <domain> <carrier> <target>
-        ```
-        
-        To scan a range of carriers against a range of targets, subnets or IP ranges may be used in a comma delimited list:
-        ```bash
-        python -m cornershot <user> <password> <domain> 192.168.1.10-192.168.1.20 192.168.5.0/24,192.168.6.0/24
-        ```
-        
-        By default, CornerShot will try to scan the following ports: 135, 445, 3389, 5985, 5986. The user can provide a comma delimited list of ports and port ranges:
-        ```bash
-        python -m cornershot -tp 22,8080,45000-45005 <user> <password> <domain> <carrier> <target>
-        ```  
-        
-        ## As a Package
-        Within code, one needs to instantiate a CornerShot object with the username, password and domain name of a valid domain user. 
-        Adding carriers, target and ports is achieved via the *add_shots* method. Once ready, the *open_fire* method can be called, which performs only the relevant RPC calls based on the required ports.  
-        
-        ```python
-        from cornershot import CornerShot
-        cs = CornerShot("username", "password", "fqdn")
-        cs.add_shots(carriers=["192.168.1.1"],targets=["192.168.1.2","192.168.1.3"])
-        results = cs.open_fire()
-        ```
-        
-        The result of *open_fire* is a dictionary with keys of carriers, each carrier has another set of keys for targets, and finally, each target holds a dictionary of ports and their respective states. 
-        This is an example format of a result: 
-        ```javascript
-        {'carrier_1': 
-        	{'target_1': 
-        		{135: 'unknown', 445: 'filtered', 3389: 'filtered', 5986: 'filtered', 5985: 'filtered'},
-        	'target_2': 
-        		{135: 'unknown', 445: 'open', 5985: 'unknown', 5986: 'filtered', 3389: 'open'}
-        	}, 
-        'carrier_2': 
-        	{'target_1': 
-        		{3389: 'filtered', 135: 'filtered', 5985: 'filtered', 445: 'filtered', 5986: 'unknown'}, 
-        	'target_2': 
-        		{5985: 'filtered', 5986: 'filtered', 445: 'filtered', 135: 'filtered', 3389: 'open'}
-        	}
-        }
-        ```
-        
-        # How CornerShot Works?
-        
-        CornerShot relies on various, well documented, standard Remote Procedure Call (RPC) methods that are used by various Microsoft services. 
-        By using methods that only require an authenticated account in the domain, CornerShot is able to trigger network traffic from a carrier host to a target.
-        
-        CornerShot is able to determine the remote's port state by measuring the time an RPC call took, and using different error codes for each RPC method.
-        
-        ## RPC Methods
-        
-        The reader may be familiar with the ["printer bug"](https://www.slideshare.net/harmj0y/derbycon-the-unintended-risks-of-trusting-active-directory/41), which was discovered by [Lee Christensen](https://twitter.com/tifkin_). While it is called a bug, it is a well documented behaviour of the printing service, which allows any authenticated user to coerce a remote server to authenticate to any machine, using the [RpcRemoteFindFirstPrinterChangeNotificationEx](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/eb66b221-1c1f-4249-b8bc-c5befec2314d) method.     
-          
-        CornerShot utilizes the following RPC methods from several Microsoft protocols (there are many additional methods, which will be implemented in future versions): 
-         - RPRN    : [RpcOpenPrinter](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/989357e2-446e-4872-bb38-1dce21e1313f)
-         - RRP     : [BaseRegSaveKey](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/f022247d-6ef1-4f46-b195-7f60654f4a0d)
-         - EVEN    : [ElfrOpenBELW](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even/4db1601c-7bc2-4d5c-8375-c58a6f8fc7e1)
-         - EVEN6   : [EvtRpcOpenLogHandle](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even6/30a294b1-4e95-468a-a90a-185a5ea63ea0)
-         
-        Implementation of the protocols themselves is achieved via the wonderful [impacket](https://github.com/SecureAuthCorp/impacket) package.
-           
-        ### RpcOpenPrinter
-        This method receives a [printerName](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/24fcd124-035c-4988-a858-3a7d8d6f7b43) as parameter. 
-        The printerName name can be a path to a local file, a remote file or even to a web printer. By supplying a name that conforms with the WEB_PRINT_SERVER format, it is possible to query any remote port.
-        One example of a web print server name which will trigger HTTP traffic to a remote host and port is: "http://<target_ip>:<target_port>/printers/ppp/.printer".
-        ### BaseRegSaveKey
-        To utilize this method, we need a two step approach: first, open a registry key on the remote host - which results with a valid handle, and second, try and save a backup of this handle to a remote file. 
-        The BaseRegSaveKey method receives a file path to which it can save a backup of a registry, which triggers SMB traffic over port 445 (and 135 as backup) to a target.
-        The registry key CornerShot opens is the HKEY_CURRENT_USER, which is open for reading by default on most client hosts.
-        ### ElfrOpenBELW
-        This function tries to backup Windows events into a file path, which can be remote - in such a case the service will try and access the remote host and path.
-        ### EvtRpcOpenLogHandle
-        Similarly to the EVEN method, only this method utilizes a different version of the Windows Events protocol, which is done directly over TCP - no need for SMB port to be open.
-         
-        ## Determining Port State
-        CornerShot estimates the remote ports' state based on timing factors and error messages received by the RPC method or underlying transport.
-        By experimenting with different Windows hosts and various RPC protocols, we came up with 3 different timing thresholds that prove to work in most network environments.
-        These thresholds are best illustrated with the following figure:
-        ```
-                        +                           +                 +     
-                        |                           |                 |
-             unknown    |       open / closed       |     filtered    |  open
-             /          |                           |                 |
-             open       |                           |                 |
-                        |                           |                 |
-          +-------------+------------------+-----------------+--------------+
-          0            0.5                          20                40    Seconds
-                       MIN                        FILTERED           UPPER  
-        ``` 
-        
-        The MIN threshold is 0.5 seconds, responses below this threshold either mean an error in the underlying RPC method or underlying transport, or a response could have been received from the target host.
-        
-        Replies below FILTERED threshold of 20 seconds could indicate either an open or a closed port, depending on the type of error message received for the method. 
-        
-        Replies between the FILTERED and UPPER threshold of 40 seconds indicate a filtered port for all tested methods (so far...). And requests taking more than the UPPER limit indicate a prolonged open TCP connection.
-        
-        ## OS support
-        Executing Corenershot against different OS versions and configurations will yield different results. Not all Windows versions have the same named pipes or behave the same when queried with the same RPC method. 
-        Most Windows OOTB will not expose SMB and other RPC services over the network, however, experience has shown that in large environments these ports tend to be open and accessible for most of the assets.
-        
-        The following table shows default support for various RPC protocols, given that the appropriate ports are accessible to the carrier host and no configuration changes were made to the host: 
-        
-        | OS            | Supported RPC Protocols   | Required Open Carrier Ports  | Possible Target Ports to Scan | 
-        | ------------- |:-------------------------:| --------------------------------:|  ---------------------------------:|
-        | Windows 7     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
-        | Windows 8     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
-        | Windows 10    | EVEN,EVEN6,RPRN           |     445 / 135 & even6 tcp port   |            **ANY**                 |
-        | Server 2008   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        | Server 2012   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        | Server 2016   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        | Server 2019   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
-        
-        \* If Webclient service is running on a client machine, additional ports can be scanned. Currently CornerShot does not support this option.
-        
-        \** RPRN protocol is supported on server hosts, however opening a remote web printer does not work (which is why we can't scan ANY target port) - until we find a workaround :wink:  
-        
-        # Developers
-        Additional RPC shots, or any other contribution is welcome! 
-        
-        All RPC methods are implemented under */shots*, and inherit from an abstract class named *BaseRPCShot*. 
-        The */example* folder shows how to create a custom RPC shot and use it in code.  
-        
-        # License
-        CornerShot is released under the Apache 2.0 license. For more details see [LICENSE](https://github.com/zeronetworks/cornershot/blob/expansion_doc/LICENSE.txt).
-        
-        # Contact Us
-        We are happy to hear from you! 
-        For bugs, patches, suggestions on this package, please contact us at [support@zeronetworks.com](mailto:support@zeronetworks.com)
-        
-        
 Keywords: cornershot zerotrust ztna zeronetworks network scanner networkscanner
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: impacket==0.9.23
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
+
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/zeronetworks/cornershot)](https://github.com/zeronetworks/cornershot/releases/latest)
+![GitHub all releases](https://img.shields.io/github/downloads/zeronetworks/cornershot/total)
+
+# What is CornerShot
+In warfare, CornerShot is a weapon that allows a soldier to look past a corner (and possibly take a shot), without risking exposure.
+Similarly, the CornerShot package allows one to look at a remote host’s network access without the need to have any special privileges on that host.
+
+Using CornerShot, a **source**, with network access to **carrier**, can determine whether there is network access between the **carrier** and **target** for a specific port **p**.
+
+For example, let's assume an red team is trying to propagate from a "compromised" source host A, to a target host X, for which host A has no access to. 
+If they propagate through host B, only then they will discover that there is not network access between host B and X. 
+
+By using CornerShot, the team can discover that host C actually has access to target X, so propagation towards target X should go through host C first.   
+
+```
++-----+        +-----+          +-----+
+|     |        |     | filtered |     |
+|  A  +-------->  B  +----X--->(p) X  |
+|     |        |     |          |     |
++-----+        +-----+          +-(p)-+
+ source      carrier        target
+   +                               ^
+   |                               |
+   |           +-----+             |
+   |           |     |   open      |
+   +---------->+  C  +-------------+
+               |     |
+               +-----+
+
+
+```
+
+Similarly to [nmap](https://nmap.org/), CornerShot differentiates between the following state of ports: *open*,*closed*, *filtered* and *unknown* (if it can't be determined).
+
+The following demo shows running CornerShot against two carriers hosts 172.0.1.12 & 172.0.1.13, in order to determine if the have network access to 192.168.200.1:
+
+![cornershot demo](./demos/csdemo.gif)  
+
+Read more [here](https://zeronetworks.com/blog/adversary-resilience-via-least-privilege-networking-part-1/).
+
+# Use Cases
+
+## Single Deployment for Complete Network Visibility
+The seemingly simple task of identifying if some host B in the network has access to host C may require large deployment of network sensors, device agents or collection of a multitude of firewall rules, router configurations and host policies. 
+
+CornerShot can simplify this process by using one (or very few) agents that can query other hosts in the network, to determine their access to remote hosts.  
+  
+## Validate BloodHound Paths
+Security teams that utilize BloodHound to find, and mitigate, privilege escalation paths inside their network, often struggle with millions of logical paths discovered by BloodHound.
+
+[ShotHound](https://github.com/zeronetworks/BloodHound-Tools/tree/main/ShotHound) is a tool that integrated CornerShot with BloodHound, in order to discover practical paths that are supported by network access. 
+
+# Getting Started
+CornerShot can be used as a package, or as a standalone module. The only requirements are Python 3 and the impacket package.
+
+## Installation 
+
+```bash
+pip install cornershot
+```
+
+## Standalone Usage
+
+Basic usage requires credentials from a valid domain user, a FQDN domain, a carrier IP and target IP.
+```bash
+python -m cornershot <user> <password> <domain> <carrier> <target>
+```
+
+To scan a range of carriers against a range of targets, subnets or IP ranges may be used in a comma delimited list:
+```bash
+python -m cornershot <user> <password> <domain> 192.168.1.10-192.168.1.20 192.168.5.0/24,192.168.6.0/24
+```
+
+By default, CornerShot will try to scan the following ports: 135, 445, 3389, 5985, 5986. The user can provide a comma delimited list of ports and port ranges:
+```bash
+python -m cornershot -tp 22,8080,45000-45005 <user> <password> <domain> <carrier> <target>
+```  
+
+## As a Package
+Within code, one needs to instantiate a CornerShot object with the username, password and domain name of a valid domain user. 
+Adding carriers, target and ports is achieved via the *add_shots* method. Once ready, the *open_fire* method can be called, which performs only the relevant RPC calls based on the required ports.  
+
+```python
+from cornershot import CornerShot
+cs = CornerShot("username", "password", "fqdn")
+cs.add_shots(carriers=["192.168.1.1"],targets=["192.168.1.2","192.168.1.3"])
+results = cs.open_fire()
+```
+
+The result of *open_fire* is a dictionary with keys of carriers, each carrier has another set of keys for targets, and finally, each target holds a dictionary of ports and their respective states. 
+This is an example format of a result: 
+```javascript
+{'carrier_1': 
+	{'target_1': 
+		{135: 'unknown', 445: 'filtered', 3389: 'filtered', 5986: 'filtered', 5985: 'filtered'},
+	'target_2': 
+		{135: 'unknown', 445: 'open', 5985: 'unknown', 5986: 'filtered', 3389: 'open'}
+	}, 
+'carrier_2': 
+	{'target_1': 
+		{3389: 'filtered', 135: 'filtered', 5985: 'filtered', 445: 'filtered', 5986: 'unknown'}, 
+	'target_2': 
+		{5985: 'filtered', 5986: 'filtered', 445: 'filtered', 135: 'filtered', 3389: 'open'}
+	}
+}
+```
+
+# How CornerShot Works?
+
+CornerShot relies on various, well documented, standard Remote Procedure Call (RPC) methods that are used by various Microsoft services. 
+By using methods that only require an authenticated account in the domain, CornerShot is able to trigger network traffic from a carrier host to a target.
+
+CornerShot is able to determine the remote's port state by measuring the time an RPC call took, and using different error codes for each RPC method.
+
+## RPC Methods
+
+The reader may be familiar with the ["printer bug"](https://www.slideshare.net/harmj0y/derbycon-the-unintended-risks-of-trusting-active-directory/41), which was discovered by [Lee Christensen](https://twitter.com/tifkin_). While it is called a bug, it is a well documented behaviour of the printing service, which allows any authenticated user to coerce a remote server to authenticate to any machine, using the [RpcRemoteFindFirstPrinterChangeNotificationEx](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/eb66b221-1c1f-4249-b8bc-c5befec2314d) method.     
+  
+CornerShot utilizes the following RPC methods from several Microsoft protocols (there are many additional methods, which will be implemented in future versions): 
+ - RPRN    : [RpcOpenPrinter](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/989357e2-446e-4872-bb38-1dce21e1313f)
+ - RRP     : [BaseRegSaveKey](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rrp/f022247d-6ef1-4f46-b195-7f60654f4a0d)
+ - EVEN    : [ElfrOpenBELW](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even/4db1601c-7bc2-4d5c-8375-c58a6f8fc7e1)
+ - EVEN6   : [EvtRpcOpenLogHandle](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-even6/30a294b1-4e95-468a-a90a-185a5ea63ea0)
+ 
+Implementation of the protocols themselves is achieved via the wonderful [impacket](https://github.com/SecureAuthCorp/impacket) package.
+   
+### RpcOpenPrinter
+This method receives a [printerName](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-rprn/24fcd124-035c-4988-a858-3a7d8d6f7b43) as parameter. 
+The printerName name can be a path to a local file, a remote file or even to a web printer. By supplying a name that conforms with the WEB_PRINT_SERVER format, it is possible to query any remote port.
+One example of a web print server name which will trigger HTTP traffic to a remote host and port is: "http://<target_ip>:<target_port>/printers/ppp/.printer".
+### BaseRegSaveKey
+To utilize this method, we need a two step approach: first, open a registry key on the remote host - which results with a valid handle, and second, try and save a backup of this handle to a remote file. 
+The BaseRegSaveKey method receives a file path to which it can save a backup of a registry, which triggers SMB traffic over port 445 (and 135 as backup) to a target.
+The registry key CornerShot opens is the HKEY_CURRENT_USER, which is open for reading by default on most client hosts.
+### ElfrOpenBELW
+This function tries to backup Windows events into a file path, which can be remote - in such a case the service will try and access the remote host and path.
+### EvtRpcOpenLogHandle
+Similarly to the EVEN method, only this method utilizes a different version of the Windows Events protocol, which is done directly over TCP - no need for SMB port to be open.
+ 
+## Determining Port State
+CornerShot estimates the remote ports' state based on timing factors and error messages received by the RPC method or underlying transport.
+By experimenting with different Windows hosts and various RPC protocols, we came up with 3 different timing thresholds that prove to work in most network environments.
+These thresholds are best illustrated with the following figure:
+```
+                +                           +                 +     
+                |                           |                 |
+     unknown    |       open / closed       |     filtered    |  open
+     /          |                           |                 |
+     open       |                           |                 |
+                |                           |                 |
+  +-------------+------------------+-----------------+--------------+
+  0            0.5                          20                40    Seconds
+               MIN                        FILTERED           UPPER  
+``` 
+
+The MIN threshold is 0.5 seconds, responses below this threshold either mean an error in the underlying RPC method or underlying transport, or a response could have been received from the target host.
+
+Replies below FILTERED threshold of 20 seconds could indicate either an open or a closed port, depending on the type of error message received for the method. 
+
+Replies between the FILTERED and UPPER threshold of 40 seconds indicate a filtered port for all tested methods (so far...). And requests taking more than the UPPER limit indicate a prolonged open TCP connection.
+
+## OS support
+Executing Corenershot against different OS versions and configurations will yield different results. Not all Windows versions have the same named pipes or behave the same when queried with the same RPC method. 
+Most Windows OOTB will not expose SMB and other RPC services over the network, however, experience has shown that in large environments these ports tend to be open and accessible for most of the assets.
+
+The following table shows default support for various RPC protocols, given that the appropriate ports are accessible to the carrier host and no configuration changes were made to the host: 
+
+| OS            | Supported RPC Protocols   | Required Open Carrier Ports  | Possible Target Ports to Scan | 
+| ------------- |:-------------------------:| --------------------------------:|  ---------------------------------:|
+| Windows 7     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
+| Windows 8     | EVEN,EVEN6                |     445 / 135 & even6 tcp port   |            445*                    |
+| Windows 10    | EVEN,EVEN6,RPRN           |     445 / 135 & even6 tcp port   |            **ANY**                 |
+| Server 2008   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+| Server 2012   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+| Server 2016   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+| Server 2019   | EVEN,EVEN6,RRP,RPRN**     |     445 / 135 & even6 tcp port   |            445                     |
+
+\* If Webclient service is running on a client machine, additional ports can be scanned. Currently CornerShot does not support this option.
+
+\** RPRN protocol is supported on server hosts, however opening a remote web printer does not work (which is why we can't scan ANY target port) - until we find a workaround :wink:  
+
+# Developers
+Additional RPC shots, or any other contribution is welcome! 
+
+All RPC methods are implemented under */shots*, and inherit from an abstract class named *BaseRPCShot*. 
+The */example* folder shows how to create a custom RPC shot and use it in code.  
+
+# License
+CornerShot is released under the Apache 2.0 license. For more details see [LICENSE](https://github.com/zeronetworks/cornershot/blob/expansion_doc/LICENSE.txt).
+
+# Contact Us
+We are happy to hear from you! 
+For bugs, patches, suggestions on this package, please contact us at [support@zeronetworks.com](mailto:support@zeronetworks.com)
+
```

### Comparing `cornershot-0.2.9/setup.py` & `cornershot-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     dependencies = f.read().splitlines()
     dependencies = filter(str, dependencies)
     dependencies = list(dependencies)
 
 setup(
     name='cornershot',
     python_requires='>=3',
-    version='0.2.9',
+    version='0.3.0',
     description='Library to test network connectivity',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/zeronetworks/cornershot',
     author='Sagie Dulce, Zero Networks',
     author_email='support@zeronetworks.com',
     license='Apache v2',
```

