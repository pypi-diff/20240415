# Comparing `tmp/hiraid-1.0.42-py3-none-any.whl.zip` & `tmp/hiraid-1.0.46-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,31 @@
-Zip file size: 155192 bytes, number of entries: 48
+Zip file size: 163336 bytes, number of entries: 58
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-09 15:47 hiraid/__init__.py
 -rw-r--r--  2.0 unx     7022 b- defN 20-Dec-22 14:14 hiraid/cmcustomviews.py
--rw-r--r--  2.0 unx      722 b- defN 23-Jan-13 22:33 hiraid/cmdview.py
+-rw-r--r--  2.0 unx      753 b- defN 24-Mar-14 16:46 hiraid/cmdview.py
 -rw-r--r--  2.0 unx     8282 b- defN 22-Jan-29 20:20 hiraid/cmrest.py
 -rw-r--r--  2.0 unx     3027 b- defN 20-Dec-22 14:13 hiraid/cmrestparser.py
 -rw-r--r--  2.0 unx     3442 b- defN 20-Jan-13 12:30 hiraid/cmrestswagger.py
 -rw-r--r--  2.0 unx    10376 b- defN 20-Dec-22 14:14 hiraid/cmviews.py
 -rw-r--r--  2.0 unx     7018 b- defN 20-Dec-10 14:32 hiraid/customhostviews.py
 -rw-r--r--  2.0 unx     8792 b- defN 22-Jan-20 17:53 hiraid/customviews.py
 -rw-r--r--  2.0 unx   102494 b- defN 20-Jun-19 08:07 hiraid/gadedgemigration.py
 -rw-r--r--  2.0 unx    23617 b- defN 21-Jan-19 12:22 hiraid/gadmigration.py
+-rw-r--r--  2.0 unx     2223 b- defN 24-Mar-15 18:27 hiraid/hiraidexception.py
 -rw-r--r--  2.0 unx    23947 b- defN 22-Jul-12 12:25 hiraid/horcm_instance_manager.py
 -rw-r--r--  2.0 unx      380 b- defN 22-Jul-09 15:47 hiraid/horcm_template.py
 -rw-r--r--  2.0 unx     2222 b- defN 21-Jan-19 12:05 hiraid/hostlib.py
 -rw-r--r--  2.0 unx     3958 b- defN 21-Jan-19 12:05 hiraid/hostviews.py
 -rw-r--r--  2.0 unx     1748 b- defN 20-Jan-13 12:33 hiraid/hvexception.py
 -rw-r--r--  2.0 unx     3213 b- defN 20-Dec-22 08:57 hiraid/hvutil.py
 -rw-r--r--  2.0 unx      351 b- defN 23-Jan-13 23:15 hiraid/ldev.py
 -rw-r--r--  2.0 unx     7265 b- defN 20-Jun-17 11:14 hiraid/messaging.py
 -rw-r--r--  2.0 unx     6009 b- defN 20-Jun-25 15:51 hiraid/raidadmin.py
--rw-r--r--  2.0 unx    76219 b- defN 23-Sep-22 14:32 hiraid/raidcom.py
--rw-r--r--  2.0 unx    66535 b- defN 23-Jul-25 08:37 hiraid/raidcomparser.py
+-rw-r--r--  2.0 unx    91898 b- defN 24-Apr-15 18:34 hiraid/raidcom.py
+-rw-r--r--  2.0 unx    73703 b- defN 24-Mar-15 17:42 hiraid/raidcomparser.py
 -rw-r--r--  2.0 unx     5112 b- defN 23-May-16 13:26 hiraid/raidcomstats.py
 -rw-r--r--  2.0 unx    53851 b- defN 22-Mar-15 11:10 hiraid/raidlib.py
 -rw-r--r--  2.0 unx      308 b- defN 20-Jun-02 08:08 hiraid/raidlibStart.py
 -rw-r--r--  2.0 unx     9006 b- defN 22-Jan-31 14:41 hiraid/raidlibput.py
 -rw-r--r--  2.0 unx    38782 b- defN 21-Jan-19 12:05 hiraid/redhatmultipathdparser.py
 -rw-r--r--  2.0 unx     2887 b- defN 21-Mar-07 12:47 hiraid/scriptconf.py
 -rw-r--r--  2.0 unx     7075 b- defN 21-Jan-19 12:05 hiraid/sshhost.py
@@ -34,17 +35,26 @@
 -rw-r--r--  2.0 unx   168313 b- defN 21-Mar-07 12:46 hiraid/storagemigration.py
 -rw-r--r--  2.0 unx     9930 b- defN 22-Jan-30 15:45 hiraid/storagestate.py
 -rw-r--r--  2.0 unx     5860 b- defN 23-Jun-23 13:30 hiraid/v_id.py
 -rw-r--r--  2.0 unx    12461 b- defN 22-Jan-12 13:08 hiraid/views.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-25 11:42 hiraid/historutils/__init__.py
 -rw-r--r--  2.0 unx     9044 b- defN 22-Sep-02 14:40 hiraid/historutils/historutils.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-09 15:47 hiraid/horcm/__init__.py
--rw-r--r--  2.0 unx    33272 b- defN 23-Nov-29 11:47 hiraid/horcm/horcm_cci.py
+-rw-r--r--  2.0 unx      162 b- defN 24-Apr-11 19:16 hiraid/horcm/cci_exceptions.py
+-rw-r--r--  2.0 unx     1747 b- defN 24-Apr-11 13:46 hiraid/horcm/cci_parser.py
+-rw-r--r--  2.0 unx     1847 b- defN 24-Apr-15 18:34 hiraid/horcm/execute_cci.py
+-rw-r--r--  2.0 unx    35377 b- defN 24-Apr-11 19:57 hiraid/horcm/horcm_cci.py
 -rw-r--r--  2.0 unx    23947 b- defN 22-Jul-12 12:25 hiraid/horcm/horcm_instance_manager.py
 -rw-r--r--  2.0 unx      470 b- defN 23-May-18 15:10 hiraid/horcm/horcm_template.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Dec-02 16:28 hiraid-1.0.42.dist-info/LICENSE
--rw-r--r--  2.0 unx     4754 b- defN 23-Dec-02 16:28 hiraid-1.0.42.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-02 16:28 hiraid-1.0.42.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 23-Dec-02 16:28 hiraid-1.0.42.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Dec-02 16:28 hiraid-1.0.42.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3811 b- defN 23-Dec-02 16:28 hiraid-1.0.42.dist-info/RECORD
-48 files, 797456 bytes uncompressed, 149252 bytes compressed:  81.3%
+-rw-r--r--  2.0 unx      151 b- defN 24-Apr-11 11:46 hiraid/horcm/raidqry.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-11 11:53 hiraid/horcm/cci_cmds/__init__.py
+-rw-r--r--  2.0 unx      873 b- defN 24-Apr-11 14:58 hiraid/horcm/cci_cmds/cci_horcmshutdown.py
+-rw-r--r--  2.0 unx      876 b- defN 24-Apr-11 14:50 hiraid/horcm/cci_cmds/cci_horcmstart.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-11 14:11 hiraid/horcm/cci_cmds/cci_raidqry.py
+-rw-r--r--  2.0 unx      151 b- defN 24-Apr-11 11:46 hiraid/horcm/cci_cmds/raidqry.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-Apr-15 18:34 hiraid-1.0.46.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4782 b- defN 24-Apr-15 18:34 hiraid-1.0.46.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 18:34 hiraid-1.0.46.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 24-Apr-15 18:34 hiraid-1.0.46.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-15 18:34 hiraid-1.0.46.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4686 b- defN 24-Apr-15 18:34 hiraid-1.0.46.dist-info/RECORD
+58 files, 832392 bytes uncompressed, 156010 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -27,14 +27,17 @@
 
 Filename: hiraid/gadedgemigration.py
 Comment: 
 
 Filename: hiraid/gadmigration.py
 Comment: 
 
+Filename: hiraid/hiraidexception.py
+Comment: 
+
 Filename: hiraid/horcm_instance_manager.py
 Comment: 
 
 Filename: hiraid/horcm_template.py
 Comment: 
 
 Filename: hiraid/hostlib.py
@@ -111,35 +114,62 @@
 
 Filename: hiraid/historutils/historutils.py
 Comment: 
 
 Filename: hiraid/horcm/__init__.py
 Comment: 
 
+Filename: hiraid/horcm/cci_exceptions.py
+Comment: 
+
+Filename: hiraid/horcm/cci_parser.py
+Comment: 
+
+Filename: hiraid/horcm/execute_cci.py
+Comment: 
+
 Filename: hiraid/horcm/horcm_cci.py
 Comment: 
 
 Filename: hiraid/horcm/horcm_instance_manager.py
 Comment: 
 
 Filename: hiraid/horcm/horcm_template.py
 Comment: 
 
-Filename: hiraid-1.0.42.dist-info/LICENSE
+Filename: hiraid/horcm/raidqry.py
+Comment: 
+
+Filename: hiraid/horcm/cci_cmds/__init__.py
+Comment: 
+
+Filename: hiraid/horcm/cci_cmds/cci_horcmshutdown.py
+Comment: 
+
+Filename: hiraid/horcm/cci_cmds/cci_horcmstart.py
+Comment: 
+
+Filename: hiraid/horcm/cci_cmds/cci_raidqry.py
+Comment: 
+
+Filename: hiraid/horcm/cci_cmds/raidqry.py
+Comment: 
+
+Filename: hiraid-1.0.46.dist-info/LICENSE
 Comment: 
 
-Filename: hiraid-1.0.42.dist-info/METADATA
+Filename: hiraid-1.0.46.dist-info/METADATA
 Comment: 
 
-Filename: hiraid-1.0.42.dist-info/WHEEL
+Filename: hiraid-1.0.46.dist-info/WHEEL
 Comment: 
 
-Filename: hiraid-1.0.42.dist-info/entry_points.txt
+Filename: hiraid-1.0.46.dist-info/entry_points.txt
 Comment: 
 
-Filename: hiraid-1.0.42.dist-info/top_level.txt
+Filename: hiraid-1.0.46.dist-info/top_level.txt
 Comment: 
 
-Filename: hiraid-1.0.42.dist-info/RECORD
+Filename: hiraid-1.0.46.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hiraid/cmdview.py

```diff
@@ -13,16 +13,17 @@
         self.data = []
         self.undocmds = []
         self.undodefs = []
         self.stats = {}
         self.actions = {}
 
 class CmdviewConcurrent():
-    def __init__(self,returncode=[],stdout=[],stderr=[]):
-        self.returncode = returncode
+    def __init__(self,returncodes=[],stdout=[],stderr=[]):
+        self.returncodes = returncodes
+        self.returncode = 0
         self.stdout = stdout
         self.stderr = stderr
         self.view = {}
         self.data = []
         self.cmds = []
         self.undocmds = []
         self.undodefs = []
```

## hiraid/raidcom.py

```diff
@@ -4,32 +4,37 @@
 # Copyright (c) 2021 Hitachi Vantara, Inc. All rights reserved.
 # Author: Darren Chambers <@Darren-Chambers>
 # Author: Giacomo Chiapparini <@gchiapparini-hv>
 # Author: Clive Meakin
 # GNU General Public License v3.0+ (see COPYING or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 import re
+import ast
 import time
+import json
 import logging
 import subprocess
 import collections
 import concurrent.futures
 from .raidcomparser import Raidcomparser
 from .cmdview import Cmdview,CmdviewConcurrent
 from .raidcomstats import Raidcomstats
 from .storagecapabilities import Storagecapabilities
+from .hiraidexception import RaidcomException
+from hicciexceptions.cci_exceptions import *
+from hicciexceptions.cci_exceptions import cci_exceptions_table
 
 
-version = "v1.0.32"
+version = "v1.0.35"
 
 class Raidcom:    
 
     version = version
     
-    def __init__(self,serial,instance,path="/usr/bin/",cciextension='.sh',log=logging,username=None,password=None):
+    def __init__(self,serial,instance,path="/usr/bin/",cciextension='.sh',log=logging,username=None,password=None,asyncmode=False,unlockOnException=True):
 
         self.serial = serial
         self.log = log
         self.instance = instance
         self.path = path
         self.cciextension = cciextension
         self.username = username
@@ -39,14 +44,16 @@
         self.data = {}
         self.stats = {}
         self.successfulcmds = []
         self.undocmds = []
         self.undodefs = []
         self.parser = Raidcomparser(self,log=self.log)
         self.updatestats = Raidcomstats(self,log=self.log)
+        self.asyncmode = asyncmode
+        self.lock = None
         self.login()
         self.identify()
         self.limitations()
 
     def updateview(self,view: dict,viewupdate: dict) -> dict:
         ''' Update dict view with new dict data '''
         for k, v in viewupdate.items():
@@ -69,14 +76,15 @@
         '''
         raidcom get command_status\n
         request_id = <optional request_id>
         '''
         requestid_cmd = ('',f"-request_id {request_id}")[request_id is not None]
         cmd = f"{self.path}raidcom get command_status {requestid_cmd} -I{self.instance} -s {self.serial}"
         cmdreturn = self.execute(cmd,**kwargs)
+        self.parser.getcommandstatus(cmdreturn)
         return cmdreturn
 
     def resetcommandstatus(self, request_id: str='', requestid_cmd='', **kwargs) -> object:
         '''
         raidcom reset command_status
         request_id = <optional request_id>
         '''
@@ -91,23 +99,29 @@
         raidcom lock resource -time <seconds>\n
         arguments\n
         time = <seconds>\n
         '''
         time = ('',f"-time {kwargs.get('time')}")[kwargs.get('time') is not None]
         cmd = f"{self.path}raidcom lock resource {time} -I{self.instance} -s {self.serial}"
         undocmd = ['{}raidcom unlock resource -I{} -s {}'.format(self.path,self.instance,self.serial)]
-        return self.execute(cmd,undocmd,**kwargs)
+        cmdreturn = self.execute(cmd,undocmd,**kwargs)
+        if not cmdreturn.returncode:
+            self.lock = True
+        return cmdreturn
 
     def unlockresource(self, **kwargs) -> object:
         cmd = f"{self.path}raidcom unlock resource -I{self.instance} -s {self.serial}"
         undocmd = [f"{self.path}raidcom lock resource -I{self.instance} -s {self.serial}"]
-        return self.execute(cmd,undocmd,**kwargs)
-
+        cmdreturn = self.execute(cmd,undocmd,**kwargs)
+        if not cmdreturn.returncode:
+            self.lock = False
+        return cmdreturn
+    
     def identify(self, view_keyname: str='_identity', **kwargs) -> object:
-        self.getresource()
+        self.concurrent_getresource()
         self.raidqry()
         cmdreturn = self.parser.identify()
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.log.info(f"Storage identity: {cmdreturn.view}")
         return cmdreturn
 
     def raidqry(self, view_keyname: str='_raidqry', **kwargs) -> object:
@@ -141,20 +155,57 @@
         cmd = f"{self.path}raidcom -logout -I{self.instance} -s {self.serial}"
         return self.execute(cmd,**kwargs)
 
     def limitations(self):
         for limitation in Storagecapabilities.default_limitations:
             setattr(self,limitation,Storagecapabilities.limitations.get(self.v_id,{}).get(limitation,Storagecapabilities.default_limitations[limitation]))
 
-    def getresource(self, view_keyname: str='_resource_groups', **kwargs) -> object:
+    def getresource(self, view_keyname: str='_resource_groups', key='opt', **kwargs) -> object:
+        optcmd = (f'-key {key}','')[not key or key == '']
+        cmd = f"{self.path}raidcom get resource {optcmd} -I{self.instance} -s {self.serial}"
+        cmdreturn = self.execute(cmd,**kwargs)
+        self.parser.getresource(cmdreturn,datafilter=kwargs.get('datafilter',{}))
+        self.updateview(self.views,{view_keyname:cmdreturn.view})
+        return cmdreturn
+    
+    def Xgetresource(self, view_keyname: str='_resource_groups', **kwargs) -> object:
         cmd = f"{self.path}raidcom get resource -key opt -I{self.instance} -s {self.serial}"
         cmdreturn = self.execute(cmd,**kwargs)
         self.parser.getresource(cmdreturn,datafilter=kwargs.get('datafilter',{}))
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         return cmdreturn
+    
+    def concurrent_getresource(self, max_workers: int=5, view_keyname: str='_resource_groups', **kwargs) -> object:
+
+        resource_outputs = []
+        def getresource(key=None):
+            optcmd = (f'-key {key}','')[not key or key == '']
+            cmd = f"{self.path}raidcom get resource {optcmd} -I{self.instance} -s {self.serial}"
+            return self.execute(cmd,**kwargs)
+
+
+        cmdreturn = CmdviewConcurrent()
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+            future_out = { executor.submit(getresource,key=key): key for key in ['opt',None]}
+            for future in concurrent.futures.as_completed(future_out):
+                resource_outputs.append(future.result())
+        
+        cmdreturn = self.parser.concurrent_getresource(resource_outputs)
+        self.updateview(self.views,{view_keyname:cmdreturn.view})
+        return cmdreturn
+
+
+
+
+
+
+
+
+
+
 
     def getresourcebyname(self,view_keyname: str='_resource_groups_named', **kwargs) -> object:
         cmd = f"{self.path}raidcom get resource -key opt -I{self.instance} -s {self.serial}"
         cmdreturn = self.execute(cmd,**kwargs)
         self.parser.getresourcebyname(cmdreturn,datafilter=kwargs.get('datafilter',{}))
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         return cmdreturn
@@ -230,18 +281,15 @@
 
         #self.portcounters()
         #raidcomstats.portcounters(self)
         #self.raidcomstats.portcounters()
         
         return cmdreturn
 
-
-
-
-    def gethostgrp(self,port: str, view_keyname: str='_ports', update_view: bool=True, **kwargs) -> object:
+    def XXXgethostgrp(self,port: str, view_keyname: str='_ports', update_view: bool=True, **kwargs) -> object:
         '''
         raidcom get host_grp\n
         Better to use gethostgrp_key_detail rather than this function.\n
         You will instead obtain unused host groups and more importantly the resource group id.\n
         raidcom host_grp\n
         examples:\n
         host_grps = gethostgrp(port="cl1-a")\n
@@ -254,20 +302,51 @@
         host_grps.view\n
         host_grps.cmd\n
         host_grps.returncode\n
         host_grps.stderr\n
         host_grps.stdout\n
         host_grps.stats\n
         '''
+        
         cmd = f"{self.path}raidcom get host_grp -port {port} -I{self.instance} -s {self.serial}"
         cmdreturn = self.execute(cmd,**kwargs)
         self.parser.gethostgrp(cmdreturn)
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         return cmdreturn
 
+    def gethostgrp(self,port: str, view_keyname: str='_ports', update_view: bool=True, **kwargs) -> object:
+        '''
+        raidcom host_grp -key detail\n
+        examples:\n
+        host_grps = gethostgrp_key_detail(port="cl1-a")\n
+        host_grps = gethostgrp_key_detail(port="cl1-a-140")\n
+        host_grps = gethostgrp_key_detail(port="cl1-a",host_grp_name="MyHostGroup")\n
+        host_grps = gethostgrp_key_detail(port="cl1-a",datafilter={'HMD':'VMWARE_EX'})\n
+        host_grps = gethostgrp_key_detail(port="cl1-a",datafilter={'GROUP_NAME':'MyGostGroup})\n
+        host_grps = gethostgrp_key_detail(port="cl1-a",datafilter={'Anykey_when_val_is_callable':lambda a : 'TEST' in a['GROUP_NAME'] })\n
+        \n
+        Returns Cmdview():\n
+        host_grps.data\n
+        host_grps.view\n
+        host_grps.cmd\n
+        host_grps.returncode\n
+        host_grps.stderr\n
+        host_grps.stdout\n
+        host_grps.stats\n
+        '''
+        
+        '''
+        raidcom get host_grp -key detail\n
+        Differs slightly from raidcom\n
+        If port format cl-port-gid or host_grp_name is supplied with cl-port host_grp is filtered.
+        '''
+        #cmdreturn = self.gethost_grp_keydetail(port=port,view_keyname=view_keyname,update_view=update_view,**kwargs)
+        return self.gethostgrp_key_detail(port=port,view_keyname=view_keyname,update_view=update_view,hostgrp_usage=['_GIDS'],**kwargs)
+        
+
     def gethostgrp_key_detail(self,port: str, view_keyname: str='_ports', update_view: bool=True, **kwargs) -> object:
         '''
         raidcom host_grp -key detail\n
         examples:\n
         host_grps = gethostgrp_key_detail(port="cl1-a")\n
         host_grps = gethostgrp_key_detail(port="cl1-a-140")\n
         host_grps = gethostgrp_key_detail(port="cl1-a",host_grp_name="MyHostGroup")\n
@@ -301,15 +380,15 @@
             #cmdparam = f" -host_grp_name '{host_grp_name}' "
             kwargs['datafilter'] = { 'GROUP_NAME': host_grp_name }
 
         resource_param = ("",f" -resource {kwargs.get('resource')} ")[kwargs.get('resource') is not None]
             
         cmd = f"{self.path}raidcom get host_grp -port {port} -key detail {resource_param} -I{self.instance} -s {self.serial}"
         cmdreturn = self.execute(cmd,**kwargs)
-        self.parser.gethostgrp_key_detail(cmdreturn,datafilter=kwargs.get('datafilter',{}))
+        self.parser.gethostgrp_key_detail(cmdreturn,datafilter=kwargs.get('datafilter',{}),hostgrp_usage=kwargs.get('hostgrp_usage',['_GIDS','_GIDS_UNUSED']))
 
         if update_view:
             self.updateview(self.views,{view_keyname:cmdreturn.view})
             self.updatestats.hostgroupcounters()
 
         return cmdreturn
 
@@ -625,64 +704,282 @@
         ldev.view\n
         ldev.cmd\n
         ldev.undocmds\n
         ldev.returncode\n
         ldev.stderr\n
         ldev.stdout\n
         '''
+        cmdreturn = Cmdview(cmd="addldev")
         cmdparam, ucmdparam, cmddict, ucmddict = '','',{},{}
         options = { 'capacity_saving': ['compression','deduplication_compression','disable'], 'compression_acceleration':['enable','disable'], 'capacity_saving_mode':['inline','postprocess']}
 
         for arg in kwargs:
             if arg in options:
                 if kwargs[arg] not in options[arg]:
-                    raise Exception(f"Optional command argument {arg} has incorrect value {kwargs[arg]}, possible options are {options[arg]}")
+                    message = f"Optional command argument {arg} has incorrect value {kwargs[arg]}, possible options are {options[arg]}"
+                    if self.asyncmode:
+                        cmdreturn.returncode = 999
+                        cmdreturn.stderr = message
+                        return cmdreturn
+                    else:
+                        raise Exception(message)
                 cmdparam = f"{cmdparam} -{arg} {kwargs[arg]} "
                 cmddict[arg] = kwargs[arg]
             if arg == "capacity_saving" and kwargs[arg] != "disable":
                 ucmdparam = f"-operation initialize_capacity_saving"
                 ucmddict['operation'] = 'initialize_capacity_saving'
 
         if ldev_id == 'auto':
             if not start or not end:
-                raise Exception(f"When ldev_id is specified as 'auto' range_start and range_end ldev_ids must also be supplied")
+                message = f"When ldev_id is specified as 'auto' range_start and range_end ldev_ids must also be supplied"
+                if self.asyncmode:
+                    cmdreturn.returncode = 999
+                    cmdreturn.stderr = message
+                    return cmdreturn
+                raise Exception(message)
             else:
                 cmd = f"{self.path}raidcom add ldev -ldev_id auto -ldev_range {start}-{end} -pool {poolid} -capacity {capacity} {cmdparam} -request_id auto -I{self.instance} -s {self.serial}"
                 cmdreturn = self.execute(cmd=cmd,raidcom_asyncronous=False,**kwargs)
         else:
             cmd = f"{self.path}raidcom add ldev -ldev_id auto -ldev_range {ldev_id}-{ldev_id} -pool {poolid} -capacity {capacity} {cmdparam} -request_id auto -I{self.instance} -s {self.serial}"
             cmdreturn = self.execute(cmd=cmd,raidcom_asyncronous=False,**kwargs)
-            
+            print(cmd)
         reqid = cmdreturn.stdout.rstrip().split(' : ')
         
         if not re.search(r'REQID',reqid[0]):
-            raise Exception(f"Unable to obtain REQID from stdout {cmdreturn}.")
+            if self.asyncmode:
+                message = f"Unable to obtain REQID from stdout {cmdreturn}"
+                cmdreturn.returncode = 999
+                cmdreturn.stderr = message
+                return cmdreturn
+            else:
+                raise Exception(message)
         try:
             getcommandstatus = self.getcommandstatus(request_id=reqid[1])
+            print(f"0 {getcommandstatus.view} error: {getcommandstatus.returncode}")
             self.parser.getcommandstatus(getcommandstatus)
+            print(f"1 {getcommandstatus.view}")
             auto_ldev_id = getcommandstatus.data[0]['ID']
             undocmd = f"{self.path}raidcom delete ldev -ldev_id {auto_ldev_id} -pool {poolid} -capacity {capacity} {ucmdparam} -I{self.instance} -s {self.serial}"
+            print(f"undocmd: {undocmd}")
             #undodef = { 'undodef': 'deleteldev', 'args':{ 'ldev_id':auto_ldev_id }.update(ucmddict)}
             undodef = { 'undodef': 'deleteldev', 'args':{ 'ldev_id':auto_ldev_id }}
             cmdreturn.undocmds.insert(0,undocmd)
             cmdreturn.undodefs.insert(0,undodef)
             echo = f'echo "Executing: {undocmd}"'
             self.undocmds.insert(0,undocmd)
             self.undocmds.insert(0,echo)
             self.resetcommandstatus(request_id=reqid[1])
         except Exception as e:
-            raise Exception(f"Failed to create ldev {ldev_id}, request_id {reqid[1]} error {e}")
+            if self.asyncmode:
+                return cmdreturn
+            else:
+                raise Exception(f"Failed to create ldev {ldev_id}, request_id {reqid[1]} error {e}")
 
-        if not kwargs.get('noexec') and return_ldev:
+        print(f"cmdreturn.returncode: {cmdreturn.returncode}")
+        print(f"cmdreturn.expectedreturn: {cmdreturn.expectedreturn}")
+        if not kwargs.get('noexec') and return_ldev and (cmdreturn.returncode == cmdreturn.expectedreturn):
             getldev = self.getldev(ldev_id=auto_ldev_id)
             cmdreturn.data = getldev.data
             cmdreturn.view = getldev.view
         
         return cmdreturn
 
+    def addldevnew(self,ldev_id: str,poolid: int,capacity: int, return_ldev: bool=True, start: int=None, end: int=None, **kwargs) -> object:
+        '''
+        raidcom add ldev -ldev_id <Ldev#> -pool <ID#> -capacity <block_size>\n
+        examples:\n
+        ldev = Raidcom.addldev(ldev_id=12025,poolid=0,capacity=2097152)\n
+        ldev = Raidcom.addldev(ldev_id=12025,poolid=0,capacity="1g")\n
+        ldev = Raidcom.addldev(ldev_id='auto',poolid=0,start=1000,end=2000,capacity="1g",capacity_saving="compression")\n
+        \n
+        Returns Cmdview():\n
+        ldev.data\n
+        ldev.view\n
+        ldev.cmd\n
+        ldev.undocmds\n
+        ldev.returncode\n
+        ldev.stderr\n
+        ldev.stdout\n
+        '''
+        cmdreturn = Cmdview(cmd="addldev")
+        cmdparam, ucmdparam, cmddict, ucmddict = '','',{},{}
+        options = { 'capacity_saving': ['compression','deduplication_compression','disable'], 'compression_acceleration':['enable','disable'], 'capacity_saving_mode':['inline','postprocess']}
+
+        def log(cmdreturn):
+            self.log.error(f"Return > {cmdreturn.returncode}")
+            self.log.error(f"Stdout > {cmdreturn.stdout}")
+            self.log.error(f"Stderr > {cmdreturn.stderr}")
+
+        try:
+            for arg in kwargs:
+                if arg in options and kwargs[arg] not in options[arg]:
+                    cmdreturn.stderr,cmdreturn.returncode = f"Optional command argument {arg} has incorrect value {kwargs[arg]}, possible options supported by this function are {options[arg]}",999
+                    log(cmdreturn)
+                    raise Exception(cmdreturn.stderr)
+                else:
+                    cmdparam = f"{cmdparam} -{arg} {kwargs[arg]} "
+                    cmddict[arg] = kwargs[arg]
+                if arg == "capacity_saving" and kwargs[arg] != "disable":
+                    ucmdparam = f"-operation initialize_capacity_saving"
+                    ucmddict['operation'] = 'initialize_capacity_saving'
+
+            if ldev_id == 'auto':
+                if not start or not end:
+                    cmdreturn.stderr,cmdreturn.returncode = f"When ldev_id is specified as 'auto' range_start and range_end ldev_ids must also be supplied",999
+                    log(cmdreturn)
+                    raise Exception(cmdreturn.stderr)
+                else:
+                    cmd = f"{self.path}raidcom add ldev -ldev_id auto -ldev_range {start}-{end} -pool {poolid} -capacity {capacity} {cmdparam} -request_id auto -I{self.instance} -s {self.serial}"
+            else:
+                cmd = f"{self.path}raidcom add ldev -ldev_id auto -ldev_range {ldev_id}-{ldev_id} -pool {poolid} -capacity {capacity} {cmdparam} -request_id auto -I{self.instance} -s {self.serial}"
+        
+        #except Exception as e:
+        except Exception as e:
+            if self.asyncmode:
+                return cmdreturn
+            else:
+                raise RaidcomException(f"Failed to create ldev {ldev_id} - error {e}",self)
+
+        try:
+            # execute function uses getcommandstatus without request_id so we need to turn it off and check
+            cmdreturn = self.execute(cmd=cmd,raidcom_asyncronous=False,**kwargs)
+            print(f"cmdreturn1: {vars(cmdreturn)}")
+            reqid = cmdreturn.stdout.rstrip().split(' : ')
+            print(f"reqid: {reqid}")
+            if not re.search(r'REQID',reqid[0]):
+                cmdreturn.stderr = f"Unable to obtain REQID from stdout {cmdreturn}"
+                raise Exception(cmdreturn.stderr)
+            getcommandstatus = self.getcommandstatus(request_id=reqid[1])
+            if getcommandstatus.returncode:
+                print(f"getcommandstatus.returncode: {getcommandstatus.returncode}")
+                cmdreturn.stderr = getcommandstatus.stdout
+                cmdreturn.returncode = getcommandstatus.returncode
+                cmdreturn.view = getcommandstatus.view
+                cmdreturn.data = getcommandstatus.data
+                raise Exception(cmdreturn.stderr)
+            else:
+                created_ldev_id = getcommandstatus.data[0]['ID']
+                getldev = self.getldev(ldev_id=created_ldev_id)
+                cmdreturn.data = getldev.data
+                cmdreturn.view = getldev.view
+        except Exception as e:
+            if self.asyncmode:
+                return cmdreturn
+            else:
+                raise RaidcomException(f"Failed to create ldev {ldev_id} - error {e}",self)
+        #finally:
+        return cmdreturn
+        '''
+            getcommandstatus = self.getcommandstatus(request_id=reqid[1])
+            # This should only trigger if we're asyncmode = True otherwise getcommandstatus will kill the process
+            if getcommandstatus.returncode != cmdreturn.expectedreturn:
+                raise Exception(f"Failed to create ldev, error {e}")
+            print(f"VARS----- {vars(getcommandstatus)}")
+            auto_ldev_id = getcommandstatus.data[0]['ID']
+            undocmd = f"{self.path}raidcom delete ldev -ldev_id {auto_ldev_id} -pool {poolid} -capacity {capacity} {ucmdparam} -I{self.instance} -s {self.serial}"
+            undodef = { 'undodef': 'deleteldev', 'args':{ 'ldev_id':auto_ldev_id }}
+            cmdreturn.undocmds.insert(0,undocmd)
+            cmdreturn.undodefs.insert(0,undodef)
+            echo = f'echo "Executing: {undocmd}"'
+            self.undocmds.insert(0,undocmd)
+            self.undocmds.insert(0,echo)
+            self.resetcommandstatus(request_id=reqid[1])
+        except Exception as e:
+            if self.asyncmode:
+                return cmdreturn
+            else:
+                #raise Exception(f"Failed to create ldev {ldev_id}, request_id {reqid[1]} error {e}")
+                raise Exception(f"Failed to create ldev {ldev_id}, error {e}")
+
+        if not kwargs.get('noexec') and return_ldev and (cmdreturn.returncode == cmdreturn.expectedreturn):
+            getldev = self.getldev(ldev_id=auto_ldev_id)
+            cmdreturn.data = getldev.data
+            cmdreturn.view = getldev.view
+        
+        return cmdreturn
+        '''
+        '''
+        for arg in kwargs:
+            if arg in options:
+                if kwargs[arg] not in options[arg]:
+                    message = f"Optional command argument {arg} has incorrect value {kwargs[arg]}, possible options supported by this function are {options[arg]}"
+                    if self.asyncmode:
+                        cmdreturn.returncode = 999
+                        cmdreturn.stderr = message
+                        return cmdreturn
+                    else:
+                        raise Exception(message)
+                cmdparam = f"{cmdparam} -{arg} {kwargs[arg]} "
+                cmddict[arg] = kwargs[arg]
+            if arg == "capacity_saving" and kwargs[arg] != "disable":
+                ucmdparam = f"-operation initialize_capacity_saving"
+                ucmddict['operation'] = 'initialize_capacity_saving'
+
+        if ldev_id == 'auto':
+            if not start or not end:
+                message = f"When ldev_id is specified as 'auto' range_start and range_end ldev_ids must also be supplied"
+                if self.asyncmode:
+                    cmdreturn.returncode = 999
+                    cmdreturn.stderr = message
+                    return cmdreturn
+                raise Exception(message)
+            else:
+                cmd = f"{self.path}raidcom add ldev -ldev_id auto -ldev_range {start}-{end} -pool {poolid} -capacity {capacity} {cmdparam} -request_id auto -I{self.instance} -s {self.serial}"
+                cmdreturn = self.execute(cmd=cmd,raidcom_asyncronous=False,**kwargs)
+        else:
+            cmd = f"{self.path}raidcom add ldev -ldev_id auto -ldev_range {ldev_id}-{ldev_id} -pool {poolid} -capacity {capacity} {cmdparam} -request_id auto -I{self.instance} -s {self.serial}"
+            cmdreturn = self.execute(cmd=cmd,raidcom_asyncronous=False,**kwargs)
+            print(cmd)
+        reqid = cmdreturn.stdout.rstrip().split(' : ')
+        
+        if not re.search(r'REQID',reqid[0]):
+            if self.asyncmode:
+                message = f"Unable to obtain REQID from stdout {cmdreturn}"
+                cmdreturn.returncode = 999
+                cmdreturn.stderr = message
+                return cmdreturn
+            else:
+                raise Exception(message)
+        try:
+            getcommandstatus = self.getcommandstatus(request_id=reqid[1])
+            print(f"0 {getcommandstatus.view} error: {getcommandstatus.returncode}")
+            self.parser.getcommandstatus(getcommandstatus)
+            print(f"1 {getcommandstatus.view}")
+            auto_ldev_id = getcommandstatus.data[0]['ID']
+            undocmd = f"{self.path}raidcom delete ldev -ldev_id {auto_ldev_id} -pool {poolid} -capacity {capacity} {ucmdparam} -I{self.instance} -s {self.serial}"
+            print(f"undocmd: {undocmd}")
+            #undodef = { 'undodef': 'deleteldev', 'args':{ 'ldev_id':auto_ldev_id }.update(ucmddict)}
+            undodef = { 'undodef': 'deleteldev', 'args':{ 'ldev_id':auto_ldev_id }}
+            cmdreturn.undocmds.insert(0,undocmd)
+            cmdreturn.undodefs.insert(0,undodef)
+            echo = f'echo "Executing: {undocmd}"'
+            self.undocmds.insert(0,undocmd)
+            self.undocmds.insert(0,echo)
+            self.resetcommandstatus(request_id=reqid[1])
+        except Exception as e:
+            if self.asyncmode:
+                return cmdreturn
+            else:
+                raise Exception(f"Failed to create ldev {ldev_id}, request_id {reqid[1]} error {e}")
+
+        print(f"cmdreturn.returncode: {cmdreturn.returncode}")
+        print(f"cmdreturn.expectedreturn: {cmdreturn.expectedreturn}")
+        if not kwargs.get('noexec') and return_ldev and (cmdreturn.returncode == cmdreturn.expectedreturn):
+            getldev = self.getldev(ldev_id=auto_ldev_id)
+            cmdreturn.data = getldev.data
+            cmdreturn.view = getldev.view
+        
+        return cmdreturn
+        '''
+
+
+
+
+
     def extendldev(self, ldev_id: str, capacity: int, **kwargs) -> object:
         '''
         ldev_id   = Ldevid to extend\n
         capacity = capacity in blk\n
         Where 'capacity' will add specified blks to current capacity 
         '''
         #self.resetcommandstatus()
@@ -789,15 +1086,15 @@
         cmdreturn = self.execute(cmd,undocmd,**kwargs)
         return cmdreturn
 
     def addhostgrp(self,port: str,host_grp_name: str, **kwargs) -> object:
         cmd = f"{self.path}raidcom add host_grp -host_grp_name '{host_grp_name}' -port {port} -I{self.instance} -s {self.serial}"
         undocmd = [f"{self.path}raidcom delete host_grp -port {'-'.join(port.split('-')[:2])} '{host_grp_name}' -I{self.instance} -s {self.serial}"]
         cmdreturn = self.execute(cmd,undocmd,**kwargs)
-        if not kwargs.get('noexec'):
+        if not kwargs.get('noexec') and (cmdreturn.returncode == cmdreturn.expectedreturn):
             host_grp = self.gethostgrp_key_detail(port='-'.join(port.split('-')[:2]),host_grp_name=host_grp_name)
             cmdreturn.data = host_grp.data
             cmdreturn.view = host_grp.view
         return cmdreturn
 
     def addhostgroup(self,port: str,hostgroupname: str, **kwargs) -> object:
         '''Deprecated in favour of addhostgrp'''
@@ -901,15 +1198,14 @@
         self.resetcommandstatus(reqid[1])
         return cmdreturn
 
     #def addlun(self, port: str, ldev_id: str, lun_id: int='', host_grp_name: str='', gid: int='', **kwargs) -> object:
 
     def addlun(self, port: str, ldev_id: str, **kwargs) -> object:
 
-
         cmdparam = self.cmdparam(port=port, ldev_id=ldev_id, **kwargs)
         if kwargs.get('lun_id'):
             lun_id = kwargs['lun_id']
             cmd = f"{self.path}raidcom add lun -port {port}{cmdparam} -ldev_id {ldev_id} -lun_id {kwargs['lun_id']} -I{self.instance} -s {self.serial}"
             
             #echo = f'echo "Executing: {undocmd}"'
             #self.undocmds.insert(0,undocmd)
@@ -1128,34 +1424,68 @@
     def getquorum(self, view_keyname='_quorum', **kwargs) -> object:
         cmd = f"{self.path}raidcom get quorum -I{self.instance} -s {self.serial}"
         cmdreturn = self.execute(cmd,**kwargs)
         self.parser.getquorum(cmdreturn,datafilter=kwargs.get('datafilter',{}))
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         return cmdreturn
 
+    def getdrive(self,view_keyname: str='_parity_grp', update_view=True, **kwargs) -> object:
+        '''
+        raidcom get drive\n
+        examples:\n
+        drives = getparitygrp()\n
+        drives = getparitygrp(datafilter={'R_TYPE':'14D+2P'})\n
+        drives = getparitygrp(datafilter={'Anykey_when_val_is_callable':lambda a : a['DRIVE_TYPE'] != 'DKS5E-J900SS'})\n\n
+        Returns Cmdview():\n
+        parity_grps.serial\n
+        parity_grps.data\n
+        parity_grps.view\n
+        parity_grps.cmd\n
+        parity_grps.returncode\n
+        parity_grps.stderr\n
+        parity_grps.stdout\n
+        parity_grps.stats\n
+        '''
+        cmd = f"{self.path}raidcom get drive -key opt -I{self.instance} -s {self.serial}"
+        cmdreturn = self.execute(cmd,**kwargs)
+        self.parser.getdrive(cmdreturn,datafilter=kwargs.get('datafilter',{}),**kwargs)
+        if update_view:
+            self.updateview(self.views,{view_keyname:cmdreturn.view})
+            #self.updatestats.portcounters()
+        
+        return cmdreturn        
+
     '''
     concurrent_{functions}
     '''
 
+    def update_concurrent_cmdreturn(self,cmdreturn,future):
+        cmdreturn.stdout.append(future.result().stdout)
+        cmdreturn.stderr.append(future.result().stderr)
+        cmdreturn.data.extend(future.result().data)
+        cmdreturn.cmds.append(future.result().cmd)
+        cmdreturn.undocmds.extend(future.result().undocmds)
+        cmdreturn.returncodes.append(future.result().returncode)
+        cmdreturn.returncode += future.result().returncode
+        self.updateview(cmdreturn.view,future.result().view)
+
     def concurrent_gethostgrps(self,ports: list=[], max_workers: int=30, view_keyname: str='_ports', **kwargs) -> object:
         '''
         host_grps = concurrent_gethostgrps(ports=['cl1-a','cl2-a'])\n
         host_grps = concurrent_gethostgrps(ports=['cl1-a','cl2-a'],datafilter={'HMD':'VMWARE_EX'})\n
         host_grps = concurrent_gethostgrps(port=['cl1-a','cl2-a'],datafilter={'GROUP_NAME':'MyGostGroup})\n
         host_grps = gethostgrp(port=['cl1-a','cl2-a'],datafilter={'Anykey_when_val_is_callable':lambda a : 'TEST' in a['GROUP_NAME'] })\n
         '''
         cmdreturn = CmdviewConcurrent()
         for port in ports: self.checkport(port)
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.gethostgrp_key_detail,port=port,update_view=False,**kwargs): port for port in ports}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
+                
         cmdreturn.serial = self.serial
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.updateview(self.data,{view_keyname:cmdreturn.data})
         self.updatestats.hostgroupcounters()
 
         return cmdreturn
@@ -1166,18 +1496,15 @@
         '''
         cmdreturn = CmdviewConcurrent()
         
         for portgid in portgids: self.checkportgid(portgid)
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.gethbawwn,port=portgid,update_view=False,**kwargs): portgid for portgid in portgids}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
         cmdreturn.serial = self.serial
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))    
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.updateview(self.data,{view_keyname:cmdreturn.data})
         self.updatestats.hbawwncounters()
         return cmdreturn
 
@@ -1187,18 +1514,15 @@
         '''
         cmdreturn = CmdviewConcurrent()
         
         for portgid in portgids: self.checkportgid(portgid)
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.getlun,port=portgid,update_view=False,**kwargs): portgid for portgid in portgids}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
         cmdreturn.serial = self.serial
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.updateview(self.data,{view_keyname:cmdreturn.data})
         self.updatestats.luncounters()
         return cmdreturn
 
@@ -1206,18 +1530,15 @@
         '''
         ldev_ids = [1234,1235,1236]\n
         '''
         cmdreturn = CmdviewConcurrent()
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.getldev,ldev_id=ldev_id,update_view=False,**kwargs): ldev_id for ldev_id in ldev_ids}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
         cmdreturn.serial = self.serial
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))
         
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.updatestats.ldevcounts()
         return cmdreturn
 
@@ -1226,18 +1547,15 @@
         ports=['cl1-a','cl1-a'] \n
         '''
         cmdreturn = CmdviewConcurrent()
         for port in ports: self.checkport(port)
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.getportlogin,port=port,update_view=False,**kwargs): port for port in ports}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
         cmdreturn.serial = self.serial
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.updateview(self.data,{view_keyname:cmdreturn.data})
         self.updatestats.portlogincounters()
         return cmdreturn
 
@@ -1249,18 +1567,15 @@
         '''
         #def raidscanremote(self,port: str, gid=None, mode='TC', view_keyname='_remotereplication', **kwargs) -> object:
         cmdreturn = CmdviewConcurrent()
         for portgid in portgids: self.checkportgid(portgid)
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.raidscanremote,port=portgid,update_view=False,**kwargs): portgid for portgid in portgids}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
         cmdreturn.serial = self.serial
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))
         
         self.updateview(self.views,{view_keyname:cmdreturn.view})
         self.updatestats.ldevcounts()
         return cmdreturn
 
@@ -1300,72 +1615,81 @@
         request_data = []
         for d in ldev_data:
             request_data.append({'ldev_id':d.get('LDEV',d.get('ldev_id')), 'capacity': d.get('VOL_Capacity(BLK)',d.get('capacity')), 'poolid':d.get('B_POOLID',d.get('poolid'))})
         
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_out = { executor.submit(self.addldev,ldev_id=ldev['ldev_id'],capacity=ldev['capacity'],poolid=ldev['poolid'],return_ldev=return_ldevs): ldev for ldev in request_data}
             for future in concurrent.futures.as_completed(future_out):
-                cmdreturn.stdout.append(future.result().stdout)
-                cmdreturn.stderr.append(future.result().stderr)
-                cmdreturn.data.extend(future.result().data)
-                cmdreturn.undocmds.extend(future.result().undocmds)
-                self.updateview(cmdreturn.view,future.result().view)
+                self.update_concurrent_cmdreturn(cmdreturn,future)
         cmdreturn.view = dict(sorted(cmdreturn.view.items()))
         return cmdreturn
 
     def obfuscatepwd(self,cmd):
         if re.search(r' -login ',cmd):
             c = cmd.split()
             c[2] = "******"
             c[3] = "******"
             return ' '.join(c)
         else:
             return cmd
         
-    def execute(self,cmd,undocmds=[],undodefs=[],expectedreturn=0,**kwargs) -> object:
+    def exception_string(self,cmdreturn):
+        return json.dumps(ast.literal_eval(str(vars(cmdreturn))))
+
+    def return_cci_exception(self,cmdreturn):
+        try:
+            errorcode = re.match(r".*\[(.*?)\].*",cmdreturn.stderr,re.DOTALL).group(1)
+            if cci_exceptions_table.get(errorcode,{}).get('return_value',99999) == cmdreturn.returncode:
+                cmdreturn.cci_error = errorcode
+                return cci_exceptions_table[errorcode]['Exception']
+        except:
+            cmdreturn.cci_error = 'Unknown'
+            return Exception
+        
+    def execute(self,cmd,undocmds=[],undodefs=[],expectedreturn=0,raise_err=True,**kwargs) -> object:
 
         cmdreturn = Cmdview(cmd=cmd)
         cmdreturn.expectedreturn = expectedreturn
         cmdreturn.serial = self.serial
         if kwargs.get('noexec'):
             return cmdreturn
         if kwargs.get('raidcom_asyncronous'):
             self.resetcommandstatus()
         self.log.debug(f"Executing: {self.obfuscatepwd(cmd)}")
         #self.log.info(f"Expecting return code {expectedreturn}")
         proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True)
         cmdreturn.stdout, cmdreturn.stderr = proc.communicate()
         cmdreturn.returncode = proc.returncode
         cmdreturn.executed = True
-        
+
         if proc.returncode and proc.returncode != expectedreturn:
             self.log.error("Return > "+str(proc.returncode))
             self.log.error("Stdout > "+cmdreturn.stdout)
             self.log.error("Stderr > "+cmdreturn.stderr)
-            message = {'return':proc.returncode,'stdout':cmdreturn.stdout, 'stderr':cmdreturn.stderr }
-            raise Exception(f"Unable to execute Command '{self.obfuscatepwd(cmd)}'. Command dump > {message}")
-
+            if raise_err:
+                raise self.return_cci_exception(cmdreturn)(self.exception_string(cmdreturn))
+            
         for undocmd in undocmds: 
             echo = f'echo "Executing: {undocmd}"'
             self.undocmds.insert(0,undocmd)
             self.undocmds.insert(0,echo)
             cmdreturn.undocmds.insert(0,undocmd)
-                
+            
         for undodef in undodefs:
             self.undodefs.insert(0,undodef)
             cmdreturn.undodefs.insert(0,undodef)
-
         if self.cmdoutput:
             self.log.info(f"stdout: {cmdreturn.stdout}")
-
         if kwargs.get('raidcom_asyncronous'):
             self.getcommandstatus()
 
-        return cmdreturn
 
+        
+        return cmdreturn
+        
 
 
     # BELOW IS OLD
     '''
 
     def pairevtwaitexec(self,cmd):
         self.log.info('Executing: {}'.format(cmd))
```

## hiraid/raidcomparser.py

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python3.6
 # -----------------------------------------------------------------------------------------------------------------------------------
-# Version v1.1.02
+# Version v1.1.03
 # -----------------------------------------------------------------------------------------------------------------------------------
 #
 # License Terms
 # -------------
 # Unless stated otherwise, Hitachi Vantara Limited and/or its group companies is/are the owner or the licensee
 # of all intellectual property rights in this script. This work is protected by copyright laws and treaties around
 # the world. This script is solely for use by Hitachi Vantara Limited and/or its group companies in the provision
@@ -18,14 +18,18 @@
 #
 # 14/01/2020    v1.1.00     Initial Release - DC
 #
 # 24/01/2020    v1.1.01     Add functions getportlogin getrcu - CM
 #
 # 10/08/2022    v1.1.02     Bug fix, gethbawwn broken view missing wwns - DC
 #
+# 11/02/2023    v1.1.03     Added getdrive - DC
+#
+# 08/03/2024    v1.1.04     Updated gethostgrp_key_detail to allow gethostgrp to be dropped - DC
+#
 # -----------------------------------------------------------------------------------------------------------------------------------
 
 import re
 import collections
 from typing import Callable
 from .historutils.historutils import Storcapunits
 from .cmdview import Cmdview
@@ -150,14 +154,53 @@
             prefilter.append(dict(zip(cmdreturn.headers, row)))
 
         cmdreturn.data = list(filter(lambda r: self.applyfilter(r,datafilter),prefilter))
         createview(cmdreturn)
         self.altview(cmdreturn,altview)
         return cmdreturn
 
+    def concurrent_getresource(self, cmdreturns: list, datafilter: dict={}, altview: Callable=None, **kwargs ) -> dict:
+
+        newcmdreturn = Cmdview("concurrent_getresource")
+        newcmdreturn.rawdata = []
+        newcmdreturn.stats = { 'resource_group_count':0 }
+        prefilter_dict = {}
+        precombine = []
+
+        def createview(cmdreturn):
+            for datadict in cmdreturn.data:
+                #self.log.info(datadict)
+                rgid = datadict['RGID']
+                cmdreturn.view[rgid] = datadict
+                cmdreturn.stats['resource_group_count'] += 1
+
+        for cmdreturn in cmdreturns:
+            print(f"{vars(cmdreturn)}\n\n")
+            #newcmdreturn.rawdata.append(cmdreturn.rawdata)
+            prefilter = []
+            self.initload(cmdreturn)
+            
+            for line in cmdreturn.rawdata:
+                row = line.split()
+                for item in row:
+                    precombine.append(dict(zip(cmdreturn.headers, row)))
+        
+        for r in precombine:
+            rgid = r['RGID']
+            prefilter_dict[rgid] = prefilter_dict.get(rgid,{})
+            for k, v in r.items():
+                prefilter_dict[rgid][k] = v
+
+        prefilter = [value for value in prefilter_dict.values()]
+        newcmdreturn.data = list(filter(lambda r: self.applyfilter(r,datafilter),prefilter))
+        createview(newcmdreturn)
+        return newcmdreturn
+
+
+
     def getresourcebyname(self, cmdreturn: object, datafilter: dict={}, **kwargs) -> dict:
         '''
         stdout as input from get resource command
         '''
         self.initload(cmdreturn)
         cmdreturn.stats = { 'resource_group_count':0 }
 
@@ -319,15 +362,15 @@
         for ldev in listofldevs:
             ldevobj = type('obj', (object,), {'stdout' : ldev, 'view': {}})
             parsedldev = self.getldev(ldevobj)
             self.updateview(cmdreturn.view,parsedldev.view)
             cmdreturn.data.extend(parsedldev.data)
         return cmdreturn
 
-    def gethostgrp(self,cmdreturn: object) -> object:
+    def XXgethostgrp(self,cmdreturn: object) -> object:
 
         self.initload(cmdreturn)
         cmdreturn.stats = { 'hostgroupcount':0 }
 
         for line in cmdreturn.rawdata:
             hmos = ""
             hmolist = []
@@ -354,15 +397,15 @@
 
             for value,head in zip(values,cmdreturn.headers):
                 cmdreturn.view[port]['_GIDS'][gid][head] = value
 
         if cmdreturn.header: cmdreturn.rawdata.insert(0,cmdreturn.header)
         return cmdreturn
 
-    def gethostgrp_key_detail(self,cmdreturn: object, datafilter: dict={}) -> object:
+    def gethostgrp(self,cmdreturn: object, datafilter: dict={}) -> object:
 
         '''
         host_grp_filter = { 'KEY': 'VALUE' | ['VALUE1','VALUE2'], 'KEY2': 'VALUE' | ['VALUE1','VALUE2'] }\n
         e.g. host_grp_filter = { 'HMD': ['LINUX/IRIX','VMWARE_EX'] } filters host groups where HMD is LINUX/IRIX or VMWARE_EX\n
         host_grp_filter is case sensitive in both the key and the value and allows host_grps through only if ALL criteria matches.\n
         Remember that pretty much all of the values are parsed into strings, RGID for example is a string.\n
         '''
@@ -398,20 +441,73 @@
                 #host_mode_options = sorted([int(host_mode) for host_mode in host_mode_options.split(':')])
                 host_mode_options = [str(hmo) for hmo in sorted([int(opt) for opt in host_mode_options.split(':')])]
 
             values = (host_grp_id,port,gid,rgid,nameSpace,serial,hostmode,host_mode_options)
             
             prefiltered_host_grps.append(dict(zip(cmdreturn.headers, values)))
 
-        filtered_host_grps = list(filter(lambda l: self.applyfilter(l,datafilter),prefiltered_host_grps))
+        filtered_host_grps = list(filter(lambda l: self.applyfilter(l,datafilter),filter_unused_grps))
         #filtered_host_grps = list(filter(filter_host_grps,prefiltered_host_grps))
         used_host_grps = list(filter(lambda x: (x['GROUP_NAME'] != '-'),filtered_host_grps))
-        unused_host_grps = list(filter(lambda x: (x['GROUP_NAME'] == '-'),filtered_host_grps))
+        #unused_host_grps = list(filter(lambda x: (x['GROUP_NAME'] == '-'),filtered_host_grps))
         hostgrpsview('_GIDS',used_host_grps)
-        hostgrpsview('_GIDS_UNUSED',unused_host_grps)
+        #hostgrpsview('_GIDS_UNUSED',unused_host_grps)
+        #if cmdreturn.header: cmdreturn.rawdata.insert(0,cmdreturn.header)
+        return cmdreturn
+
+    def gethostgrp_key_detail(self,cmdreturn: object, datafilter: dict={}, hostgrp_usage: list=['_GIDS','_GIDS_UNUSED']) -> object:
+
+        '''
+        host_grp_filter = { 'KEY': 'VALUE' | ['VALUE1','VALUE2'], 'KEY2': 'VALUE' | ['VALUE1','VALUE2'] }\n
+        e.g. host_grp_filter = { 'HMD': ['LINUX/IRIX','VMWARE_EX'] } filters host groups where HMD is LINUX/IRIX or VMWARE_EX\n
+        host_grp_filter is case sensitive in both the key and the value and allows host_grps through only if ALL criteria matches.\n
+        Remember that pretty much all of the values are parsed into strings, RGID for example is a string.\n
+        '''
+        self.initload(cmdreturn)
+        cmdreturn.stats = { '_GIDS':0, '_GIDS_UNUSED':0 }
+
+        def hostgrpsview(gid_key,data):
+            for host_grp_dict in data:
+                #self.log.info(host_grp_dict)
+                port = host_grp_dict['PORT']
+                gid = host_grp_dict['GID']
+                cmdreturn.view[port] = cmdreturn.view.get(port,{})
+                cmdreturn.view[port][gid_key] = cmdreturn.view[port].get(gid_key,{})
+                cmdreturn.view[port][gid_key][gid] = host_grp_dict
+                cmdreturn.data.append(host_grp_dict)
+                cmdreturn.stats[gid_key] += 1
+
+        prefiltered_host_grps = []
+        cmdreturn.headers.insert(0,"HOST_GRP_ID")
+        for line in cmdreturn.rawdata:
+            hostgroupName = re.findall(r'"([^"]*)"', line)
+            if hostgroupName:
+                line = line.replace(f'"{hostgroupName[0]}"','-')
+            port,gid,rgid,nameSpace,serial,hostmode,host_mode_options = line.split()
+            port = re.sub(r'\d+$','', port)
+            host_grp_id = f"{port}-{gid}"
+
+            if hostgroupName:
+                nameSpace = hostgroupName[0]
+            if host_mode_options == "-":
+                host_mode_options = []
+            else:
+                #host_mode_options = sorted([int(host_mode) for host_mode in host_mode_options.split(':')])
+                host_mode_options = [str(hmo) for hmo in sorted([int(opt) for opt in host_mode_options.split(':')])]
+
+            values = (host_grp_id,port,gid,rgid,nameSpace,serial,hostmode,host_mode_options)
+            
+            prefiltered_host_grps.append(dict(zip(cmdreturn.headers, values)))
+
+        filtered_host_grps = list(filter(lambda l: self.applyfilter(l,datafilter),prefiltered_host_grps))
+        host_grps_usage = { '_GIDS': list(filter(lambda x: (x['GROUP_NAME'] != '-'),filtered_host_grps)), '_GIDS_UNUSED': list(filter(lambda x: (x['GROUP_NAME'] == '-'),filtered_host_grps)) }
+
+        for usage in hostgrp_usage:    
+            hostgrpsview(usage,host_grps_usage[usage])
+
         #if cmdreturn.header: cmdreturn.rawdata.insert(0,cmdreturn.header)
         return cmdreturn
 
     def getlun(self,cmdreturn: object,datafilter: dict={}) -> object:
 
         self.initload(cmdreturn)
         cmdreturn.stats = { 'luncount':0 }
@@ -941,15 +1037,86 @@
                 qrdid = datadict['QRDID']
                 cmdreturn.view[qrdid] = cmdreturn.view.get(qrdid,datadict)
                 cmdreturn.stats['quorumcount'] += 1
 
         createview(cmdreturn.data)
         return cmdreturn
 
+    '''
+     def getparitygrp(self,cmdreturn: object, datafilter: dict={}, **kwargs ) -> object:
+
+        self.initload(cmdreturn)
+        cmdreturn.stats = { 'parity_grp_count':0 }
+
+        def createview(cmdreturn):
+            for datadict in cmdreturn.data:
+                #PHG GROUP STS CM IF MP# PORT   WWN                 PR LUN PHS  Serial# PRODUCT_ID LB PM DM QD TO(s) PBW(
+                group = datadict['GROUP']
+                cmdreturn.view[group] = datadict
+                cmdreturn.stats['parity_grp_count'] += 1
+
+        prefilter = []
+        for line in cmdreturn.rawdata:
+            row = line.split()
+            prefilter.append(dict(zip(cmdreturn.headers, row)))
+            
+        cmdreturn.data = list(filter(lambda r: self.applyfilter(r,datafilter),prefilter))
+        createview(cmdreturn)
+        return cmdreturn
+    '''
+
+    '''
+    def getport(self,cmdreturn: object, datafilter: dict={}, **kwargs ) -> object:
+    
+        self.initload(cmdreturn)
+        cmdreturn.stats = { 'portcount':0 }
+
+        def createview(cmdreturn):
+            for datadict in cmdreturn.data:
+                port = datadict['PORT']
+                if port not in cmdreturn.view:
+                    cmdreturn.view[port] = copy.deepcopy(datadict)
+                    cmdreturn.view[port]['ATTR'] = []
+                    cmdreturn.stats['portcount'] += 1
+                cmdreturn.view[port]['ATTR'].append(datadict['ATTR'])
+
+        prefilter = []
+        for line in cmdreturn.rawdata:
+            row = line.split()
+            row[0] = re.sub(r'\d+$','',row[0])
+            prefilter.append(dict(zip(cmdreturn.headers, row)))
+            
+        cmdreturn.data = list(filter(lambda r: self.applyfilter(r,datafilter),prefilter))
+        createview(cmdreturn)
+        return cmdreturn
+    '''
+
+    def getdrive(self,cmdreturn: object,datafilter: dict={}) -> object:
 
+        self.initload(cmdreturn)
+        cmdreturn.stats = { 'drivecount':0 }
+        
+        def createview(data):
+            for datadict in data:
+                group = datadict['GROUP']
+                location = datadict['LOCATION']
+                cmdreturn.view[group] = cmdreturn.view.get(group,{'_DRIVES':{}})
+                cmdreturn.view[group]['_DRIVES'][location] = datadict
+                cmdreturn.stats['drivecount'] += 1 
+
+        prefilter = []
+        for line in cmdreturn.rawdata:
+            row = line.split()
+            prefilter.append(dict(zip(cmdreturn.headers, row)))
+
+        cmdreturn.data = list(filter(lambda l: self.applyfilter(l,datafilter),prefilter))
+        createview(cmdreturn.data)
+
+        return cmdreturn
+    
     def gethostgrpkeyhostgrprgid(self,cmdreturn: object,resourcegroupid):
 
         self.initload(cmdreturn)
         cmdreturn.stats = { 'hostgroupcount':0 }
 
         for line in cmdreturn.rawdata:
             hmos = ""
```

## hiraid/horcm/horcm_cci.py

```diff
@@ -2,19 +2,30 @@
 import os
 import re
 import json
 import time
 import copy
 import logging
 import subprocess
+from .execute_cci import execute as cci_execute
+#from .cci_exceptions import EX_ATTHOR as EX_ATTHOR
+from hiexceptions.horcm.cci_exceptions import *
+from hiexceptions.horcm.cci_exceptions import cci_exceptions_table
+import ast
+#from .cci_cmds import *
+#from .cci_cmds import cci_raidqry
+#from .cci_cmds.cci_raidqry import *
+#from .cci_cmds.cci_horcmshutdown import *
+#from .cci_cmds.cci_horcmstart import *
 from glob import glob
 from string import Template
 from datetime import datetime
 from ..historutils.historutils import Storcapunits as storagecaps
 from ..cmdview import Cmdview
+from .cci_parser import Cci_parser
 
 
 
 try:
     from .horcm_template import default_template
 except:
     from horcm_template import default_template
@@ -41,15 +52,15 @@
     end: Ending instance number to search up to. default = 500\n
     local_inst: 'odd' | 'even' - Specify if you prefer the local horcm instance to be an even number ( default ) or an odd number.\n
     path: horcm binary path default = '/usr/bin'\n
     cciextension: '.sh' ( default ) | '.exe' ( windows )\n
     horcm_template_file: Use an alternate file as your horcm template rather than using the default_template.\n
     Add this horcm and see it break!! /etc/horcm21_tmp.conf
     '''
-    def __init__(self,log=logging,base_service_port: int=11000,horcm_dir: str='/etc',start: int=0,end: int=500,local_inst: str='even',path: str='/usr/bin/',cciextension: str='.sh',horcm_template_file: str=None,):
+    def __init__(self,log=logging,base_service_port: int=11000,horcm_dir: str='/etc',start: int=0,end: int=500,local_inst: str='even',path: str='/usr/bin/',cciextension: str='.sh',horcm_template_file: str=None,raise_err=True):
         
         self.log = log
         self.horcm_template_file = horcm_template_file
         self.horcm_dir = horcm_dir
         self.base_service_port=base_service_port
         self.start = start
         self.end = end
@@ -58,26 +69,61 @@
         self.poll = -1
         self.ip_address = "localhost"
         self.remote_ip_address = "localhost"
         self.timeout = 3000
         self.path = path
         self.cciextension = cciextension
         self.undocmds = []
+        self.parser = Cci_parser(log=self.log)
+        self.raise_err = raise_err
 
     def now(self,format='%d-%m-%Y_%H.%M.%S'):
         return datetime.now().strftime(format)
     
-    def raidqry(self, inst: int):
+    def Xraidqry(self, inst: int):
         cmd = '{}raidqry -l -I{}'.format(self.path,inst)
         stdout, stderr, cmdreturn = self.execute(cmd)
         cmdreturn = Cmdview("raidqry")
         cmdreturn.rawdata = stdout
         self.parse_raidqry(cmdreturn)
         return cmdreturn
 
+    def Xraidqry2(self, inst: int, **kwargs):
+        cmd = '{}raidqry -l -I{}'.format(self.path,inst)
+        cmdreturn = Raidqry(log=self.log,raise_err=self.raise_err).execute(cmd)
+        return cmdreturn
+
+
+    def exception_string(self,cmdreturn):
+        return json.dumps(ast.literal_eval(str(vars(cmdreturn))))
+
+    def raidqry(self, inst: int, acceptable_returns:list=[0], **kwargs):
+        cmd = '{}raidqry -l -I{}'.format(self.path,inst)
+        cmdreturn = cci_execute(cmd,log=self.log,acceptable_returns=acceptable_returns,raise_err=self.raise_err)
+        if cmdreturn.returncode in acceptable_returns:
+            self.parser.raidqry(cmdreturn,datafilter=kwargs.get('datafilter',{}))
+        
+        return cmdreturn
+ 
+    def horcmshutdown(self, inst: int, acceptable_returns:list=[0], **kwargs):
+        self.log.info(f'Shutdown horcm instance {inst}')
+        cmd = f'{self.path}horcmshutdown{self.cciextension} {inst}'
+        cmdreturn = cci_execute(cmd,log=self.log,acceptable_returns=acceptable_returns,raise_err=self.raise_err)
+        return cmdreturn
+    
+    def horcmstart(self, inst: int, acceptable_returns:list=[0], **kwargs):
+        self.log.info(f'Start horcm instance {inst}')
+        cmd = f'{self.path}horcmstart{self.cciextension} {inst}'
+        cmdreturn = cci_execute(cmd,log=self.log,acceptable_returns=acceptable_returns,raise_err=self.raise_err)
+        return cmdreturn
+    
+    def Xhorcmstart(self,inst):
+        self.log.info(f'Start horcm instance {inst}')
+        cmd = f'{self.path}horcmstart{self.cciextension} {inst}'
+        return self.nexecute(cmd)    
 
     def parse_raidqry(self,cmdreturn):
         
         rawdata = [row.strip() for row in list(filter(None,cmdreturn.rawdata.split('\n')))]
         header = rawdata.pop(0)
         cmdreturn.headers = header.split()
 
@@ -89,33 +135,14 @@
         for line in rawdata:
             row = line.split()
             cmdreturn.data.append(dict(zip(cmdreturn.headers, row)))
 
         createview(cmdreturn)
         return cmdreturn
 
-    def XXXXparse_pairdisplay(self,pairdisplay: list) -> dict:
-        '''
-        Returns dictionary of parsed pairdisplay:
-        { Group: { PairVol: { L/R: { heading:data } } } }
-        '''
-        headings = pairdisplay.pop(0).split()
-        view = { 'pairs': {} }
-        for line in pairdisplay:
-            sline = line.split()
-            if len(sline) != len(headings): raise("header and data length mismatch")
-            data = {head:item for item,head in zip(sline,headings)}
-            view['pairs'][data['Group']] = view['pairs'].get(data['Group'],{})
-            view['pairs'][data['Group']][data['PairVol']] = view['pairs'][data['Group']].get(data['PairVol'],{})
-            view['pairs'][data['Group']][data['PairVol']][data['L/R']] = data
-
-        return view
-
-
-
     def return_used_horcm_insts(self):
         with cd(self.horcm_dir) as horcm_dir:
             horcm_files = glob('horcm[0-9]*.conf')
         self.used_insts = sorted([ int(horcm.strip().replace('horcm','').replace('.conf','')) for horcm in horcm_files])
         return self.used_insts
 
     def find_free_horcm_partners(self,start: int=0, end: int=500, local_inst: str='even') -> list:
@@ -258,30 +285,20 @@
         try:
             os.rename(fqfile,fqfilebackup)
             self.log.info('Backed up file {} to {}'.format(fqfile,fqfilebackup))
         except FileNotFoundError:
             self.log.warn('File does not exist \'{}\', backup not required'.format(fqfile))
         except Exception as e:
             raise Exception('Unable to backup files \'{}\''.format(e))
-
-    def horcmshutdown(self,inst):
-        self.log.info(f'Shutdown horcm instance {inst}')
-        cmd = f'{self.path}horcmshutdown{self.cciextension} {inst}'
-        return self.nexecute(cmd)
-    
-    def horcmstart(self,inst):
-        self.log.info(f'Start horcm instance {inst}')
-        cmd = f'{self.path}horcmstart{self.cciextension} {inst}'
-        return self.nexecute(cmd)
     
     def removehorcmfile(self,inst):
         self.log.info(f'Remove horcm file {self.horcm_dir}{os.sep}horcm{inst}.conf')
         os.remove(f'{self.horcm_dir}{os.sep}horcm{inst}.conf')
 
-    def nexecute(self,cmd,undocmds=[],acceptable_returns=[0],**kwargs) -> object:
+    def nexecute(self,cmd,undocmds=[],acceptable_returns=[0],raise_err=True,**kwargs) -> object:
 
         cmdreturn = Cmdview(cmd=cmd)
         cmdreturn.expectedreturn = acceptable_returns
 
         self.log.info(f"Executing: {cmd}")
         self.log.debug(f"Acceptable return codes {acceptable_returns}")
         proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True)
@@ -290,15 +307,19 @@
         cmdreturn.executed = True
         
         if proc.returncode and proc.returncode not in acceptable_returns:
             self.log.error("Return > "+str(proc.returncode))
             self.log.error("Stdout > "+cmdreturn.stdout)
             self.log.error("Stderr > "+cmdreturn.stderr)
             message = {'return':proc.returncode,'stdout':cmdreturn.stdout, 'stderr':cmdreturn.stderr }
-            raise Exception(f"Unable to execute Command '{cmd}'. Command dump > {message}")
+            #raise Exception(f"Unable to execute Command '{cmd}'. Command dump > {message}")
+            if raise_err:
+                raise Exception(f"{message}")
+            else:
+                return cmdreturn
         
         for undocmd in undocmds: 
             echo = f'echo "Executing: {undocmd}"'
             self.undocmds.insert(0,undocmd)
             self.undocmds.insert(0,echo)
             cmdreturn.undocmds.insert(0,undocmd)
         
@@ -624,15 +645,15 @@
         return view
     
     def pairevtwaitexec(self,cmd):
         self.log.info('Executing: {}'.format(cmd))
         proc = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         return proc
     
-    def execute(self,cmd,expectedreturn=0):
+    def OLDexecute(self,cmd,expectedreturn=0):
         self.log.info(f"Executing: {cmd}")
         self.log.debug(f"Expecting return code {expectedreturn}")
         proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True)
         stdout, stderr = proc.communicate()
         self.log.info(f"Return Code: {proc.returncode}")
   
         if proc.returncode and proc.returncode != expectedreturn and expectedreturn is not None:
@@ -640,14 +661,32 @@
             self.log.error("Stdout > "+stdout.strip())
             self.log.error("Stderr > "+stderr.strip())
             message = {'return':proc.returncode,'stdout':stdout, 'stderr':stderr }
             raise Exception('Unable to execute Command "{}". Command dump > {}'.format(cmd,message))
     
         return stdout, stderr, proc.returncode
 
+
+    def execute(self,cmd,expectedreturn=0):
+        self.log.info(f"Executing: {cmd}")
+        self.log.debug(f"Expecting return code {expectedreturn}")
+        proc = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True)
+        stdout, stderr = proc.communicate()
+        self.log.info(f"Return Code: {proc.returncode}")
+  
+        if proc.returncode and proc.returncode != expectedreturn and expectedreturn is not None:
+            #self.log.error("Return > "+str(proc.returncode))
+            #self.log.error("Stdout > "+stdout.strip())
+            #self.log.error("Stderr > "+stderr.strip())
+            message = {"return":proc.returncode,"stdout":stdout, "stderr":stderr, "cmd":cmd }
+            #raise Exception('Unable to execute Command "{}". Command dump > {}'.format(cmd,message))
+            
+            raise Exception(message)
+        return stdout, stderr, proc.returncode
+
 if __name__ == "__main__":
 
     horcm_manager = Cci()
     now = datetime.now().strftime('%d-%m-%Y_%H.%M.%S')
 
     manual_horcm_dict = {
         "local" : { "service":11018, "instance":18, "HORCM_CMD": [r"\\.\CMD-350147:/dev/sd"], "HORCM_LDEV":["group\tdevice\tserial\tldevid"], "site":"local", "date":now },
```

## Comparing `hiraid-1.0.42.dist-info/LICENSE` & `hiraid-1.0.46.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hiraid-1.0.42.dist-info/METADATA` & `hiraid-1.0.46.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hiraid
-Version: 1.0.42
+Version: 1.0.46
 Summary: Hitachi raidcom wrapper
 Home-page: https://github.com/hv-ps/hiraid
 Author: Darren Chambers
 Author-email: darren.chambers@hitachivantara.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: hiexceptions
 
 # Work in progress
 hiraid is a Python raidcom wrapper for communicating with Hitachi enterprise storage arrays.
 raidcom output is parsed to json and also stored beneath storageobject.views.
 
 The primary purpose of this library is to underpin the Hitachi Vantara opensource ansible project: https://github.com/hv-ps/Hitachi.Raidcom.Ansible
```

