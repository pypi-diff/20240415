# Comparing `tmp/ressimpy-2.0.9.tar.gz` & `tmp/ressimpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-2.0.9.tar", max compression
+gzip compressed data, was "ressimpy-2.1.0.tar", max compression
```

## Comparing `ressimpy-2.0.9.tar` & `ressimpy-2.1.0.tar`

### file list

```diff
@@ -1,190 +1,194 @@
--rw-r--r--   0        0        0     9156 2024-03-05 13:51:34.234753 ressimpy-2.0.9/LICENSE.MD
--rw-r--r--   0        0        0     5660 2024-03-05 13:51:34.234753 ressimpy-2.0.9/README.md
--rw-r--r--   0        0        0      504 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0     8573 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1419 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1908 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     3926 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/DataObjectMixin.py
--rw-r--r--   0        0        0     4109 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0      358 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/FluidTypeEnums.py
--rw-r--r--   0        0        0      369 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/FrequencyEnum.py
--rw-r--r--   0        0        0      168 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      214 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/OutputType.py
--rw-r--r--   0        0        0      282 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/PenetrationDirectionEnum.py
--rw-r--r--   0        0        0      253 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/TimeSteppingMethodEnum.py
--rw-r--r--   0        0        0      507 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0      377 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/WellTypeEnum.py
--rw-r--r--   0        0        0       62 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      506 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     8911 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/File.py
--rw-r--r--   0        0        0     2257 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/FileBase.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/FileOperations/__init__.py
--rw-r--r--   0        0        0    22606 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/FileOperations/file_operations.py
--rw-r--r--   0        0        0      413 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     2631 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Grid.py
--rw-r--r--   0        0        0      393 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Grids.py
--rw-r--r--   0        0        0      470 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     3147 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0      588 2024-03-05 13:51:34.234753 ressimpy-2.0.9/ResSimpy/Network.py
--rw-r--r--   0        0        0      545 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    23652 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0    21550 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    17761 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     1718 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     4917 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     6436 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     6543 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     4071 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProc.py
--rw-r--r--   0        0        0     1124 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
--rw-r--r--   0        0        0     2084 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
--rw-r--r--   0        0        0     6763 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
--rw-r--r--   0        0        0     6510 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     6647 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     2191 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
--rw-r--r--   0        0        0     2780 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     5892 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     4535 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     5815 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0      329 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     8313 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    14155 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0    10788 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    32379 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     6211 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    13247 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    30699 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     2718 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    19602 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0     9467 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     9032 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0    15015 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
--rw-r--r--   0        0        0     6112 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0    11098 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     8247 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0      781 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellList.py
--rw-r--r--   0        0        0     2858 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellMod.py
--rw-r--r--   0        0        0    14838 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0       67 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0       77 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0     3396 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      273 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0      106 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0     3374 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     3345 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0       43 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     3418 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0       47 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      757 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1210 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1368 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      170 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1159 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2658 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      795 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0     5130 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.238753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2547 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1579 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      896 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     4957 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      880 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3082 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4492 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      306 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      243 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      902 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0    17025 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     3287 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     3560 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0    12256 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     3337 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     3678 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    35694 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0    16873 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusSolverParameters.py
--rw-r--r--   0        0        0     3376 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     3371 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    23059 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0      404 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    12453 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0      115 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0    22655 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14101 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    16194 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     8573 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     7107 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    23162 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     4132 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_load_well_list.py
--rw-r--r--   0        0        0     2046 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     7768 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     5422 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    18379 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0     9027 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      744 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Node.py
--rw-r--r--   0        0        0      918 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      456 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      398 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Nodes.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     2368 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
--rw-r--r--   0        0        0     2812 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/__init__.py
--rw-r--r--   0        0        0      199 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Enums/__init__.py
--rw-r--r--   0        0        0      525 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/Model_Parts/__init__.py
--rw-r--r--   0        0        0     2892 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
--rw-r--r--   0        0        0    10767 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
--rw-r--r--   0        0        0      462 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimWells.py
--rw-r--r--   0        0        0        0 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OpenGoSim/__init__.py
--rw-r--r--   0        0        0     2382 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      442 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/PVT.py
--rw-r--r--   0        0        0      467 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     3389 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0      473 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Rock.py
--rw-r--r--   0        0        0      493 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Separator.py
--rw-r--r--   0        0        0     4356 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Simulator.py
--rw-r--r--   0        0        0      407 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/SolverParameter.py
--rw-r--r--   0        0        0      671 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/SolverParameters.py
--rw-r--r--   0        0        0     1484 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Target.py
--rw-r--r--   0        0        0      412 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Targets.py
--rw-r--r--   0        0        0     1223 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Units/AttributeMapping.py
--rw-r--r--   0        0        0     2082 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
--rw-r--r--   0        0        0     8560 2024-03-05 13:51:34.242753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
--rw-r--r--   0        0        0    17243 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
--rw-r--r--   0        0        0    29827 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
--rw-r--r--   0        0        0    15234 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
--rw-r--r--   0        0        0       96 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/__init__.py
--rw-r--r--   0        0        0    14870 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/Units.py
--rw-r--r--   0        0        0       45 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Units/__init__.py
--rw-r--r--   0        0        0       95 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2355 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0     1315 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1585 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      453 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1364 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2359 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      477 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Valve.py
--rw-r--r--   0        0        0      479 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Water.py
--rw-r--r--   0        0        0     4369 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Well.py
--rw-r--r--   0        0        0     1027 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0      435 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0      474 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/WellLists.py
--rw-r--r--   0        0        0      755 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      439 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      809 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      426 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     3070 2024-03-05 13:51:34.246753 ressimpy-2.0.9/ResSimpy/Wells.py
--rw-r--r--   0        0        0      289 2024-03-05 13:52:01.130866 ressimpy-2.0.9/ResSimpy/__init__.py
--rw-r--r--   0        0        0     2741 2024-03-05 13:52:01.130866 ressimpy-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 ressimpy-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0     9156 2024-04-15 14:16:46.310383 ressimpy-2.1.0/LICENSE.MD
+-rw-r--r--   0        0        0     5660 2024-04-15 14:16:46.310383 ressimpy-2.1.0/README.md
+-rw-r--r--   0        0        0      504 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0    10562 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1620 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1908 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     4148 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/DataObjectMixin.py
+-rw-r--r--   0        0        0     4373 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      358 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/FluidTypeEnums.py
+-rw-r--r--   0        0        0      369 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/FrequencyEnum.py
+-rw-r--r--   0        0        0      413 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/GridFunctionTypes.py
+-rw-r--r--   0        0        0      168 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      214 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/OutputType.py
+-rw-r--r--   0        0        0      282 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/PenetrationDirectionEnum.py
+-rw-r--r--   0        0        0      253 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/TimeSteppingMethodEnum.py
+-rw-r--r--   0        0        0      507 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0      377 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/WellTypeEnum.py
+-rw-r--r--   0        0        0       62 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      606 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     9279 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/File.py
+-rw-r--r--   0        0        0     2257 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/FileOperations/__init__.py
+-rw-r--r--   0        0        0    23457 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/FileOperations/file_operations.py
+-rw-r--r--   0        0        0      413 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     4554 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Grid.py
+-rw-r--r--   0        0        0     1713 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/GridArrayFunction.py
+-rw-r--r--   0        0        0      393 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      470 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     3785 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0     1443 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Network.py
+-rw-r--r--   0        0        0      768 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    27814 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    21507 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    18204 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     1872 2024-04-15 14:16:46.310383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     5081 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     6609 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     6806 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     4071 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProc.py
+-rw-r--r--   0        0        0     1286 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
+-rw-r--r--   0        0        0     2242 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
+-rw-r--r--   0        0        0     6924 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
+-rw-r--r--   0        0        0     7148 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     6675 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     2367 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
+-rw-r--r--   0        0        0     2936 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     6153 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     4691 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     5980 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      329 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     8894 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    19487 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0    11368 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    33223 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     6727 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    13660 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    31918 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     5635 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    20322 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0    10027 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     9709 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0    15015 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
+-rw-r--r--   0        0        0     6629 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0    11840 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     8933 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0     1069 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellList.py
+-rw-r--r--   0        0        0     3044 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellMod.py
+-rw-r--r--   0        0        0    40063 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0      822 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
+-rw-r--r--   0        0        0       67 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     3812 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      381 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     3802 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     3761 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0       43 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     3850 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0       47 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0     5130 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     4957 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3121 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2024-04-15 14:16:46.314383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0    17204 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     3709 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     3997 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0    12720 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     3763 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     4132 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    35469 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0    16873 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusSolverParameters.py
+-rw-r--r--   0        0        0     3806 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     3801 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    23296 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    22968 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0      115 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    24390 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14101 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    16640 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     8573 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     7107 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    23162 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     4132 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_load_well_list.py
+-rw-r--r--   0        0        0     2212 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     8133 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5422 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    18379 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0    20201 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      744 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Node.py
+-rw-r--r--   0        0        0      918 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     3041 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
+-rw-r--r--   0        0        0     3090 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Enums/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/Model_Parts/__init__.py
+-rw-r--r--   0        0        0     2892 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
+-rw-r--r--   0        0        0    10910 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
+-rw-r--r--   0        0        0      462 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimWells.py
+-rw-r--r--   0        0        0        0 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OpenGoSim/__init__.py
+-rw-r--r--   0        0        0     2553 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      442 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      467 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     6301 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0      573 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      594 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     4365 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0      407 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/SolverParameter.py
+-rw-r--r--   0        0        0      671 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/SolverParameters.py
+-rw-r--r--   0        0        0     1484 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Target.py
+-rw-r--r--   0        0        0      412 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Targets.py
+-rw-r--r--   0        0        0     1223 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMapping.py
+-rw-r--r--   0        0        0     2249 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
+-rw-r--r--   0        0        0     8727 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
+-rw-r--r--   0        0        0    17410 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
+-rw-r--r--   0        0        0    31056 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
+-rw-r--r--   0        0        0    15398 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
+-rw-r--r--   0        0        0       96 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/__init__.py
+-rw-r--r--   0        0        0    14870 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/Units.py
+-rw-r--r--   0        0        0       45 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Units/__init__.py
+-rw-r--r--   0        0        0       95 2024-04-15 14:16:46.318383 ressimpy-2.1.0/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0      365 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/general_utilities.py
+-rw-r--r--   0        0        0     1315 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1364 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2359 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      477 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      479 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Water.py
+-rw-r--r--   0        0        0     4790 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Well.py
+-rw-r--r--   0        0        0     1411 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0     1946 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0     1057 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/WellLists.py
+-rw-r--r--   0        0        0      755 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      439 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      809 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     3244 2024-04-15 14:16:46.322383 ressimpy-2.1.0/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      289 2024-04-15 14:16:57.954518 ressimpy-2.1.0/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     2733 2024-04-15 14:16:57.950518 ressimpy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 ressimpy-2.1.0/PKG-INFO
```

### Comparing `ressimpy-2.0.9/LICENSE.MD` & `ressimpy-2.1.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/README.md` & `ressimpy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Completion.py` & `ressimpy-2.1.0/ResSimpy/Completion.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,14 +71,41 @@
                  x: Optional[float] = None, y: Optional[float] = None, angle_a: Optional[float] = None,
                  angle_v: Optional[float] = None, grid: Optional[str] = None, depth_to_top: Optional[float] = None,
                  depth_to_bottom: Optional[float] = None, perm_thickness_ovr: Optional[float] = None,
                  dfactor: Optional[float] = None, rel_perm_method: Optional[int] = None,
                  status: Optional[str] = None, date_format: Optional[DateFormatEnum.DateFormat] = None,
                  peaceman_well_block_radius: Optional[float] = None, start_date: Optional[str] = None,
                  unit_system: Optional[UnitSystem] = None) -> None:
+        """Initialises the Completion class.
+
+        Args:
+            date: (str): The starting date of the completion.
+            i: (Optional[int]): The structured grid cell location in the x direction.
+            j: (Optional[int]): The structured grid cell location in the y direction.
+            k: Optional[int]: The structured grid cell location in the z direction.
+            skin: Optional[float]: The skin value for the completion.
+            depth: Optional[float]: The depth of the completion.
+            well_radius: Optional[float]: The well radius.
+            x: Optional[float]: The x location of the well in distance units/coordinates.
+            y: Optional[float]: The y location of the well in distance units/coordinates.
+            angle_a: Optional[float]: the angle relative to the local I axis.
+            angle_v: Optional[float]: the angle relative to the true vertical axis (global Z axis).
+            grid: Optional[str]: the grid name to which the completion data applies.
+            depth_to_top: Optional[float]: depth to the top of a completion interval.
+            depth_to_bottom: Optional[float]: depth to the bottom of the completion interval.
+            perm_thickness_ovr: Optional[float]: permeability thickness override value to use for the
+            completion interval.
+            dfactor: Optional[float]: non-darcy factor to use for rate dependent skin calculations.
+            rel_perm_method: Optional[int]: rel perm method to use for the completion.
+            status: Optional[str]: the status of the layer, can be 'ON' or 'OFF'
+            date_format: Optional[DateFormatEnum.DateFormat]: The date format to use for the date as an enum.
+            peaceman_well_block_radius: Optional[float]: The pressure equivalent radius of the grid block
+            start_date: Optional[str]: The start date of the simulation.
+            unit_system: Optional[UnitSystem]: The unit system to use for the completion.
+        """
         super().__init__({})
         self._date_format = date_format
         self.__well_radius = well_radius
         self.__date = date
         self.__i = i
         self.__j = j
         self.__k = k
```

### Comparing `ressimpy-2.0.9/ResSimpy/Constraint.py` & `ressimpy-2.1.0/ResSimpy/Constraint.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     max_surface_gas_rate: Optional[float] = None
     max_surface_water_rate: Optional[float] = None
     max_surface_liquid_rate: Optional[float] = None
     max_reservoir_oil_rate: Optional[float] = None
     max_reservoir_gas_rate: Optional[float] = None
     max_reservoir_water_rate: Optional[float] = None
     max_reservoir_liquid_rate: Optional[float] = None
+    min_surface_oil_rate: Optional[float] = None
+    min_surface_gas_rate: Optional[float] = None
+    min_surface_water_rate: Optional[float] = None
+    min_surface_liquid_rate: Optional[float] = None
     bottom_hole_pressure: Optional[float] = None
     tubing_head_pressure: Optional[float] = None
     max_reservoir_total_fluids_rate: Optional[float] = None
 
     @property
     def units(self) -> ConstraintUnits:
         """Returns the attribute to unit map for the constraint."""
```

### Comparing `ressimpy-2.0.9/ResSimpy/Constraints.py` & `ressimpy-2.1.0/ResSimpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/DataObjectMixin.py` & `ressimpy-2.1.0/ResSimpy/DataObjectMixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 @dataclass()
 class DataObjectMixin(ABC):
     """Base class representing a data object in ResSimpy."""
     __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False, repr=False)
 
     def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        """Initialises the DataObjectMixin class.
+
+        Args:
+            properties_dict (dict): dict of the properties to set on the object.
+        """
         # properties dict is a parameter to make the call signature equivalent to subclasses.
         self.__id = uuid.uuid4()
         if properties_dict:
             raise ValueError('No properties should be passed to the DataObjectMixin')
 
     def __repr__(self) -> str:
         return generic_repr(self)
@@ -28,19 +33,19 @@
         return generic_str(self)
 
     def to_dict(self, keys_in_keyword_style: bool = False, add_date: bool = True, add_units: bool = True,
                 include_nones: bool = True) -> dict[str, None | str | int | float]:
         """Returns a dictionary of the attributes of the object.
 
         Args:
-            include_nones (bool):
             keys_in_keyword_style (bool): if True returns the key values as simulator keywords, otherwise returns the \
                 attribute name as stored by ressimpy.
             add_date (bool): if True adds the date to the dictionary
             add_units (bool): if True adds the units to the dictionary
+            include_nones (bool): if True includes None values from the object in the dictionary.
 
         Returns:
             a dictionary keyed by attributes and values as the value of the attribute
         """
         result_dict = to_dict_generic.to_dict(self, keys_in_keyword_style, add_date=add_date, add_units=add_units,
                                               include_nones=include_nones)
         return result_dict
```

### Comparing `ressimpy-2.0.9/ResSimpy/DynamicProperty.py` & `ressimpy-2.1.0/ResSimpy/DynamicProperty.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     """
 
     input_number: int
     file: File
     properties: dict
 
     def __init__(self, input_number: int, file: File) -> None:
+        """Initialises the DynamicProperty class.
+
+        Args:
+            input_number (int): Method, table or input number, in order as entered in the simulation input deck.
+            file (File): The File that the dynamic property is read from.
+        """
         self.input_number: int = input_number
         self.file: File = file
 
     @property
     def units(self) -> BaseUnitMapping:
         """Returns the attribute to unit map for the constraint."""
         raise NotImplementedError('Implement in the derived class.')
```

### Comparing `ressimpy-2.0.9/ResSimpy/File.py` & `ressimpy-2.1.0/ResSimpy/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,21 @@
     __file_modified: bool = False
     __file_loading_skipped: bool = False
 
     def __init__(self, location: str,
                  file_content_as_list: Optional[list[str]] = None,
                  include_objects: Optional[Sequence[File]] = None, create_as_modified: bool = False,
                  file_loading_skipped: bool = False) -> None:
+        """Initialises the File class.
 
+        Args:
+            file_content_as_list (Optional[list[str]]): The file content as a list of strings.
+            include_objects (Optional[Sequence[File]]): The files included in the file.
+            file_loading_skipped (bool): Whether the file loading was skipped due to the file being too large an array.
+        """
         self.location = location
         self._location_in_including_file = location
         self.include_objects: Optional[list[File]] = get_empty_list_file() \
             if include_objects is None else include_objects
         if file_content_as_list is None:
             self.file_content_as_list = []
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/FileBase.py` & `ressimpy-2.1.0/ResSimpy/FileBase.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/FileOperations/file_operations.py` & `ressimpy-2.1.0/ResSimpy/FileOperations/file_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import partial
 from typing import Optional, Union
 import re
 
-from ResSimpy.Grid import VariableEntry
+from ResSimpy.Grid import GridArrayDefinition
 
 
 def strip_file_of_comments(file_as_list: list[str], strip_str: bool = False,
                            comment_characters: Optional[list[str]] = None,
                            square_bracket_comments: bool = False) -> list[str]:
     """Strips all of the inline, single and multi line comments out of a file.
     Comment characters assumed are: ! and square brackets. Escaped characters are ones wrapped in quotation marks.
@@ -17,27 +17,30 @@
                                                   Nexus format (!)
         file_as_list (list[str]): a list of strings containing each line of the file as a new entry
         strip_str (bool, optional): if True strips the lines of whitespace. Defaults to False.
 
     Returns:
         list[str]: a list of strings containing each line of the file as a new entry without comments
     """
-    # TODO: support VIP comment out single C character at the start of a line
     if comment_characters is None:
         comment_characters = ['!']
     file_as_list = list(filter(None, file_as_list))
 
-    # remove any empty lines
-    # regex: look back and forward 1 character from an ! and check if it's a quotation mark and
-    # exclude it from the match if it is
     file_without_comments = file_as_list
 
     for comment_character in comment_characters:
-        file_without_comments = [re.split(fr'(?<!\"){comment_character}(?!\")', x)[0]
-                                 for x in file_without_comments if x and x[0] != comment_character]
+        if comment_character == 'C':  # handle VIP comment with single C character at the start of a line
+            file_without_comments = [line for line in file_without_comments if not line.startswith('C ') and not
+                                     line.strip() == 'C']
+        else:
+            # remove any empty lines
+            # regex: look back and forward 1 character from an ! and check if it's a quotation mark and
+            # exclude it from the match if it is
+            file_without_comments = [re.split(fr'(?<!\"){comment_character}(?!\")', x)[0]
+                                     for x in file_without_comments if x and x[0] != comment_character]
 
     flat_file = '\n'.join(file_without_comments)
 
     if square_bracket_comments:
         # regex: look back and forward 1 character from a square bracket and check if it's a quotation mark and
         # exclude it from the match if it is
         flatfile_minus_square_brackets = flat_file
@@ -75,15 +78,15 @@
         file_content = strip_file_of_comments(file_content, strip_str=strip_str)
 
     return file_content
 
 
 def get_next_value(start_line_index: int, file_as_list: list[str], search_string: None | str = None,
                    ignore_values: None | list[str] = None,
-                   replace_with: str | VariableEntry | None = None,
+                   replace_with: str | GridArrayDefinition | None = None,
                    comment_characters: None | list[str] = None,
                    single_c_acts_as_comment: bool = True) -> Optional[str]:
     """Gets the next non blank value in a list of lines.
 
     Args:
         start_line_index (int): line number to start reading file_as_list from
         file_as_list (list[str]): a list of strings containing each line of the file as a new entry
@@ -163,15 +166,15 @@
 
     if not value_found:
         return None
 
     return value
 
 
-def __replace_value_in_file_as_list(file_as_list: list[str], line_index: int, replace_with: str | VariableEntry,
+def __replace_value_in_file_as_list(file_as_list: list[str], line_index: int, replace_with: str | GridArrayDefinition,
                                     value: str) -> str:
     """Replaces a value in a file_as_list with a new value.
 
     Args:
         file_as_list (list[str]): a list of strings containing each line of the file as a new entry
         line_index (int): line number from file_as_list to replace the value in.
         replace_with (str | VariableEntry): a value to replace the existing value with.
@@ -183,15 +186,15 @@
     original_line = file_as_list[line_index]
     if not isinstance(original_line, str):
         raise ValueError(f'No valid value found, hit INCLUDE statement instead on line number \
                                             {line_index}')
     new_line = original_line
     if isinstance(replace_with, str):
         new_value = replace_with
-    elif isinstance(replace_with, VariableEntry):
+    elif isinstance(replace_with, GridArrayDefinition):
         new_line, new_value, value = __replace_with_variable_entry(new_line, original_line,
                                                                    replace_with, value)
     if new_value is None:
         raise ValueError(f'Value for replacing has returned a null value,\
                             check replace_with input, {replace_with=}')
     new_line = new_line.replace(value, new_value, 1)
     file_as_list[line_index] = new_line
@@ -216,33 +219,48 @@
     Returns:
         int: new character location in the search_string
         bool: whether we are starting a new search string
         str: new search string if a value has been ignored
         str: the value that has been built up, or blank if a value has been ignored
     """
     value_string = search_string[character_location: len(search_string)]
+    if ignore_values is not None:
+        ignore_values = [x.upper() for x in ignore_values]
+    confirm_exclude: bool = False
+
     for value_character in value_string:
-        # If we've formed a string we're supposed to ignore, ignore it and get the next value
-        if ignore_values is not None and (value in ignore_values or value.upper() in ignore_values):
+        if value_character not in invalid_characters:
+            value += value_character
+
+        if confirm_exclude and value_character in invalid_characters:
+            # String to ignore found, ignore it and get the next value
             search_string = search_string[character_location: len(search_string)]
             new_search_string = True
             value = ""
 
-        if value_character not in invalid_characters:
-            value += value_character
+        confirm_exclude = False
+
+        # If we've formed a string value we're supposed to ignore, check the next character ends the value on the next
+        # loop through. Avoids us excluding values that happen to occur in a longer string.
+        if ignore_values is not None and value.upper() in ignore_values:
+            if character_location >= len(value_string) - 1:
+                value = ""
+                break
+            else:
+                confirm_exclude = True
 
         character_location += 1
 
         # stop adding to the value once we hit an invalid_character
         if value_character in invalid_characters and value != '':
             break
     return character_location, new_search_string, search_string, value
 
 
-def __replace_with_variable_entry(new_line: str, original_line: str, replace_with: VariableEntry, value: str):
+def __replace_with_variable_entry(new_line: str, original_line: str, replace_with: GridArrayDefinition, value: str):
     new_value = replace_with.value if replace_with.value is not None else ''
     if replace_with.modifier != 'VALUE':
         new_line = new_line.replace('INCLUDE ', '')
     elif 'INCLUDE' not in original_line:
         new_value = 'INCLUDE ' + replace_with.value if replace_with.value is not None else ''
     # If we are replacing the first value from a mult, remove the space as well
     if replace_with.modifier == 'MULT' and replace_with.value == '':
@@ -299,15 +317,15 @@
     token_found = any(map(partial(check_token, token), file))
 
     return token_found
 
 
 def get_token_value(token: str, token_line: str, file_list: list[str],
                     ignore_values: Optional[list[str]] = None,
-                    replace_with: Union[str, VariableEntry, None] = None) -> Optional[str]:
+                    replace_with: Union[str, GridArrayDefinition, None] = None) -> Optional[str]:
     """Gets the value following a token if supplied with a line containing the token.
 
     Arguments:
         token (str): the token being searched for.
         token_line (str): string value of the line that the token was found in.
         file_list (list[str]): a list of strings containing each line of the file as a new entry
         ignore_values (list[str], optional): a list of values that should be ignored if found. \
@@ -340,15 +358,15 @@
         raise ValueError
     value = get_next_value(line_index, file_list, search_string, ignore_values, replace_with)
     return value
 
 
 def get_expected_token_value(token: str, token_line: str, file_list: list[str],
                              ignore_values: Optional[list[str]] = None,
-                             replace_with: Union[str, VariableEntry, None] = None,
+                             replace_with: Union[str, GridArrayDefinition, None] = None,
                              custom_message: Optional[str] = None) -> str:
     """Function that returns the result of get_token_value if a value is found, otherwise it raises a ValueError.
 
     Args:
         token (str): the token being searched for.
         token_line (str): string value of the line that the token was found in.
         file_list (list[str]): a list of strings containing each line of the file as a new entry
@@ -405,15 +423,15 @@
 
     full_date = f"{first_date_part} {second_date_part} {third_date_part}"
     return full_date
 
 
 def get_expected_next_value(start_line_index: int, file_as_list: list[str], search_string: Optional[str] = None,
                             ignore_values: Optional[list[str]] = None,
-                            replace_with: Union[str, VariableEntry, None] = None,
+                            replace_with: Union[str, GridArrayDefinition, None] = None,
                             custom_message: Optional[str] = None) -> str:
     """Gets the next non blank value in a list of lines.
 
     Args:
         start_line_index (int): line number to start reading file_as_list from
         file_as_list (list[str]): a list of strings containing each line of the file as a new entry
         search_string (str): string to search from within the first indexed line
```

### Comparing `ressimpy-2.0.9/ResSimpy/ISODateTime.py` & `ressimpy-2.1.0/ResSimpy/ISODateTime.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,22 +56,34 @@
         elif ISODateTime.isfloat(date) and start_date is not None:
             if date_format == DateFormat.DD_MM_YYYY:
                 converted_date = ISODateTime.strptime(start_date, '%d/%m/%Y') + timedelta(days=float(date))
             elif date_format == DateFormat.MM_DD_YYYY:
                 converted_date = ISODateTime.strptime(start_date, '%m/%d/%Y') + timedelta(days=float(date))
 
         elif date_format == DateFormat.DD_MM_YYYY:
-            converted_date = ISODateTime.strptime(date, '%d/%m/%Y')
+            try:
+                converted_date = ISODateTime.strptime(date, '%d/%m/%Y')
+            except ValueError:  # Handling the case where a time has been added
+                converted_date = ISODateTime.strptime(date, '%d/%m/%Y(%H:%M:%S)')
 
         elif date_format == DateFormat.MM_DD_YYYY:
-            converted_date = ISODateTime.strptime(date, '%m/%d/%Y')
+            try:
+                converted_date = ISODateTime.strptime(date, '%m/%d/%Y')
+            except ValueError:  # Handling the case where a time has been added
+                converted_date = ISODateTime.strptime(date, '%m/%d/%Y(%H:%M:%S)')
 
         elif date_format == DateFormat.DD_MMM_YYYY:
             converted_date = ISODateTime.strptime(date, '%d %b %Y')
 
+        elif date_format == DateFormat.DD_MM_YYYY_h_m_s:
+            converted_date = ISODateTime.strptime(date, '%d/%m/%Y(%H:%M:%S)')
+
+        elif date_format == DateFormat.MM_DD_YYYY_h_m_s:
+            converted_date = ISODateTime.strptime(date, '%m/%d/%Y(%H:%M:%S)')
+
         if converted_date is None:
             raise ValueError('Invalid date format or missing start_date.')
 
         return converted_date
 
     @classmethod
     def datetime_to_iso(cls, date: datetime, datetime_format: str = '%Y-%m-%d') -> ISODateTime:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,15 +86,75 @@
             choke_files: Optional[dict[int, NexusFile]] = None,
             icd_files: Optional[dict[int, NexusFile]] = None,
             esp_files: Optional[dict[int, NexusFile]] = None,
             polymer_files: Optional[dict[int, NexusFile]] = None,
             adsorption_files: Optional[dict[int, NexusFile]] = None,
             flux_in_files: Optional[dict[int, NexusFile]] = None
     ) -> None:
+        """Initialises the FcsNexusFile class.
+
+        Args:
+            location: str: The file path to the fcs file.
+            include_locations: Optional[list[str]]: list of file paths to the included files.
+            origin: Optional[str]: The file path to the file that included this file. None for top level files.
+            include_objects: Optional[list[NexusFile]: list of NexusFile objects that are included in this file.
+            file_content_as_list: Optional[list[str]]: list of strings representing the content of the file.
+            restart_file: Optional[NexusFile]: The restart file for the fcs file.
+            structured_grid_file: Optional[NexusFile]: The structured grid file for the fcs file.
+            options_file: Optional[NexusFile]: The options file for the fcs file.
+            runcontrol_file: Optional[NexusFile]: The runcontrol file for the fcs file.
+            override_file: Optional[NexusFile]: The override file for the fcs file.
+            eos_default_file: Optional[NexusFile]: The eos default file for the fcs file.
+            well_files: Optional[dict[int, NexusFile]: Collection of well files for the fcs file. Indexed by method
+            number.
+            surface_files: Optional[dict[int, NexusFile]: Collection of surface files for the fcs file. Indexed by
+            method number.
+            rock_files: Optional[dict[int, NexusFile]: Collection of rock files for the fcs file. Indexed by method
+            number.
+            relperm_files: Optional[dict[int, NexusFile]: Collection of relperm files for the fcs file. Indexed by
+            method number.
+            pvt_files: Optional[dict[int, NexusFile]: Collection of pvt files for the fcs file. Indexed by method
+            number.
+            water_files: Optional[dict[int, NexusFile]: Collection of water files for the fcs file. Indexed by method
+            number.
+            equil_files: Optional[dict[int, NexusFile]: Collection of equil files for the fcs file. Indexed by method
+            number.
+            tracer_init_files: Optional[dict[int, NexusFile]: Collection of tracer init files for the fcs file. Indexed
+            by method number.
+            aquifer_files: Optional[dict[int, NexusFile]: Collection of aquifer files for the fcs file. Indexed by
+            method number.
+            hyd_files: Optional[dict[int, NexusFile]: Collection of hyd files for the fcs file. Indexed by method
+            number.
+            valve_files: Optional[dict[int, NexusFile]: Collection of valve files for the fcs file. Indexed by method
+            number.
+            separator_files: Optional[dict[int, NexusFile]: Collection of separator files for the fcs file. Indexed by
+            method number.
+            ipr_files: Optional[dict[int, NexusFile]: Collection of ipr files for the fcs file. Indexed by method
+            number.
+            gas_lift_files: Optional[dict[int, NexusFile]: Collection of gas lift files for the fcs file. Indexed by
+            method number.
+            pump_files: Optional[dict[int, NexusFile]: Collection of pump files for the fcs file. Indexed by method
+            number.
+            compressor_files: Optional[dict[int, NexusFile]: Collection of compressor files for the fcs file. Indexed by
+            method number.
+            choke_files: Optional[dict[int, NexusFile]: Collection of choke files for the fcs file. Indexed by method
+            number.
+            icd_files: Optional[dict[int, NexusFile]: Collection of icd files for the fcs file. Indexed by method
+            number.
+            esp_files: Optional[dict[int, NexusFile]: Collection of esp files for the fcs file. Indexed by method
+            number.
+            polymer_files: Optional[dict[int, NexusFile]: Collection of polymer files for the fcs file. Indexed by
+            method number.
+            adsorption_files: Optional[dict[int, NexusFile]: Collection of adsorption files for the fcs file. Indexed by
+            method number.
+            flux_in_files: Optional[dict[int, NexusFile]: Collection of flux in files for the fcs file. Indexed by
+            method number.
+        """
         self.restart_file = restart_file
+
         self.structured_grid_file = structured_grid_file
         self.options_file = options_file
         self.runcontrol_file = runcontrol_file
         self.override_file = override_file
         self.eos_default_file = eos_default_file
         self.surface_files = surface_files
         self.well_files = well_files if well_files is not None else get_empty_dict_int_nexus_file()
@@ -318,14 +378,15 @@
 
         Args:
             new_file_path (str): new file path for the fcs file e.g. /new_path/new_fcs_file.fcs
             new_include_file_location (str): new location for the included files either absolute or relative
             to the new fcs file path
             case_suffix (str): suffix to append to the end of the file name e.g. case_1
         """
+
         def new_include_file_name(file_name: str) -> str:
             """Returns the new include file name based on the original file name plus the suffix provided."""
             file_name = os.path.basename(file_name)
             file_name, file_extension = os.path.splitext(file_name)
             file_name = f'{file_name}_{case_suffix}{file_extension}'
             return os.path.join(new_include_file_location, file_name)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,18 +125,14 @@
     max_pressure: Optional[float] = None
     max_wag_water_pressure: Optional[float] = None
     max_wag_gas_pressure: Optional[float] = None
     min_reverse_surface_oil_rate: Optional[float] = None
     min_reverse_surface_gas_rate: Optional[float] = None
     min_reverse_surface_water_rate: Optional[float] = None
     min_reverse_surface_liquid_rate: Optional[float] = None
-    min_surface_oil_rate: Optional[float] = None
-    min_surface_gas_rate: Optional[float] = None
-    min_surface_water_rate: Optional[float] = None
-    min_surface_liquid_rate: Optional[float] = None
     min_reservoir_oil_rate: Optional[float] = None
     min_reservoir_gas_rate: Optional[float] = None
     min_reservoir_water_rate: Optional[float] = None
     min_reservoir_liquid_rate: Optional[float] = None
     min_reservoir_total_fluids_rate: Optional[float] = None
     min_reservoir_hc_rate: Optional[float] = None
     min_reverse_reservoir_oil_rate: Optional[float] = None
@@ -195,14 +191,19 @@
     clear_all: Optional[bool] = None
     clear_q: Optional[bool] = None
     clear_limit: Optional[bool] = None
     clear_alq: Optional[bool] = None
     clear_p: Optional[bool] = None
 
     def __init__(self, properties_dict: dict[str, None | int | str | float | UnitSystem]) -> None:
+        """Initialises the NexusConstraint class.
+
+        Args:
+            properties_dict (dict): dict of the properties to set on the object.
+        """
         super(Constraint, self).__init__({})
         for key, prop in properties_dict.items():
             self.__setattr__(key, prop)
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the mapping of nexus keywords to attribute definitions."""
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,28 @@
 
 
 @dataclass
 class NexusConstraints(Constraints):
     """Class that holds all the constraints for a NexusNetwork object. This class is responsible for loading,
     modifying and removing constraints from the NexusNetwork object. This class is also responsible for
     writing the constraints to the Nexus deck.
+
+    Attributes:
+        constraints: dict[str, list[NexusConstraint]]: dictionary of all constraints defined within a model,
+        keyed by the node or well name.
     """
     _constraints: dict[str, list[NexusConstraint]] = field(default_factory=dict)
 
     def __init__(self, parent_network: NexusNetwork, model: NexusSimulator) -> None:
+        """Initialises the NexusConstraints class.
+
+        Args:
+            parent_network (NexusNetwork): the network object that the constraints are associated with.
+            model (NexusSimulator): the model object that the constraints are associated with.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self._constraints: dict[str, list[NexusConstraint]] = {}
         self.__model: NexusSimulator = model
 
     def get_all(self, object_name: Optional[str] = None, date: Optional[str] = None) -> \
             dict[str, list[NexusConstraint]]:
         """Get the constraints of the existing model with optional parameters to filter for name and date
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
     number: Optional[int] = None
     temp: Optional[float] = None
     station: Optional[str] = None
 
     def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        """Initialises the NexusNode class.
+
+        Args:
+            properties_dict (dict): A dictionary of properties to set on the node.
+        """
         # call the init of the DataObjectMixin
         super(Node, self).__init__({})
         for key, prop in properties_dict.items():
             self.__setattr__(key, prop)
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,19 @@
     insulation_thickness: Optional[float] = None
     insulation_conductivity: Optional[float] = None
     gravity_pressure_gradient_mult: Optional[float] = None
     friction_pressure_gradient_mult: Optional[float] = None
     acceleration_pressure_gradient_mult: Optional[float] = None
 
     def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        """Initialises the NexusNodeConnection class.
+
+        Args:
+            properties_dict (dict): A dictionary of properties to set on the node.
+        """
         # call the init of the DataObjectMixin
         super(NodeConnection, self).__init__({})
         for key, prop in properties_dict.items():
             self.__setattr__(key, prop)
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 class NexusNodeConnections(NodeConnections):
     """Holds all the node connections in a network. This class is responsible for loading, modifying and removing
     connections from a network. It also holds the list of connections in memory.
     """
     __connections: list[NexusNodeConnection] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusNodeConnections class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the connections are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__connections: list[NexusNodeConnection] = []
         self.__add_object_operations = AddObjectOperations(NexusNodeConnection, self.table_header, self.table_footer,
                                                            self.__parent_network.model)
         self.__remove_object_operations = RemoveObjectOperations(self.__parent_network, self.table_header,
                                                                  self.table_footer)
         self.__modify_object_operations = ModifyObjectOperations(self)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,19 +22,25 @@
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusNetwork import NexusNetwork
 
 
 @dataclass(kw_only=True)
 class NexusNodes(Nodes):
     """Class to store and manipulate the nodes in a NexusNetwork.
-    It is stored as an instance in the NexusNetwork class as "nodes".
+    It is stored as an instance in the NexusNetwork class as "nodes". A list of nodes in the network are stored in
+    memory these can be accessed through the get_all method.
     """
     __nodes: list[NexusNode] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusNodes class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the nodes are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__nodes: list[NexusNode] = []
         self.__add_object_operations = AddObjectOperations(NexusNode, self.table_header, self.table_footer,
                                                            self.__parent_network.model)
         self.__remove_object_operations = RemoveObjectOperations(self.__parent_network, self.table_header,
                                                                  self.table_footer)
         self.__modify_object_operations = ModifyObjectOperations(self)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProc.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProc.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusProcs.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusProcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     """Class for handling procedures in the Nexus Network. This class is used to store and collect information about
     certain procedures written in the Nexus surface file.
     """
     # need field function to make a new unique empty list
     __procs: list[NexusProc] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusProcs class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the procedures are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__procs = []
 
     def get_all(self) -> Sequence[NexusProc]:
         """Returns a list of procs loaded from the simulator."""
         self.__parent_network.get_load_status()
         return self.__procs
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTarget.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTarget.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from ResSimpy.Target import Target
 
 
 @dataclass(kw_only=True, repr=False)
 class NexusTarget(Target):
     """Class that represents a single nexus target in the NexusSimulator."""
     def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        """Initialises the NexusTarget class.
+
+        Args:
+            properties_dict (dict): A dictionary of properties to set on the object.
+        """
         # call the init of the DataObjectMixin
         super(Target, self).__init__({})
         for key, prop in properties_dict.items():
             self.__setattr__(key, prop)
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusTargets.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusTargets.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 class NexusTargets(Targets):
     """Class for handling targets in the Nexus Network. This class is used to store and manipulate the targets in a
     NexusNetwork. It is stored as an instance in the NexusNetwork class as "targets".
     """
     __targets: list[NexusTarget] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusTargets class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the targets are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__targets: list[NexusTarget] = []
         self.__add_object_operations = AddObjectOperations(None, self.table_header,
                                                            self.table_footer, self.__parent_network.model)
         self.__remove_object_operations = RemoveObjectOperations(self.__parent_network, self.table_header,
                                                                  self.table_footer)
         self.__modify_object_operations = ModifyObjectOperations(self)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Class for handling well connections in the Nexus Network. This class is used to store and manipulate the well
 connections in a NexusNetwork. It is stored as an instance in the NexusNetwork class as "well_connections".
 In Nexus this is the WELLS table.
 """
 from __future__ import annotations
 from dataclasses import dataclass, field
-from typing import Optional, TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING, Sequence
 from uuid import UUID
 
 import pandas as pd
 
 from ResSimpy.File import File
 from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
 from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
@@ -23,68 +23,65 @@
     from ResSimpy.Nexus.NexusNetwork import NexusNetwork
 
 
 @dataclass
 class NexusWellConnections(WellConnections):
     """Class for handling well connections in the Nexus Network. This class is used to store and manipulate the well
     connections in a NexusNetwork. It is stored as an instance in the NexusNetwork class as "well_connections".
-    In Nexus this is the WELLS table.
+    In Nexus this is the WELLS table. The list of well connections can be accessed in the NexusNetwork class through the
+    get_all method.
     """
-    __well_connections: list[NexusWellConnection] = field(default_factory=list)
+    _well_connections: list[NexusWellConnection] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusWellConnections class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the well connections are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
-        self.__well_connections: list[NexusWellConnection] = []
+
         self.__add_object_operations = AddObjectOperations(NexusWellConnection, self.table_header, self.table_footer,
                                                            self.__parent_network.model)
         self.__remove_object_operations = RemoveObjectOperations(self.__parent_network, self.table_header,
                                                                  self.table_footer)
         self.__modify_object_operations = ModifyObjectOperations(self)
+        super().__init__(parent_network=parent_network)
 
-    def get_all(self) -> list[NexusWellConnection]:
+    def get_all(self) -> Sequence[NexusWellConnection]:
         """Returns a list of well connections loaded from the simulator."""
         self.__parent_network.get_load_status()
-        return self.__well_connections
+        return self._well_connections
 
     def get_by_name(self, name: str) -> Optional[NexusWellConnection]:
         """Returns a single well connection with the provided name loaded from the simulator.
 
         Args:
             name (str): name of the requested well connection
 
         Returns:
             NexusWellConnection: which has the same name as requested
         """
         self.__parent_network.get_load_status()
         to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
-                           self.__well_connections)
+                           self._well_connections)
         return next(to_return, None)
 
     def get_df(self) -> pd.DataFrame:
         """Creates a dataframe representing all processed well connections data in a surface file
         Returns:
             DataFrame: of the properties of the well connections through time with each row representing a single well \
             connection.
         """
         self.__parent_network.get_load_status()
-        return obj_to_dataframe(self.__well_connections)
+        return obj_to_dataframe(self._well_connections)
 
     def get_overview(self) -> str:
         raise NotImplementedError('To be implemented')
 
-    def _add_to_memory(self, additional_list: Optional[list[NexusWellConnection]]) -> None:
-        """Extends the nodes object by a list of connections provided to it.
-
-        Args:
-            additional_list (Sequence[NexusWellConnection]): list of nexus connections to add to the nodes list.
-        """
-        if additional_list is None:
-            return
-        self.__well_connections.extend(additional_list)
-
     def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
         new_well_connections, _ = collect_all_tables_to_objects(surface_file, {'WELLS': NexusWellConnection},
                                                                 start_date=start_date,
                                                                 default_units=default_units)
         cons_list = new_well_connections.get('WELLS')
         self._add_to_memory(cons_list)
 
@@ -93,15 +90,15 @@
 
         Args:
             obj_to_remove (UUID | dict[str, None | str | float | int]): UUID of the wellbore to remove or a dictionary \
             with sufficient matching parameters to uniquely identify a wellbore
 
         """
         self.__remove_object_operations.remove_object_from_network_main(
-            obj_to_remove, self._network_element_name, self.__well_connections)
+            obj_to_remove, self._network_element_name, self._well_connections)
 
     def add(self, obj_to_remove: dict[str, None | str | float | int]) -> None:
         """Adds a well connection to a network, taking a dictionary with properties for the new well connection.
 
         Args:
             obj_to_remove (dict[str, None | str | float | int]): dictionary taking all the properties for the new
             well connection.
@@ -129,7 +126,12 @@
     @property
     def table_header(self) -> str:
         return 'WELLS'
 
     @property
     def table_footer(self) -> str:
         return 'END' + self.table_header
+
+    @property
+    def well_connections(self) -> Sequence[NexusWellConnection]:
+        self.__parent_network.get_load_status()
+        return self._well_connections
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,30 @@
 
 @dataclass(kw_only=True)
 class NexusWellLists(WellLists):
     """Class for representing a set of WellList objects for the Nexus model."""
     __well_lists: list[NexusWellList] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusWellLists class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the well lists are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__well_lists: list[NexusWellList] = []
 
     def get_all(self) -> list[NexusWellList]:
         """Returns all WellList names."""
         self.__parent_network.get_load_status()
         return self.__well_lists
 
     @property
     def welllists(self) -> list[NexusWellList]:
-        """Returns all WellList names."""
+        """Returns list of all WellList objects."""
         self.__parent_network.get_load_status()
         return self.__well_lists
 
     @property
     def table_header(self) -> str:
         """Start of the Node definition table."""
         return 'WELLLISTS'
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,19 @@
     elevation_profile: Optional[str] = None
     temperature_profile: Optional[str] = None
     heat_transfer_coeff: Optional[float] = None
     pvt_method: Optional[int] = None
     water_method: Optional[int] = None
 
     def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        """Initialises the NexusWellbore class.
+
+        Args:
+            properties_dict (dict): dict of the properties to set on the object.
+        """
         # call the init of the DataObjectMixin
         super(Wellbore, self).__init__({})
         for key, prop in properties_dict.items():
             self.__setattr__(key, prop)
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,25 @@
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusNetwork import NexusNetwork
 
 
 @dataclass
 class NexusWellbores(Wellbores):
     """Class for handling wellbores in the Nexus Network. This class is used to store and manipulate the wellbores in a
-    NexusNetwork. It is stored as an instance in the NexusNetwork class as "wellbores".
+    NexusNetwork. It is stored as an instance in the NexusNetwork class as "wellbores". The list of wellbores can be
+    accessed in the NexusNetwork class through the get_all method.
     """
     __wellbores: list[NexusWellbore] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusWellbores class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the wellbores are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__wellbores: list[NexusWellbore] = []
         self.__add_object_operations = AddObjectOperations(NexusWellbore, self.table_header, self.table_footer,
                                                            self.__parent_network.model)
         self.__remove_object_operations = RemoveObjectOperations(self.__parent_network, self.table_header,
                                                                  self.table_footer)
         self.__modify_object_operations = ModifyObjectOperations(self)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,19 @@
     dp_add: Optional[float] = None
     rate_mult: Optional[float] = None
     delta_depth: Optional[float] = None
     heat_transfer_coeff: Optional[float] = None
     dt_add: Optional[float] = None
 
     def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        """Initialises the NexusWellhead class.
+
+        Args:
+            properties_dict (dict): dict of the properties to set on the object.
+        """
         super(Wellhead, self).__init__({})
         for key, prop in properties_dict.items():
             self.__setattr__(key, prop)
 
     @staticmethod
     def get_keyword_mapping() -> dict[str, tuple[str, type]]:
         """Gets the mapping of nexus keywords to attribute definitions."""
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
 
 @dataclass
 class NexusWellheads(Wellheads):
     __wellheads: list[NexusWellhead] = field(default_factory=list)
 
     def __init__(self, parent_network: NexusNetwork) -> None:
+        """Initialises the NexusWellheads class.
+
+        Args:
+            parent_network (NexusNetwork): The network that the wellheads are a part of.
+        """
         self.__parent_network: NexusNetwork = parent_network
         self.__wellheads: list[NexusWellhead] = []
         self.__add_object_operations = AddObjectOperations(NexusWellhead, self.table_header, self.table_footer,
                                                            self.__parent_network.model)
         self.__remove_object_operations = RemoveObjectOperations(self.__parent_network, self.table_header,
                                                                  self.table_footer)
         self.__modify_object_operations = ModifyObjectOperations(self)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,24 @@
     properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                 dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusAquiferMethod class.
+
+        Args:
+            file (NexusFile): NexusFile object associated with the aquifer method.
+            input_number (int): method number for the aquifer method.
+            model_unit_system (UnitSystem): unit system used in the model.
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the aquifer
+                                 method. Defaults to None.
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,24 @@
                                 pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusEquilMethod class.
+
+        Args:
+            file (NexusFile): NexusFile object associated with the equil method.
+            input_number (int): method number for the equil method.
+            model_unit_system (UnitSystem): unit system used in the model.
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of key properties for the equil
+                                    method. Defaults to None.
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,26 @@
                  include_locations: Optional[list[str]] = None,
                  origin: Optional[str] = None,
                  include_objects: Optional[Sequence[File]] = None,
                  file_content_as_list: Optional[list[str]] = None,
                  linked_user: Optional[str] = None,
                  last_modified: Optional[datetime] = None,
                  file_loading_skipped: bool = False) -> None:
+        """Initialises the NexusFile class.
 
+        Args:
+            location: str: The file path to the fcs file.
+            include_locations: Optional[list[str]]: list of file paths to the included files.
+            origin: Optional[str]: The file path to the file that included this file. None for top level files.
+            include_objects: Optional[list[NexusFile]: list of NexusFile objects that are included in this file.
+            file_content_as_list: Optional[list[str]]: list of strings representing the content of the file.
+            linked_user (Optional[str]): user or owner of the file. Defaults to None
+            last_modified (Optional[datetime]): last modified date of the file, Defaults to None
+            file_loading_skipped (bool): If set to True, the file loading was skipped. Defaults to False.
+        """
         super().__init__(location=location, file_content_as_list=file_content_as_list, include_objects=include_objects,
                          file_loading_skipped=file_loading_skipped)
         if origin is not None:
             self.location = nfo.get_full_file_path(location, origin)
         else:
             self.location = location
         self.include_locations: Optional[list[str]] = get_empty_list_str() if include_locations is None else \
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,23 @@
     properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                      dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusGasliftMethod class.
+
+        Args:
+            file (NexusFile): NexusFile object associated with the gaslift method
+            input_number (int): method number for the gaslift method
+            model_unit_system (UnitSystem): unit system from the model
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the gaslift
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,24 @@
     unit_system: UnitSystem
     ratio_thousands: bool
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  ratio_thousands: bool = True,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusHydraulicsMethod class.
+
+        Args:
+            file (NexusFile): ??
+            input_number (int): ??
+            model_unit_system (UnitSystem): ??
+            ratio_thousands (bool): ??
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): ??
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         self.ratio_thousands = ratio_thousands
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ResSimpy.Units.AttributeMappings.DynamicPropertyUnitMapping import PVTUnits
 
 from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_str, get_empty_eosopt_dict_union
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
 
 
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+@dataclass(kw_only=True, repr=False)
 class NexusPVTMethod(DynamicProperty):
     """Class to hold Nexus PVT properties.
 
     Attributes:
         file (NexusFile): Nexus PVT file object
         input_number (int): PVT method number in Nexus fcs file
         pvt_type (Optional[str]): Type of PVT method, e.g., BLACKOIL, GASWATER or EOS. Defaults to None
@@ -61,14 +61,30 @@
                  pvt_type: Optional[PvtType] = None,
                  eos_nhc: Optional[int] = None, eos_temp: Optional[float] = None,
                  eos_components: Optional[list[str]] = None,
                  eos_options: Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
                                        tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]] = None,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusGasliftMethod class.
+
+        Args:
+            file (NexusFile): NexusFile object associated with the PVT method.
+            input_number (int): method number for the PVT method.
+            model_unit_system (UnitSystem): unit system from the model.
+            pvt_type (Optional[PvtType]): Type of PVT method, e.g., BLACKOIL, GASWATER or EOS. Defaults to None.
+            eos_nhc (Optional[int]): Number of hydrocarbon components for EOS method. Defaults to None.
+            eos_temp (Optional[float]): Default temperature for EOS method. Defaults to None.
+            eos_components (Optional[list[str]]): Specifies component names for EOS method. Defaults to None.
+            eos_options (Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
+                                       tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]]): Dictionary containing
+                                        various EOS options as specified in the PVT file. Defaults to None.
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the PVT method.
+        """
         if pvt_type is not None:
             self.pvt_type = pvt_type
         if eos_nhc is not None:
             self.eos_nhc = eos_nhc
         if eos_temp is not None:
             self.eos_temp = eos_temp
         if eos_components is not None:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,25 @@
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None,
                  hysteresis_params: Optional[dict[str, Union[str, float, dict[str, Union[str, float,
                                              dict[str, Union[str, float]]]]]]] = None) -> None:
+        """Initialises the NexusRelPermMethod class.
+
+        Args:
+            file (NexusFile): Nexus file object associated with the relperm method
+            input_number (int): method number for the relperm method
+            model_unit_system (UnitSystem): unit system from the model
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                dict[str, Union[float, pd.DataFrame]]]]]): properties for the relperm method.
+            hysteresis_params (Optional[dict[str, Union[str, float, dict[str, Union[str, float,
+                                dict[str, Union[str, float]]]]]]]): hysteresis parameters for the relperm method.
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         if hysteresis_params is not None:
             self.hysteresis_params = hysteresis_params
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,24 @@
     properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                 dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusRockMethod class.
+
+        Args:
+            file (NexusFile): Nexus file containing the rock method.
+            input_number (int): method number for the rock method
+            model_unit_system (UnitSystem): unit system from the model
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of the properties for the rock
+                                    method. Defaults to None.
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,25 @@
         = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  separator_type: Optional[SeparatorType] = None,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusSeparatorMethod class.
+
+        Args:
+            file (NexusFile): NexusFile object associated with the separator method
+            input_number (int): method number for the separator method
+            model_unit_system (UnitSystem): unit system from the model
+            separator_type (Optional[SeparatorType]): type of separator method, e.g., BLACKOIL, GASPLANT or EOS
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): dictionary of properties for the separator
+                                 method.
+        """
         if separator_type is not None:
             self.separator_type = separator_type
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusSolverParameter.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusSolverParameter.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusValveMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,23 @@
     properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                      dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        """Initialises the NexusValveMethod class.
+
+        Args:
+            file (NexusFile): NexusFile object associated with the valve method.
+            input_number (int): method number for the valve method.
+            model_unit_system (UnitSystem): unit system used in the model.
+            properties (Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                 dict[str, Union[float, pd.DataFrame]]]]]): The properties found in the valve method.
+        """
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         self.unit_system = model_unit_system
         super().__init__(input_number=input_number, file=file)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,26 @@
     unit_system: UnitSystem
 
     def __init__(self, file: NexusFile, input_number: int, model_unit_system: UnitSystem,
                  reference_pressure: Optional[float] = None,
                  properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
                                       dict[str, Union[float, pd.DataFrame]]]]] = None,
                  parameters: Optional[list[NexusWaterParams]] = None) -> None:
+        """Initialises the NexusWaterMethod class.
+
+        Args:
+            file (NexusFile): Nexus water file object
+            input_number (int): Water method number in Nexus fcs file
+            reference_pressure (float): Reference pressure for BW and, if CVW is present, for VISW
+            properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                        dict[str, Union[float, pd.DataFrame]]]]):
+                Dictionary holding properties for generic dynamic method. Defaults to empty dictionary.
+            parameters (list[NexusWaterParams]): list of water parameters, such as density, viscosity, etc.
+            model_unit_system (UnitSystem): unit system used in the model.
+        """
         self.reference_pressure = reference_pressure
         if properties is not None:
             self.properties = properties
         else:
             self.properties = {}
         if parameters is not None:
             self.parameters = parameters
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWell.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Class for representing a well in Nexus. Consists of a list of completions and a well name."""
 from __future__ import annotations
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional, Sequence, Union, TYPE_CHECKING
 from uuid import UUID
 
 from ResSimpy.Enums.WellTypeEnum import WellType
 from ResSimpy.Nexus.DataModels.NexusCompletion import NexusCompletion
 from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Nexus.DataModels.NexusWellMod import NexusWellMod
@@ -16,19 +16,29 @@
     from ResSimpy.Nexus.NexusWells import NexusWells
 
 
 @dataclass(kw_only=True)
 class NexusWell(Well):
     """Class for representing a well in Nexus. Consists of a list of completions and a well name."""
     _wellmods: list[NexusWellMod]
-    _parent_wells_instance: NexusWells
+    _parent_wells_instance: NexusWells = field(compare=False)
 
     def __init__(self, well_name: str, completions: Sequence[NexusCompletion], unit_system: UnitSystem,
                  parent_wells_instance: NexusWells, wellmods: Sequence[NexusWellMod] | None = None,
                  well_type: Optional[WellType] = None) -> None:
+        """Initialises the NexusWell class.
+
+        Args:
+            well_name (str): Name of the well
+            completions (Sequence[NexusCompletion]): List of completions for the well.
+            unit_system (UnitSystem): Unit system for the well.
+            parent_wells_instance (NexusWells): Instance of the parent wells class that the well belongs to.
+            wellmods (Sequence[NexusWellMod] | None): List of wellmods for the well. Defaults to None.
+            well_type (Optional[WellType]): Type of the well as an enum. Defaults to None.
+        """
         self._parent_wells_instance = parent_wells_instance
         if not isinstance(completions, list):
             completions = list(completions)
         if wellmods is None:
             wellmods = []
         elif not isinstance(wellmods, list):
             wellmods = list(wellmods)
@@ -124,14 +134,15 @@
         ----
             date (str): date at which the perforation should be added
             completion_properties (dict[str, str | float | int]):
             completion_index (Optional[int]):
         """
         completion_properties['date'] = date
         completion_properties['unit_system'] = self.unit_system
+        completion_properties['start_date'] = self._parent_wells_instance.start_date
         new_completion = NexusCompletion.from_dict(completion_properties, date_format)
         if completion_index is None:
             completion_index = len(self._completions)
         self._completions.insert(completion_index, new_completion)
         return new_completion
 
     def _remove_completion_from_memory(self, completion_to_remove: NexusCompletion | UUID) -> None:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/DataModels/NexusWellMod.py` & `ressimpy-2.1.0/ResSimpy/Nexus/DataModels/NexusWellMod.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     delta_swr: float | list[float] | None = None
     delta_sgr: float | list[float] | None = None
     delta_krw: float | list[float] | None = None
     delta_krg: float | list[float] | None = None
     perm_thickness_mult: float | list[float] | None = None
 
     def __init__(self, wellmod_dict: dict[str, None | str | float | int | list[float]]) -> None:
+        """Initialises the NexusWellMod class.
+
+        Args:
+            wellmod_dict (dict[str, None | str | float | int | list[float]]): Dictionary of wellmod properties.
+        """
         for key, prop in wellmod_dict.items():
             self.__setattr__(key, prop)
 
     def __repr__(self) -> str:
         return generic_repr(self)
 
     def __str__(self) -> str:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     __inputs: MutableMapping[int, NexusAquiferMethod]
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem, inputs: Optional[MutableMapping[int, NexusAquiferMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusAquiferMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusAquiferMethod]]): Collection of Nexus aquifer methods.
+            files (Optional[dict[int, NexusFile]]): Collection of aquifer files, as defined in Nexus fcs file.
+            Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusAquiferMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     __inputs: MutableMapping[int, NexusEquilMethod]
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem, inputs: Optional[MutableMapping[int, NexusEquilMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusEquilMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusEquilMethod]]): Collection of Nexus equilibration methods.
+            files (Optional[dict[int, NexusFile]]): Collection of equilibration files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusEquilMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusGasliftMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusGasliftMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusGasliftMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusGasliftMethod]]): Collection of Nexus gaslift methods.
+            files (Optional[dict[int, NexusFile]]): Collection of gaslift files, as defined in Nexus fcs file.
+            Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusGasliftMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusHydraulicsMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusHydraulicsMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusHydraulicsMethod]]): Collection of Nexus hydraulics methods.
+            files (Optional[dict[int, NexusFile]]): Collection of hydraulics files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusHydraulicsMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/proc_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/proc_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 PROPERTY_ARRAYS = ['POROSITY', 'POR', 'POROSITY', 'PV', 'KX', 'KY', 'KZ', 'COMPR', 'CR', 'NETGRS', 'KWX',
                    'KWY', 'KWZ', 'PEMDMAT', 'PEMGMAT', 'PEMKMAT', 'BW_SAL', 'BW_T']
 
 GRID_GEOMETRY_ARRAYS = ['CORP', 'EIGHT', 'DX', 'DY', 'DZ', 'DXB', 'DYB', 'DZB', 'MDEPTH', 'DEPTH', 'DBZNET']
 
 GRID_OPERATION_KEYWORDS = ['ADD', 'SUB', 'DIV', 'MULT', 'EQ']
 
-GRID_ARRAY_FORMAT_KEYWORDS = ['VALUE', 'XVAR', 'YVAR', 'ZVAR']
+GRID_ARRAY_FORMAT_KEYWORDS = ['CON', 'VALUE', 'XVAR', 'YVAR', 'ZVAR', 'MULT', 'LAYER', 'DIP']
 
 GRID_ARRAY_KEYWORDS = INTEGER_ARRAYS + WORK_ARRAYS + ROCK_ARRAYS + USER_INIT_ARRAYS + MULTIPLIER_ARRAYS + \
                       PROPERTY_ARRAYS + GRID_GEOMETRY_ARRAYS
 
 STRUCTURED_GRID_KEYWORDS = ['ADD', 'ALL', 'ANALYT', 'ARRAYS', 'B', 'BLOCKS', 'C', 'CARTREF', 'COARSEN', 'COMPR', 'CON',
                             'CONCENTRATION', 'CORNER', 'CORP', 'CORTOL', 'DEADCELL', 'DECOMP', 'DEPTH', 'DIP', 'DIV',
                             'DX', 'DY', 'DZ', 'END', 'ENDAQ', 'ENDDEC', 'ENDREF', 'EXP', 'FNAME', 'FRAC', 'FTRANS',
@@ -35,8 +35,8 @@
                             'KRW_SWU', 'KX', 'KXEFF', 'KY', 'KYEFF', 'KZ', 'KZEFF', 'LAYER', 'LE', 'LGR', 'LIVECELL',
                             'LX', 'LY', 'LZ', 'MAPBINARY', 'MAPOUT', 'MAPVDB', 'MDEPTH', 'MIN', 'MINUS', 'MOD', 'MODX',
                             'MODY', 'MODZ', 'MULT', 'MULTBV', 'MULTFL', 'MULTIR', 'NETGRS', 'NEWTRAN', 'NOLIST', 'NONE',
                             'NONSTD', 'NX', 'NY', 'NZ', 'OMIT', 'OUTPUT', 'OVER', 'PINCHOUT', 'POR', 'POROSITY',
                             'PRINT', 'PV', 'PVMULT', 'RANGE', 'RIGHTHANDED', 'ROOT', 'SALINITY', 'SG', 'SGL', 'SGR',
                             'SGRO', 'SGRW', 'SGU', 'SINF', 'STD', 'SW', 'SWL', 'SWR', 'SWRO', 'SWRO_LS', 'SWU', 'TMX',
                             'TMY', 'TMZ', 'TOLPV', 'TX', 'TY', 'TZ', 'V98', 'VALUE', 'WATER', 'WINDOW', 'WORKA1', 'X',
-                            'XREG', 'Z', 'ZVAR']
+                            'XREG', 'Z', 'ZVAR', 'LIST']
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusKeywords/wells_keywords.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,19 @@
     constraints: NexusConstraints
     procs: NexusProcs
     targets: NexusTargets
     welllists: NexusWellLists
     __has_been_loaded: bool = False
 
     def __init__(self, model: NexusSimulator) -> None:
+        """Initialises the NexusNetwork class.
+
+        Args:
+            model (NexusSimulator): NexusSimulator object to be used to loading of the network object.
+        """
         self.__has_been_loaded: bool = False
         self.__model: NexusSimulator = model
         self.nodes: NexusNodes = NexusNodes(self)
         self.connections: NexusNodeConnections = NexusNodeConnections(self)
         self.well_connections: NexusWellConnections = NexusWellConnections(self)
         self.wellheads: NexusWellheads = NexusWellheads(self)
         self.wellbores: NexusWellbores = NexusWellbores(self)
@@ -109,15 +114,15 @@
         files_dict = self.__model.model_files.surface_files
         if files_dict is None:
             raise ValueError('Surface files not found for this model.')
 
         for file in files_dict.values():
 
             # for every surface file, grab the lines as a list
-            file_contents = file.file_content_as_list
+            file_contents = file.get_flat_list_str_file
             if file_contents is None:
                 raise ValueError(f'No file contents found for surface file {file.location}.')
 
             # boolean to determine if we are interested in a specific line or not
             grab_line = False
 
             # the contents of a specific procedure as a list
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     __inputs: MutableMapping[int, NexusPVTMethod]
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem, inputs: Optional[MutableMapping[int, NexusPVTMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusPVTMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusPVTMethod]]): Collection of Nexus PVT property methods.
+            files (Optional[dict[int, NexusFile]]): Collection of PVT property files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusPVTMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusRelPermMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusRelPermMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusRelPermMethod]]): Collection of Nexus relperm property inputs.
+            files (Optional[dict[int, NexusFile]]): Collection of relperm property files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusRelPermMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusReporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Class for handling all Reporting and runcontrol related tasks."""
+from __future__ import annotations
+
 import warnings
 from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
 from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Enums.FrequencyEnum import FrequencyEnum
 from ResSimpy.Enums.OutputType import OutputType
 from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
 from ResSimpy.Units.AttributeMappings.BaseUnitMapping import BaseUnitMapping
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
 
 
 @dataclass(kw_only=True)
 class NexusOutputRequest(DataObjectMixin):
     """Class for handling output requests in Nexus."""
     date: str
     output: str
@@ -55,15 +60,20 @@
     __array_output_requests: list[NexusOutputRequest]
     __ss_output_contents: list[NexusOutputContents]
     __array_output_contents: list[NexusOutputContents]
 
     table_header = 'OUTPUT'
     table_footer = 'ENDOUTPUT'
 
-    def __init__(self, model) -> None:
+    def __init__(self, model: NexusSimulator) -> None:
+        """Initialises the NexusReporting class.
+
+        Args:
+            model (NexusSimulator): The Nexus model to get the reporting information from.
+        """
         self.__model = model
         self.__add_object_operations = AddObjectOperations(NexusOutputRequest, self.table_header, self.table_footer,
                                                            model)
 
     @property
     def ss_output_requests(self) -> list[NexusOutputRequest]:
         return self.__ss_output_requests
@@ -252,14 +262,16 @@
 
     def _add_array_output_request(self, output_request: NexusOutputRequest) -> None:
         """Adds an output request to the array output requests list.
 
         Args:
             output_request (NexusOutputRequest): The output request to add the model and associated in memory files.
         """
+        if self.__model.model_files.runcontrol_file is None:
+            raise ValueError("No file found for runcontrol file path.")
         file_as_list = self.__model.model_files.runcontrol_file.get_flat_list_str_file
         obj_props = output_request.to_dict(add_units=False)
         self.__add_object_operations.add_object_to_file(date=output_request.date,
                                                         file_as_list=file_as_list,
                                                         file_to_add_to=self.__model.model_files.runcontrol_file,
                                                         new_object=output_request,
                                                         object_properties=obj_props,
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusRockMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusRockMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusRockMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusRockMethod]]): Collection of Nexus rock property methods.
+            files (Optional[dict[int, NexusFile]]): Collection of rock property files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusRockMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusSeparatorMethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,23 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusSeparatorMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusSeparatorMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusSeparatorMethod]]): Collection of Nexus separator property
+            methods.
+            files (Optional[dict[int, NexusFile]]): Collection of separator property files, as defined in Nexus fcs
+            file. Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusSeparatorMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,31 +302,23 @@
             ValueError: If fluid types are inconsistent between models
 
         Returns:
             Optional[str]: The fluid type used for the model for the first surface network
         """
         fluid_type = None
         for model in models:
+            model_obj = NexusSimulator(origin=model)
             model_fluid_type = None
-            fcs_file = NexusFile.generate_file_include_structure(model).get_flat_list_str_file
-            surface_filename = None
-            if fcs_file is None:
-                warnings.warn(UserWarning(f'No file found for {model}'))
-                continue
-            for line in fcs_file:
-                if nfo.check_token("SURFACE Network 1", line):
-                    surface_filename = nfo.get_expected_token_value(token="SURFACE Network 1", token_line=line,
-                                                                    file_list=fcs_file)
-                    break
-
-            if surface_filename is not None:
-                surface_filename = surface_filename if os.path.isabs(surface_filename) else \
-                    os.path.dirname(model) + "/" + surface_filename
+            # get the first surface method and expand out all include files
+            if model_obj.model_files.surface_files is None or model_obj.model_files.surface_files[1].location is None:
+                raise ValueError(f"No surface file found for {model}")
+            surface_file_content = model_obj.model_files.surface_files[1].get_flat_list_str_file
+            if surface_file_content is not None:
                 model_fluid_type = NexusSimulator.get_fluid_type(
-                    surface_file_name=surface_filename)
+                    surface_file_content=surface_file_content)
 
             if fluid_type is None:
                 fluid_type = model_fluid_type
             elif fluid_type != model_fluid_type:
                 raise ValueError(
                     f"Inconsistent Oil / Gas types: {model_fluid_type} found for {model}")
 
@@ -344,69 +336,65 @@
         """
         eos_string: str = ''
         eos_found: bool = False
         for line in surface_file:
             if nfo.check_token("EOS", line):
                 eos_string += line
                 eos_found = True
-            elif eos_found:
+            elif eos_found and nfo.get_next_value(0, [line]) is not None:
                 eos_string += line
             if nfo.check_token("COMPONENTS", line):
                 break
 
         return eos_string
 
     @staticmethod
-    def get_fluid_type(surface_file_name: str) -> str:
+    def get_fluid_type(surface_file_content: list[str]) -> str:
         """Gets the fluid type for a single model from a surface file.
+        Defaults to BLACKOIL if no explicit fluid type is found.
 
         Args:
-            surface_file_name (str): path to the surface file in a Nexus model
-
-        Raises:
-            ValueError: if no fluid type is found within the provided file path
+            surface_file_content (str): list of strings with a new line per entry from the surface file
 
         Returns:
             str: fluid type as one of [BLACKOIL, WATEROIL, GASWATER, API] or the full details from an EOS model
         """
-        surface_file = nfo.load_file_as_list(surface_file_name)
         fluid_type = None
 
-        for line in surface_file:
+        for line in surface_file_content:
             if nfo.check_token("BLACKOIL", line):
                 fluid_type = "BLACKOIL"
                 break
             elif nfo.check_token("WATEROIL", line):
                 fluid_type = "WATEROIL"
                 break
             elif nfo.check_token("GASWATER", line):
                 fluid_type = "GASWATER"
                 break
             elif nfo.check_token("EOS", line):
-                fluid_type = NexusSimulator.get_eos_details(surface_file)
+                fluid_type = NexusSimulator.get_eos_details(surface_file_content)
             elif nfo.check_token("API", line):
                 fluid_type = "API"
-
         if fluid_type is None:
-            raise ValueError("No Oil / Gas type detected")
-
+            warnings.warn("No explicit fluid type found in the file. Defaulting to BLACKOIL", UserWarning)
+            fluid_type = "BLACKOIL"
         return fluid_type
 
     def get_model_oil_type(self) -> str:
         """Returns the get_fluid_type method on the existing NexusSimulator instance.
 
         Raises:
             ValueError: If no file path is provided for the surface file path
 
         Returns:
             str: fluid type as one of [BLACKOIL, WATEROIL, GASWATER,] or the full details from an EOS model
         """
         if self.model_files.surface_files is None or self.model_files.surface_files[1].location is None:
             raise ValueError("No value found for the path to the surface file")
-        return NexusSimulator.get_fluid_type(self.model_files.surface_files[1].location)
+        return NexusSimulator.get_fluid_type(self.model_files.surface_files[1].get_flat_list_str_file)
 
     def check_output_path(self) -> None:
         """Confirms that the output path has been set (used to stop accidental writing operations in the original
         directory).
 
         Raises:
             ValueError: if the destination provided is set to None.
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusSolverParameters.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusSolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusValveMethods.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusValveMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusValveMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusValveMethod]]): Collection of Nexus valve property methods.
+            files (Optional[dict[int, NexusFile]]): Collection of valve property files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusValveMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     __files: dict[int, NexusFile]
     __properties_loaded: bool = False  # Used in lazy loading
     __model_unit_system: UnitSystem
 
     def __init__(self, model_unit_system: UnitSystem,
                  inputs: Optional[MutableMapping[int, NexusWaterMethod]] = None,
                  files: Optional[dict[int, NexusFile]] = None) -> None:
+        """Initialises the NexusWaterMethods class.
+
+        Args:
+            model_unit_system (UnitSystem): Unit system used in the model.
+            inputs (Optional[MutableMapping[int, NexusWaterMethod]]): Collection of Nexus water property methods.
+            files (Optional[dict[int, NexusFile]]): Collection of water property files, as defined in Nexus fcs file.
+                Keyed by the method number.
+        """
         if inputs:
             self.__inputs = inputs
         else:
             self.__inputs: MutableMapping[int, NexusWaterMethod] = {}
         if files:
             self.__files = files
         else:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/NexusWells.py` & `ressimpy-2.1.0/ResSimpy/Nexus/NexusWells.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,38 @@
 class NexusWells(Wells):
     """A class for collecting all NexusWell objects in a NexusSimulator. Handles adding and removing completions
     as well as rescheduling wells. This is usually accessed through the model.wells property.
 
     Arguments:
         model (Simulator): NexusSimulator object that has the instance of wells on.
     """
-    __model: NexusSimulator
-    __date_format: DateFormat
+    __model: NexusSimulator = field(compare=False)
+    __date_format: DateFormat = field(repr=False)
     _wells: list[NexusWell] = field(default_factory=list)
 
     def __init__(self, model: NexusSimulator) -> None:
+        """Initialises the NexusWells class.
+
+        Args:
+            model (NexusSimulator)
+        """
         self.__model = model
         self.__add_object_operations = AddObjectOperations(NexusCompletion, self.table_header, self.table_footer, model)
         super().__init__()
 
     @property
     def model(self) -> NexusSimulator:
         """The model object that contains this NexusWells instance."""
         return self.__model
 
     @property
+    def start_date(self) -> str:
+        return self.__model.start_date
+
+    @property
     def date_format(self) -> DateFormat:
         if not self._wells_loaded:
             self._load()
         return self.__date_format
 
     @property
     def table_header(self) -> str:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/load_wells.py` & `ressimpy-2.1.0/ResSimpy/Nexus/load_wells.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import warnings
 from typing import Optional, Sequence, TYPE_CHECKING
+from datetime import time, timedelta
 
 from ResSimpy.ISODateTime import ISODateTime
 from ResSimpy.Nexus.DataModels.NexusWellMod import NexusWellMod
 from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 import ResSimpy.Nexus.nexus_file_operations as nfo
 import ResSimpy.FileOperations.file_operations as fo
 from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
@@ -163,17 +164,36 @@
 
             if not hasattr(DateFormat, converted_format_str):
                 raise ValueError(f"Invalid Date Format found: '{new_date_format_str}' at line {index}")
 
             date_format = DateFormat[converted_format_str]
 
         if nfo.check_token('TIME', line):
-            current_date = fo.get_expected_token_value(token='TIME', token_line=line, file_list=file_as_list,
-                                                       custom_message="Cannot find the date associated with the TIME "
-                                                                      f"card in {line=} at line number {index}")
+            time_value = fo.get_expected_token_value(token='TIME', token_line=line, file_list=file_as_list,
+                                                     custom_message="Cannot find the date associated with the TIME "
+                                                                    f"card in {line=} at line number {index}")
+            if time_value.upper() != 'PLUS':
+                current_date = time_value
+            else:
+                plus_value = fo.get_expected_token_value(token='PLUS', token_line=line, file_list=file_as_list,
+                                                         custom_message="Cannot find the date associated with the TIME "
+                                                         f"PLUS card in {line=} at line number {index}")
+                new_datetime = ISODateTime.convert_to_iso(
+                    current_date, date_format, start_date) + timedelta(days=float(plus_value))
+
+                if date_format == DateFormat.DD_MM_YYYY:
+                    if new_datetime.time() == time(0, 0, 0, 0):
+                        current_date = new_datetime.strftime('%d/%m/%Y')
+                    else:
+                        current_date = new_datetime.strftime('%d/%m/%Y(%H:%M:%S)')
+                elif date_format == DateFormat.MM_DD_YYYY:
+                    if new_datetime.time() == time(0, 0, 0, 0):
+                        current_date = new_datetime.strftime('%m/%d/%Y')
+                    else:
+                        current_date = new_datetime.strftime('%m/%d/%Y(%H:%M:%S)')
 
         if nfo.check_token('WELLMOD', line):
             wellmod = __get_inline_well_mod(line, current_date=current_date, unit_system=wellspec_file_units,
                                             wells_loaded=wells, start_date=start_date, date_format=date_format)
             wellmodname = wellmod.well_name
             if wellmodname.upper() not in well_name_list:
                 raise ValueError(f"Cannot find well name {wellmodname} in wellspec file: {nexus_file.location}")
@@ -203,43 +223,49 @@
             header_values = {k: None for k in header_values}
             if wellspec_file_units is None:
                 wellspec_file_units = default_units
 
             # Load in each line of the table
             completions = __load_wellspec_table_completions(
                 nexus_file, header_index, header_values, headers, current_date, end_point_scaling_header_values,
-                date_format, unit_system=wellspec_file_units)
+                date_format, unit_system=wellspec_file_units, start_date=start_date)
 
             if well_name.upper() in well_name_list:
                 wells[well_name_list.index(well_name.upper())].completions.extend(completions)
             else:
                 new_well = NexusWell(completions=completions, well_name=well_name, unit_system=wellspec_file_units,
                                      wellmods=[], parent_wells_instance=parent_wells_instance)
                 well_name_list.append(well_name.upper())
                 wells.append(new_well)
             wellspec_found = False
     return wells, date_format
 
 
 def __load_wellspec_table_completions(nexus_file: NexusFile, header_index: int,
                                       header_values: dict[str, None | int | float | str],
-                                      headers: list[str], start_date: str,
+                                      headers: list[str], date: str,
                                       end_point_scaling_header_values: dict[str, None | int | float | str],
                                       date_format: DateFormat,
                                       unit_system: UnitSystem,
+                                      start_date: None | str = None,
                                       ) -> list[NexusCompletion]:
     """Loads a completion table in for a single WELLSPEC keyword. \
         Loads in the next available completions following a WELLSPEC keyword and a header line.
 
     Args:
         header_index (int): index number of the header in the file as list parameter
         header_values (dict[str, Union[Optional[int], Optional[float], Optional[str]]]): dictionary of column \
             headings to populate from the table
         headers (list[str]): list of strings containing the headers from the wellspec table
-        start_date (str): date to populate the completion class with.
+        date (str): date to populate the completion class with.
+        end_point_scaling_header_values (dict): dictionary containing the header values for thes special end point
+        scaling columns.
+        date_format (DateFormat): date format as a DateFormat Enum to use for the completion.
+        unit_system (UnitSystem): unit system as a UnitSystem Enum to use for the completion.
+        start_date (Optional[str]): start date of the model.
 
     Returns:
         list[NexusCompletion]: list of nexus completions for a given table.
     """
 
     def convert_header_value_float(key: str) -> Optional[float]:
         value = header_values[key]
@@ -279,15 +305,15 @@
                          in header_values if key in end_point_scaling_header_values}
         if any(rel_perm_dict.values()):
             new_rel_perm_end_point = NexusRelPermEndPoint(**rel_perm_dict)
         else:
             new_rel_perm_end_point = None
 
         new_completion = NexusCompletion(
-            date=start_date,
+            date=date,
             i=convert_header_value_int('IW'),
             j=convert_header_value_int('JW'),
             k=convert_header_value_int('L'),
             skin=convert_header_value_float('SKIN'),
             depth=convert_header_value_float('DEPTH'),
             well_radius=convert_header_value_float('RADW'),
             x=convert_header_value_float('X'),
@@ -326,14 +352,15 @@
             polymer_bore_radius=convert_header_value_float('RADBP'),
             polymer_well_radius=convert_header_value_float('RADWP'),
             portype=(None if header_values['PORTYPE'] is None else str(header_values['PORTYPE'])),
             rel_perm_end_point=new_rel_perm_end_point,
             kh_mult=convert_header_value_float('KHMULT'),
             date_format=date_format,
             unit_system=unit_system,
+            start_date=start_date,
         )
 
         nexus_file.add_object_locations(new_completion.id, [index + header_index + 1])
 
         completions.append(new_completion)
 
     return completions
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-2.1.0/ResSimpy/Nexus/logfile_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_add_new_object_to_file.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
 
 class AddObjectOperations:
     """Class for handling adding objects to a nexus file and memory."""
 
     def __init__(self, obj_type: Optional[type[T]], table_header: str, table_footer: str,
                  model: NexusSimulator) -> None:
+        """Initialises the AddObjectOperations class.
+
+        Args:
+            obj_type (Optional[type[T]]): type of object to add to the file.
+            table_header (str): The string that represents the start of the table in the file.
+            table_footer (str): The string that represents the end of the table in the file.
+            model (NexusSimulator): model to add the object to.
+        """
         self.__model = model
         self.table_header = table_header
         self.table_footer = table_footer
         self.obj_type = obj_type
 
     def find_which_file_from_id(self, obj_id: UUID, file_type_to_search: str) -> NexusFile:
         """Finds a file based on the presence of an object in the file.
@@ -88,16 +96,19 @@
         # TODO move out the additional headers mutability to a separate method that explicitly sets it
         keyword_map = {x: y[0] for x, y in nexus_mapping.items()}
         inverted_nexus_map = invert_nexus_map(nexus_mapping)
         table = file_content[index::]
         header_index, headers = nfo.get_table_header(file_as_list=table, header_values=keyword_map)
         header_index += index
         headers_original = copy.copy(headers)
+
+        keys_to_skip = ['date', 'unit_system', 'date_format', 'start_date']
+
         for key in object_properties:
-            if key == 'date' or key == 'unit_system' or key == 'date_format':
+            if key in keys_to_skip:
                 continue
             if inverted_nexus_map[key] not in headers:
                 headers.append(inverted_nexus_map[key])
                 additional_headers.append(inverted_nexus_map[key])
         additional_column_string = ' '.join(additional_headers)
         split_comments = str(file_content[header_index]).split('!', 1)
         if len(split_comments) == 1:
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_constraint_operations.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_constraint_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_file_operations.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_file_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_load_well_list.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_load_well_list.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusNetwork import NexusNetwork
 
 
 class ModifyObjectOperations:
     def __init__(self, object_to_modify: Any) -> None:
+        """Initialises the ModifyObjectOperations class.
+
+        Args:
+            object_to_modify (Any): Passed in object to modify and pass back out.
+        """
         self.object_to_modify = object_to_modify
 
     def modify_network_object(self, object_to_modify: dict[str, None | str | float | int],
                               new_properties: dict[str, None | str | float | int], network: NexusNetwork) -> None:
         """Modifies an existing object based on a matching dictionary of properties (partial matches allowed if
         precisely 1 matching object is found).
         Updates the properties with properties in the new_properties dictionary.
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-2.1.0/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusNetwork import NexusNetwork
 
 
 class RemoveObjectOperations:
     def __init__(self, network: Optional[NexusNetwork], table_header: str, table_footer: str) -> None:
+        """Initialises the RemoveObjectOperations class.
+
+        Args:
+            network (Optional[NexusNetwork]): NexusNetwork object to remove the object from.
+            table_header (str): The string that represents the start of the table in the file.
+            table_footer (str): The string that represents the end of the table in the file.
+        """
         self.table_header = table_header
         self.table_footer = table_footer
         self.__network = network
 
     @staticmethod
     def remove_object_from_memory_by_id(list_obj: list[T], id_to_remove: UUID) -> tuple[Any, list[Any]]:
         """Directly removes an object from a list of objects based on the id attribute of that object."""
```

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/rel_perm_operations.py` & `ressimpy-2.1.0/ResSimpy/Nexus/rel_perm_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-2.1.0/ResSimpy/Nexus/runcontrol_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Node.py` & `ressimpy-2.1.0/ResSimpy/Node.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/NodeConnection.py` & `ressimpy-2.1.0/ResSimpy/NodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py` & `ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,26 @@
     __penetration_direction: Optional[PenetrationDirectionEnum]
     __is_open: bool
     __refinement_name: Optional[str]
 
     def __init__(self, date: str, i: Optional[int] = None, j: Optional[int] = None, k: Optional[int] = None,
                  penetration_direction: Optional[PenetrationDirectionEnum] = None, is_open: Optional[bool] = None,
                  refinement_name: Optional[str] = None) -> None:
+        """Initialises the OpenGoSimCompletion class.
+
+        Args:
+            date (str): The date of the completion.
+            i (Optional[int]): The i index of the completion.
+            j (Optional[int]): The j index of the completion.
+            k (Optional[int]): The k index of the completion.
+            penetration_direction (Optional[PenetrationDirectionEnum]): The direction of the penetration for the
+            completion.
+            is_open (Optional[bool]): Whether the completion is open or closed. If True the completion is open.
+            refinement_name (Optional[str]): The grid refinement name that the completion is applied to.
+        """
         self.__penetration_direction = penetration_direction
         self.__is_open = is_open if is_open is not None else True
         self.__refinement_name = refinement_name
         super().__init__(i=i, j=j, k=k, date=date, date_format=DateFormat.DD_MMM_YYYY)
 
     def __repr__(self) -> str:
         return f"i: {self.i} j: {self.j} k: {self.k}"
```

### Comparing `ressimpy-2.0.9/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py` & `ressimpy-2.1.0/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 from ResSimpy.Well import Well
 
 
 @dataclass(kw_only=True)
 class OpenGoSimWell(Well):
 
     def __init__(self, well_name: str, completions: Sequence[Completion], well_type: WellType) -> None:
+        """Initialises the OpenGoSimWell class.
+
+        Args:
+            well_name (str): The name of the well.
+            completions (Sequence[Completion]): The completions of the well.
+            well_type (WellType): The type of the well as a WellType Enum.
+        """
         if not isinstance(completions, list):
             completions = list(completions)
 
         super().__init__(well_name=well_name, completions=completions, unit_system=UnitSystem.ENGLISH,
                          well_type=well_type)
 
     @property
```

### Comparing `ressimpy-2.0.9/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py` & `ressimpy-2.1.0/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 
 @dataclass(kw_only=True, init=False)
 class OpenGoSimNetwork(Network):
     # Class to be implemented later
 
     def __init__(self) -> None:
+        """Initialises the OpenGoSimNetwork class.
+
+        Args:
+            To be implemented later.
+        """
         self.nodes = None
         self.connections = None
         self.constraints = None
         self.targets = None
 
     def __repr__(self) -> str:
         # TODO: implement this
```

### Comparing `ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py` & `ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/OpenGoSim/OpenGoSimSimulator.py` & `ressimpy-2.1.0/ResSimpy/OpenGoSim/OpenGoSimSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,19 @@
 
 @dataclass(kw_only=True)
 class OpenGoSimSimulator(Simulator):
     __simulation_type: SimulationType
     __final_date: Optional[str]
 
     def __init__(self, origin: str) -> None:
+        """Initialises the OpenGoSimSimulator class.
+
+        Args:
+            origin (str): The path to the model file.
+        """
         super().__init__()
         self._origin = origin
         self._wells: OpenGoSimWells = OpenGoSimWells()
 
         self.__final_date = None
 
         # Model parts not implemented yet. Will be replaced by OGS specific classes
@@ -204,15 +209,15 @@
 
         loaded_well = OpenGoSimWell(well_type=well_type, well_name=well_name, completions=completions_to_add)
 
         self._wells._wells.append(loaded_well)
         self._wells._wells_loaded = True
 
     @staticmethod
-    def get_fluid_type(surface_file_name: str) -> str:
+    def get_fluid_type(surface_file_content: list[str]) -> str:
         raise NotImplementedError("Not implemented for OGS yet")
 
     def set_output_path(self, path: str) -> None:
         raise NotImplementedError("Not implemented for OGS yet")
 
     def get_date_format(self) -> str:
         """Returns date format as a string."""
```

### Comparing `ressimpy-2.0.9/ResSimpy/OperationsMixin.py` & `ressimpy-2.1.0/ResSimpy/OperationsMixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from ResSimpy.File import File
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusNetwork import Network
 
 
 class NetworkOperationsMixIn(ABC):
     def __init__(self, parent_network: Network) -> None:
+        """Initialises the NetworkOperationsMixIn class.
+
+        Args:
+            parent_network (Network): The parent network that the object is a part of.
+        """
         self.__parent_network = parent_network
 
     @abstractmethod
     def get_all(self) -> Sequence[Any]:
         raise NotImplementedError("Implement this in the derived class")
 
     @abstractmethod
```

### Comparing `ressimpy-2.0.9/ResSimpy/Simulator.py` & `ressimpy-2.1.0/ResSimpy/Simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     def model_files(self) -> File:
         return self._model_files
 
     """ Class Methods """
 
     @staticmethod
     @abstractmethod
-    def get_fluid_type(surface_file_name: str) -> str:
+    def get_fluid_type(surface_file_content: list[str]) -> str:
         raise NotImplementedError("This method has not been implemented for this simulator yet")
 
     @abstractmethod
     def set_output_path(self, path: str) -> None:
         raise NotImplementedError("Implement this method on the derived class")
 
     @abstractmethod
```

### Comparing `ressimpy-2.0.9/ResSimpy/SolverParameters.py` & `ressimpy-2.1.0/ResSimpy/SolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Target.py` & `ressimpy-2.1.0/ResSimpy/Target.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Units/AttributeMapping.py` & `ressimpy-2.1.0/ResSimpy/Units/AttributeMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py` & `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 
 class BaseUnitMapping(ABC):
     """Base class for handling the mapping between ResSimpy attributes and the unit type of the attribute."""
     attribute_map: Mapping[str, UnitDimension]
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the BaseUnitMapping class.
+
+        Args:
+            unit_system (None | UnitSystem): The unit system to use for the unit mapping.
+        """
         self.unit_system = unit_system
 
     def get_unit_for_attribute(self, attribute_name: str, uppercase: bool = False) -> str:
         """Returns the unit variable for the given unit system.
 
         Args:
             attribute_name (str): name of the attribute to get the unit for
```

### Comparing `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py` & `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,19 @@
         'polymer_block_radius': Length(),
         'polymer_well_radius': Length(),
         'rel_perm_end_point': Dimensionless(),
         'kh_mult': Dimensionless(),
     }
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the CompletionUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): The unit system to use for the unit mapping.
+        """
         super().__init__(unit_system=unit_system)
 
     @property
     def i(self) -> str:
         """Returns the unit for i."""
         return self.get_unit_for_attribute('i')
```

### Comparing `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py` & `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,19 @@
         'max_cum_liquid_prod': SurfaceVolumesLiquid(),
         'qmult_oil_rate': SurfaceRatesLiquid(),
         'qmult_water_rate': SurfaceRatesLiquid(),
         'qmult_gas_rate': SurfaceRatesGas(),
     }
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the ConstraintUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): The unit system to use for the unit mapping.
+        """
         super().__init__(unit_system=unit_system)
 
     @property
     def max_surface_oil_rate(self) -> str:
         """Returns the unit for max_surface_oil_rate."""
         return self.get_unit_for_attribute('max_surface_oil_rate')
```

### Comparing `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py` & `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
                                   )
 
 
 class WaterUnits(BaseUnitMapping):
     """Unit types for the attributes of water methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the WaterUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): The unit system to use for the unit mapping.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'temperature': Temperature(),
         'reference_pressure': Pressure(),
         'water_density': Density(),
         'water_compressibility': Compressibility(),
@@ -64,14 +69,19 @@
         return self.get_unit_for_attribute('water_viscosity_compressibility')
 
 
 class SeparatorUnits(BaseUnitMapping):
     """Unit types for the attributes of separator methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the SeparatorUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'temperature': Temperature(),
         'pressure': Pressure(),
         'standard_temperature': Temperature(),
         'standard_pressure': Pressure(),
@@ -98,14 +108,19 @@
         return self.get_unit_for_attribute('standard_pressure')
 
 
 class RockUnits(BaseUnitMapping):
     """Unit types for the attributes of rock methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the RockUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'rock_compressibility': Compressibility(),
         'rock_permeability_compressibility': Compressibility(),
         'reference_pressure': Pressure(),
         'pressure': Pressure(),
@@ -138,14 +153,19 @@
         return self.get_unit_for_attribute('delta_pressure')
 
 
 class RelPermUnits(BaseUnitMapping):
     """Unit types for the attributes of relative permeability and capillary pressure methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the RelPermUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'water_oil_capillary_pressure': Pressure(),
         'gas_oil_capillary_pressure': Pressure(),
         'gas_water_capillary_pressure': Pressure(),
         'interfacial_tension_threshold_for_relperm_adjustment': InterfacialTension(),
@@ -178,14 +198,19 @@
         return self.get_unit_for_attribute('reference_interfacial_tension_for_capillary_pressure_adjustment')
 
 
 class HydraulicsUnits(BaseUnitMapping):
     """Unit types for the attributes of hydraulics, gaslift, valve, etc. methods."""
 
     def __init__(self, unit_system: None | UnitSystem, ratio_thousands: bool = True) -> None:
+        """Initialises the HydraulicsUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         self.ratio_thousands = ratio_thousands
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'surface_oil_rate': SurfaceRatesLiquid(),  # For use in hyd & gaslift methods
         'surface_liquid_rate': SurfaceRatesLiquid(),
         'surface_water_rate': SurfaceRatesLiquid(),
@@ -375,14 +400,19 @@
         return self.get_unit_for_attribute('valve_coefficient')
 
 
 class EquilUnits(BaseUnitMapping):
     """Unit types for the attributes of equilibration methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the EquilUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'initial_pressure': Pressure(),
         'datum_depth': Length(),
         'depth': Length(),
         'x': Length(),
@@ -475,14 +505,19 @@
         return self.get_unit_for_attribute('oil_api_gravity')
 
 
 class AquiferUnits(BaseUnitMapping):
     """Unit types for the attributes of Aquifer methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the AquiferUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'carter_tracy_constant': ReservoirVolumeOverPressure(),
         'total_compressibility': Compressibility(),
         'porosity': Dimensionless(),
         'thickness': Length(),
@@ -587,14 +622,19 @@
         return self.get_unit_for_attribute('initial_aquifer_volume')
 
 
 class PVTUnits(BaseUnitMapping):
     """Unit types for the attributes of PVT methods."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the PVTUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): unit system to get the unit from.
+        """
         super().__init__(unit_system=unit_system)
 
     attribute_map: Mapping[str, UnitDimension] = {
         'pressure': Pressure(),
         'temperature': Temperature(),
         'delta_pressure': DeltaPressure(),
         'oil_density': Density(),
```

### Comparing `ressimpy-2.0.9/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py` & `ressimpy-2.1.0/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,19 @@
                                   NonDarcySkin, ThermalConductivity)
 
 
 class NetworkUnits(BaseUnitMapping):
     """Unit types for the attributes of a well connection, wellhead, wellbore, etc."""
 
     def __init__(self, unit_system: None | UnitSystem) -> None:
+        """Initialises the NetworkUnits class.
+
+        Args:
+            unit_system (None | UnitSystem): The unit system to use for the unit mapping.
+        """
         super().__init__(unit_system=unit_system)
         self.attribute_map: Mapping[str, UnitDimension] = {
             'bhdepth': Length(),
             'depth': Length(),
             'datum_depth': Length(),
             'x_pos': Length(),
             'y_pos': Length(),
```

### Comparing `ressimpy-2.0.9/ResSimpy/Units/Units.py` & `ressimpy-2.1.0/ResSimpy/Units/Units.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Utils/factory_methods.py` & `ressimpy-2.1.0/ResSimpy/Utils/factory_methods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Utils/generic_repr.py` & `ressimpy-2.1.0/ResSimpy/Utils/generic_repr.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-2.1.0/ResSimpy/Utils/invert_nexus_map.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-2.1.0/ResSimpy/Utils/obj_to_table_string.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-2.1.0/ResSimpy/Utils/to_dict_generic.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.0.9/ResSimpy/Well.py` & `ressimpy-2.1.0/ResSimpy/Well.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,22 @@
     _completions: list[Completion]
     _well_name: str
     __unit_system: UnitSystem
     _well_type: Optional[WellType]
 
     def __init__(self, well_name: str, completions: list[Completion], unit_system: UnitSystem,
                  well_type: Optional[WellType] = None) -> None:
+        """Initialises the ConstraintUnits class.
+
+        Args:
+            well_name (str): The name of the well.
+            completions (list[Completion]): A list of all of the completions on the well.
+            unit_system (None | UnitSystem): The unit system associated with the properties on this well.
+            well_type (Optional[WellType]): The type of the well represented by a WellType Enum.
+        """
         self._well_name = well_name
         self._completions = completions
         self.__unit_system = unit_system
         self._well_type = well_type
 
     @property
     def completions(self) -> list[Completion]:
```

### Comparing `ressimpy-2.0.9/ResSimpy/WellConnection.py` & `ressimpy-2.1.0/ResSimpy/Wellbore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from __future__ import annotations
+
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
 from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
-class WellConnection(DataObjectMixin, ABC):
-    name: Optional[str] = None
+class Wellbore(DataObjectMixin, ABC):
     date: Optional[str] = None
     unit_system: Optional[UnitSystem] = None
-
-    bhdepth: Optional[float] = None
-    datum_depth: Optional[float] = None
-    x_pos: Optional[float] = None
-    y_pos: Optional[float] = None
-    length: Optional[float] = None
-    temperature: Optional[float] = None
+    name: Optional[str] = None
     diameter: Optional[float] = None
-    roughness: Optional[float] = None
     inner_diameter: Optional[float] = None
-    productivity_index: Optional[float] = None
+    roughness: Optional[float] = None
 
     @property
     def units(self) -> NetworkUnits:
         """Returns the attribute to unit map for the WellConnection."""
         return NetworkUnits(self.unit_system)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Wellbore.py` & `ressimpy-2.1.0/ResSimpy/Wellhead.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
-
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
-from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.DataObjectMixin import DataObjectMixin
+from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
-class Wellbore(DataObjectMixin, ABC):
+class Wellhead(DataObjectMixin, ABC):
+    well: Optional[str] = None
+    name: Optional[str] = None
     date: Optional[str] = None
     unit_system: Optional[UnitSystem] = None
-    name: Optional[str] = None
-    diameter: Optional[float] = None
-    inner_diameter: Optional[float] = None
-    roughness: Optional[float] = None
+    wellhead_type: Optional[str] = None
+    depth: Optional[float] = None
+    x_pos: Optional[float] = None
+    y_pos: Optional[float] = None
 
     @property
     def units(self) -> NetworkUnits:
         """Returns the attribute to unit map for the WellConnection."""
         return NetworkUnits(self.unit_system)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Wellhead.py` & `ressimpy-2.1.0/ResSimpy/WellConnection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,42 @@
 from __future__ import annotations
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
-from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.DataObjectMixin import DataObjectMixin
 from ResSimpy.Units.AttributeMappings.NetworkUnitMapping import NetworkUnits
 
 
 @dataclass(repr=False)
-class Wellhead(DataObjectMixin, ABC):
-    well: Optional[str] = None
+class WellConnection(DataObjectMixin, ABC):
     name: Optional[str] = None
     date: Optional[str] = None
     unit_system: Optional[UnitSystem] = None
-    wellhead_type: Optional[str] = None
-    depth: Optional[float] = None
+
+    bhdepth: Optional[float] = None
+    datum_depth: Optional[float] = None
     x_pos: Optional[float] = None
     y_pos: Optional[float] = None
+    length: Optional[float] = None
+    temperature: Optional[float] = None
+    diameter: Optional[float] = None
+    roughness: Optional[float] = None
+    inner_diameter: Optional[float] = None
+    productivity_index: Optional[float] = None
+    hyd_method: Optional[str] = None
+    crossflow: Optional[str] = None
+    crossshut: Optional[str] = None
+    inj_mobility: Optional[str] = None
+    polymer: Optional[str] = None
+    stream: Optional[str] = None
+    group: Optional[str] = None
+    i: Optional[int] = None
+    j: Optional[int] = None
+    drainage_radius: Optional[float] = None
+    pvt_method: Optional[int] = None
 
     @property
     def units(self) -> NetworkUnits:
         """Returns the attribute to unit map for the WellConnection."""
         return NetworkUnits(self.unit_system)
```

### Comparing `ressimpy-2.0.9/ResSimpy/Wells.py` & `ressimpy-2.1.0/ResSimpy/Wells.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 @dataclass(kw_only=True)
 class Wells(ABC):
     _wells: Sequence[Well] = field(default_factory=list)
     _wells_loaded: bool = False
 
     def __init__(self, assume_loaded: bool = False) -> None:
+        """Initialises the Wells class.
+
+        Args:
+            assume_loaded (bool): whether the class should assume that the Wells have already been loaded.
+        """
         self._wells_loaded = assume_loaded
         self._wells = []
 
     @property
     def wells(self) -> Sequence[Well]:
         if not self._wells_loaded:
             self._load()
```

### Comparing `ressimpy-2.0.9/pyproject.toml` & `ressimpy-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ResSimpy"
-version = "2.0.9" # Set at build time
+version = "2.1.0" # Set at build time
 description = "A Python library for working with Reservoir Simulator Models."
 authors = ["BP"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["ResSimpy", "Reservoir Engineering"]
 classifiers = [
     "Operating System :: OS Independent",
@@ -65,15 +65,15 @@
 ignore = ["UP007",  "ANN101", "N999", "UP035", "S105", "N802", "S106", "S107", "UP015", "ANN401", "ANN102", "D202",
     "D105", "D203", "D213", "RUF010", "I001", "B028", "COM812", "PD901",
     # To fix later:
     "ANN001", # Types
    "ANN201", # Types
    "ANN202", # Types
     "C901", # Complexity
-    "D102", "D100", "D103", "D107", "D101", "D205", "D401", "D417", "D104", "D106", # Docstrings
+    "D102", "D100", "D103", "D101", "D205", "D401", "D417", "D104", "D106", # Docstrings
     "FA100", # TODO need to remove references to Union, Optional, capital lettered typing (e.g. List)
              # from typings module.
     ]
 exclude = ["./tests"]
 
 [tool.ruff.pydocstyle]
 # Use Google-style docstrings.
```

### Comparing `ressimpy-2.0.9/PKG-INFO` & `ressimpy-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResSimpy
-Version: 2.0.9
+Version: 2.1.0
 Summary: A Python library for working with Reservoir Simulator Models.
 License: Apache-2.0
 Keywords: ResSimpy,Reservoir Engineering
 Author: BP
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

