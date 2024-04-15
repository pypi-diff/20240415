# Comparing `tmp/panda_server-0.3.1.tar.gz` & `tmp/panda_server-0.3.3.tar.gz`

## Comparing `panda_server-0.3.1.tar` & `panda_server-0.3.3.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.1/ChangeLog.txt
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 panda_server-0.3.1/Dockerfile
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.1/INSTALL.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.1/INSTALL_ATLAS.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.1/PandaPkgInfo.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.1/panda-server.spec
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.1/package/hatch_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0        0        0    85926 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/brokerage/broker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/config/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/config/config_utils.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/config/daemon_config.py
--rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/config/panda_config.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/configurator/Carbon.py
--rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/configurator/Configurator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/configurator/__init__.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/configurator/aux.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/master.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/master_systemd.py
--rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/cache_pilots.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/cache_schedconfig.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0        0        0    63605 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0        0        0    53969 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0        0        0     4702 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0        0        0    54196 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0        0        0    25299 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/DDM.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/DataServiceUtils.py
--rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/EventPicker.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0        0        0     8820 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0        0        0   111781 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/__init__.py
--rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/activator.py
--rwxr-xr-x   0        0        0    10978 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/closer.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/closer_atlas_plugin.py
--rw-r--r--   0        0        0    35228 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/dyn_data_distributer.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/finisher.py
--rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/dataservice/forkSetupper.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0        0        0    58912 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0        0        0    16481 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0        0        0     9415 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/jobdispatcher/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/proxycache/__init__.py
--rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/proxycache/panda_proxy_cache.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/server/.gacl
--rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/server/panda.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/__init__.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/allowed_methods.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/panda_request.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/srvcore/srv_msg_utils.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0        0        0  1267350 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/PickleFileSpec.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/PickleJobSpec.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/SQLManager.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0        0        0   143607 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/task_split_rules.py
--rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/taskbuffer/workflow_processor.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/SchemaChecker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/banUser.py
--rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/boostPrio.py
--rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/boostUser.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/callbackDDM.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/daod_on_demand.py
--rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/finishJob.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/finishTaskJEDI.py
--rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/getJobs.py
--rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killJob.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killTask.py
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/killUser.py
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/reassignJobs.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/reassignSite.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/reassignTask.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/reassignWaiting.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/reloadInputDS.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/setPriority.py
--rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testEvgen.py
--rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testG4sim.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testG4sim17.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testGlobalShares.py
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testReco.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testSiteMap.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/testutils.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/alice/README.txt
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/alice/mysetup
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/lsst/README.txt
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
--rwxr-xr-x   0        0        0    80304 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/userinterface/Client.py
--rw-r--r--   0        0        0    91604 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/userinterface/UserIF.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/userinterface/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/__init__.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/psnakemake_container.json
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/psnakemake_task.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/psnakemake_test.py
--rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.1/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/conda_meta.yaml.template
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/panda_server-httpd.conf.rpmnew.template
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/panda_server.cfg.rpmnew.template
--rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/bin/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/bin/panda_server-vomsrenew.exe.template
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/init.d/panda_server.exe.template
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/sysconfig/panda_server_env.systemd.rpmnew.template
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/systemd/panda.service.template
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/systemd/panda_daemon.service.template
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.1/templates/systemd/panda_httpd.service.template
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.1/README.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 panda_server-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 panda_server-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 panda_server-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    81265 2020-02-02 00:00:00.000000 panda_server-0.3.3/ChangeLog.txt
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 panda_server-0.3.3/Dockerfile
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 panda_server-0.3.3/INSTALL.md
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 panda_server-0.3.3/INSTALL_ATLAS.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 panda_server-0.3.3/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_server-0.3.3/PandaPkgInfo.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 panda_server-0.3.3/panda-server.spec
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 panda_server-0.3.3/package/hatch_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0        0        0    85928 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/brokerage/broker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/config_utils.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0        0        0     6900 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/config/panda_config.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/Carbon.py
+-rw-r--r--   0        0        0    38070 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/Configurator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/configurator/aux.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/master.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/master_systemd.py
+-rw-r--r--   0        0        0    25423 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/cache_pilots.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/cache_schedconfig.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0        0        0    63605 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0        0        0    41997 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0        0        0    15357 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0        0        0    54210 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0        0        0    42448 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/AdderSimplePlugin.py
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/DataServiceUtils.py
+-rwxr-xr-x   0        0        0      390 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0        0        0     8820 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0        0        0   111777 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/__init__.py
+-rwxr-xr-x   0        0        0     2553 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/activator.py
+-rwxr-xr-x   0        0        0    10782 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/closer.py
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/closer_atlas_plugin.py
+-rwxr-xr-x   0        0        0    39928 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ddm.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/ddm_handler.py
+-rw-r--r--   0        0        0    35028 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/dyn_data_distributer.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/event_lookup_client_ei.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/event_picker.py
+-rwxr-xr-x   0        0        0     7248 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/finisher.py
+-rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/dataservice/forkSetupper.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0        0        0    58971 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0        0        0    16520 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0        0        0     9377 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/jobdispatcher/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/proxycache/__init__.py
+-rw-r--r--   0        0        0     9933 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/proxycache/panda_proxy_cache.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/server/.gacl
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/server/panda.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/allowed_methods.py
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/panda_request.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/srvcore/srv_msg_utils.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0        0        0    27241 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0        0        0  1267473 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PickleFileSpec.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PickleJobSpec.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SQLManager.py
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0        0        0   143625 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0        0        0    18729 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/task_split_rules.py
+-rw-r--r--   0        0        0    12538 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/taskbuffer/workflow_processor.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/banUser.py
+-rwxr-xr-x   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0        0        0     1225 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/boostUser.py
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/callbackDDM.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/daod_on_demand.py
+-rwxr-xr-x   0        0        0    10154 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/finishJob.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/finishTaskJEDI.py
+-rwxr-xr-x   0        0        0     1238 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/getJobs.py
+-rwxr-xr-x   0        0        0     2032 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killJob.py
+-rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killTask.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/killUser.py
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignJobs.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignSite.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0        0        0      936 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/setPriority.py
+-rwxr-xr-x   0        0        0     1726 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0        0        0     1700 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testG4sim.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testG4sim17.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0        0        0     3540 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testReco.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0        0        0      708 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testSiteMap.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/testutils.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/README.txt
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/mysetup
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/README.txt
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh
+-rwxr-xr-x   0        0        0    80304 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/userinterface/Client.py
+-rw-r--r--   0        0        0    91604 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/userinterface/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/__init__.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/psnakemake_container.json
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/psnakemake_task.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/psnakemake_test.py
+-rw-r--r--   0        0        0    39025 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 panda_server-0.3.3/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/conda_meta.yaml.template
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/panda_server-httpd.conf.rpmnew.template
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/panda_server.cfg.rpmnew.template
+-rwxr-xr-x   0        0        0    15351 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/bin/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/bin/panda_server-vomsrenew.exe.template
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/init.d/panda_server.exe.template
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/systemd/panda.service.template
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 panda_server-0.3.3/templates/systemd/panda_httpd.service.template
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 panda_server-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 panda_server-0.3.3/README.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 panda_server-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 panda_server-0.3.3/PKG-INFO
```

### Comparing `panda_server-0.3.1/ChangeLog.txt` & `panda_server-0.3.3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/Dockerfile` & `panda_server-0.3.3/Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ARG PYTHON_VERSION
 
 RUN yum update -y
 RUN yum install -y epel-release
 
 RUN yum install -y httpd httpd-devel gcc gridsite git psmisc less wget logrotate procps which \
-    openssl-devel readline-devel bzip2-devel libffi-devel zlib-devel
+    openssl-devel readline-devel bzip2-devel libffi-devel zlib-devel systemd-udev
 
 # install python
 RUN mkdir /tmp/python && cd /tmp/python && \
     wget https://www.python.org/ftp/python/${PYTHON_VERSION}/Python-${PYTHON_VERSION}.tgz && \
     tar -xzf Python-*.tgz && rm -f Python-*.tgz && \
     cd Python-* && \
     ./configure --enable-shared --enable-optimizations --with-lto && \
@@ -21,14 +21,19 @@
     cd / && rm -rf /tmp/pyton
 
 # install postgres
 RUN yum install -y https://download.postgresql.org/pub/repos/yum/reporpms/EL-9-x86_64/pgdg-redhat-repo-latest.noarch.rpm
 RUN yum install --nogpgcheck -y postgresql16
 RUN  yum clean all && rm -rf /var/cache/yum
 
+# update network limitations
+# RUN echo 4096 > /proc/sys/net/core/somaxconn
+# RUN sysctl -w net.core.somaxconn=4096
+RUN echo 'net.core.somaxconn=4096' >> /etc/sysctl.d/999-net.somax.conf
+
 # setup venv with pythonX.Y
 RUN python$(echo ${PYTHON_VERSION} | sed -E 's/\.[0-9]+$//') -m venv /opt/panda
 RUN /opt/panda/bin/pip install --no-cache-dir -U pip
 RUN /opt/panda/bin/pip install --no-cache-dir -U setuptools
 RUN /opt/panda/bin/pip install --no-cache-dir -U gnureadline
 RUN adduser atlpan
 RUN groupadd zp
```

### Comparing `panda_server-0.3.1/INSTALL.md` & `panda_server-0.3.3/INSTALL.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/INSTALL_ATLAS.md` & `panda_server-0.3.3/INSTALL_ATLAS.md`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/panda-server.spec` & `panda_server-0.3.3/panda-server.spec`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/package/hatch_build.py` & `panda_server-0.3.3/package/hatch_build.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/brokerage/SiteMapper.py` & `panda_server-0.3.3/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/brokerage/broker.py` & `panda_server-0.3.3/pandaserver/brokerage/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import uuid
 
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandaserver.brokerage import ErrorCode
 from pandaserver.config import panda_config
 from pandaserver.dataservice import DataServiceUtils
 from pandaserver.dataservice.DataServiceUtils import select_scope
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.taskbuffer import ProcessGroups
 
 _log = PandaLogger().getLogger("broker")
 
 # all known sites
 _allSites = []
 
@@ -95,15 +95,15 @@
         tmpLog.debug(f"getOkFiles for {v_ce.sitename} with rucio_site:{rucio_site}, rucio_url:{rucio_url}, SE:{str(tmpSE)}")
     anyID = "any"
     # use bulk lookup
     if allLFNs != []:
         # get all replicas
         if rucio_url not in allOkFilesMap:
             allOkFilesMap[rucio_url] = {}
-            tmpStat, tmpAvaFiles = rucioAPI.listFileReplicas(allScopeList, allLFNs, tmpSE)
+            tmpStat, tmpAvaFiles = rucioAPI.list_file_replicas(allScopeList, allLFNs, tmpSE)
             if not tmpStat and tmpLog is not None:
                 tmpLog.debug("getOkFile failed to get file replicas")
                 tmpAvaFiles = {}
             allOkFilesMap[rucio_url][anyID] = tmpAvaFiles
         # get files for each rucio_site
         if rucio_site not in allOkFilesMap[rucio_url]:
             allOkFilesMap[rucio_url][rucio_site] = allOkFilesMap[rucio_url][anyID]
```

### Comparing `panda_server-0.3.1/pandaserver/config/daemon_config.py` & `panda_server-0.3.3/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/config/panda_config.py` & `panda_server-0.3.3/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/configurator/Carbon.py` & `panda_server-0.3.3/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/configurator/Configurator.py` & `panda_server-0.3.3/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/configurator/aux.py` & `panda_server-0.3.3/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/master.py` & `panda_server-0.3.3/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/master_systemd.py` & `panda_server-0.3.3/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/utils.py` & `panda_server-0.3.3/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/add_main.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/add_sub.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/cache_pilots.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/cache_pilots.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/cache_schedconfig.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/cache_schedconfig.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/carbon.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/configurator.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/copyArchive.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/datasetManager.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/datasetManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandacommon.pandautils.thread_utils import GenericThread
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
 from pandaserver.dataservice import DataServiceUtils
 from pandaserver.dataservice.closer import Closer
 from pandaserver.dataservice.DataServiceUtils import select_scope
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.dataservice.finisher import Finisher
 from pandaserver.taskbuffer import EventServiceUtils
 
 # logger
 _logger = PandaLogger().getLogger("datasetManager")
 
 
@@ -194,19 +194,19 @@
                         or name.startswith("group.")
                         or name.startswith("hc_test.")
                         or name.startswith("panda.um.")
                     ):
                         dsExists = False
                     if dsExists:
                         # check if dataset exists
-                        status, out = rucioAPI.getMetaData(name)
+                        status, out = rucioAPI.get_metadata(name)
                         if status is True:
                             if out is not None:
                                 try:
-                                    rucioAPI.closeDataset(name)
+                                    rucioAPI.close_dataset(name)
                                     status = True
                                 except Exception:
                                     errtype, errvalue = sys.exc_info()[:2]
                                     out = f"failed to freeze : {errtype} {errvalue}"
                                     status = False
                             else:
                                 # dataset not exist
@@ -229,26 +229,26 @@
                         self.proxyLock.release()
                         # set tobedeleted to dis
                         setTobeDeletedToDis(name)
                         # skip if dataset is not real
                         if not dsExists:
                             continue
                         # count # of files
-                        status, out = rucioAPI.getNumberOfFiles(name)
+                        status, out = rucioAPI.get_number_of_files(name)
                         if status is not True:
                             if status is False:
                                 _logger.error(out)
                         else:
                             _logger.debug(out)
                             try:
                                 nFile = int(out)
                                 if nFile == 0:
                                     # erase dataset
                                     _logger.debug(f"erase {name}")
-                                    status, out = rucioAPI.eraseDataset(name)
+                                    status, out = rucioAPI.erase_dataset(name)
                                     _logger.debug(f"OK with {name}")
                             except Exception:
                                 pass
             except Exception:
                 pass
             self.pool.remove(self)
             self.lock.release()
@@ -397,19 +397,19 @@
                                     else:
                                         _logger.debug(f"failed to get merging job for {name} ")
                                 else:
                                     _logger.debug(f"failed to get merging file for {name} ")
                                 status, out = True, ""
                             elif dsExists:
                                 # check if dataset exists
-                                status, out = rucioAPI.getMetaData(name)
+                                status, out = rucioAPI.get_metadata(name)
                                 if status is True:
                                     if out is not None:
                                         try:
-                                            rucioAPI.closeDataset(name)
+                                            rucioAPI.close_dataset(name)
                                             status = True
                                         except Exception:
                                             errtype, errvalue = sys.exc_info()[:2]
                                             out = f"failed to freeze : {errtype} {errvalue}"
                                             status = False
                                     else:
                                         # dataset not exist
@@ -430,27 +430,27 @@
                                 )
                                 self.proxyLock.release()
                                 if name.startswith("pandaddm_") or name.startswith("panda.um.") or not dsExists:
                                     continue
                                 # set tobedeleted to dis
                                 setTobeDeletedToDis(name)
                                 # count # of files
-                                status, out = rucioAPI.getNumberOfFiles(name)
+                                status, out = rucioAPI.get_number_of_files(name)
                                 if status is not True:
                                     if status is False:
                                         _logger.error(out)
                                 else:
                                     _logger.debug(out)
                                     try:
                                         nFile = int(out)
                                         _logger.debug(nFile)
                                         if nFile == 0:
                                             # erase dataset
                                             _logger.debug(f"erase {name}")
-                                            status, out = rucioAPI.eraseDataset(name)
+                                            status, out = rucioAPI.erase_dataset(name)
                                             _logger.debug(f"OK with {name}")
                                     except Exception:
                                         pass
                         else:
                             _logger.debug(f"wait {name} ")
                             self.proxyLock.acquire()
                             taskBuffer.querySQLS(
@@ -563,15 +563,15 @@
                     if re.search("_dis\d+$", name) is None:
                         _logger.error(f"Eraser : non disDS {name}")
                         continue
                     # delete
                     _logger.debug(f"Eraser {self.operationType} dis {modDate} {name}")
                     # delete or shorten
                     endStatus = "deleted"
-                    status, out = rucioAPI.eraseDataset(name)
+                    status, out = rucioAPI.erase_dataset(name)
                     if not status:
                         _logger.error(out)
                         continue
                     _logger.debug(f"OK with {name}")
                     # update
                     self.proxyLock.acquire()
                     varMap = {}
@@ -695,15 +695,15 @@
                                 continue
                             lfns.append(file.lfn)
                             guids.append(file.GUID)
                             scopes.append(file.scope)
                             nTokens += len(file.destinationDBlockToken.split(","))
                     # get files in LRC
                     _logger.debug(f"{job.PandaID} Cloud:{job.cloud}")
-                    tmpStat, okFiles = rucioAPI.listFileReplicas(scopes, lfns, seList)
+                    tmpStat, okFiles = rucioAPI.list_file_replicas(scopes, lfns, seList)
                     if not tmpStat:
                         _logger.error(f"{job.PandaID} failed to get file replicas")
                         okFiles = {}
                     # count files
                     nOkTokens = 0
                     for okLFN in okFiles:
                         okSEs = okFiles[okLFN]
@@ -848,15 +848,15 @@
                     for tmpFile in tmpJob.Files:
                         # only input files are checked
                         if tmpFile.type == "input" and tmpFile.status != "ready":
                             lfns.append(tmpFile.lfn)
                             scopes.append(tmpFile.scope)
                     # get file replicas
                     _logger.debug(f"{tmpJob.PandaID} check input files at {tmpJob.computingSite}")
-                    tmpStat, okFiles = rucioAPI.listFileReplicas(scopes, lfns)
+                    tmpStat, okFiles = rucioAPI.list_file_replicas(scopes, lfns)
                     if not tmpStat:
                         pass
                     else:
                         # check if locally available
                         siteSpec = siteMapper.getSite(tmpJob.computingSite)
                         scope_input, scope_output = select_scope(siteSpec, tmpJob.prodSourceLabel, tmpJob.job_label)
                         allOK = True
@@ -951,15 +951,15 @@
                     scope_input, scope_output = select_scope(siteSpec, tmpJob.prodSourceLabel, tmpJob.job_label)
                     allOK = True
                     for tmpFile in tmpJob.Files:
                         # only input files are checked
                         if tmpFile.type == "input" and tmpFile.status != "ready":
                             # get replicas
                             if tmpFile.dispatchDBlock not in replicaMap:
-                                tmpStat, repMap = rucioAPI.listDatasetReplicas(tmpFile.dispatchDBlock)
+                                tmpStat, repMap = rucioAPI.list_dataset_replicas(tmpFile.dispatchDBlock)
                                 if tmpStat != 0:
                                     repMap = {}
                                 replicaMap[tmpFile.dispatchDBlock] = repMap
                             # check RSEs
                             for rse in replicaMap[tmpFile.dispatchDBlock]:
                                 repInfo = replicaMap[tmpFile.dispatchDBlock][rse]
                                 if (
@@ -1084,15 +1084,15 @@
                                     _logger.debug(f"skip delete sub {name} PandaID={pandaID} is active {jobStatus}")
                                     allDone = False
                                     break
                             self.proxyLock.release()
                             if allDone:
                                 _logger.debug(f"deleting sub {name}")
                                 try:
-                                    rucioAPI.eraseDataset(name, grace_period=4)
+                                    rucioAPI.erase_dataset(name, grace_period=4)
                                     status = True
                                 except Exception:
                                     errtype, errvalue = sys.exc_info()[:2]
                                     out = f"{errtype} {errvalue}"
                                     _logger.error(f"{name} failed to erase with {out}")
                             else:
                                 _logger.debug(f"wait sub {name}")
```

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/evpPD2P.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import threading
 import time
 
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandacommon.pandautils.thread_utils import GenericThread
 from pandaserver.brokerage import SiteMapper
 from pandaserver.config import panda_config
-from pandaserver.dataservice.EventPicker import EventPicker
+from pandaserver.dataservice.event_picker import EventPicker
 
 # logger
 _logger = PandaLogger().getLogger("evpPD2P")
 
 
 # main
 def main(tbuf=None, **kwargs):
```

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/metric_collector.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/pilotStreaming.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/task_evaluator.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/tmpwatch.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/daemons/scripts/worker_synchronization.py` & `panda_server-0.3.3/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda_server-0.3.3/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import time
 import traceback
 
 from pandaserver.config import panda_config
 from pandaserver.dataservice import DataServiceUtils, ErrorCode
 from pandaserver.dataservice.AdderPluginBase import AdderPluginBase
 from pandaserver.dataservice.DataServiceUtils import select_scope
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.srvcore.MailUtils import MailUtils
 from pandaserver.taskbuffer import EventServiceUtils, JobUtils
 from rucio.common.exception import (
     DataIdentifierNotFound,
     FileConsistencyMismatch,
     InsufficientAccountLimit,
     InvalidObject,
@@ -612,17 +612,17 @@
             try:
                 if not self.useCentralLFC():
                     regMsgStr = f"File registraion for {regNumFiles} files "
                 else:
                     regMsgStr = f"File registration with backend={self.ddmBackEnd} for {regNumFiles} files "
                 if len(zipFiles) > 0:
                     self.logger.debug(f"registerZipFiles {str(zipFiles)}")
-                    rucioAPI.registerZipFiles(zipFiles)
+                    rucioAPI.register_zip_files(zipFiles)
                 self.logger.debug(f"registerFilesInDatasets {str(destIdMap)} zip={str(contZipMap)}")
-                out = rucioAPI.registerFilesInDataset(destIdMap, contZipMap)
+                out = rucioAPI.register_files_in_dataset(destIdMap, contZipMap)
             except (
                 DataIdentifierNotFound,
                 FileConsistencyMismatch,
                 UnsupportedOperation,
                 InvalidPath,
                 InvalidObject,
                 RSENotFound,
@@ -705,15 +705,15 @@
                                     "replica_lifetime": repLifeTime,
                                 },
                             )
                         )
                         for iDDMTry in range(3):
                             isFailed = False
                             try:
-                                status = rucioAPI.registerDatasetSubscription(
+                                status = rucioAPI.register_dataset_subscription(
                                     tmpName,
                                     [dq2ID],
                                     owner="panda",
                                     activity=subActivity,
                                     lifetime=repLifeTime,
                                 )
                                 out = "OK"
@@ -759,15 +759,15 @@
                                     {"lifetime": "14 days"},
                                 )
                             )
                             for iDDMTry in range(3):
                                 out = "OK"
                                 isFailed = False
                                 try:
-                                    rucioAPI.registerDatasetLocation(
+                                    rucioAPI.register_dataset_location(
                                         tmpDsNameLoc,
                                         [tmpLocName],
                                         owner="panda",
                                         activity=subActivity,
                                         lifetime=repLifeTime,
                                     )
                                     out = "OK"
@@ -850,15 +850,15 @@
                             # use group account for group.*
                             if tmpDsName.startswith("group") and self.job.workingGroup not in ["", "NULL", None]:
                                 tmpDN = self.job.workingGroup
                             else:
                                 tmpDN = userInfo["nickname"]
                             tmpMsg = f"registerDatasetLocation for Rucio ds={tmpDsName} site={tmpDQ2ID} id={tmpDN}"
                             self.logger.debug(tmpMsg)
-                            rucioAPI.registerDatasetLocation(
+                            rucioAPI.register_dataset_location(
                                 tmpDsName,
                                 [tmpDQ2ID],
                                 owner=tmpDN,
                                 activity="Analysis Output",
                             )
                     # set dataset status
                     for tmpName in subMap:
@@ -993,15 +993,15 @@
                     if esDataset not in idMap[epName]:
                         idMap[epName][esDataset] = []
                     idMap[epName][esDataset].append(fileData)
             # add files to dataset
             if idMap != {}:
                 self.logger.debug(f"adding ES files {str(idMap)}")
                 try:
-                    rucioAPI.registerFilesInDataset(idMap)
+                    rucioAPI.register_files_in_dataset(idMap)
                 except DataIdentifierNotFound:
                     self.logger.debug("ignored DataIdentifierNotFound")
         except Exception:
             errtype, errvalue = sys.exc_info()[:2]
             errStr = f" : {errtype} {errvalue}"
             errStr += traceback.format_exc()
             self.logger.error(errStr)
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/AdderGen.py` & `panda_server-0.3.3/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/AdderResult.py` & `panda_server-0.3.3/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/AdderSimplePlugin.py` & `panda_server-0.3.3/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime
 import time
 import traceback
 import uuid
 
 from pandaserver.dataservice import DataServiceUtils, ErrorCode
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from rucio.common.exception import (
     DataIdentifierNotFound,
     FileConsistencyMismatch,
     InsufficientAccountLimit,
     InvalidObject,
     InvalidPath,
     InvalidRSEExpression,
@@ -69,15 +69,15 @@
                 nTry = 3
                 for iTry in range(nTry):
                     isFatal = False
                     isFailed = False
                     regStart = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
                     try:
                         self.logger.debug(f"registerFilesInDatasets {str(destIdMap)}")
-                        out = rucioAPI.registerFilesInDataset(destIdMap, {})
+                        out = rucioAPI.register_files_in_dataset(destIdMap, {})
                     except (
                         DataIdentifierNotFound,
                         FileConsistencyMismatch,
                         UnsupportedOperation,
                         InvalidPath,
                         InvalidObject,
                         RSENotFound,
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/DDM.py` & `panda_server-0.3.3/pandaserver/taskbuffer/JobSpec.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,709 +1,892 @@
 """
-provide primitive methods for DDM
+job specification
 
 """
 
-import hashlib
+import datetime
+import json
 import re
-import sys
-import traceback
 
-from rucio.client import Client as RucioClient
-from rucio.common.exception import (
-    DataIdentifierAlreadyExists,
-    DataIdentifierNotFound,
-    Duplicate,
-    DuplicateContent,
-    DuplicateRule,
-    FileAlreadyExists,
-    UnsupportedOperation,
-)
+from pandaserver.taskbuffer.FileSpec import FileSpec
 
-from pandaserver.srvcore import CoreUtils
+reserveChangedState = False
 
 
-# rucio
-class RucioAPI:
+class JobSpec(object):
+    # attributes
+    _attributes = (
+        "PandaID",
+        "jobDefinitionID",
+        "schedulerID",
+        "pilotID",
+        "creationTime",
+        "creationHost",
+        "modificationTime",
+        "modificationHost",
+        "AtlasRelease",
+        "transformation",
+        "homepackage",
+        "prodSeriesLabel",
+        "prodSourceLabel",
+        "prodUserID",
+        "assignedPriority",
+        "currentPriority",
+        "attemptNr",
+        "maxAttempt",
+        "jobStatus",
+        "jobName",
+        "maxCpuCount",
+        "maxCpuUnit",
+        "maxDiskCount",
+        "maxDiskUnit",
+        "ipConnectivity",
+        "minRamCount",
+        "minRamUnit",
+        "startTime",
+        "endTime",
+        "cpuConsumptionTime",
+        "cpuConsumptionUnit",
+        "commandToPilot",
+        "transExitCode",
+        "pilotErrorCode",
+        "pilotErrorDiag",
+        "exeErrorCode",
+        "exeErrorDiag",
+        "supErrorCode",
+        "supErrorDiag",
+        "ddmErrorCode",
+        "ddmErrorDiag",
+        "brokerageErrorCode",
+        "brokerageErrorDiag",
+        "jobDispatcherErrorCode",
+        "jobDispatcherErrorDiag",
+        "taskBufferErrorCode",
+        "taskBufferErrorDiag",
+        "computingSite",
+        "computingElement",
+        "jobParameters",
+        "metadata",
+        "prodDBlock",
+        "dispatchDBlock",
+        "destinationDBlock",
+        "destinationSE",
+        "nEvents",
+        "grid",
+        "cloud",
+        "cpuConversion",
+        "sourceSite",
+        "destinationSite",
+        "transferType",
+        "taskID",
+        "cmtConfig",
+        "stateChangeTime",
+        "prodDBUpdateTime",
+        "lockedby",
+        "relocationFlag",
+        "jobExecutionID",
+        "VO",
+        "pilotTiming",
+        "workingGroup",
+        "processingType",
+        "prodUserName",
+        "nInputFiles",
+        "countryGroup",
+        "batchID",
+        "parentID",
+        "specialHandling",
+        "jobsetID",
+        "coreCount",
+        "nInputDataFiles",
+        "inputFileType",
+        "inputFileProject",
+        "inputFileBytes",
+        "nOutputDataFiles",
+        "outputFileBytes",
+        "jobMetrics",
+        "workQueue_ID",
+        "jediTaskID",
+        "jobSubStatus",
+        "actualCoreCount",
+        "reqID",
+        "maxRSS",
+        "maxVMEM",
+        "maxSWAP",
+        "maxPSS",
+        "avgRSS",
+        "avgVMEM",
+        "avgSWAP",
+        "avgPSS",
+        "maxWalltime",
+        "nucleus",
+        "eventService",
+        "failedAttempt",
+        "hs06sec",
+        "gshare",
+        "hs06",
+        "totRCHAR",
+        "totWCHAR",
+        "totRBYTES",
+        "totWBYTES",
+        "rateRCHAR",
+        "rateWCHAR",
+        "rateRBYTES",
+        "rateWBYTES",
+        "resource_type",
+        "diskIO",
+        "memory_leak",
+        "memory_leak_x2",
+        "container_name",
+        "job_label",
+        "gco2_regional",
+        "gco2_global",
+        "cpu_architecture_level",
+    )
+    # slots
+    __slots__ = _attributes + ("Files", "_changedAttrs", "_reserveChangedState")
+    # attributes which have 0 by default
+    _zeroAttrs = (
+        "assignedPriority",
+        "currentPriority",
+        "attemptNr",
+        "maxAttempt",
+        "maxCpuCount",
+        "maxDiskCount",
+        "minRamCount",
+        "cpuConsumptionTime",
+        "pilotErrorCode",
+        "exeErrorCode",
+        "supErrorCode",
+        "ddmErrorCode",
+        "brokerageErrorCode",
+        "jobDispatcherErrorCode",
+        "taskBufferErrorCode",
+        "nEvents",
+        "relocationFlag",
+        "jobExecutionID",
+        "nOutputDataFiles",
+        "outputFileBytes",
+    )
+    # attribute to be suppressed. They are in another table
+    _suppAttrs = ("jobParameters", "metadata")
+    # mapping between sequence and attr
+    _seqAttrMap = {"PandaID": "ATLAS_PANDA.JOBSDEFINED4_PANDAID_SEQ.nextval"}
+    # limit length
+    _limitLength = {
+        "ddmErrorDiag": 500,
+        "taskBufferErrorDiag": 300,
+        "jobDispatcherErrorDiag": 250,
+        "brokerageErrorDiag": 250,
+        "pilotErrorDiag": 500,
+        "exeErrorDiag": 500,
+        "jobSubStatus": 80,
+        "supErrorDiag": 250,
+        "commandToPilot": 250,
+    }
+    # tag for special handling
+    _tagForSH = {
+        "altStgOut": "ao",
+        "acceptPartial": "ap",
+        "allOkEvents": "at",
+        "notDiscardEvents": "de",
+        "decAttOnFailedES": "df",
+        "debugMode": "dm",
+        "dynamicNumEvents": "dy",
+        "encJobParams": "ej",
+        "fakeJobToIgnore": "fake",
+        "homeCloud": "hc",
+        "hpoWorkflow": "ho",
+        "inFilePosEvtNum": "if",
+        "inputPrestaging": "ip",
+        "lumiBlock": "lb",
+        "noLoopingCheck": "lc",
+        "mergeAtOs": "mo",
+        "noExecStrCnv": "nc",
+        "onSiteMerging": "om",
+        "pushStatusChanges": "pc",
+        "pushJob": "pj",
+        "putLogToOS": "po",
+        "registerEsFiles": "re",
+        "retryRam": "rr",
+        "resurrectConsumers": "rs",
+        "requestType": "rt",
+        "jobCloning": "sc",
+        "scoutJob": "sj",
+        "usePrefetcher": "up",
+        "useSecrets": "us",
+        "useZipToPin": "uz",
+        "writeInputToFile": "wf",
+    }
+
     # constructor
     def __init__(self):
-        pass
+        # install attributes
+        for attr in self._attributes:
+            object.__setattr__(self, attr, None)
+        # files list
+        object.__setattr__(self, "Files", [])
+        # map of changed attributes
+        object.__setattr__(self, "_changedAttrs", {})
+        # reserve changed state at instance level
+        object.__setattr__(self, "_reserveChangedState", False)
+
+    # override __getattribute__ for SQL
+    def __getattribute__(self, name):
+        ret = object.__getattribute__(self, name)
+        if ret is None:
+            return "NULL"
+        return ret
+
+    # override __setattr__ to collecte the changed attributes
+    def __setattr__(self, name, value):
+        oldVal = getattr(self, name)
+        object.__setattr__(self, name, value)
+        newVal = getattr(self, name)
+        if name == "jobStatus":
+            if oldVal != newVal:
+                self.stateChangeTime = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
+        # collect changed attributes
+        if oldVal != newVal and name not in self._suppAttrs:
+            self._changedAttrs[name] = value
+
+    # reset changed attribute list
+    def resetChangedList(self):
+        object.__setattr__(self, "_changedAttrs", {})
+
+    # add File to files list
+    def addFile(self, file):
+        # set owner
+        file.setOwner(self)
+        # append
+        self.Files.append(file)
+
+    # pack tuple into JobSpec
+    def pack(self, values):
+        for i in range(len(self._attributes)):
+            attr = self._attributes[i]
+            val = values[i]
+            object.__setattr__(self, attr, val)
+
+    # return a tuple of values
+    def values(self):
+        ret = []
+        for attr in self._attributes:
+            val = getattr(self, attr)
+            ret.append(val)
+        return tuple(ret)
+
+    # return map of values
+    def valuesMap(self, useSeq=False, onlyChanged=False):
+        ret = {}
+        for attr in self._attributes:
+            if useSeq and attr in self._seqAttrMap:
+                continue
+            if onlyChanged:
+                if attr not in self._changedAttrs:
+                    continue
+            val = getattr(self, attr)
+            if val == "NULL":
+                if attr in self._zeroAttrs:
+                    val = 0
+                else:
+                    val = None
+            # jobParameters/metadata go to another table
+            if attr in self._suppAttrs:
+                val = None
+            # truncate too long values
+            if attr in self._limitLength:
+                if val is not None:
+                    val = val[: self._limitLength[attr]]
+            ret[f":{attr}"] = val
+        return ret
+
+    # return state values to be pickled
+    def __getstate__(self):
+        state = []
+        for attr in self._attributes:
+            val = getattr(self, attr)
+            state.append(val)
+        if reserveChangedState or self._reserveChangedState:
+            state.append(self._changedAttrs)
+        # append File info
+        state.append(self.Files)
+        return state
+
+    # restore state from the unpickled state values
+    def __setstate__(self, state):
+        for i in range(len(self._attributes)):
+            # schema evolution is supported only when adding attributes
+            if i + 1 < len(state):
+                object.__setattr__(self, self._attributes[i], state[i])
+            else:
+                object.__setattr__(self, self._attributes[i], "NULL")
+        object.__setattr__(self, "Files", state[-1])
+        if not hasattr(self, "_reserveChangedState"):
+            object.__setattr__(self, "_reserveChangedState", False)
+        if reserveChangedState or self._reserveChangedState:
+            object.__setattr__(self, "_changedAttrs", state[-2])
+        else:
+            object.__setattr__(self, "_changedAttrs", {})
 
-    # extract scope
-    def extract_scope(self, dsn):
-        if ":" in dsn:
-            return dsn.split(":")[:2]
-        scope = dsn.split(".")[0]
-        if dsn.startswith("user") or dsn.startswith("group"):
-            scope = ".".join(dsn.split(".")[0:2])
-        return scope, dsn
-
-    # register dataset
-    def registerDataset(
-        self,
-        dsn,
-        lfns=None,
-        guids=None,
-        sizes=None,
-        checksums=None,
-        lifetime=None,
-        scope=None,
-        metadata=None,
-    ):
-        if lfns is None:
-            lfns = []
-        if guids is None:
-            guids = []
-        if sizes is None:
-            sizes = []
-        if checksums is None:
-            checksums = []
-        presetScope = scope
-        files = []
-        for lfn, guid, size, checksum in zip(lfns, guids, sizes, checksums):
-            if lfn.find(":") > -1:
-                s, lfn = lfn.split(":")[0], lfn.split(":")[1]
+    # return column names for INSERT or full SELECT
+    def columnNames(cls):
+        ret = ""
+        for attr in cls._attributes:
+            if ret != "":
+                ret += ","
+            ret += attr
+        return ret
+
+    columnNames = classmethod(columnNames)
+
+    # return expression of values for INSERT
+    def valuesExpression(cls):
+        ret = "VALUES("
+        for attr in cls._attributes:
+            ret += "%s"
+            if attr != cls._attributes[len(cls._attributes) - 1]:
+                ret += ","
+        ret += ")"
+        return ret
+
+    valuesExpression = classmethod(valuesExpression)
+
+    # return expression of bind values for INSERT
+    def bindValuesExpression(cls, useSeq=False):
+        from pandaserver.config import panda_config
+
+        ret = "VALUES("
+        for attr in cls._attributes:
+            if useSeq and attr in cls._seqAttrMap:
+                if panda_config.backend == "mysql":
+                    # mysql
+                    ret += f"NULL,"
+                else:
+                    # oracle
+                    ret += f"{cls._seqAttrMap[attr]},"
             else:
-                s = scope
-            file = {"scope": s, "name": lfn, "bytes": size, "meta": {"guid": guid}}
-            if checksum.startswith("md5:"):
-                file["md5"] = checksum[4:]
-            elif checksum.startswith("ad:"):
-                file["adler32"] = checksum[3:]
-            files.append(file)
-        # register dataset
-        client = RucioClient()
-        try:
-            scope, dsn = self.extract_scope(dsn)
-            if presetScope is not None:
-                scope = presetScope
-            client.add_dataset(scope=scope, name=dsn, meta=metadata)
-            if lifetime is not None:
-                client.set_metadata(scope, dsn, key="lifetime", value=lifetime * 86400)
-        except DataIdentifierAlreadyExists:
-            pass
-        # open dataset just in case
-        try:
-            client.set_status(scope, dsn, open=True)
-        except Exception:
-            pass
-        # add files
-        if len(files) > 0:
-            iFiles = 0
-            nFiles = 1000
-            while iFiles < len(files):
-                tmpFiles = files[iFiles : iFiles + nFiles]
-                try:
-                    client.add_files_to_dataset(scope=scope, name=dsn, files=tmpFiles, rse=None)
-                except FileAlreadyExists:
-                    for f in tmpFiles:
-                        try:
-                            client.add_files_to_dataset(scope=scope, name=dsn, files=[f], rse=None)
-                        except FileAlreadyExists:
-                            pass
-                iFiles += nFiles
-        vuid = hashlib.md5((scope + ":" + dsn).encode()).hexdigest()
-        vuid = f"{vuid[0:8]}-{vuid[8:12]}-{vuid[12:16]}-{vuid[16:20]}-{vuid[20:32]}"
-        duid = vuid
-        return {"duid": duid, "version": 1, "vuid": vuid}
-
-    # register dataset location
-    def registerDatasetLocation(
-        self,
-        dsn,
-        rses,
-        lifetime=None,
-        owner=None,
-        activity=None,
-        scope=None,
-        asynchronous=False,
-        grouping="DATASET",
-        notify="N",
-    ):
-        if grouping is None:
-            grouping = "DATASET"
-        presetScope = scope
-        if lifetime is not None:
-            lifetime = lifetime * 24 * 60 * 60
-        scope, dsn = self.extract_scope(dsn)
-        if presetScope is not None:
-            scope = presetScope
-        dids = []
-        did = {"scope": scope, "name": dsn}
-        dids.append(did)
-        # make location
-        rses.sort()
-        location = "|".join(rses)
-        # check if a replication rule already exists
-        client = RucioClient()
-        # owner
-        if owner is None:
-            owner = client.account
-        for rule in client.list_did_rules(scope=scope, name=dsn):
-            if (rule["rse_expression"] == location) and (rule["account"] == owner):
+                ret += f":{attr},"
+        ret = ret[:-1]
+        ret += ")"
+        return ret
+
+    bindValuesExpression = classmethod(bindValuesExpression)
+
+    # return an expression for UPDATE
+    def updateExpression(cls):
+        ret = ""
+        for attr in cls._attributes:
+            ret = ret + attr + "=%s"
+            if attr != cls._attributes[len(cls._attributes) - 1]:
+                ret += ","
+        return ret
+
+    updateExpression = classmethod(updateExpression)
+
+    # return an expression of bind variables for UPDATE
+    def bindUpdateExpression(cls):
+        ret = ""
+        for attr in cls._attributes:
+            ret += f"{attr}=:{attr},"
+        ret = ret[:-1]
+        ret += " "
+        return ret
+
+    bindUpdateExpression = classmethod(bindUpdateExpression)
+
+    # comparison function for sort
+    def compFunc(cls, a, b):
+        iPandaID = list(cls._attributes).index("PandaID")
+        iPriority = list(cls._attributes).index("currentPriority")
+        if a[iPriority] > b[iPriority]:
+            return -1
+        elif a[iPriority] < b[iPriority]:
+            return 1
+        else:
+            if a[iPandaID] > b[iPandaID]:
+                return 1
+            elif a[iPandaID] < b[iPandaID]:
+                return -1
+            else:
+                return 0
+
+    compFunc = classmethod(compFunc)
+
+    # return an expression of bind variables for UPDATE to update only changed attributes
+    def bindUpdateChangesExpression(self):
+        ret = ""
+        for attr in self._attributes:
+            if attr in self._changedAttrs:
+                ret += f"{attr}=:{attr},"
+        ret = ret[:-1]
+        ret += " "
+        return ret
+
+    # check if goint to merging
+    def produceUnMerge(self):
+        for tmpFile in self.Files:
+            if tmpFile.isUnMergedOutput():
                 return True
-        try:
-            client.add_replication_rule(
-                dids=dids,
-                copies=1,
-                rse_expression=location,
-                weight=None,
-                lifetime=lifetime,
-                grouping=grouping,
-                account=owner,
-                locked=False,
-                activity=activity,
-                notify=notify,
-                ignore_availability=True,
-            )
-        except (Duplicate, DuplicateRule):
-            pass
-        return True
+        return False
 
-    # get user
-    def getUser(self, client, dn):
-        tmp_list = [i for i in client.list_accounts("user", dn)]
-        if tmp_list != []:
-            owner = l[0]["account"]
-            return owner
-        return client.account
-
-    # register dataset subscription
-    def registerDatasetSubscription(self, dsn, rses, lifetime=None, owner=None, activity=None, dn=None, comment=None):
-        if lifetime is not None:
-            lifetime = lifetime * 24 * 60 * 60
-        scope, dsn = self.extract_scope(dsn)
-        dids = []
-        did = {"scope": scope, "name": dsn}
-        dids.append(did)
-        # make location
-        rses.sort()
-        location = "|".join(rses)
-        # check if a replication rule already exists
-        client = RucioClient()
-        # owner
-        if owner is None:
-            if dn is not None:
-                owner = self.getUser(client, dn)
+    # truncate string attribute
+    def truncateStringAttr(cls, attr, val):
+        if attr not in cls._limitLength:
+            return val
+        if val is None:
+            return val
+        return val[: cls._limitLength[attr]]
+
+    truncateStringAttr = classmethod(truncateStringAttr)
+
+    # set DDM backend
+    def setDdmBackEnd(self, backEnd):
+        if self.specialHandling in [None, ""]:
+            self.specialHandling = "ddm:" + backEnd
+        else:
+            if "ddm:" in self.specialHandling:
+                self.specialHandling = re.sub("ddm:[,]+", "ddm:" + backEnd, self.specialHandling)
             else:
-                owner = client.account
-        for rule in client.list_did_rules(scope=scope, name=dsn):
-            if (rule["rse_expression"] == location) and (rule["account"] == owner):
-                return True
-        try:
-            client.add_replication_rule(
-                dids=dids,
-                copies=1,
-                rse_expression=location,
-                weight=None,
-                lifetime=lifetime,
-                grouping="DATASET",
-                account=owner,
-                locked=False,
-                activity=activity,
-                notify="C",
-                ignore_availability=True,
-                comment=comment,
-            )
-        except (Duplicate, DuplicateRule):
-            pass
-        return True
+                self.specialHandling = self.specialHandling + "," + "ddm:" + backEnd
 
-    # convert file attribute
-    def convFileAttr(self, tmpFile, scope):
-        # extract scope from LFN if available
-        if "name" in tmpFile:
-            lfn = tmpFile["name"]
+    # set LB number
+    def setLumiBlockNr(self, lumiBlockNr):
+        if self.specialHandling in ["", None, "NULL"]:
+            self.specialHandling = f"lb:{lumiBlockNr}"
         else:
-            lfn = tmpFile["lfn"]
-        if ":" in lfn:
-            s, lfn = lfn.split(":")
+            self.specialHandling += f",lb:{lumiBlockNr}"
+
+    # get LB number
+    def getLumiBlockNr(self):
+        if self.specialHandling is not None:
+            for tmpItem in self.specialHandling.split(","):
+                if tmpItem.startswith("lb:"):
+                    return int(tmpItem.split(":")[-1])
+        return None
+
+    # get DDM backend
+    def getDdmBackEnd(self):
+        if self.specialHandling is None:
+            return None
+        for tmpItem in self.specialHandling.split(","):
+            if tmpItem.startswith("ddm:"):
+                return tmpItem.split(":")[-1]
+        return None
+
+    # set to accept partial finish
+    def setToAcceptPartialFinish(self):
+        self.set_special_handling("acceptPartial")
+
+    # accept partial finish
+    def acceptPartialFinish(self):
+        return self.check_special_handling("acceptPartial")
+
+    # set home cloud
+    def setHomeCloud(self, homeCloud):
+        if self.specialHandling in ["", None, "NULL"]:
+            self.specialHandling = f"hc:{homeCloud}"
         else:
-            s = scope
-        # set metadata
-        meta = {}
-        if "guid" in tmpFile:
-            meta["guid"] = tmpFile["guid"]
-        if "events" in tmpFile:
-            meta["events"] = tmpFile["events"]
-        if "lumiblocknr" in tmpFile:
-            meta["lumiblocknr"] = tmpFile["lumiblocknr"]
-        if "panda_id" in tmpFile:
-            meta["panda_id"] = tmpFile["panda_id"]
-        if "campaign" in tmpFile:
-            meta["campaign"] = tmpFile["campaign"]
-        if "task_id" in tmpFile:
-            meta["task_id"] = tmpFile["task_id"]
-        if "bytes" in tmpFile:
-            fsize = tmpFile["bytes"]
+            self.specialHandling += f",hc:{homeCloud}"
+
+    # get cloud
+    def getCloud(self):
+        if self.specialHandling is not None:
+            for tmpItem in self.specialHandling.split(","):
+                if tmpItem.startswith("hc:"):  # hc: Home Cloud
+                    return tmpItem.split(":")[-1]
+        return self.cloud
+
+    # check if cancelled or it's flavor
+    def isCancelled(self):
+        return self.jobStatus in ["cancelled", "closed"]
+
+    # get file names which were uploaded to alternative locations
+    def altStgOutFileList(self):
+        try:
+            if self.jobMetrics is not None:
+                for item in self.jobMetrics.split():
+                    if item.startswith("altTransferred="):
+                        return item.split("=")[-1].split(",")
+        except Exception:
+            pass
+        return []
+
+    # check special handling
+    def check_special_handling(self, key):
+        if self.specialHandling:
+            return self._tagForSH[key] in self.specialHandling.split(",")
+        return False
+
+    # set special handling
+    def set_special_handling(self, key):
+        if self.specialHandling:
+            items = self.specialHandling.split(",")
         else:
-            fsize = tmpFile["size"]
-        # set mandatory fields
-        file = {"scope": s, "name": lfn, "bytes": fsize, "meta": meta}
-        if "checksum" in tmpFile:
-            checksum = tmpFile["checksum"]
-            if checksum.startswith("md5:"):
-                file["md5"] = checksum[4:]
-            elif checksum.startswith("ad:"):
-                file["adler32"] = checksum[3:]
-        if "surl" in tmpFile:
-            file["pfn"] = tmpFile["surl"]
-        return file
-
-    # register files in dataset
-    def registerFilesInDataset(self, idMap, filesWoRSEs=None):
-        # loop over all rse
-        attachmentList = []
-        for rse in idMap:
-            tmpMap = idMap[rse]
-            # loop over all datasets
-            for datasetName in tmpMap:
-                fileList = tmpMap[datasetName]
-                # extract scope from dataset
-                scope, dsn = self.extract_scope(datasetName)
-                filesWithRSE = []
-                filesWoRSE = []
-                for tmpFile in fileList:
-                    # convert file attribute
-                    file = self.convFileAttr(tmpFile, scope)
-                    # append files
-                    if rse is not None and (filesWoRSEs is None or file["name"] not in filesWoRSEs):
-                        filesWithRSE.append(file)
-                    else:
-                        if "pfn" in file:
-                            del file["pfn"]
-                        filesWoRSE.append(file)
-                # add attachment
-                if len(filesWithRSE) > 0:
-                    nFiles = 100
-                    iFiles = 0
-                    while iFiles < len(filesWithRSE):
-                        attachment = {
-                            "scope": scope,
-                            "name": dsn,
-                            "dids": filesWithRSE[iFiles : iFiles + nFiles],
-                            "rse": rse,
-                        }
-                        attachmentList.append(attachment)
-                        iFiles += nFiles
-                if len(filesWoRSE) > 0:
-                    nFiles = 100
-                    iFiles = 0
-                    while iFiles < len(filesWoRSE):
-                        attachment = {
-                            "scope": scope,
-                            "name": dsn,
-                            "dids": filesWoRSE[iFiles : iFiles + nFiles],
-                        }
-                        attachmentList.append(attachment)
-                        iFiles += nFiles
-        # add files
-        client = RucioClient()
-        client.add_files_to_datasets(attachmentList, ignore_duplicate=True)
-        return True
-
-    # register zip files
-    def registerZipFiles(self, zipMap):
-        # no zip files
-        if len(zipMap) == 0:
-            return
-        client = RucioClient()
-        # loop over all zip files
-        for zipFileName in zipMap:
-            zipFileAttr = zipMap[zipFileName]
-            # convert file attribute
-            zipFile = self.convFileAttr(zipFileAttr, zipFileAttr["scope"])
-            # loop over all contents
-            files = []
-            for conFileAttr in zipFileAttr["files"]:
-                # get scope
-                scope, dsn = self.extract_scope(conFileAttr["ds"])
-                # convert file attribute
-                conFile = self.convFileAttr(conFileAttr, scope)
-                conFile["type"] = "FILE"
-                if "pfn" in conFile:
-                    del conFile["pfn"]
-                # append files
-                files.append(conFile)
-            # register zip file
-            for rse in zipFileAttr["rse"]:
-                client.add_replicas(rse=rse, files=[zipFile])
-            # add files
-            nFiles = 100
-            iFiles = 0
-            while iFiles < len(files):
-                client.add_files_to_archive(
-                    scope=zipFile["scope"],
-                    name=zipFile["name"],
-                    files=files[iFiles : iFiles + nFiles],
-                )
-                iFiles += nFiles
-
-    # list datasets
-    def listDatasets(self, datasetName, old=False):
-        result = {}
-        # extract scope from dataset
-        scope, dsn = self.extract_scope(datasetName)
-        if dsn.endswith("/"):
-            dsn = dsn[:-1]
-            collection = "container"
+            items = []
+        if self._tagForSH[key] not in items:
+            items.append(self._tagForSH[key])
+        self.specialHandling = ",".join(items)
+
+    # get mode for alternative stage-out
+    def getAltStgOut(self):
+        if self.specialHandling is not None:
+            for tmpItem in self.specialHandling.split(","):
+                if tmpItem.startswith(f"{self._tagForSH['altStgOut']}:"):
+                    return tmpItem.split(":")[-1]
+        return None
+
+    # set alternative stage-out
+    def setAltStgOut(self, mode):
+        if self.specialHandling is not None:
+            items = self.specialHandling.split(",")
         else:
-            collection = "dataset"
-        filters = {"name": dsn}
-        try:
-            # get dids
-            client = RucioClient()
-            for name in client.list_dids(scope, filters, collection):
-                vuid = hashlib.md5((scope + ":" + name).encode()).hexdigest()
-                vuid = f"{vuid[0:8]}-{vuid[8:12]}-{vuid[12:16]}-{vuid[16:20]}-{vuid[20:32]}"
-                duid = vuid
-                # add /
-                if datasetName.endswith("/") and not name.endswith("/"):
-                    name += "/"
-                if old or ":" not in datasetName:
-                    keyName = name
-                else:
-                    keyName = str(f"{scope}:{name}")
-                if keyName not in result:
-                    result[keyName] = {"duid": duid, "vuids": [vuid]}
-            return result, ""
-        except Exception as e:
-            return None, f"{str(e)} {traceback.format_exc()}"
-
-    # list datasets in container
-    def listDatasetsInContainer(self, containerName):
-        result = []
-        # extract scope from dataset
-        scope, cn = self.extract_scope(containerName)
-        if cn.endswith("/"):
-            cn = cn[:-1]
-        try:
-            # get dids
-            client = RucioClient()
-            for i in client.list_content(scope, cn):
-                if i["type"] == "DATASET":
-                    result.append(str(f"{i['scope']}:{i['name']}"))
-            return result, ""
+            items = []
+        # remove old value
+        newItems = []
+        for tmpItem in items:
+            if tmpItem.startswith(f"{self._tagForSH['altStgOut']}:"):
+                continue
+            newItems.append(tmpItem)
+        newItems.append(f"{self._tagForSH['altStgOut']}:{mode}")
+        self.specialHandling = ",".join(newItems)
+
+    # put log files to OS
+    def putLogToOS(self):
+        return self.check_special_handling("putLogToOS")
+
+    # set to put log files to OS
+    def setToPutLogToOS(self):
+        self.set_special_handling("putLogToOS")
+
+    # write input to file
+    def writeInputToFile(self):
+        return self.check_special_handling("writeInputToFile")
+
+    # set to write input to file
+    def setToWriteInputToFile(self):
+        self.set_special_handling("writeInputToFile")
+
+    # set request type
+    def setRequestType(self, reqType):
+        if self.specialHandling is not None:
+            items = self.specialHandling.split(",")
+        else:
+            items = []
+        newItems = []
+        setFlag = False
+        for item in items:
+            if not item.startswith(self._tagForSH["requestType"]):
+                newItems.append(item)
+        newItems.append(f"{self._tagForSH['requestType']}={reqType}")
+        self.specialHandling = ",".join(newItems)
+
+    # sort files
+    def sortFiles(self):
+        try:
+            lfnMap = {}
+            for tmpFile in self.Files:
+                if tmpFile.lfn not in lfnMap:
+                    lfnMap[tmpFile.lfn] = []
+                lfnMap[tmpFile.lfn].append(tmpFile)
+            lfns = sorted(lfnMap)
+            newFiles = []
+            for tmpLFN in lfns:
+                for tmpFile in lfnMap[tmpLFN]:
+                    newFiles.append(tmpFile)
+            self.Files = newFiles
         except Exception:
-            errType, errVale = sys.exc_info()[:2]
-            return None, f"{errType} {errVale}"
+            pass
 
-    # list dataset replicas
-    def listDatasetReplicas(self, datasetName):
-        retMap = {}
-        # extract scope from dataset
-        scope, dsn = self.extract_scope(datasetName)
-        try:
-            # get replicas
-            client = RucioClient()
-            itr = client.list_dataset_replicas(scope, dsn)
-            for item in itr:
-                rse = item["rse"]
-                retMap[rse] = [
-                    {
-                        "total": item["length"],
-                        "found": item["available_length"],
-                        "immutable": 1,
-                    }
-                ]
-            return 0, retMap
+    # get zip file map
+    def getZipFileMap(self):
+        zipMap = dict()
+        try:
+            if self.jobParameters is not None:
+                zipStr = re.search("<ZIP_MAP>(.+)</ZIP_MAP>", self.jobParameters)
+                if zipStr is not None:
+                    for item in zipStr.group(1).split():
+                        zipFile, conFiles = item.split(":")
+                        conFiles = conFiles.split(",")
+                        zipMap[zipFile] = conFiles
         except Exception:
-            errType, errVale = sys.exc_info()[:2]
-            return 1, f"{errType} {errVale}"
+            pass
+        return zipMap
 
-    # set metadata
-    def setMetaData(self, dsn, metadata=None):
-        # register dataset
-        client = RucioClient()
-        try:
-            scope, dsn = self.extract_scope(dsn)
-            for tmpKey in metadata:
-                tmpValue = metadata[tmpKey]
-                client.set_metadata(scope, dsn, key=tmpKey, value=tmpValue)
+    # add multi step exec
+    def addMultiStepExec(self, steps):
+        if not self.jobParameters:
+            self.jobParameters = ""
+        self.jobParameters += "<MULTI_STEP_EXEC>" + json.dumps(steps) + "</MULTI_STEP_EXEC>"
+
+    # extract multi step exec
+    def extractMultiStepExec(self):
+        try:
+            if "<MULTI_STEP_EXEC>" in self.jobParameters and "</MULTI_STEP_EXEC>" in self.jobParameters:
+                pp_1, pp_2 = self.jobParameters.split("<MULTI_STEP_EXEC>")
+                pp_2 = pp_2.split("</MULTI_STEP_EXEC>")[0]
+                return pp_1, json.loads(pp_2)
         except Exception:
-            errType, errVale = sys.exc_info()[:2]
-            return False, f"{errType} {errVale}"
-        return True, ""
-
-    # get metadata
-    def getMetaData(self, dsn):
-        # register dataset
-        client = RucioClient()
-        try:
-            scope, dsn = self.extract_scope(dsn)
-            return True, client.get_metadata(scope, dsn)
-        except DataIdentifierNotFound:
-            return True, None
-        except Exception:
-            errType, errVale = sys.exc_info()[:2]
-            return False, f"{errType} {errVale}"
-
-    # delete dataset
-    def eraseDataset(self, dsn, scope=None, grace_period=None):
-        presetScope = scope
-        # register dataset
-        client = RucioClient()
-        try:
-            scope, dsn = self.extract_scope(dsn)
-            if presetScope is not None:
-                scope = presetScope
-            if grace_period is not None:
-                value = grace_period * 60 * 60
-            else:
-                value = 0.0001
-            client.set_metadata(scope=scope, name=dsn, key="lifetime", value=value)
-        except DataIdentifierNotFound:
-            pass
-        except Exception as e:
-            return False, f"{str(e)}"
-        return True, ""
-
-    # close dataset
-    def closeDataset(self, dsn):
-        # register dataset
-        client = RucioClient()
-        try:
-            scope, dsn = self.extract_scope(dsn)
-            client.set_status(scope, dsn, open=False)
-        except (UnsupportedOperation, DataIdentifierNotFound):
             pass
-        return True
+        return self.jobParameters, None
 
-    # list file replicas
-    def listFileReplicas(self, scopes, lfns, rses=None):
+    # suppress execute string conversion
+    def noExecStrCnv(self):
+        return self.check_special_handling("noExecStrCnv")
+
+    # set to suppress execute string conversion
+    def setNoExecStrCnv(self):
+        self.set_special_handling("noExecStrCnv")
+
+    # in-file positional event number
+    def inFilePosEvtNum(self):
+        return self.check_special_handling("inFilePosEvtNum")
+
+    # set to use in-file positional event number
+    def setInFilePosEvtNum(self):
+        self.set_special_handling("inFilePosEvtNum")
+
+    # register event service files
+    def registerEsFiles(self):
+        return self.check_special_handling("registerEsFiles")
+
+    # set to register event service files
+    def setRegisterEsFiles(self):
+        self.set_special_handling("registerEsFiles")
+
+    # set background-able flag
+    def setBackgroundableFlag(self):
+        self.jobExecutionID = 0
+        if self.prodSourceLabel not in ["managed", "test"]:
+            return
         try:
-            client = RucioClient()
-            dids = []
-            iGUID = 0
-            nGUID = 1000
-            retVal = {}
-            for scope, lfn in zip(scopes, lfns):
-                iGUID += 1
-                dids.append({"scope": scope, "name": lfn})
-                if len(dids) % nGUID == 0 or iGUID == len(lfns):
-                    for tmpDict in client.list_replicas(dids):
-                        tmpLFN = str(tmpDict["name"])
-                        tmpRses = list(tmpDict["rses"])
-                        # RSE selection
-                        if rses is not None:
-                            newRSEs = []
-                            for tmpRse in tmpRses:
-                                if tmpRse in rses:
-                                    newRSEs.append(tmpRse)
-                            tmpRses = newRSEs
-                        if len(tmpRses) > 0:
-                            retVal[tmpLFN] = tmpRses
-                    dids = []
-            return True, retVal
+            if self.inputFileBytes / self.maxWalltime > 5000:
+                return
         except Exception:
-            errType, errVale = sys.exc_info()[:2]
-            return False, f"{errType} {errVale}"
-
-    # get zip files
-    def getZipFiles(self, dids, rses):
+            return
         try:
-            client = RucioClient()
-            data = []
-            iGUID = 0
-            nGUID = 1000
-            retVal = {}
-            for did in dids:
-                iGUID += 1
-                scope, lfn = did.split(":")
-                data.append({"scope": scope, "name": lfn})
-                if len(data) % nGUID == 0 or iGUID == len(dids):
-                    for tmpDict in client.list_replicas(data):
-                        tmpScope = str(tmpDict["scope"])
-                        tmpLFN = str(tmpDict["name"])
-                        tmpDID = f"{tmpScope}:{tmpLFN}"
-                        # RSE selection
-                        for pfn in tmpDict["pfns"]:
-                            pfnData = tmpDict["pfns"][pfn]
-                            if (rses is None or pfnData["rse"] in rses) and pfnData["domain"] == "zip":
-                                zipFileName = pfn.split("/")[-1]
-                                zipFileName = re.sub("\?.+$", "", zipFileName)
-                                retVal[tmpDID] = client.get_metadata(tmpScope, zipFileName)
-                                break
-                    data = []
-            return True, retVal
+            if self.coreCount <= 1:
+                return
         except Exception:
-            errType, errVale = sys.exc_info()[:2]
-            return False, f"{errType} {errVale}"
+            return
+        if self.currentPriority > 250:
+            return
+        self.jobExecutionID = 1
 
-    # list files in dataset
-    def listFilesInDataset(self, datasetName, long=False, fileList=None):
-        # extract scope from dataset
-        scope, dsn = self.extract_scope(datasetName)
-        if dsn.endswith("/"):
-            dsn = dsn[:-1]
-        client = RucioClient()
-        return_dict = {}
-        for x in client.list_files(scope, dsn, long=long):
-            tmpLFN = str(x["name"])
-            if fileList is not None:
-                genLFN = re.sub("\.\d+$", "", tmpLFN)
-                if tmpLFN not in fileList and genLFN not in fileList:
-                    continue
-            dq2attrs = {}
-            dq2attrs["chksum"] = "ad:" + str(x["adler32"])
-            dq2attrs["md5sum"] = dq2attrs["chksum"]
-            dq2attrs["checksum"] = dq2attrs["chksum"]
-            dq2attrs["fsize"] = x["bytes"]
-            dq2attrs["filesize"] = dq2attrs["fsize"]
-            dq2attrs["scope"] = str(x["scope"])
-            dq2attrs["events"] = str(x["events"])
-            if long:
-                dq2attrs["lumiblocknr"] = str(x["lumiblocknr"])
-            guid = str(f"{x['guid'][0:8]}-{x['guid'][8:12]}-{x['guid'][12:16]}-{x['guid'][16:20]}-{x['guid'][20:32]}")
-            dq2attrs["guid"] = guid
-            return_dict[tmpLFN] = dq2attrs
-        return (return_dict, None)
-
-    # get # of files in dataset
-    def getNumberOfFiles(self, datasetName, presetScope=None):
-        # extract scope from dataset
-        scope, dsn = self.extract_scope(datasetName)
-        if presetScope is not None:
-            scope = presetScope
-        client = RucioClient()
-        nFiles = 0
-        try:
-            for x in client.list_files(scope, dsn):
-                nFiles += 1
-            return True, nFiles
-        except DataIdentifierNotFound:
-            return None, "dataset not found"
-        except Exception:
-            errtype, errvalue = sys.exc_info()[:2]
-            errMsg = f"{errtype.__name__} {errvalue}"
-            return False, errMsg
-
-    # get dataset size
-    def getDatasetSize(self, datasetName):
-        if datasetName.endswith("/"):
-            datasetName = datasetName[:-1]
-        # extract scope from dataset
-        scope, dsn = self.extract_scope(datasetName)
-        client = RucioClient()
-        tSize = 0
+    # use prefetcher
+    def usePrefetcher(self):
+        return self.check_special_handling("usePrefetcher")
+
+    # set to use prefetcher
+    def setUsePrefetcher(self):
+        self.set_special_handling("usePrefetcher")
+
+    # use zip to pin
+    def useZipToPin(self):
+        return self.check_special_handling("useZipToPin")
+
+    # set to use zip to pin
+    def setUseZipToPin(self):
+        self.set_special_handling("useZipToPin")
+
+    # use secrets
+    def use_secrets(self):
+        return self.check_special_handling("useSecrets")
+
+    # set to use secrets
+    def set_use_secrets(self):
+        self.set_special_handling("useSecrets")
+
+    # not discard events
+    def notDiscardEvents(self):
+        return self.check_special_handling("notDiscardEvents")
+
+    # set not to discard events
+    def setNotDiscardEvents(self):
+        self.set_special_handling("notDiscardEvents")
+
+    # all events are done
+    def allOkEvents(self):
+        return self.check_special_handling("allOkEvents")
+
+    # set all events are done
+    def setAllOkEvents(self):
+        self.set_special_handling("allOkEvents")
+
+    # set scout job flag
+    def setScoutJobFlag(self):
+        self.set_special_handling("scoutJob")
+
+    # check if scout job
+    def isScoutJob(self):
+        return self.check_special_handling("scoutJob")
+
+    # decrement attemptNr of events only when failed
+    def decAttOnFailedES(self):
+        return self.check_special_handling("decAttOnFailedES")
+
+    # set to decrement attemptNr of events only when failed
+    def setDecAttOnFailedES(self):
+        self.set_special_handling("decAttOnFailedES")
+
+    # set fake flag to ignore in monigoring
+    def setFakeJobToIgnore(self):
+        self.set_special_handling("fakeJobToIgnore")
+
+    # remove fake flag to ignore in monigoring
+    def removeFakeJobToIgnore(self):
+        if self.specialHandling is not None:
+            items = self.specialHandling.split(",")
+        else:
+            items = []
+        if self._tagForSH["fakeJobToIgnore"] in items:
+            items.remove(self._tagForSH["fakeJobToIgnore"])
+        self.specialHandling = ",".join(items)
+
+    # set task attribute
+    def set_task_attribute(self, key, value):
+        if not isinstance(self.metadata, list):
+            self.metadata = [None, None]
+        if len(self.metadata) != 3:
+            self.metadata.append({})
+        self.metadata[2][key] = value
+
+    # get task attribute
+    def get_task_attribute(self, key):
         try:
-            for x in client.list_files(scope, dsn):
-                tSize += x["bytes"]
-            return True, tSize
-        except DataIdentifierNotFound:
-            return None, "dataset not found"
+            return self.metadata[2][key]
         except Exception:
-            errtype, errvalue = sys.exc_info()[:2]
-            errMsg = f"{errtype.__name__} {errvalue}"
-            return False, errMsg
-
-    # register files
-    def registerFiles(self, files, rse):
-        client = RucioClient()
-        try:
-            # add replicas
-            client.add_replicas(files=files, rse=rse)
-        except FileAlreadyExists:
-            pass
-        try:
-            # add rule
-            client.add_replication_rule(files, copies=1, rse_expression=rse)
-        except DuplicateRule:
-            pass
+            return None
 
-    # delete files from dataset
-    def deleteFilesFromDataset(self, datasetName, files):
-        # extract scope from dataset
-        scope, dsn = self.extract_scope(datasetName)
-        client = RucioClient()
-        try:
-            # delete files
-            client.detach_dids(scope=scope, name=dsn, dids=files)
-        except DataIdentifierNotFound:
-            pass
+    # set input prestaging
+    def setInputPrestaging(self):
+        self.set_special_handling("inputPrestaging")
+
+    # use input prestaging
+    def useInputPrestaging(self):
+        return self.check_special_handling("inputPrestaging")
+
+    # to a dictionary
+    def to_dict(self):
+        ret = {}
+        for a in self._attributes:
+            v = getattr(self, a)
+            if isinstance(v, datetime.datetime):
+                v = str(v)
+            elif v == "NULL":
+                v = None
+            ret[a] = v
+        return ret
+
+    # check if HPO workflow flag
+    def is_hpo_workflow(self):
+        return self.check_special_handling("hpoWorkflow")
+
+    # set HPO workflow flag
+    def set_hpo_workflow(self):
+        self.set_special_handling("hpoWorkflow")
+
+    # check if looping check is disabled
+    def is_no_looping_check(self):
+        return self.check_special_handling("noLoopingCheck")
+
+    # disable looping check
+    def disable_looping_check(self):
+        self.set_special_handling("noLoopingCheck")
+
+    # check if encode job parameters
+    def to_encode_job_params(self):
+        return self.check_special_handling("encJobParams")
+
+    # encode job parameters
+    def set_encode_job_params(self):
+        self.set_special_handling("encJobParams")
+
+    # check if debug mode
+    def is_debug_mode(self):
+        if self.specialHandling is not None:
+            items = self.specialHandling.split(",")
+            return self._tagForSH["debugMode"] in items or "debug" in items
+        return False
+
+    # set debug mode
+    def set_debug_mode(self):
+        self.set_special_handling("debugMode")
+
+    # set push status changes
+    def set_push_status_changes(self):
+        self.set_special_handling("pushStatusChanges")
+
+    # check if to push status changes
+    def push_status_changes(self):
+        return push_status_changes(self.specialHandling)
+
+    # set push job
+    def set_push_job(self):
+        self.set_special_handling("pushJob")
+
+    # check if to push job
+    def is_push_job(self):
+        return self.check_special_handling("pushJob")
+
+    # set on-site merging
+    def set_on_site_merging(self):
+        self.set_special_handling("onSiteMerging")
+
+    # check if on-site merging
+    def is_on_site_merging(self):
+        return self.check_special_handling("onSiteMerging")
+
+    # get RAM for retry
+    def get_ram_for_retry(self):
+        if self.specialHandling is not None:
+            for tmpItem in self.specialHandling.split(","):
+                if tmpItem.startswith(f"{self._tagForSH['retryRam']}:"):
+                    return int(tmpItem.split(":")[-1])
+        return None
+
+    # set RAM for retry
+    def set_ram_for_retry(self, val):
+        if self.specialHandling:
+            items = self.specialHandling.split(",")
+        else:
+            items = []
+        # remove old value
+        newItems = []
+        for tmpItem in items:
+            if tmpItem.startswith(f"{self._tagForSH['retryRam']}:"):
+                continue
+            newItems.append(tmpItem)
+        newItems.append(f"{self._tagForSH['retryRam']}:{val}")
+        self.specialHandling = ",".join(newItems)
+
+    # dump to json-serializable
+    def dump_to_json_serializable(self):
+        job_state = self.__getstate__()
+        file_state_list = []
+        for file_spec in job_state[-1]:
+            file_stat = file_spec.dump_to_json_serializable()
+            file_state_list.append(file_stat)
+        job_state = job_state[:-1]
+        # append files
+        job_state.append(file_state_list)
+        return job_state
+
+    # load from json-serializable
+    def load_from_json_serializable(self, job_state):
+        # initialize with empty file list
+        self.__setstate__(job_state[:-1] + [[]])
+        # add files
+        for file_stat in job_state[-1]:
+            file_spec = FileSpec()
+            file_spec.__setstate__(file_stat)
+            self.addFile(file_spec)
 
-    # list datasets with GUIDs
-    def listDatasetsByGUIDs(self, guids):
-        client = RucioClient()
-        result = {}
-        for guid in guids:
-            datasets = [str(f"{i['scope']}:{i['name']}") for i in client.get_dataset_by_guid(guid)]
-            result[guid] = datasets
-        return result
 
-    # finger
-    def finger(self, dn):
-        try:
-            # get rucio API
-            client = RucioClient()
-            userInfo = None
-            retVal = False
-            x509_user_name = CoreUtils.get_bare_dn(dn)
-            oidc_user_name = CoreUtils.get_id_from_dn(dn)
-            if oidc_user_name == x509_user_name:
-                oidc_user_name = None
-            else:
-                x509_user_name = None
-            for accType in ["USER", "GROUP"]:
-                if x509_user_name is not None:
-                    userName = x509_user_name
-                    for i in client.list_accounts(account_type=accType, identity=userName):
-                        userInfo = {"nickname": i["account"], "email": i["email"]}
-                        break
-                    if userInfo is None:
-                        userName = CoreUtils.get_bare_dn(dn, keep_digits=False)
-                        for i in client.list_accounts(account_type=accType, identity=userName):
-                            userInfo = {"nickname": i["account"], "email": i["email"]}
-                            break
-                else:
-                    userName = oidc_user_name
-                try:
-                    if userInfo is None:
-                        i = client.get_account(userName)
-                        userInfo = {"nickname": i["account"], "email": i["email"]}
-                except Exception:
-                    pass
-                if userInfo is not None:
-                    retVal = True
-                    break
-        except Exception as e:
-            errMsg = f"{str(e)}"
-            userInfo = errMsg
-        return retVal, userInfo
-
-    # register container
-    def registerContainer(self, cname, datasets=[], presetScope=None):
-        if cname.endswith("/"):
-            cname = cname[:-1]
-        # register container
-        client = RucioClient()
-        try:
-            scope, dsn = self.extract_scope(cname)
-            if presetScope is not None:
-                scope = presetScope
-            client.add_container(scope=scope, name=cname)
-        except DataIdentifierAlreadyExists:
-            pass
-        # add files
-        if len(datasets) > 0:
-            try:
-                dsns = []
-                for ds in datasets:
-                    ds_scope, ds_name = self.extract_scope(ds)
-                    if ds_scope:
-                        dsn = {"scope": ds_scope, "name": ds_name}
-                    else:
-                        dsn = {"scope": scope, "name": ds}
-                    dsns.append(dsn)
-                client.add_datasets_to_container(scope=scope, name=cname, dsns=dsns)
-            except DuplicateContent:
-                for ds in dsns:
-                    try:
-                        client.add_datasets_to_container(scope=scope, name=cname, dsns=[ds])
-                    except DuplicateContent:
-                        pass
-        return True
-
-
-# instantiate
-rucioAPI = RucioAPI()
-del RucioAPI
+# utils
+
+
+# check if to push status changes without class instance
+def push_status_changes(special_handling):
+    if special_handling is not None:
+        items = special_handling.split(",")
+        return JobSpec._tagForSH["pushStatusChanges"] in items
+    return False
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/DataServiceUtils.py` & `panda_server-0.3.3/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/EventPicker.py` & `panda_server-0.3.3/pandaserver/jobdispatcher/Protocol.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,373 +1,446 @@
-"""
-add data to dataset
-
-"""
-
-import datetime
-import fcntl
-import os
+import base64
+import json
 import re
-import sys
-import traceback
+from urllib.parse import urlencode
 
-import pandaserver.brokerage.broker
-from pandacommon.pandalogger.LogWrapper import LogWrapper
-from pandacommon.pandalogger.PandaLogger import PandaLogger
-from pandaserver.dataservice import dyn_data_distributer
-from pandaserver.dataservice.DataServiceUtils import select_scope
-from pandaserver.dataservice.DDM import rucioAPI
-from pandaserver.srvcore import CoreUtils
-from pandaserver.srvcore.MailUtils import MailUtils
-from pandaserver.taskbuffer import JobUtils
-from pandaserver.taskbuffer.JobSpec import JobSpec
-from pandaserver.userinterface import Client
+from pandaserver.dataservice import DataServiceUtils
+from pandaserver.taskbuffer import EventServiceUtils
 
-# logger
-_logger = PandaLogger().getLogger("EventPicker")
+# constants
+TimeOutToken = "TimeOut"
+NoJobsToken = "NoJobs"
+
+# status codes
+# succeeded
+SC_Success = 0
+# timeout
+SC_TimeOut = 10
+# no available jobs
+SC_NoJobs = 20
+# failed
+SC_Failed = 30
+# Not secure connection
+SC_NonSecure = 40
+# invalid token
+SC_Invalid = 50
+# invalid role
+SC_Role = 60
+# permission denied
+SC_Perms = 70
+# key missing
+SC_MissKey = 80
+# failure of proxy retrieval
+SC_ProxyError = 90
 
 
-class EventPicker:
+# response
+class Response:
     # constructor
-    def __init__(self, taskBuffer, siteMapper, evpFileName, ignoreError):
-        self.taskBuffer = taskBuffer
-        self.siteMapper = siteMapper
-        self.ignoreError = ignoreError
-        self.evpFileName = evpFileName
-        self.token = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat(" ")
-        # logger
-        self.logger = LogWrapper(_logger, self.token)
-        self.pd2p = dyn_data_distributer.DynDataDistributer([], self.siteMapper, token=" ")
-        self.userDatasetName = ""
-        self.creationTime = ""
-        self.params = ""
-        self.lockedBy = ""
-        self.evpFile = None
-        self.userTaskName = ""
-        # message buffer
-        self.msgBuffer = []
-        self.lineLimit = 100
-        # JEDI
-        self.jediTaskID = None
-        self.prodSourceLabel = None
-        self.job_label = None
+    def __init__(self, statusCode, errorDialog=None):
+        # create data object
+        self.data = {"StatusCode": statusCode}
+        if errorDialog is not None:
+            self.data["errorDialog"] = errorDialog
+
+    # URL encode
+    def encode(self, acceptJson=False):
+        if not acceptJson:
+            return urlencode(self.data)
+        else:
+            return {"type": "json", "content": json.dumps(self.data)}
 
-    # main
-    def run(self):
-        try:
-            self.putLog(f"start {self.evpFileName}")
-            # lock evp file
-            self.evpFile = open(self.evpFileName)
+    # append Node
+    def appendNode(self, name, value):
+        self.data[name] = value
+
+    # append job
+    def appendJob(self, job, siteMapperCache=None):
+        # event service merge
+        if EventServiceUtils.isEventServiceMerge(job):
+            isEventServiceMerge = True
+        else:
+            isEventServiceMerge = False
+        # PandaID
+        self.data["PandaID"] = job.PandaID
+        # prodSourceLabel
+        self.data["prodSourceLabel"] = job.prodSourceLabel
+        # swRelease
+        self.data["swRelease"] = job.AtlasRelease
+        # homepackage
+        self.data["homepackage"] = job.homepackage
+        # transformation
+        self.data["transformation"] = job.transformation
+        # job name
+        self.data["jobName"] = job.jobName
+        # job definition ID
+        self.data["jobDefinitionID"] = job.jobDefinitionID
+        # cloud
+        self.data["cloud"] = job.cloud
+        # files
+        strIFiles = ""
+        strOFiles = ""
+        strDispatch = ""
+        strDisToken = ""
+        strDisTokenForOutput = ""
+        strDestination = ""
+        strRealDataset = ""
+        strRealDatasetIn = ""
+        strProdDBlock = ""
+        strDestToken = ""
+        strProdToken = ""
+        strProdTokenForOutput = ""
+        strGUID = ""
+        strFSize = ""
+        strCheckSum = ""
+        strFileDestinationSE = ""
+        strScopeIn = ""
+        strScopeOut = ""
+        strScopeLog = ""
+        logFile = ""
+        logGUID = ""
+        ddmEndPointIn = []
+        ddmEndPointOut = []
+        noOutput = []
+        siteSpec = None
+        inDsLfnMap = {}
+        inLFNset = set()
+        if siteMapperCache is not None:
+            siteMapper = siteMapperCache.getObj()
+            siteSpec = siteMapper.getSite(job.computingSite)
+            # resolve destSE
             try:
-                fcntl.flock(self.evpFile.fileno(), fcntl.LOCK_EX | fcntl.LOCK_NB)
+                job.destinationSE = siteMapper.resolveNucleus(job.destinationSE)
+                for tmpFile in job.Files:
+                    tmpFile.destinationSE = siteMapper.resolveNucleus(tmpFile.destinationSE)
             except Exception:
-                # relase
-                self.putLog(f"cannot lock {self.evpFileName}")
-                self.evpFile.close()
-                return True
-            # options
-            runEvtList = []
-            eventPickDataType = ""
-            eventPickStreamName = ""
-            eventPickDS = []
-            eventPickAmiTag = ""
-            eventPickNumSites = 1
-            inputFileList = []
-            tagDsList = []
-            tagQuery = ""
-            tagStreamRef = ""
-            skipDaTRI = False
-            runEvtGuidMap = {}
-            ei_api = ""
-            # read evp file
-            for tmpLine in self.evpFile:
-                tmpMatch = re.search("^([^=]+)=(.+)$", tmpLine)
-                # check format
-                if tmpMatch is None:
-                    continue
-                tmpItems = tmpMatch.groups()
-                if tmpItems[0] == "runEvent":
-                    # get run and event number
-                    tmpRunEvt = tmpItems[1].split(",")
-                    if len(tmpRunEvt) == 2:
-                        runEvtList.append(tmpRunEvt)
-                elif tmpItems[0] == "eventPickDataType":
-                    # data type
-                    eventPickDataType = tmpItems[1]
-                elif tmpItems[0] == "eventPickStreamName":
-                    # stream name
-                    eventPickStreamName = tmpItems[1]
-                elif tmpItems[0] == "eventPickDS":
-                    # dataset pattern
-                    eventPickDS = tmpItems[1].split(",")
-                elif tmpItems[0] == "eventPickAmiTag":
-                    # AMI tag
-                    eventPickAmiTag = tmpItems[1]
-                elif tmpItems[0] == "eventPickNumSites":
-                    # the number of sites where datasets are distributed
-                    try:
-                        eventPickNumSites = int(tmpItems[1])
-                    except Exception:
-                        pass
-                elif tmpItems[0] == "userName":
-                    # user name
-                    self.userDN = tmpItems[1]
-                    self.putLog(f"user={self.userDN}")
-                elif tmpItems[0] == "userTaskName":
-                    # user task name
-                    self.userTaskName = tmpItems[1]
-                elif tmpItems[0] == "userDatasetName":
-                    # user dataset name
-                    self.userDatasetName = tmpItems[1]
-                elif tmpItems[0] == "lockedBy":
-                    # client name
-                    self.lockedBy = tmpItems[1]
-                elif tmpItems[0] == "creationTime":
-                    # creation time
-                    self.creationTime = tmpItems[1]
-                elif tmpItems[0] == "params":
-                    # parameters
-                    self.params = tmpItems[1]
-                elif tmpItems[0] == "ei_api":
-                    # ei api parameter for MC
-                    ei_api = tmpItems[1]
-                elif tmpItems[0] == "inputFileList":
-                    # input file list
-                    inputFileList = tmpItems[1].split(",")
-                    try:
-                        inputFileList.remove("")
-                    except Exception:
-                        pass
-                elif tmpItems[0] == "tagDS":
-                    # TAG dataset
-                    tagDsList = tmpItems[1].split(",")
-                elif tmpItems[0] == "tagQuery":
-                    # query for TAG
-                    tagQuery = tmpItems[1]
-                elif tmpItems[0] == "tagStreamRef":
-                    # StreamRef for TAG
-                    tagStreamRef = tmpItems[1]
-                    if not tagStreamRef.endswith("_ref"):
-                        tagStreamRef += "_ref"
-                elif tmpItems[0] == "runEvtGuidMap":
-                    # GUIDs
-                    try:
-                        runEvtGuidMap = eval(tmpItems[1])
-                    except Exception:
-                        pass
-            # extract task name
-            if self.userTaskName == "" and self.params != "":
-                try:
-                    tmpMatch = re.search("--outDS(=| ) *([^ ]+)", self.params)
-                    if tmpMatch is not None:
-                        self.userTaskName = tmpMatch.group(2)
-                        if not self.userTaskName.endswith("/"):
-                            self.userTaskName += "/"
-                except Exception:
+                pass
+            siteMapperCache.releaseObj()
+        for file in job.Files:
+            if file.type == "input":
+                if EventServiceUtils.isJumboJob(job) and file.lfn in inLFNset:
                     pass
-            # suppress DaTRI
-            if self.params != "":
-                if "--eventPickSkipDaTRI" in self.params:
-                    skipDaTRI = True
-            # get compact user name
-            compactDN = self.taskBuffer.cleanUserID(self.userDN)
-            # get jediTaskID
-            self.jediTaskID = self.taskBuffer.getTaskIDwithTaskNameJEDI(compactDN, self.userTaskName)
-            # get prodSourceLabel
-            (
-                self.prodSourceLabel,
-                self.job_label,
-            ) = self.taskBuffer.getProdSourceLabelwithTaskID(self.jediTaskID)
-            # convert run/event list to dataset/file list
-            tmpRet, locationMap, allFiles = self.pd2p.convert_evt_run_to_datasets(
-                runEvtList,
-                eventPickDataType,
-                eventPickStreamName,
-                eventPickDS,
-                eventPickAmiTag,
-                self.userDN,
-                runEvtGuidMap,
-                ei_api,
-            )
-            if not tmpRet:
-                if "isFatal" in locationMap and locationMap["isFatal"] is True:
-                    self.ignoreError = False
-                self.endWithError("Failed to convert the run/event list to a dataset/file list")
-                return False
-            # use only files in the list
-            if inputFileList != []:
-                tmpAllFiles = []
-                for tmpFile in allFiles:
-                    if tmpFile["lfn"] in inputFileList:
-                        tmpAllFiles.append(tmpFile)
-                allFiles = tmpAllFiles
-            # remove redundant CN from DN
-            tmpDN = CoreUtils.get_id_from_dn(self.userDN)
-            # make dataset container
-            tmpRet = self.pd2p.register_dataset_container_with_datasets(
-                self.userDatasetName,
-                allFiles,
-                locationMap,
-                n_sites=eventPickNumSites,
-                owner=tmpDN,
-            )
-            if not tmpRet:
-                self.endWithError(f"Failed to make a dataset container {self.userDatasetName}")
-                return False
-            # skip DaTRI
-            if skipDaTRI:
-                # successfully terminated
-                self.putLog("skip DaTRI")
-                # update task
-                self.taskBuffer.updateTaskModTimeJEDI(self.jediTaskID)
-            else:
-                # get candidates
-                tmpRet, candidateMaps = self.pd2p.get_candidates(
-                    self.userDatasetName,
-                    self.prodSourceLabel,
-                    self.job_label,
-                    check_used_file=False,
-                )
-                if not tmpRet:
-                    self.endWithError("Failed to find candidate for destination")
-                    return False
-                # collect all candidates
-                allCandidates = []
-                for tmpDS in candidateMaps:
-                    tmpDsVal = candidateMaps[tmpDS]
-                    for tmpCloud in tmpDsVal:
-                        tmpCloudVal = tmpDsVal[tmpCloud]
-                        for tmpSiteName in tmpCloudVal[0]:
-                            if tmpSiteName not in allCandidates:
-                                allCandidates.append(tmpSiteName)
-                if allCandidates == []:
-                    self.endWithError("No candidate for destination")
-                    return False
-                # get list of dataset (container) names
-                if eventPickNumSites > 1:
-                    # decompose container to transfer datasets separately
-                    tmpRet, tmpOut = self.pd2p.get_list_dataset_replicas_in_container(self.userDatasetName)
-                    if not tmpRet:
-                        self.endWithError(f"Failed to get replicas in {self.userDatasetName}")
-                        return False
-                    userDatasetNameList = list(tmpOut)
                 else:
-                    # transfer container at once
-                    userDatasetNameList = [self.userDatasetName]
-                # loop over all datasets
-                sitesUsed = []
-                for tmpUserDatasetName in userDatasetNameList:
-                    # get size of dataset container
-                    tmpRet, totalInputSize = rucioAPI.getDatasetSize(tmpUserDatasetName)
-                    if not tmpRet:
-                        self.endWithError(f"Failed to get the size of {tmpUserDatasetName} with {totalInputSize}")
-                        return False
-                    # run brokerage
-                    tmpJob = JobSpec()
-                    tmpJob.AtlasRelease = ""
-                    self.putLog(f"run brokerage for {tmpDS}")
-                    pandaserver.brokerage.broker.schedule(
-                        [tmpJob],
-                        self.taskBuffer,
-                        self.siteMapper,
-                        True,
-                        allCandidates,
-                        True,
-                        datasetSize=totalInputSize,
-                    )
-                    if tmpJob.computingSite.startswith("ERROR"):
-                        self.endWithError(f"brokerage failed with {tmpJob.computingSite}")
-                        return False
-                    self.putLog(f"site -> {tmpJob.computingSite}")
-                    # send transfer request
-                    try:
-                        tmpSiteSpec = self.siteMapper.getSite(tmpJob.computingSite)
-                        scope_input, scope_output = select_scope(tmpSiteSpec, JobUtils.PROD_PS, JobUtils.PROD_PS)
-                        tmpDQ2ID = tmpSiteSpec.ddm_output[scope_output]
-                        tmpMsg = f"registerDatasetLocation for EventPicking  ds={tmpUserDatasetName} site={tmpDQ2ID} id={None}"
-                        self.putLog(tmpMsg)
-                        rucioAPI.registerDatasetLocation(
-                            tmpDS,
-                            [tmpDQ2ID],
-                            lifetime=14,
-                            owner=None,
-                            activity="Analysis Output",
-                        )
-                        self.putLog("OK")
-                    except Exception:
-                        errType, errValue = sys.exc_info()[:2]
-                        tmpStr = f"Failed to send transfer request : {errType} {errValue}"
-                        tmpStr.strip()
-                        tmpStr += traceback.format_exc()
-                        self.endWithError(tmpStr)
-                        return False
-                    # list of sites already used
-                    sitesUsed.append(tmpJob.computingSite)
-                    self.putLog(f"used {len(sitesUsed)} sites")
-                    # set candidates
-                    if len(sitesUsed) >= eventPickNumSites:
-                        # reset candidates to limit the number of sites
-                        allCandidates = sitesUsed
-                        sitesUsed = []
+                    inLFNset.add(file.lfn)
+                    if strIFiles != "":
+                        strIFiles += ","
+                    strIFiles += file.lfn
+                    if strDispatch != "":
+                        strDispatch += ","
+                    strDispatch += file.dispatchDBlock
+                    if strDisToken != "":
+                        strDisToken += ","
+                    strDisToken += file.dispatchDBlockToken
+                    strProdDBlock += f"{file.prodDBlock},"
+                    if not isEventServiceMerge:
+                        strProdToken += f"{file.prodDBlockToken},"
                     else:
-                        # remove site
-                        allCandidates.remove(tmpJob.computingSite)
-                # send email notification for success
-                tmpMsg = "A transfer request was successfully sent to Rucio.\n"
-                tmpMsg += "Your task will get started once transfer is completed."
-
+                        strProdToken += f"{job.metadata[1][file.lfn]},"
+                    if strGUID != "":
+                        strGUID += ","
+                    strGUID += file.GUID
+                    strRealDatasetIn += f"{file.dataset},"
+                    strFSize += f"{file.fsize},"
+                    if file.checksum not in ["", "NULL", None]:
+                        strCheckSum += f"{file.checksum},"
+                    else:
+                        strCheckSum += f"{file.md5sum},"
+                    strScopeIn += f"{file.scope},"
+                    ddmEndPointIn.append(
+                        self.getDdmEndpoint(
+                            siteSpec,
+                            file.dispatchDBlockToken,
+                            "input",
+                            job.prodSourceLabel,
+                            job.job_label,
+                        )
+                    )
+                    if file.dataset not in inDsLfnMap:
+                        inDsLfnMap[file.dataset] = []
+                    inDsLfnMap[file.dataset].append(file.lfn)
+            if file.type == "output" or file.type == "log":
+                if strOFiles != "":
+                    strOFiles += ","
+                strOFiles += file.lfn
+                if strDestination != "":
+                    strDestination += ","
+                strDestination += file.destinationDBlock
+                if strRealDataset != "":
+                    strRealDataset += ","
+                strRealDataset += file.dataset
+                strFileDestinationSE += f"{file.destinationSE},"
+                if file.type == "log":
+                    logFile = file.lfn
+                    logGUID = file.GUID
+                    strScopeLog = file.scope
+                else:
+                    strScopeOut += f"{file.scope},"
+                if strDestToken != "":
+                    strDestToken += ","
+                strDestToken += re.sub("^ddd:", "dst:", file.destinationDBlockToken.split(",")[0])
+                strDisTokenForOutput += f"{file.dispatchDBlockToken},"
+                strProdTokenForOutput += f"{file.prodDBlockToken},"
+                ddmEndPointOut.append(
+                    self.getDdmEndpoint(
+                        siteSpec,
+                        file.destinationDBlockToken.split(",")[0],
+                        "output",
+                        job.prodSourceLabel,
+                        job.job_label,
+                    )
+                )
+                if file.isAllowedNoOutput():
+                    noOutput.append(file.lfn)
+        # inFiles
+        self.data["inFiles"] = strIFiles
+        # dispatch DBlock
+        self.data["dispatchDblock"] = strDispatch
+        # dispatch DBlock space token
+        self.data["dispatchDBlockToken"] = strDisToken
+        # dispatch DBlock space token for output
+        self.data["dispatchDBlockTokenForOut"] = strDisTokenForOutput[:-1]
+        # outFiles
+        self.data["outFiles"] = strOFiles
+        # destination DBlock
+        self.data["destinationDblock"] = strDestination
+        # destination DBlock space token
+        self.data["destinationDBlockToken"] = strDestToken
+        # prod DBlocks
+        self.data["prodDBlocks"] = strProdDBlock[:-1]
+        # prod DBlock space token
+        self.data["prodDBlockToken"] = strProdToken[:-1]
+        # real output datasets
+        self.data["realDatasets"] = strRealDataset
+        # real output datasets
+        self.data["realDatasetsIn"] = strRealDatasetIn[:-1]
+        # file's destinationSE
+        self.data["fileDestinationSE"] = strFileDestinationSE[:-1]
+        # log filename
+        self.data["logFile"] = logFile
+        # log GUID
+        self.data["logGUID"] = logGUID
+        # jobPars
+        self.data["jobPars"], ppSteps = job.extractMultiStepExec()
+        if ppSteps is not None:
+            self.data.update(ppSteps)
+        if job.to_encode_job_params():
+            self.data["jobPars"] = base64.b64encode(self.data["jobPars"].encode()).decode()
+        # attempt number
+        self.data["attemptNr"] = job.attemptNr
+        # GUIDs
+        self.data["GUID"] = strGUID
+        # checksum
+        self.data["checksum"] = strCheckSum[:-1]
+        # fsize
+        self.data["fsize"] = strFSize[:-1]
+        # scope
+        self.data["scopeIn"] = strScopeIn[:-1]
+        self.data["scopeOut"] = strScopeOut[:-1]
+        self.data["scopeLog"] = strScopeLog
+        # DDM endpoints
+        try:
+            self.data["ddmEndPointIn"] = ",".join(ddmEndPointIn)
+        except TypeError:
+            self.data["ddmEndPointIn"] = ""
+        try:
+            self.data["ddmEndPointOut"] = ",".join(ddmEndPointOut)
+        except TypeError:
+            self.data["ddmEndPointOut"] = ""
+        # destinationSE
+        self.data["destinationSE"] = job.destinationSE
+        # user ID
+        self.data["prodUserID"] = job.prodUserID
+        # CPU count
+        self.data["maxCpuCount"] = job.maxCpuCount
+        # RAM count
+        self.data["minRamCount"] = job.minRamCount
+        # disk count
+        self.data["maxDiskCount"] = job.maxDiskCount
+        # cmtconfig
+        if ppSteps is None or job.cmtConfig not in ["NULL", None]:
+            self.data["cmtConfig"] = job.cmtConfig
+        else:
+            self.data["cmtConfig"] = ""
+        # processingType
+        self.data["processingType"] = job.processingType
+        # transferType
+        self.data["transferType"] = job.transferType
+        # sourceSite
+        self.data["sourceSite"] = job.sourceSite
+        # current priority
+        self.data["currentPriority"] = job.currentPriority
+        # taskID
+        if job.lockedby == "jedi":
+            self.data["taskID"] = job.jediTaskID
+        else:
+            self.data["taskID"] = job.taskID
+        # core count
+        if job.coreCount in ["NULL", None]:
+            self.data["coreCount"] = 1
+        else:
+            self.data["coreCount"] = job.coreCount
+        # jobsetID
+        self.data["jobsetID"] = job.jobsetID
+        # requestID
+        self.data["reqID"] = job.reqID
+        # nucleus
+        self.data["nucleus"] = job.nucleus
+        # walltime
+        self.data["maxWalltime"] = job.maxWalltime
+        # resource type
+        self.data["resource_type"] = job.resource_type
+        # looping check
+        if job.is_no_looping_check():
+            self.data["loopingCheck"] = False
+        # debug mode
+        if job.is_debug_mode():
+            self.data["debug"] = "True"
+        # event service or job cloning or fine-grained
+        if EventServiceUtils.isJobCloningJob(job):
+            self.data["cloneJob"] = EventServiceUtils.getJobCloningType(job)
+        elif EventServiceUtils.isEventServiceJob(job) or EventServiceUtils.isJumboJob(job):
+            self.data["eventService"] = "True"
+            # prod DBlock space token for pre-merging output
+            self.data["prodDBlockTokenForOutput"] = strProdTokenForOutput[:-1]
+        elif EventServiceUtils.is_fine_grained_job(job):
+            self.data["eventService"] = "True"
+        # event service merge
+        if isEventServiceMerge:
+            self.data["eventServiceMerge"] = "True"
+            # write to file for ES merge
+            writeToFileStr = ""
             try:
-                # unlock and delete evp file
-                fcntl.flock(self.evpFile.fileno(), fcntl.LOCK_UN)
-                self.evpFile.close()
-                os.remove(self.evpFileName)
+                for outputName in job.metadata[0]:
+                    inputList = job.metadata[0][outputName]
+                    writeToFileStr += f"inputFor_{outputName}:"
+                    for tmpInput in inputList:
+                        writeToFileStr += f"{tmpInput},"
+                    writeToFileStr = writeToFileStr[:-1]
+                    writeToFileStr += "^"
+                writeToFileStr = writeToFileStr[:-1]
             except Exception:
                 pass
-            # successfully terminated
-            self.putLog(f"end {self.evpFileName}")
-            return True
-        except Exception:
-            errType, errValue = sys.exc_info()[:2]
-            self.endWithError(f"Got exception {errType}:{errValue} {traceback.format_exc()}")
-            return False
-
-    # end with error
-    def endWithError(self, message):
-        self.putLog(message, "error")
-        # unlock evp file
-        try:
-            fcntl.flock(self.evpFile.fileno(), fcntl.LOCK_UN)
-            self.evpFile.close()
-            if not self.ignoreError:
-                # remove evp file
-                os.remove(self.evpFileName)
-        except Exception:
-            pass
-        # upload log
-        if self.jediTaskID is not None:
-            outLog = self.uploadLog()
-            self.taskBuffer.updateTaskErrorDialogJEDI(self.jediTaskID, "event picking failed. " + outLog)
-            # update task
-            if not self.ignoreError:
-                self.taskBuffer.updateTaskModTimeJEDI(self.jediTaskID, "tobroken")
-            self.putLog(outLog)
-        self.putLog(f"end {self.evpFileName}")
-
-    # put log
-    def putLog(self, msg, type="debug"):
-        tmpMsg = msg
-        if type == "error":
-            self.logger.error(tmpMsg)
-        else:
-            self.logger.debug(tmpMsg)
+            self.data["writeToFile"] = writeToFileStr
+        elif job.writeInputToFile():
+            try:
+                # write input to file
+                writeToFileStr = ""
+                for inDS in inDsLfnMap:
+                    inputList = inDsLfnMap[inDS]
+                    inDS = re.sub("/$", "", inDS)
+                    inDS = inDS.split(":")[-1]
+                    writeToFileStr += f"tmpin_{inDS}:"
+                    writeToFileStr += ",".join(inputList)
+                    writeToFileStr += "^"
+                writeToFileStr = writeToFileStr[:-1]
+                self.data["writeToFile"] = writeToFileStr
+            except Exception:
+                pass
+        # replace placeholder
+        if EventServiceUtils.isJumboJob(job) or EventServiceUtils.isCoJumboJob(job):
+            try:
+                for inDS in inDsLfnMap:
+                    inputList = inDsLfnMap[inDS]
+                    inDS = re.sub("/$", "", inDS)
+                    inDS = inDS.split(":")[-1]
+                    srcStr = f"tmpin__cnt_{inDS}"
+                    dstStr = ",".join(inputList)
+                    self.data["jobPars"] = self.data["jobPars"].replace(srcStr, dstStr)
+            except Exception:
+                pass
+        # no output
+        if noOutput != []:
+            self.data["allowNoOutput"] = ",".join(noOutput)
+        # alternative stage-out
+        if job.getAltStgOut() is not None:
+            self.data["altStageOut"] = job.getAltStgOut()
+        # log to OS
+        if job.putLogToOS():
+            self.data["putLogToOS"] = "True"
+        # suppress execute string conversion
+        if job.noExecStrCnv():
+            self.data["noExecStrCnv"] = "True"
+        # in-file positional event number
+        if job.inFilePosEvtNum():
+            self.data["inFilePosEvtNum"] = "True"
+        # use prefetcher
+        if job.usePrefetcher():
+            self.data["usePrefetcher"] = "True"
+        # image name
+        if job.container_name not in ["NULL", None]:
+            self.data["container_name"] = job.container_name
+        # IO
+        self.data["ioIntensity"] = job.get_task_attribute("ioIntensity")
+        self.data["ioIntensityUnit"] = job.get_task_attribute("ioIntensityUnit")
+        # HPO
+        if job.is_hpo_workflow():
+            self.data["isHPO"] = "True"
+        # VP
+        if siteSpec is not None:
+            scope_input, scope_output = DataServiceUtils.select_scope(siteSpec, job.prodSourceLabel, job.job_label)
+            if siteSpec.use_vp(scope_input):
+                self.data["useVP"] = "True"
+        # on-site merging
+        if job.is_on_site_merging():
+            self.data["onSiteMerging"] = "True"
+
+    # set proxy key
+    def setProxyKey(self, proxyKey):
+        names = ["credname", "myproxy"]
+        for name in names:
+            if name in proxyKey:
+                self.data[name] = proxyKey[name]
+            else:
+                self.data[name] = ""
 
-    # upload log
-    def uploadLog(self):
-        if self.jediTaskID is None:
-            return "cannot find jediTaskID"
-        strMsg = self.logger.dumpToString()
-        s, o = Client.uploadLog(strMsg, self.jediTaskID)
-        if s != 0:
-            return f"failed to upload log with {s}."
-        if o.startswith("http"):
-            return f'<a href="{o}">log</a>'
-        return o
+    # set secret key for panda proxy
+    def setPandaProxySecretKey(self, secretKey):
+        self.data["pandaProxySecretKey"] = secretKey
+
+    # get ddm endpoint
+    def getDdmEndpoint(self, siteSpec, spaceToken, mode, prodSourceLabel, job_label):
+        scope_input, scope_output = DataServiceUtils.select_scope(siteSpec, prodSourceLabel, job_label)
+        if siteSpec is None or mode not in ["input", "output"]:
+            return ""
+
+        if mode == "input":
+            connected_endpoints = siteSpec.ddm_endpoints_input.get(scope_input)
+        elif mode == "output":
+            connected_endpoints = siteSpec.ddm_endpoints_output.get(scope_output)
+
+        endPoint = DataServiceUtils.getDestinationSE(spaceToken)
+        if endPoint and connected_endpoints and connected_endpoints.isAssociated(endPoint):
+            return endPoint
+
+        endPoint = DataServiceUtils.getDistributedDestination(spaceToken)
+        if endPoint and connected_endpoints and connected_endpoints.isAssociated(endPoint):
+            return endPoint
+
+        if mode == "input":
+            setokens = siteSpec.setokens_input.get(scope_input, [])
+            ddm = siteSpec.ddm_input.get(scope_input)
+        elif mode == "output":
+            setokens = siteSpec.setokens_output.get(scope_output, [])
+            ddm = siteSpec.ddm_output.get(scope_output)
+        if spaceToken in setokens:
+            return setokens[spaceToken]
+
+        # Protection against misconfigured sites
+        if not ddm:
+            ddm = ""
+
+        return ddm
+
+
+# check if secure connection
+def isSecure(req):
+    if "SSL_CLIENT_S_DN" not in req.subprocess_env:
+        return False
+    return True
+
+
+# get user DN
+def getUserDN(req):
+    try:
+        return req.subprocess_env["SSL_CLIENT_S_DN"]
+    except Exception:
+        return "None"
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/ProcessLimiter.py` & `panda_server-0.3.3/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda_server-0.3.3/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 
 from pandacommon.pandautils.thread_utils import GenericThread
 from pandaserver.config import panda_config
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.userinterface import Client
 from rucio.client import Client as RucioClient
 from rucio.common.exception import DataIdentifierNotFound
 
 
 # get files form rucio
 def get_files_from_rucio(ds_name, log_stream):
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/Setupper.py` & `panda_server-0.3.3/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda_server-0.3.3/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import uuid
 
 import pandaserver.brokerage.broker
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
 from pandaserver.dataservice import DataServiceUtils, ErrorCode
 from pandaserver.dataservice.DataServiceUtils import select_scope
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.dataservice.SetupperPluginBase import SetupperPluginBase
 from pandaserver.taskbuffer import EventServiceUtils, JobUtils
 from pandaserver.taskbuffer.DatasetSpec import DatasetSpec
 from rucio.common.exception import (
     DataIdentifierAlreadyExists,
     DataIdentifierNotFound,
     Duplicate,
@@ -222,15 +222,15 @@
             # production datablock
             if job.prodDBlock != "NULL" and job.prodDBlock and (job.prodSourceLabel not in ["user", "panda"]):
                 # get VUID and record prodDBlock into DB
                 if job.prodDBlock not in prodError:
                     self.logger.debug("listDatasets " + job.prodDBlock)
                     prodError[job.prodDBlock] = ""
                     for iDDMTry in range(3):
-                        newOut, errMsg = rucioAPI.listDatasets(job.prodDBlock)
+                        newOut, errMsg = rucioAPI.list_datasets(job.prodDBlock)
                         if newOut is None:
                             time.sleep(10)
                         else:
                             break
                     if newOut is None:
                         prodError[job.prodDBlock] = f"Setupper._setupSource() could not get VUID of prodDBlock with {errMsg}"
                         self.logger.error(prodError[job.prodDBlock])
@@ -348,15 +348,15 @@
             if (not self.pandaDDM) and job.prodSourceLabel != "ddm":
                 # register dispatch dataset
                 self.dispFileList[dispatchDBlock] = fileList[dispatchDBlock]
                 if not useZipToPinMap[dispatchDBlock]:
                     disFiles = fileList[dispatchDBlock]
                 else:
                     dids = fileList[dispatchDBlock]["lfns"]
-                    tmpZipStat, tmpZipOut = rucioAPI.getZipFiles(dids, None)
+                    tmpZipStat, tmpZipOut = rucioAPI.get_zip_files(dids, None)
                     if not tmpZipStat:
                         self.logger.debug(f"failed to get zip files : {tmpZipOut}")
                         tmpZipOut = {}
                     disFiles = {"lfns": [], "guids": [], "fsizes": [], "chksums": []}
                     for tmpLFN, tmpGUID, tmpFSize, tmpChksum in zip(
                         fileList[dispatchDBlock]["lfns"],
                         fileList[dispatchDBlock]["guids"],
@@ -387,15 +387,15 @@
                 tmpMsg = "registerDataset {ds} {meta}"
                 self.logger.debug(tmpMsg.format(ds=dispatchDBlock, meta=str(metadata)))
                 nDDMTry = 3
                 isOK = False
                 errStr = ""
                 for iDDMTry in range(nDDMTry):
                     try:
-                        out = rucioAPI.registerDataset(
+                        out = rucioAPI.register_dataset(
                             dispatchDBlock,
                             disFiles["lfns"],
                             disFiles["guids"],
                             disFiles["fsizes"],
                             disFiles["chksums"],
                             lifetime=7,
                             scope="panda",
@@ -417,15 +417,15 @@
                 self.logger.debug(out)
                 newOut = out
                 # freezeDataset dispatch dataset
                 self.logger.debug("closeDataset " + dispatchDBlock)
                 for iDDMTry in range(3):
                     status = False
                     try:
-                        rucioAPI.closeDataset(dispatchDBlock)
+                        rucioAPI.close_dataset(dispatchDBlock)
                         status = True
                         break
                     except Exception:
                         errtype, errvalue = sys.exc_info()[:2]
                         out = f"failed to close : {errtype} {errvalue}"
                         time.sleep(10)
                 if not status:
@@ -628,15 +628,15 @@
                                 if ddmBackEnd is None:
                                     ddmBackEnd = "rucio"
                                 # register dataset
                                 self.logger.debug(f"registerNewDataset {name} metadata={tmpMetadata}")
                                 isOK = False
                                 for iDDMTry in range(3):
                                     try:
-                                        out = rucioAPI.registerDataset(
+                                        out = rucioAPI.register_dataset(
                                             name,
                                             metadata=tmpMetadata,
                                             lifetime=tmpLifeTime,
                                         )
                                         self.logger.debug(out)
                                         newVUID = out["vuid"]
                                         isOK = True
@@ -698,15 +698,15 @@
                                         # invalid location
                                         if dq2ID is None:
                                             out = f"wrong location : {dq2ID}"
                                             self.logger.error(out)
                                             break
                                         for iDDMTry in range(3):
                                             try:
-                                                out = rucioAPI.registerDatasetLocation(
+                                                out = rucioAPI.register_dataset_location(
                                                     name,
                                                     [dq2ID],
                                                     lifetime=repLifeTime,
                                                     activity=activity,
                                                     grouping=grouping,
                                                 )
                                                 self.logger.debug(out)
@@ -731,15 +731,15 @@
                         # already failed
                         if destError[dest] != "" and name == originalName:
                             break
                         # get vuid
                         if newVUID is None:
                             self.logger.debug("listDatasets " + name)
                             for iDDMTry in range(3):
-                                newOut, errMsg = rucioAPI.listDatasets(name)
+                                newOut, errMsg = rucioAPI.list_datasets(name)
                                 if newOut is None:
                                     time.sleep(10)
                                 else:
                                     break
                             if newOut is None:
                                 errMsg = f"failed to get VUID for {name} with {errMsg}"
                                 self.logger.error(errMsg)
@@ -1017,20 +1017,20 @@
                                         "dn": optOwner,
                                         "comment": optComment,
                                     },
                                 )
                             )
                             for iDDMTry in range(3):
                                 try:
-                                    status = rucioAPI.registerDatasetSubscription(
+                                    status = rucioAPI.register_dataset_subscription(
                                         job.dispatchDBlock,
                                         [dq2ID],
                                         activity=optActivity,
                                         lifetime=7,
-                                        dn=optOwner,
+                                        distinguished_name=optOwner,
                                         comment=optComment,
                                     )
                                     out = "OK"
                                     break
                                 except Exception as e:
                                     status = False
                                     out = f"registerDatasetSubscription failed with {str(e)} {traceback.format_exc()}"
@@ -1435,15 +1435,15 @@
     def getListFilesInDataset(self, dataset, fileList=None, useCache=True):
         # use cache data
         if useCache and dataset in self.lfnDatasetMap:
             return 0, self.lfnDatasetMap[dataset]
         for iDDMTry in range(3):
             try:
                 self.logger.debug("listFilesInDataset " + dataset)
-                items, tmpDummy = rucioAPI.listFilesInDataset(dataset, fileList=fileList)
+                items, tmpDummy = rucioAPI.list_files_in_dataset(dataset, file_list=fileList)
                 status = 0
                 break
             except DataIdentifierNotFound:
                 status = -1
                 break
             except Exception:
                 status = -2
@@ -1456,29 +1456,29 @@
         return status, items
 
     # get list of datasets in container
     def getListDatasetInContainer(self, container):
         # get datasets in container
         self.logger.debug("listDatasetsInContainer " + container)
         for iDDMTry in range(3):
-            datasets, out = rucioAPI.listDatasetsInContainer(container)
+            datasets, out = rucioAPI.list_datasets_in_container(container)
             if datasets is None:
                 time.sleep(10)
             else:
                 break
         if datasets is None:
             self.logger.error(out)
             return False, out
         return True, datasets
 
     def getListDatasetReplicasInContainer(self, container, getMap=False):
         # get datasets in container
         self.logger.debug("listDatasetsInContainer " + container)
         for iDDMTry in range(3):
-            datasets, out = rucioAPI.listDatasetsInContainer(container)
+            datasets, out = rucioAPI.list_datasets_in_container(container)
             if datasets is None:
                 time.sleep(10)
             else:
                 break
         if datasets is None:
             self.logger.error(out)
             if getMap:
@@ -1530,15 +1530,15 @@
         return 0, str(allRepMap)
 
     # get list of replicas for a dataset
     def getListDatasetReplicas(self, dataset, getMap=True):
         nTry = 3
         for iDDMTry in range(nTry):
             self.logger.debug(f"{iDDMTry}/{nTry} listDatasetReplicas {dataset}")
-            status, out = rucioAPI.listDatasetReplicas(dataset)
+            status, out = rucioAPI.list_dataset_replicas(dataset)
             if status != 0:
                 time.sleep(10)
             else:
                 break
         # result
         if status != 0:
             self.logger.error(out)
@@ -1695,15 +1695,15 @@
                         lfns = []
                         guids = []
                         fsizes = []
                         chksums = []
                         tmpZipOut = {}
                         if tmpJob.useZipToPin():
                             dids = [tmpFileList[tmpSubFileName]["lfn"] for tmpSubFileName in subFileNames]
-                            tmpZipStat, tmpZipOut = rucioAPI.getZipFiles(dids, [tmpLocation])
+                            tmpZipStat, tmpZipOut = rucioAPI.get_zip_files(dids, [tmpLocation])
                             if not tmpZipStat:
                                 self.logger.debug(f"failed to get zip files : {tmpZipOut}")
                                 tmpZipOut = {}
                         for tmpSubFileName in subFileNames:
                             tmpLFN = tmpFileList[tmpSubFileName]["lfn"]
                             if tmpLFN in tmpZipOut:
                                 tmpZipFileName = f"{tmpZipOut[tmpLFN]['scope']}:{tmpZipOut[tmpLFN]['name']}"
@@ -1737,15 +1737,15 @@
                                 fsizes=str(fsizes),
                                 chksums=str(chksums),
                                 meta=str(metadata),
                             )
                         )
                         for iDDMTry in range(nDDMTry):
                             try:
-                                out = rucioAPI.registerDataset(
+                                out = rucioAPI.register_dataset(
                                     disDBlock,
                                     lfns,
                                     guids,
                                     fsizes,
                                     chksums,
                                     lifetime=7,
                                     scope="panda",
@@ -1781,15 +1781,15 @@
                             self.logger.error(f"ext registerNewDataset : failed to decode VUID for {disDBlock} - {errType} {errValue}")
                             continue
                         # freezeDataset dispatch dataset
                         self.logger.debug("freezeDataset " + disDBlock)
                         for iDDMTry in range(3):
                             status = False
                             try:
-                                rucioAPI.closeDataset(disDBlock)
+                                rucioAPI.close_dataset(disDBlock)
                                 status = True
                                 break
                             except Exception:
                                 errtype, errvalue = sys.exc_info()[:2]
                                 out = f"failed to close : {errtype} {errvalue}"
                                 time.sleep(10)
                         if not status:
@@ -1797,21 +1797,20 @@
                             continue
                         # register location
                         isOK = False
                         self.logger.debug(f"ext registerDatasetLocation {disDBlock} {tmpLocation} {7}days asynchronous=True")
                         nDDMTry = 3
                         for iDDMTry in range(nDDMTry):
                             try:
-                                out = rucioAPI.registerDatasetLocation(
+                                out = rucioAPI.register_dataset_location(
                                     disDBlock,
                                     [tmpLocation],
                                     7,
                                     activity="Production Input",
                                     scope="panda",
-                                    asynchronous=True,
                                     grouping="NONE",
                                 )
                                 self.logger.debug(out)
                                 isOK = True
                                 break
                             except Exception:
                                 errType, errValue = sys.exc_info()[:2]
@@ -1991,15 +1990,15 @@
         # return for failuer
         retFailed = False
         self.logger.debug(f"registerDatasetSubscription {dataset} {dq2ID}")
         nTry = 3
         for iDDMTry in range(nTry):
             try:
                 # register subscription
-                status = rucioAPI.registerDatasetSubscription(dataset, [dq2ID], activity="Production Input")
+                status = rucioAPI.register_dataset_subscription(dataset, [dq2ID], activity="Production Input")
                 out = "OK"
                 break
             except Exception:
                 status = False
                 errType, errValue = sys.exc_info()[:2]
                 out = f"{errType} {errValue}"
                 time.sleep(10)
@@ -2085,17 +2084,17 @@
             # register and subscribe dis dataset
             if len(lfns) != 0:
                 # set dis dataset
                 jumboJobSpec.dispatchDBlock = dispatchDBlock
                 # register dis dataset
                 try:
                     self.logger.debug(f"registering jumbo dis dataset {dispatchDBlock} with {len(lfns)} files")
-                    out = rucioAPI.registerDataset(dispatchDBlock, lfns, guids, sizes, checksums, lifetime=14)
+                    out = rucioAPI.register_dataset(dispatchDBlock, lfns, guids, sizes, checksums, lifetime=14)
                     vuid = out["vuid"]
-                    rucioAPI.closeDataset(dispatchDBlock)
+                    rucioAPI.close_dataset(dispatchDBlock)
                 except Exception:
                     errType, errValue = sys.exc_info()[:2]
                     self.logger.debug(f"failed to register jumbo dis dataset {dispatchDBlock} with {errType}:{errValue}")
                     jumboJobSpec.jobStatus = "failed"
                     jumboJobSpec.ddmErrorCode = ErrorCode.EC_Setupper
                     jumboJobSpec.ddmErrorDiag = f"failed to register jumbo dispatch dataset {dispatchDBlock}"
                     ngJobs.append(jumboJobSpec)
@@ -2106,15 +2105,15 @@
                     scope_input, scope_output = select_scope(
                         tmpSiteSpec,
                         jumboJobSpec.prodSourceLabel,
                         jumboJobSpec.job_label,
                     )
                     endPoint = tmpSiteSpec.ddm_input[scope_input]
                     self.logger.debug(f"subscribing jumbo dis dataset {dispatchDBlock} to {endPoint}")
-                    rucioAPI.registerDatasetSubscription(
+                    rucioAPI.register_dataset_subscription(
                         dispatchDBlock,
                         [endPoint],
                         lifetime=14,
                         activity="Production Input",
                     )
                 except Exception:
                     errType, errValue = sys.exc_info()[:2]
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda_server-0.3.3/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/SetupperPluginBase.py` & `panda_server-0.3.3/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/activator.py` & `panda_server-0.3.3/pandaserver/dataservice/activator.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/closer.py` & `panda_server-0.3.3/pandaserver/dataservice/closer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 update dataset DB, and then close dataset and start Activator if needed
 
 """
 
-import sys
 import datetime
-
+import sys
 from typing import Dict, List
 
-from pandacommon.pandalogger.PandaLogger import PandaLogger
 from pandacommon.pandalogger.LogWrapper import LogWrapper
+from pandacommon.pandalogger.PandaLogger import PandaLogger
 
 from pandaserver.config import panda_config
+from pandaserver.dataservice import DataServiceUtils
 from pandaserver.dataservice.activator import Activator
 from pandaserver.taskbuffer import EventServiceUtils
-from pandaserver.dataservice import DataServiceUtils
 
 # logger
 _logger = PandaLogger().getLogger("closer")
 
 
 class Closer:
     """
@@ -26,16 +25,15 @@
     The class updates output-related dataset records (_sub, output, and log) in
     the database, closes _sub datasets if necessary, and activates downstream
     runJobs if the output dataset is for buildJob (libDS, library dataset).
     Activator changes job status from defined/assigned to activated.
     """
 
     # constructor
-    def __init__(self, taskBuffer, destination_data_blocks: List[str], job,
-                 dataset_map: Dict = None) -> None:
+    def __init__(self, taskBuffer, destination_data_blocks: List[str], job, dataset_map: Dict = None) -> None:
         """
         Constructor
 
         Args:
             taskBuffer: Task buffer.
             destination_data_blocks (List[str]): Destination Dispatch blocks.
             job: Job.
@@ -52,16 +50,15 @@
     def check_sub_datasets_in_jobset(self) -> bool:
         """
         Check sub datasets with the same jobset
 
         Returns:
             bool: True if all sub datasets are done, False otherwise.
         """
-        tmp_log = LogWrapper(_logger,
-                             f"check_sub_datasets_in_jobset-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}")
+        tmp_log = LogWrapper(_logger, f"check_sub_datasets_in_jobset-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}")
         # skip already checked
         if self.all_subscription_finished is not None:
             return self.all_subscription_finished
         # get consumers in the jobset
         jobs = self.task_buffer.getOriginalConsumers(self.job.jediTaskID, self.job.jobsetID, self.job.panda_id)
         checked_dataset = set()
         for job_spec in jobs:
@@ -77,16 +74,15 @@
                 # skip if already checked
                 if sub_dataset in checked_dataset:
                     continue
                 checked_dataset.add(sub_dataset)
                 # count the number of unfinished
                 not_finish = self.task_buffer.countFilesWithMap({"destinationDBlock": sub_dataset, "status": "unknown"})
                 if not_finish != 0:
-                    tmp_log.debug(
-                        f"related sub dataset {sub_dataset} from {job_spec.PandaID} has {not_finish} unfinished files")
+                    tmp_log.debug(f"related sub dataset {sub_dataset} from {job_spec.PandaID} has {not_finish} unfinished files")
                     self.all_subscription_finished = False
                     break
         if self.all_subscription_finished is None:
             tmp_log.debug("all related sub datasets are done")
             self.all_subscription_finished = True
         return self.all_subscription_finished
 
@@ -119,17 +115,15 @@
 
         Args:
             final_status_dataset (list): The final status dataset.
         """
         closer_plugin_class = panda_config.getPlugin("closer_plugins", self.job.VO)
         if closer_plugin_class is None and self.job.VO == "atlas":
             # use ATLAS plugin for ATLAS
-            from pandaserver.dataservice.closer_atlas_plugin import (
-                CloserAtlasPlugin,
-            )
+            from pandaserver.dataservice.closer_atlas_plugin import CloserAtlasPlugin
 
             closer_plugin_class = CloserAtlasPlugin
         if closer_plugin_class is not None:
             closer_plugin = closer_plugin_class(self.job, final_status_dataset, _logger)
             closer_plugin.execute()
 
     def start_activator(self, dataset):
@@ -137,47 +131,46 @@
         Start the activator
 
         Args:
             dataset: Dataset.
             final_status (str): Final status.
         """
         # start Activator
-        if not DataServiceUtils.is_sub_dataset(
-                dataset.name) and self.job.jobStatus == "finished" and self.job.prodSourceLabel != "panda" and self.job.processingType not in [
-            "merge", "unmerge"]:
+        if (
+            not DataServiceUtils.is_sub_dataset(dataset.name)
+            and self.job.jobStatus == "finished"
+            and (self.job.prodSourceLabel != "panda" or self.job.processingType not in ["merge", "unmerge"])
+        ):
             activator_thread = Activator(self.task_buffer, dataset)
             activator_thread.run()
 
     # main
     def run(self):
         """
         Main method to run the Closer class. It processes each destination dispatch block,
         updates the dataset status and finalizes pending jobs if necessary.
         """
         try:
-            tmp_log = LogWrapper(_logger,
-                                 f"run-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}-{self.panda_id}")
+            tmp_log = LogWrapper(_logger, f"run-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}-{self.panda_id}")
             tmp_log.debug(f"Start with job status: {self.job.jobStatus}")
             flag_complete = True
             final_status_dataset = []
 
             for destination_data_block in self.destination_data_blocks:
                 dataset_list = []
                 tmp_log.debug(f"start with destination dispatch block: {destination_data_block}")
 
                 # ignore task output datasets (tid) datasets
                 if DataServiceUtils.is_tid_dataset(destination_data_block):
                     tmp_log.debug(f"skip {destination_data_block}")
                     continue
 
                 # ignore HC datasets
-                if (DataServiceUtils.is_hammercloud_dataset(destination_data_block) or
-                        DataServiceUtils.is_user_gangarbt_dataset(destination_data_block)):
-                    if (not DataServiceUtils.is_sub_dataset(destination_data_block) and
-                            not DataServiceUtils.is_lib_dataset(destination_data_block)):
+                if DataServiceUtils.is_hammercloud_dataset(destination_data_block) or DataServiceUtils.is_user_gangarbt_dataset(destination_data_block):
+                    if not DataServiceUtils.is_sub_dataset(destination_data_block) and not DataServiceUtils.is_lib_dataset(destination_data_block):
                         tmp_log.debug(f"skip HC {destination_data_block}")
                         continue
 
                 # query dataset
                 if destination_data_block in self.dataset_map:
                     dataset = self.dataset_map[destination_data_block]
                 else:
@@ -193,16 +186,15 @@
                     tmp_log.debug(f"skip {destination_data_block} due to dataset status: {dataset.status}")
                     continue
 
                 dataset_list.append(dataset)
                 dataset_list.sort()
 
                 # count number of completed files
-                not_finish = self.task_buffer.countFilesWithMap(
-                    {"destinationDBlock": destination_data_block, "status": "unknown"})
+                not_finish = self.task_buffer.countFilesWithMap({"destinationDBlock": destination_data_block, "status": "unknown"})
                 if not_finish < 0:
                     tmp_log.error(f"Invalid dispatch block file count: {not_finish}")
                     flag_complete = False
                     continue
 
                 # check if completed
                 tmp_log.debug(f"Pending file count: {not_finish}")
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/closer_atlas_plugin.py` & `panda_server-0.3.3/pandaserver/dataservice/closer_atlas_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ATLAS plugin for closer
 """
 import sys
 
 from pandacommon.pandalogger.LogWrapper import LogWrapper
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.dataservice import DataServiceUtils
 
 
 # plugin for ATLAS closer
 class CloserAtlasPlugin:
     """
     A class used to represent the ATLAS closer plugin.
@@ -76,15 +76,15 @@
             for datasetSpec in self.datasets:
                 if not DataServiceUtils.is_sub_dataset(datasetSpec.name):
                     continue
                 if datasetSpec.status != "tobeclosed":
                     continue
                 try:
                     self.tmp_log.debug(f"immediate close {datasetSpec.name}")
-                    rucioAPI.closeDataset(datasetSpec.name)
+                    rucioAPI.close_dataset(datasetSpec.name)
                 except Exception:
                     errtype, errvalue = sys.exc_info()[:2]
                     self.tmp_log.warning(f"failed to close : {errtype} {errvalue}")
         except Exception:
             errtype, errvalue = sys.exc_info()[:2]
             self.tmp_log.warning(f"failed to execute : {errtype} {errvalue}")
         return True
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/dyn_data_distributer.py` & `panda_server-0.3.3/pandaserver/dataservice/dyn_data_distributer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import time
 import uuid
 from typing import Dict, List, Tuple
 
 from pandacommon.pandalogger.LogWrapper import LogWrapper
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.dataservice.DataServiceUtils import select_scope
 from pandaserver.taskbuffer import JobUtils
 
 # logger
 _logger = PandaLogger().getLogger("dyn_data_distributer")
 
 # files in datasets
@@ -207,15 +207,15 @@
         """
         tmp_log = LogWrapper(_logger,
                              f"get_list_dataset_replicas-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}")
         tmp_log.debug(f"get_list_dataset_replicas {dataset}")
 
         for attempt in range(max_attempts):
             tmp_log.debug(f"{attempt}/{max_attempts} listDatasetReplicas {dataset}")
-            status, replicas = rucioAPI.listDatasetReplicas(dataset)
+            status, replicas = rucioAPI.list_dataset_replicas(dataset)
             if status == 0:
                 tmp_log.debug(f"get_list_dataset_replicas->{str(replicas)}")
                 tmp_log.debug("end")
                 return True, replicas
             time.sleep(10)
 
         tmp_log.error(f"bad response for {dataset}")
@@ -240,15 +240,15 @@
 
         # response for failure
         res_for_failure = False, {}
 
         # get datasets in container
         for attempt in range(max_attempts):
             tmp_log.debug(f"{attempt}/{max_attempts} listDatasetsInContainer {container}")
-            datasets, out = rucioAPI.listDatasetsInContainer(container)
+            datasets, out = rucioAPI.list_datasets_in_container(container)
             if datasets is not None:
                 break
             time.sleep(60)
 
         if datasets is None:
             tmp_log.error(out)
             tmp_log.error(f"bad DDM response for {container}")
@@ -290,15 +290,15 @@
 
         # loop over all datasets
         for dataset_name in dataset_map:
             # get file list
             for attempt in range(max_attempts):
                 try:
                     tmp_log.debug(f"{attempt}/{max_attempts} listFilesInDataset {dataset_name}")
-                    file_items, out = rucioAPI.listFilesInDataset(dataset_name)
+                    file_items, out = rucioAPI.list_files_in_dataset(dataset_name)
                     status = True
                     break
                 except Exception:
                     status = False
                     err_type, err_value = sys.exc_info()[:2]
                     out = f"{err_type} {err_value}"
                     time.sleep(60)
@@ -350,15 +350,15 @@
         # get files in datasets
         global g_files_in_ds_map
         if dataset_name not in g_files_in_ds_map:
             # get file list
             for attempt in range(max_attempts):
                 try:
                     tmp_log.debug(f"{attempt}/{max_attempts} listFilesInDataset {dataset_name}")
-                    file_items, out = rucioAPI.listFilesInDataset(dataset_name)
+                    file_items, out = rucioAPI.list_files_in_dataset(dataset_name)
                     status = True
                     break
                 except Exception:
                     status = False
                     err_type, err_value = sys.exc_info()[:2]
                     out = f"{err_type} {err_value}"
                     time.sleep(60)
@@ -426,49 +426,49 @@
             tmp_locations = new_locations
             tmp_key = tuple(tmp_locations)
             files_map.setdefault(tmp_key, [])
             # append file
             files_map[tmp_key].append(tmp_file)
 
         # get nfiles per dataset
-        n_files_per_dataset = divmod(len(files), n_sites)
-        if n_files_per_dataset[0] == 0:
-            n_files_per_dataset[0] = 1
+        n_files_per_dataset, _ = divmod(len(files), n_sites)
+        if n_files_per_dataset == 0:
+            n_files_per_dataset = 1
         max_files_per_dataset = 1000
-        if n_files_per_dataset[0] >= max_files_per_dataset:
-            n_files_per_dataset[0] = max_files_per_dataset
+        if n_files_per_dataset >= max_files_per_dataset:
+            n_files_per_dataset = max_files_per_dataset
 
         # register new datasets
         dataset_names = []
         tmp_index = 1
         for tmp_locations, tmp_files in files_map.items():
             tmp_sub_index = 0
             while tmp_sub_index < len(tmp_files):
                 tmp_dataset_name = container_name[:-1] + "_%04d" % tmp_index
                 tmp_ret = self.register_dataset_with_location(
                     tmp_dataset_name,
-                    tmp_files[tmp_sub_index: tmp_sub_index + n_files_per_dataset[0]],
+                    tmp_files[tmp_sub_index: tmp_sub_index + n_files_per_dataset],
                     tmp_locations,
                     owner=None,
                 )
                 # failed
                 if not tmp_ret:
                     tmp_logger.error(f"failed to register {tmp_dataset_name}")
                     tmp_logger.debug("end")
                     return False
                 # append dataset
                 dataset_names.append(tmp_dataset_name)
                 tmp_index += 1
-                tmp_sub_index += n_files_per_dataset[0]
+                tmp_sub_index += n_files_per_dataset
 
         # register container
         for attempt in range(max_attempts):
             try:
                 tmp_logger.debug(f"{attempt}/{max_attempts} registerContainer {container_name}")
-                status = rucioAPI.registerContainer(container_name, dataset_names)
+                status = rucioAPI.register_container(container_name, dataset_names)
                 out = "OK"
                 break
             except Exception:
                 status = False
                 err_type, err_value = sys.exc_info()[:2]
                 out = f"{err_type} {err_value}"
                 time.sleep(10)
@@ -515,15 +515,15 @@
             file_sizes.append(int(tmp_file["filesize"]))
             checksums.append(tmp_file["checksum"])
 
         # register new dataset
         for attempt in range(max_attempts):
             try:
                 tmp_logger.debug(f"{attempt}/{max_attempts} registerNewDataset {dataset_name} len={len(files)}")
-                out = rucioAPI.registerDataset(dataset_name, lfns, guids, file_sizes, checksums, lifetime=14)
+                out = rucioAPI.register_dataset(dataset_name, lfns, guids, file_sizes, checksums, lifetime=14)
                 tmp_logger.debug(out)
                 break
             except Exception:
                 err_type, err_value = sys.exc_info()[:2]
                 tmp_logger.error(f"{err_type} {err_value}")
                 if attempt + 1 == max_attempts:
                     tmp_logger.error(f"failed to register {dataset_name} in rucio")
@@ -531,15 +531,15 @@
                     return res_for_failure
                 time.sleep(10)
 
         # freeze dataset
         for attempt in range(max_attempts):
             tmp_logger.debug(f"{attempt}/{max_attempts} freezeDataset {dataset_name}")
             try:
-                rucioAPI.closeDataset(dataset_name)
+                rucioAPI.close_dataset(dataset_name)
                 status = True
             except Exception:
                 err_type, err_value = sys.exc_info()[:2]
                 out = f"failed to freeze : {err_type} {err_value}"
                 status = False
             if not status:
                 time.sleep(10)
@@ -552,15 +552,15 @@
             return res_for_failure
 
         # register locations
         for tmp_location in locations:
             for attempt in range(max_attempts):
                 try:
                     tmp_logger.debug(f"{attempt}/{max_attempts} registerDatasetLocation {dataset_name} {tmp_location}")
-                    out = rucioAPI.registerDatasetLocation(dataset_name, [tmp_location], 14, owner)
+                    out = rucioAPI.register_dataset_location(dataset_name, [tmp_location], 14, owner)
                     tmp_logger.debug(out)
                     status = True
                     break
 
                 except Exception:
                     status = False
                     err_type, err_value = sys.exc_info()[:2]
@@ -662,15 +662,15 @@
         res_for_failure = (False, {})
         res_for_fatal = (False, {"isFatal": True}, [])
 
         # get size of datasets
         for attempt in range(max_attempts):
             tmp_logger.debug(f"{attempt}/{max_attempts} listDatasetsByGUIDs GUIDs={str(guids)}")
             try:
-                out = rucioAPI.listDatasetsByGUIDs(guids)
+                out = rucioAPI.list_datasets_by_guids(guids)
                 status = True
                 break
             except Exception:
                 err_type, err_value = sys.exc_info()[:2]
                 out = f"failed to get datasets with GUIDs : {err_type} {err_value}"
                 status = False
                 time.sleep(10)
@@ -693,28 +693,25 @@
         if not status:
             return res_for_failure
 
         tmp_logger.debug("end")
         return True, ret_map
 
     def convert_evt_run_to_datasets(self, event_run_list: List, dataset_type: str, stream_name: str, dataset_filters: List,
-                                    ami_tag: str, user: str,
-                                    run_evt_guid_map: Dict, ei_api: object) -> Tuple[bool, Dict, List]:
+                                    ami_tag: str, run_evt_guid_map: Dict) -> Tuple[bool, Dict, List]:
         """
         Convert event/run list to datasets.
 
         Args:
             event_run_list (list): The list of run events.
             dataset_type (str): The type of the dataset.
             stream_name (str): The name of the stream.
             dataset_filters (list): The list of dataset filters.
             ami_tag (str): The AMI tag.
-            user (str): The user.
             run_evt_guid_map (dict): The map of run events to GUIDs.
-            ei_api (str): The EventIndex API.
 
         Returns:
             tuple: A tuple containing the status (bool), the result (dict or str), and the list of all files.
         """
         tmp_logger = LogWrapper(_logger,
                              f"convert_evt_run_to_datasets-{datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None).isoformat('/')}")
         tmp_logger.debug(f"convert_evt_run_to_datasets type={dataset_type} stream={stream_name} dsPatt={str(dataset_filters)} amitag={ami_tag}")
@@ -726,32 +723,30 @@
         # import event lookup client
         if run_evt_guid_map == {}:
             if len(event_run_list) == 0:
                 tmp_logger.error("Empty list for run and events was provided")
                 tmp_logger.debug("end")
                 return failed_ret
             # Hadoop EI
-            from .eventLookupClientEI import eventLookupClientEI
+            from .event_lookup_client_ei import EventLookupClientEI
 
-            event_lookup_if = eventLookupClientEI()
+            event_lookup_if = EventLookupClientEI()
             # loop over all events
             n_events_per_loop = 500
             i_events_total = 0
             while i_events_total < len(event_run_list):
                 tmp_event_run_list = event_run_list[i_events_total: i_events_total + n_events_per_loop]
                 tmp_logger.debug(f"EI lookup for {i_events_total}/{len(event_run_list)}")
                 i_events_total += n_events_per_loop
                 reg_start = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
-                guid_list_elssi, tmp_com, tmp_out, tmp_err = event_lookup_if.doLookup(
+                guid_list_elssi, tmp_com, tmp_out, tmp_err = event_lookup_if.do_lookup(
                     tmp_event_run_list,
                     stream=stream_name,
                     tokens=stream_ref,
-                    amitag=ami_tag,
-                    user=user,
-                    ei_api=ei_api,
+                    ami_tag=ami_tag,
                 )
                 reg_time = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None) - reg_start
                 tmp_logger.debug(f"EI command: {tmp_com}")
                 tmp_logger.debug(f"took {reg_time.seconds}.{reg_time.microseconds / 1000:03f} sec for {len(tmp_event_run_list)} events")
                 # failed
                 if tmp_err not in [None, ""] or len(guid_list_elssi) == 0:
                     tmp_logger.debug(tmp_com)
```

### Comparing `panda_server-0.3.1/pandaserver/dataservice/finisher.py` & `panda_server-0.3.3/pandaserver/dataservice/finisher.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/dataservice/forkSetupper.py` & `panda_server-0.3.3/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda_server-0.3.3/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/jobdispatcher/JobDispatcher.py` & `panda_server-0.3.3/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import threading
 import time
 import traceback
 from threading import Lock
 
 from pandacommon.pandalogger.LogWrapper import LogWrapper
 from pandacommon.pandalogger.PandaLogger import PandaLogger
+
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
 from pandaserver.dataservice.AdderGen import AdderGen
 from pandaserver.jobdispatcher import DispatcherUtils, Protocol
 from pandaserver.proxycache import panda_proxy_cache
 from pandaserver.srvcore import CoreUtils
 from pandaserver.taskbuffer import EventServiceUtils
@@ -793,17 +794,17 @@
         return response.encode(True)
 
     # get active job attribute
     def getActiveJobAttributes(self, pandaID, attrs):
         return self.taskBuffer.getActiveJobAttributes(pandaID, attrs)
 
     # update job status
-    def updateWorkerPilotStatus(self, workerID, harvesterID, status, timeout, accept_json):
+    def updateWorkerPilotStatus(self, workerID, harvesterID, status, timeout, accept_json, node_id):
         tmp_wrapper = _TimedMethod(self.taskBuffer.updateWorkerPilotStatus, timeout)
-        tmp_wrapper.run(workerID, harvesterID, status)
+        tmp_wrapper.run(workerID, harvesterID, status, node_id)
 
         # make response
         if tmp_wrapper.result == Protocol.TimeOutToken:
             response = Protocol.Response(Protocol.SC_TimeOut)
         else:
             if tmp_wrapper.result:  # success
                 response = Protocol.Response(Protocol.SC_Success)
@@ -1649,18 +1650,18 @@
 
     accept_json = req.acceptJson()
     # retrieve the commands
     return jobDispatcher.getResourceTypes(timeout, accept_json)
 
 
 # update the status of a worker according to the pilot
-def updateWorkerPilotStatus(req, site, workerID, harvesterID, status, timeout=60):
+def updateWorkerPilotStatus(req, site, workerID, harvesterID, status, timeout=60, node_id=None):
     tmp_log = LogWrapper(
         _logger,
-        f"updateWorkerPilotStatus workerID={workerID} harvesterID={harvesterID} status={status} PID={os.getpid()}",
+        f"updateWorkerPilotStatus workerID={workerID} harvesterID={harvesterID} status={status} nodeID={node_id} PID={os.getpid()}",
     )
     tmp_log.debug("start")
 
     # validate the pilot permissions
     tmp_stat, tmp_out = checkPilotPermission(req, site)
     if not tmp_stat:
         tmp_log.error(f"failed with {tmp_out}")
@@ -1671,15 +1672,15 @@
     if status not in valid_states:
         message = f"Invalid worker state. The worker state has to be in {valid_states}"
         tmp_log.debug(message)
         return message
 
     accept_json = req.acceptJson()
 
-    return jobDispatcher.updateWorkerPilotStatus(workerID, harvesterID, status, timeout, accept_json)
+    return jobDispatcher.updateWorkerPilotStatus(workerID, harvesterID, status, timeout, accept_json, node_id)
 
 
 # get max workerID
 def get_max_worker_id(req, harvester_id):
     return jobDispatcher.get_max_worker_id(harvester_id)
```

### Comparing `panda_server-0.3.1/pandaserver/jobdispatcher/Watcher.py` & `panda_server-0.3.3/pandaserver/jobdispatcher/Watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,15 @@
                                 self.logger.debug("apply_retrial_rules 2 is back")
                         except IndexError:
                             pass
                         except Exception as e:
                             self.logger.error(f"apply_retrial_rules 2 excepted and needs to be investigated ({e}): {traceback.format_exc()}")
 
                         cThr = Closer(self.taskBuffer, destDBList, job)
-                        cThr.start()
-                        cThr.join()
+                        cThr.run()
                     self.logger.debug("done")
                     return
                 # single action
                 if self.single:
                     return
                 # sleep
                 time.sleep(60 * self.sleepTime)
```

### Comparing `panda_server-0.3.1/pandaserver/proxycache/panda_proxy_cache.py` & `panda_server-0.3.3/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/server/panda.py` & `panda_server-0.3.3/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/srvcore/CoreUtils.py` & `panda_server-0.3.3/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/srvcore/MailUtils.py` & `panda_server-0.3.3/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/srvcore/allowed_methods.py` & `panda_server-0.3.3/pandaserver/srvcore/allowed_methods.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/srvcore/oidc_utils.py` & `panda_server-0.3.3/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/srvcore/panda_request.py` & `panda_server-0.3.3/pandaserver/srvcore/panda_request.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/srvcore/srv_msg_utils.py` & `panda_server-0.3.3/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/CloudSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/ConBridge.py` & `panda_server-0.3.3/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/DBProxyPool.py` & `panda_server-0.3.3/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/DatasetSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/DdmSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/ErrorCode.py` & `panda_server-0.3.3/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/EventServiceUtils.py` & `panda_server-0.3.3/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/FileSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/GlobalShares.py` & `panda_server-0.3.3/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/Initializer.py` & `panda_server-0.3.3/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/JobUtils.py` & `panda_server-0.3.3/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/NucleusSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/OraDBProxy.py` & `panda_server-0.3.3/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -3165,48 +3165,50 @@
                     time.sleep(random.randint(3, 10))
                     continue
                 type, value, traceBack = sys.exc_info()
                 _logger.error(f"updateJob : {type} {value}")
                 return False
 
     # update the worker status as seen by the pilot
-    def updateWorkerPilotStatus(self, workerID, harvesterID, status):
+    def updateWorkerPilotStatus(self, workerID, harvesterID, status, node_id):
         comment = " /* DBProxy.updateWorkerPilotStatus */"
         method_name = comment.split(" ")[-2].split(".")[-1]
         tmp_logger = LogWrapper(
             _logger,
             method_name + f"< harvesterID={harvesterID} workerID={workerID} >",
         )
 
         timestamp_utc = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
         var_map = {
             ":status": status,
             ":harvesterID": harvesterID,
             ":workerID": workerID,
+            ":nodeID": node_id,
         }
-        sql = "UPDATE ATLAS_PANDA.harvester_workers SET pilotStatus=:status "
+        sql = "UPDATE ATLAS_PANDA.harvester_workers SET pilotStatus=:status,nodeID=:nodeID "
 
-        tmp_logger.debug(f"Updating to status={status} at {timestamp_utc}")
+        tmp_logger.debug(f"Updating to status={status} nodeID={node_id} at {timestamp_utc}")
 
         # add the start or end time
         if status == "started":
             sql += ", pilotStartTime=:now "
             var_map[":now"] = timestamp_utc
         elif status == "finished":
             sql += ", pilotEndTime=:now "
             var_map[":now"] = timestamp_utc
 
         sql += "WHERE workerID=:workerID AND harvesterID=:harvesterID "
 
         try:
             self.conn.begin()
             self.cur.execute(sql + comment, var_map)
+            retD = self.cur.rowcount
             if not self._commit():
                 raise RuntimeError("Commit error")
-            tmp_logger.debug("Updated successfully")
+            tmp_logger.debug(f"Updated successfully with {retD}")
             return True
 
         except Exception:
             # roll back
             self._rollback(True)
             err_type, err_value = sys.exc_info()[:2]
             tmp_logger.error(f"updateWorkerPilotStatus : {err_type} {err_value}")
@@ -19411,15 +19413,15 @@
         tmp_logger.debug("start")
 
         # SQL to extract the error definitions
         sql = """
         SELECT re.retryerror_id, re.errorsource, re.errorcode, re.errorDiag, re.parameters, re.architecture, re.release, re.workqueue_id, ra.retry_action, re.active, ra.active
         FROM ATLAS_PANDA.RETRYERRORS re, ATLAS_PANDA.RETRYACTIONS ra
         WHERE re.retryaction=ra.retryaction_id
-        AND (CURRENT_TIMESTAMP > re.expiration_date or re.expiration_date IS NULL)
+        AND (CURRENT_TIMESTAMP < re.expiration_date or re.expiration_date IS NULL)
         """
         self.cur.execute(sql + comment, {})
         definitions = self.cur.fetchall()  # example of output: [('pilotErrorCode', 1, None, None, None, None, 'no_retry', 'Y', 'Y'),...]
 
         # commit
         if not self._commit():
             raise RuntimeError("Commit error")
```

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/PickleFileSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/PickleFileSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/PickleJobSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/PickleJobSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/PrioUtil.py` & `panda_server-0.3.3/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/ProcessGroups.py` & `panda_server-0.3.3/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/ResourceSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/SQLDumper.py` & `panda_server-0.3.3/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/SQLManager.py` & `panda_server-0.3.3/pandaserver/taskbuffer/SQLManager.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/SiteSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/TaskBuffer.py` & `panda_server-0.3.3/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,19 +769,19 @@
             if tmpS and secrets:
                 ret = {"command": ret, "secrets": secrets}
         # release proxy
         self.proxyPool.putProxy(proxy)
         return ret
 
     # update worker status by the pilot
-    def updateWorkerPilotStatus(self, workerID, harvesterID, status):
+    def updateWorkerPilotStatus(self, workerID, harvesterID, status, node_id):
         # get DB proxy
         proxy = self.proxyPool.getProxy()
         # update DB and buffer
-        ret = proxy.updateWorkerPilotStatus(workerID, harvesterID, status)
+        ret = proxy.updateWorkerPilotStatus(workerID, harvesterID, status, node_id)
         # release proxy
         self.proxyPool.putProxy(proxy)
         return ret
 
     # finalize pending analysis jobs
     def finalizePendingJobs(self, prodUserName, jobDefinitionID, waitLock=False):
         # get DB proxy
```

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda_server-0.3.3/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/Utils.py` & `panda_server-0.3.3/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/WorkerSpec.py` & `panda_server-0.3.3/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/WrappedCursor.py` & `panda_server-0.3.3/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/WrappedPickle.py` & `panda_server-0.3.3/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/retryModule.py` & `panda_server-0.3.3/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/task_split_rules.py` & `panda_server-0.3.3/pandaserver/taskbuffer/task_split_rules.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,21 +122,19 @@
     ret = {}
     if is_sub_rule:
         rule_separator = "|"
         key_value_separator = ":"
     else:
         rule_separator = ","
         key_value_separator = "="
-    if is_sub_rule:
-        for tmp_name in rule_names:
-            ret[tmp_name] = None
     for tmp_rule in split_rules.split(rule_separator):
         for tmp_name in rule_names:
-            if tmp_rule.startswith(tmp_name + key_value_separator):
+            if tmp_name in split_rule_dict and tmp_rule.startswith(split_rule_dict[tmp_name] + key_value_separator):
                 ret[tmp_name] = tmp_rule.split(key_value_separator)[-1]
+                break
     for tmp_name in rule_names:
         if tmp_name not in ret:
             ret[tmp_name] = None
     return ret
 
 
 # replace a rule
@@ -145,26 +143,55 @@
     Replace a rule in the split rule string
     :param split_rules: comma separated string
     :param rule_name: rule name
     :param rule_value: rule value
     :param is_sub_rule: bool to indicate if the rule is a sub-rule
     :return: string of split rules
     """
+    if rule_name not in split_rule_dict:
+        return split_rules
     if split_rules is None:
         split_rules = ""
     if is_sub_rule:
         rule_separator = "|"
         key_value_separator = ":"
     else:
         rule_separator = ","
         key_value_separator = "="
     tmp_str = ""
     for tmp_rule in split_rules.split(rule_separator):
-        if tmp_rule.startswith(rule_name + key_value_separator):
+        if tmp_rule.startswith(split_rule_dict[rule_name] + key_value_separator):
             continue
         if tmp_str != "":
             tmp_str += rule_separator
         tmp_str += tmp_rule
     if tmp_str != "":
         tmp_str += rule_separator
-    tmp_str += rule_name + key_value_separator + str(rule_value)
+    tmp_str += split_rule_dict[rule_name] + key_value_separator + str(rule_value)
+    return tmp_str
+
+
+# remove a rule
+def remove_rule(split_rules, rule_token, is_sub_rule=False):
+    """
+    Remove a rule from the split rule string
+    :param split_rules: comma separated string
+    :param rule_token: rule token
+    :param is_sub_rule: bool to indicate if the rule is a sub-rule
+    :return: string of split rules
+    """
+    if split_rules is None:
+        split_rules = ""
+    if is_sub_rule:
+        rule_separator = "|"
+        key_value_separator = ":"
+    else:
+        rule_separator = ","
+        key_value_separator = "="
+    tmp_str = ""
+    for tmp_rule in split_rules.split(rule_separator):
+        if tmp_rule.startswith(rule_token + key_value_separator):
+            continue
+        if tmp_str != "":
+            tmp_str += rule_separator
+        tmp_str += tmp_rule
     return tmp_str
```

### Comparing `panda_server-0.3.1/pandaserver/taskbuffer/workflow_processor.py` & `panda_server-0.3.3/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/SchemaChecker.py` & `panda_server-0.3.3/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/banUser.py` & `panda_server-0.3.3/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/boostPrio.py` & `panda_server-0.3.3/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/boostUser.py` & `panda_server-0.3.3/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/callbackDDM.py` & `panda_server-0.3.3/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/daod_on_demand.py` & `panda_server-0.3.3/pandaserver/test/daod_on_demand.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/finishJob.py` & `panda_server-0.3.3/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/getJobs.py` & `panda_server-0.3.3/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/killJob.py` & `panda_server-0.3.3/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/killJobLowPrio.py` & `panda_server-0.3.3/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/killJobsInTask.py` & `panda_server-0.3.3/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/killProdJobs.py` & `panda_server-0.3.3/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/killTask.py` & `panda_server-0.3.3/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/killUser.py` & `panda_server-0.3.3/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/reassignSite.py` & `panda_server-0.3.3/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/reassignTask.py` & `panda_server-0.3.3/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/reassignWaiting.py` & `panda_server-0.3.3/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/reloadInputDS.py` & `panda_server-0.3.3/pandaserver/test/reloadInputDS.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 from pandaserver.config import panda_config
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.taskbuffer.TaskBuffer import taskBuffer
 from pandaserver.userinterface import Client
 from rucio.client import Client as RucioClient
 from rucio.common.exception import DataIdentifierNotFound
 
 taskBuffer.init(panda_config.dbhost, panda_config.dbpasswd, nDBConnection=1)
```

### Comparing `panda_server-0.3.1/pandaserver/test/sendCommandToJob.py` & `panda_server-0.3.3/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/setDebugMode.py` & `panda_server-0.3.3/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/setPriority.py` & `panda_server-0.3.3/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testEvgen.py` & `panda_server-0.3.3/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testEvgen17.py` & `panda_server-0.3.3/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testG4sim.py` & `panda_server-0.3.3/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testG4sim17.py` & `panda_server-0.3.3/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda_server-0.3.3/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testGlobalShares.py` & `panda_server-0.3.3/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testJobFlowATLAS.py` & `panda_server-0.3.3/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testReco.py` & `panda_server-0.3.3/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testSimulReco14.py` & `panda_server-0.3.3/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testSiteMap.py` & `panda_server-0.3.3/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/testutils.py` & `panda_server-0.3.3/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda_server-0.3.3/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/lsst/lsstSubmit.py` & `panda_server-0.3.3/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda_server-0.3.3/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh` & `panda_server-0.3.3/pandaserver/test/lsst/prepare-client-tarball-from-bigpanda-server.sh`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/userinterface/Client.py` & `panda_server-0.3.3/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/userinterface/UserIF.py` & `panda_server-0.3.3/pandaserver/userinterface/UserIF.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pandacommon.pandalogger.LogWrapper import LogWrapper
 from pandacommon.pandalogger.PandaLogger import PandaLogger
 
 import pandaserver.jobdispatcher.Protocol as Protocol
 import pandaserver.taskbuffer.ProcessGroups
 from pandaserver.brokerage.SiteMapper import SiteMapper
 from pandaserver.config import panda_config
-from pandaserver.dataservice.DDM import rucioAPI
+from pandaserver.dataservice.ddm import rucioAPI
 from pandaserver.srvcore import CoreUtils
 from pandaserver.srvcore.CoreUtils import clean_user_id, resolve_bool
 from pandaserver.taskbuffer import JobUtils, PrioUtil
 from pandaserver.taskbuffer.WrappedPickle import WrappedPickle
 
 try:
     import idds.common.constants
```

### Comparing `panda_server-0.3.1/pandaserver/workflow/pcwl_test.py` & `panda_server-0.3.3/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/pcwl_utils.py` & `panda_server-0.3.3/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/psnakemake_container.json` & `panda_server-0.3.3/pandaserver/workflow/psnakemake_container.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/psnakemake_task.json` & `panda_server-0.3.3/pandaserver/workflow/psnakemake_task.json`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/psnakemake_test.py` & `panda_server-0.3.3/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/workflow_utils.py` & `panda_server-0.3.3/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/snakeparser/extensions.py` & `panda_server-0.3.3/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/snakeparser/log.py` & `panda_server-0.3.3/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/snakeparser/parser.py` & `panda_server-0.3.3/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pandaserver/workflow/snakeparser/utils.py` & `panda_server-0.3.3/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/conda_meta.yaml.template` & `panda_server-0.3.3/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda_server-0.3.3/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files 10% similar despite different names*

```diff
@@ -12,26 +12,30 @@
 
 <IfModule prefork.c>
 StartServers         ${PANDA_SERVER_CONF_MIN_WORKERS}
 MinSpareServers      ${PANDA_SERVER_CONF_MIN_WORKERS}
 ServerLimit          ${PANDA_SERVER_CONF_MAX_WORKERS}
 MaxSpareServers      ${PANDA_SERVER_CONF_MAX_WORKERS}
 MaxClients           ${PANDA_SERVER_CONF_MAX_WORKERS}
-MaxRequestsPerChild  2000
+MaxRequestsPerChild  ${PANDA_SERVER_CONF_MAX_CONNECTIONS}
+ThreadsPerChild      ${PANDA_SERVER_CONF_THREADS_PER_CHILD}
 </IfModule>
 
 <IfModule mpm_event_module>
 StartServers           ${PANDA_SERVER_CONF_MIN_WORKERS}
 MinSpareThreads        ${PANDA_SERVER_CONF_MIN_WORKERS}
 ServerLimit            ${PANDA_SERVER_CONF_MAX_WORKERS}
 MaxSpareThreads        ${PANDA_SERVER_CONF_MAX_WORKERS}
 MaxRequestWorkers      ${PANDA_SERVER_CONF_MAX_WORKERS}
-MaxConnectionsPerChild 2000
+MaxConnectionsPerChild ${PANDA_SERVER_CONF_MAX_CONNECTIONS}
+ThreadsPerChild        ${PANDA_SERVER_CONF_THREADS_PER_CHILD}
 </IfModule>
 
+ListenBackLog ${PANDA_SERVER_CONF_MAX_BACKLOG}
+
 ServerName ${PANDA_SERVER_CONF_SERVERNAME}
 
 DocumentRoot "@@install_purelib@@/pandaserver"
 
 <Files ~ "\.(py|pyc|conf)$">
     Order allow,deny
     Deny from all
@@ -74,15 +78,15 @@
     Order allow,deny
     Allow from all
     Header set Content-Encoding gzip
 </Directory>
 
 <IfModule mod_wsgi.c>
    WSGIPythonHome /opt/panda
-   WSGIDaemonProcess pandasrv_daemon processes=${PANDA_SERVER_CONF_NUM_WSGI} threads=1 home=/home/atlpan
+   WSGIDaemonProcess pandasrv_daemon processes=${PANDA_SERVER_CONF_NUM_WSGI} threads=${PANDA_SERVER_CONF_NUM_WSGI_THREAD} home=/home/atlpan
    WSGIProcessGroup pandasrv_daemon
    WSGIApplicationGroup %{GLOBAL}
    WSGIScriptAliasMatch ^/server/panda/(.+)$ @@install_purelib@@/pandaserver/server/panda.py
    WSGISocketPrefix /run/httpd/wsgisocks/wsgi
    WSGIPassAuthorization On
 </IfModule>
```

### Comparing `panda_server-0.3.1/templates/panda_server-httpd.conf.rpmnew.template` & `panda_server-0.3.3/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/panda_server.cfg.rpmnew.template` & `panda_server-0.3.3/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/bin/panda_server-makeSlsXml.exe.template` & `panda_server-0.3.3/templates/bin/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/bin/panda_server-vomsrenew.exe.template` & `panda_server-0.3.3/templates/bin/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/init.d/panda_daemon.exe.template` & `panda_server-0.3.3/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/init.d/panda_httpd.exe.template` & `panda_server-0.3.3/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/init.d/panda_server.exe.template` & `panda_server-0.3.3/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/logrotate.d/panda_server.logrotate.template` & `panda_server-0.3.3/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda_server-0.3.3/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files 14% similar despite different names*

```diff
@@ -57,27 +57,47 @@
 # server name
 if [[ -z "${PANDA_SERVER_CONF_SERVERNAME}" ]]; then
   export PANDA_SERVER_CONF_SERVERNAME=pandaserver.cern.ch
 fi
 
 # min number of workers
 if [[ -z "${PANDA_SERVER_CONF_MIN_WORKERS}" ]]; then
-  export PANDA_SERVER_CONF_MIN_WORKERS=25
+  export PANDA_SERVER_CONF_MIN_WORKERS=32
 fi
 
 # max number of workers
 if [[ -z "${PANDA_SERVER_CONF_MAX_WORKERS}" ]]; then
   export PANDA_SERVER_CONF_MAX_WORKERS=512
 fi
 
 # max number of WSGI daemons
 if [[ -z "${PANDA_SERVER_CONF_NUM_WSGI}" ]]; then
-  export PANDA_SERVER_CONF_NUM_WSGI=12
+  export PANDA_SERVER_CONF_NUM_WSGI=32
+fi
+
+# max number of WSGI threads
+if [[ -z "${PANDA_SERVER_CONF_NUM_WSGI_THREAD}" ]]; then
+  export PANDA_SERVER_CONF_NUM_WSGI_THREAD=1
+fi
+
+# max number of WSGI daemons
+if [[ -z "${PANDA_SERVER_CONF_MAX_BACKLOG}" ]]; then
+  export PANDA_SERVER_CONF_MAX_BACKLOG=511
 fi
 
 # port
 if [[ -z "${PANDA_SERVER_CONF_PORT}" ]]; then
   export PANDA_SERVER_CONF_PORT=25080
 fi
 if [[ -z "${PANDA_SERVER_CONF_PORT_SSL}" ]]; then
   export PANDA_SERVER_CONF_PORT_SSL=25443
 fi
+
+# max connections per child
+if [[ -z "${PANDA_SERVER_CONF_MAX_CONNECTIONS}" ]]; then
+  export PANDA_SERVER_CONF_MAX_CONNECTIONS=2000
+fi
+
+# threads per child
+if [[ -z "${PANDA_SERVER_CONF_THREADS_PER_CHILD}" ]]; then
+  export PANDA_SERVER_CONF_THREADS_PER_CHILD=25
+fi
```

### Comparing `panda_server-0.3.1/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda_server-0.3.3/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/LICENSE.txt` & `panda_server-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/pyproject.toml` & `panda_server-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panda_server-0.3.1/PKG-INFO` & `panda_server-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panda-server
-Version: 0.3.1
+Version: 0.3.3
 Summary: PanDA Server Package
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <panda-support@cern.ch>
 License: Apache-2.0
 License-File: LICENSE.txt
 Requires-Python: >=3.8
 Requires-Dist: cwl-utils>=0.13
```

