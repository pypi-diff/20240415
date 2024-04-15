# Comparing `tmp/synrbl-0.0.5.tar.gz` & `tmp/synrbl-0.0.6.tar.gz`

## Comparing `synrbl-0.0.5.tar` & `synrbl-0.0.6.tar`

### file list

```diff
@@ -1,141 +1,142 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.5/.coveragerc
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.5/.gitattributes
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.5/lint_check.sh
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 synrbl-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.5/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 synrbl-0.0.5/.github/workflows/test-and-lint.yml
--rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Raw_data/Golden/Golden.csv
--rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Raw_data/Jaworski/complex.csv
--rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Raw_data/Jaworski/patent.csv
--rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Raw_data/Jaworski/typical.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Raw_data/USPTO/USPTO_50K.csv
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Rules/automated_rules.json.gz
--rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/Jaworski.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/USPTO_50K.csv
--rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/USPTO_diff.csv
--rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/USPTO_random_class.csv
--rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/USPTO_unbalance_class.csv
--rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/golden_dataset.csv
--rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/validation_set.csv
--rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.5/Data/Validation_set/validation_set.json
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.5/Docs/Examples/notebook.ipynb
--rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.5/Docs/Images/Flowchart.png
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.5/Docs/Paper_fig/figures.py
--rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.5/Pipeline/Validation/Analysis/Analysis_vis.ipynb
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
--rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.5/Scripts/result_evaluation.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.5/Scripts/synrbl_pilot.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.5/Scripts/validation_set_interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynChemImputer/test_appeal_reaction.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynChemImputer/test_peroxide_imputer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/test_merge.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/test_model.py
--rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/test_rules.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/test_structure.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_molcurator.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_mcs_process.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynProcessor/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynProcessor/test_check_carbon_balance.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynProcessor/test_rmsi_comparator.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynProcessor/test_rmsi_decomposer.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynProcessor/test_rmsi_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/test_auto_extract_rules.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/test_auto_extract_smiles.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/test_rule_constraint.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/test_rule_data_manager.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/test_synthetic_rule_imputer.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynRuleImputer/test_synthetic_rule_matcher.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynUtils/test_chem_utils.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynUtils/test_functional_group_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynVis/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 synrbl-0.0.5/Test/SynVis/test_reaction_visualizer.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/__main__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/confidence_prediction.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/main.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/mcs.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/postprocess.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/preprocess.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/rsmi_utils.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/rule_based.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/analysis_process.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/analysis_utils.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/eda_analysis.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/feature_analysis.py
--rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/scoring_function.dump
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynAnalysis/visualizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynChemImputer/appel_reaction.py
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynChemImputer/functional_group_checker.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynChemImputer/peroxide_imputer.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynCmd/__init__.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynCmd/cmd_benchmark.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynCmd/cmd_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynCmd/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/compound_rules.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/expand_rules.json
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/merge.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/merge_rules.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/merge_rules_example.json
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/model.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/rules.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/structure.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/molcurator.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/mcs_process.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynProcessor/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynProcessor/check_carbon_balance.py
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynProcessor/rsmi_both_side_process.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynProcessor/rsmi_comparator.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynProcessor/rsmi_decomposer.py
--rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynProcessor/rsmi_processing.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/auto_extract_rules.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/auto_extract_smiles.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/rule_data_manager.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/rules_manager.json.gz
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/synthetic_rule_constraint.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/synthetic_rule_imputer.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynRuleImputer/synthetic_rule_matcher.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynUtils/__init__.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynUtils/chem_utils.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynUtils/common.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynUtils/data_utils.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynUtils/functional_group_utils.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynUtils/rsmi_utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynVis/__init__.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynVis/mcs_visualizer.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.5/synrbl/SynVis/reaction_visualizer.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.5/LICENSE
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 synrbl-0.0.5/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 synrbl-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.6/.coveragerc
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.6/.gitattributes
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.6/lint_check.sh
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 synrbl-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.6/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 synrbl-0.0.6/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Golden/Golden.csv
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Jaworski/complex.csv
+-rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Jaworski/patent.csv
+-rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Jaworski/typical.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/USPTO/USPTO_50K.csv
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Rules/automated_rules.json.gz
+-rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/Jaworski.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_50K.csv
+-rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_diff.csv
+-rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_random_class.csv
+-rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/golden_dataset.csv
+-rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/validation_set.csv
+-rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/validation_set.json
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.6/Docs/Examples/notebook.ipynb
+-rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.6/Docs/Images/Flowchart.png
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.6/Docs/Paper_fig/figures.py
+-rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/Analysis_vis.ipynb
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.6/Scripts/result_evaluation.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.6/Scripts/synrbl_pilot.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.6/Scripts/validation_set_interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynChemImputer/test_appeal_reaction.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynChemImputer/test_peroxide_imputer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_merge.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_model.py
+-rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_rules.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_structure.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_molcurator.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_process.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_check_carbon_balance.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_rmsi_comparator.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_rmsi_decomposer.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_rmsi_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_rules.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_smiles.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_rule_constraint.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_rule_data_manager.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_matcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynUtils/__init__.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynUtils/test_chem_utils.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynUtils/test_functional_group_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynVis/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynVis/test_reaction_visualizer.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/__main__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/confidence_prediction.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/main.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/mcs.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/postprocess.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/preprocess.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/rsmi_utils.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/rule_based.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/analysis_process.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/analysis_utils.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/eda_analysis.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/feature_analysis.py
+-rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/scoring_function.dump
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/visualizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/appel_reaction.py
+-rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/functional_group_checker.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/peroxide_imputer.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/__init__.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/cmd_benchmark.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/cmd_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/compound_rules.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/expand_rules.json
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/merge.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/merge_rules.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/merge_rules_example.json
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/model.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/rules.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/structure.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/molcurator.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_process.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/check_carbon_balance.py
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_both_side_process.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_comparator.py
+-rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_decomposer.py
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_processing.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_rules.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_smiles.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/rule_data_manager.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/rules_manager.json.gz
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_constraint.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_matcher.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/__init__.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/chem_utils.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/common.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/data_utils.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/functional_group_utils.py
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/rsmi_utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynVis/__init__.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynVis/mcs_visualizer.py
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynVis/reaction_visualizer.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 synrbl-0.0.6/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 synrbl-0.0.6/PKG-INFO
```

### Comparing `synrbl-0.0.5/.github/workflows/publish-package.yml` & `synrbl-0.0.6/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/.github/workflows/test-and-lint.yml` & `synrbl-0.0.6/.github/workflows/test-and-lint.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Raw_data/Golden/Golden.csv` & `synrbl-0.0.6/Data/Raw_data/Golden/Golden.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Raw_data/Jaworski/complex.csv` & `synrbl-0.0.6/Data/Raw_data/Jaworski/complex.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Raw_data/Jaworski/patent.csv` & `synrbl-0.0.6/Data/Raw_data/Jaworski/patent.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Raw_data/Jaworski/typical.csv` & `synrbl-0.0.6/Data/Raw_data/Jaworski/typical.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Raw_data/USPTO/USPTO_50K.csv` & `synrbl-0.0.6/Data/Raw_data/USPTO/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Rules/automated_rules.json.gz` & `synrbl-0.0.6/Data/Rules/automated_rules.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/Jaworski.csv` & `synrbl-0.0.6/Data/Validation_set/Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/USPTO_50K.csv` & `synrbl-0.0.6/Data/Validation_set/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/USPTO_diff.csv` & `synrbl-0.0.6/Data/Validation_set/USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/USPTO_random_class.csv` & `synrbl-0.0.6/Data/Validation_set/USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/USPTO_unbalance_class.csv` & `synrbl-0.0.6/Data/Validation_set/USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/golden_dataset.csv` & `synrbl-0.0.6/Data/Validation_set/golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/validation_set.csv` & `synrbl-0.0.6/Data/Validation_set/validation_set.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Data/Validation_set/validation_set.json` & `synrbl-0.0.6/Data/Validation_set/validation_set.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Docs/Examples/notebook.ipynb` & `synrbl-0.0.6/Docs/Examples/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Docs/Images/Flowchart.png` & `synrbl-0.0.6/Docs/Images/Flowchart.png`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Docs/Paper_fig/figures.py` & `synrbl-0.0.6/Docs/Paper_fig/figures.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Pipeline/Validation/Analysis/Analysis_vis.ipynb` & `synrbl-0.0.6/Pipeline/Validation/Analysis/Analysis_vis.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv` & `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv` & `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv` & `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv` & `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv` & `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Scripts/result_evaluation.py` & `synrbl-0.0.6/Scripts/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Scripts/synrbl_pilot.py` & `synrbl-0.0.6/Scripts/synrbl_pilot.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Scripts/validation_set_interface.py` & `synrbl-0.0.6/Scripts/validation_set_interface.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynChemImputer/test_appeal_reaction.py` & `synrbl-0.0.6/Test/SynChemImputer/test_appeal_reaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 from synrbl.SynChemImputer.appel_reaction import (
     AppelReaction,
-)  # Make sure to import your class correctly
+)
 
 
 class TestAppelReaction(unittest.TestCase):
     def test_check_alcohol_group(self):
         # Test with a molecule containing an alcohol group
         self.assertTrue(AppelReaction.check_alcohol_group("CCO"))  # Ethanol
```

### Comparing `synrbl-0.0.5/Test/SynChemImputer/test_peroxide_imputer.py` & `synrbl-0.0.6/Test/SynChemImputer/test_peroxide_imputer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 from synrbl.SynChemImputer.peroxide_imputer import (
     PeroxidGroupImputer,
-)  # Replace with the actual module name
+)
 
 
 class TestPeroxidGroupImputer(unittest.TestCase):
     def setUp(self):
         self.pero_imputer = PeroxidGroupImputer()
 
     def test_fix_peroxid_group(self):
```

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/test_merge.py` & `synrbl-0.0.6/Test/SynMCSImputer/test_merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/test_model.py` & `synrbl-0.0.6/Test/SynMCSImputer/test_model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/test_rules.py` & `synrbl-0.0.6/Test/SynMCSImputer/test_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/test_structure.py` & `synrbl-0.0.6/Test/SynMCSImputer/test_structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/test_utils.py` & `synrbl-0.0.6/Test/SynMCSImputer/test_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py` & `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py` & `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_molcurator.py` & `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py` & `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py` & `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py` & `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_mcs_process.py` & `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py` & `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynProcessor/test_check_carbon_balance.py` & `synrbl-0.0.6/Test/SynProcessor/test_check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynProcessor/test_rmsi_comparator.py` & `synrbl-0.0.6/Test/SynProcessor/test_rmsi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynProcessor/test_rmsi_decomposer.py` & `synrbl-0.0.6/Test/SynProcessor/test_rmsi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynProcessor/test_rmsi_processing.py` & `synrbl-0.0.6/Test/SynProcessor/test_rmsi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynRuleImputer/test_auto_extract_rules.py` & `synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynRuleImputer/test_auto_extract_smiles.py` & `synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynRuleImputer/test_rule_constraint.py` & `synrbl-0.0.6/Test/SynRuleImputer/test_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynRuleImputer/test_rule_data_manager.py` & `synrbl-0.0.6/Test/SynRuleImputer/test_rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynRuleImputer/test_synthetic_rule_imputer.py` & `synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynRuleImputer/test_synthetic_rule_matcher.py` & `synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynUtils/test_chem_utils.py` & `synrbl-0.0.6/Test/SynUtils/test_chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynUtils/test_functional_group_utils.py` & `synrbl-0.0.6/Test/SynUtils/test_functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/Test/SynVis/test_reaction_visualizer.py` & `synrbl-0.0.6/Test/SynVis/test_reaction_visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import unittest
-
 from synrbl.SynVis import ReactionVisualizer
 from PIL import Image
 
 
 class TestReactionVisualizer(unittest.TestCase):
     def setUp(self):
         self.visualizer = ReactionVisualizer()
```

### Comparing `synrbl-0.0.5/synrbl/confidence_prediction.py` & `synrbl-0.0.6/synrbl/confidence_prediction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/main.py` & `synrbl-0.0.6/synrbl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ):
         self.__reaction_col = reaction_col
         self.__id_col = id_col
         self.solved_col = "solved"
         self.mcs_data_col = "mcs"
         self.columns = [
             "input_reaction",
-            "reaction",
+            reaction_col,
             "solved",
             "solved_by",
             "confidence",
             "rules",
         ]
         self.confidence_threshold = confidence_threshold
         self.input_validator = Validator(reaction_col, "input-balanced", n_jobs=n_jobs)
```

### Comparing `synrbl-0.0.5/synrbl/mcs.py` & `synrbl-0.0.6/synrbl/mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/postprocess.py` & `synrbl-0.0.6/synrbl/postprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/preprocess.py` & `synrbl-0.0.6/synrbl/preprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/rsmi_utils.py` & `synrbl-0.0.6/synrbl/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/rule_based.py` & `synrbl-0.0.6/synrbl/rule_based.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynAnalysis/analysis_process.py` & `synrbl-0.0.6/synrbl/SynAnalysis/analysis_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynAnalysis/analysis_utils.py` & `synrbl-0.0.6/synrbl/SynAnalysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynAnalysis/eda_analysis.py` & `synrbl-0.0.6/synrbl/SynAnalysis/eda_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynAnalysis/feature_analysis.py` & `synrbl-0.0.6/synrbl/SynAnalysis/feature_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynAnalysis/scoring_function.dump` & `synrbl-0.0.6/synrbl/SynAnalysis/scoring_function.dump`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynAnalysis/visualizer.py` & `synrbl-0.0.6/synrbl/SynAnalysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynChemImputer/appel_reaction.py` & `synrbl-0.0.6/synrbl/SynChemImputer/appel_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynChemImputer/functional_group_checker.py` & `synrbl-0.0.6/synrbl/SynChemImputer/functional_group_checker.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynChemImputer/peroxide_imputer.py` & `synrbl-0.0.6/synrbl/SynChemImputer/peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynCmd/__init__.py` & `synrbl-0.0.6/synrbl/SynCmd/__init__.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynCmd/cmd_benchmark.py` & `synrbl-0.0.6/synrbl/SynCmd/cmd_benchmark.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynCmd/cmd_run.py` & `synrbl-0.0.6/synrbl/SynCmd/cmd_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     test_parser.add_argument(
         "inputfile", help="Path to file containing reaction SMILES."
     )
     test_parser.add_argument("-o", default=None, help="Path to output file.")
     test_parser.add_argument(
         "-p",
         default=-1,
+        type=int,
         help="The number of parallel process. (Default -1 => # of processors)",
     )
     test_parser.add_argument(
         "--col",
         default="reaction",
         help="The reactions column name for in the input .csv file. "
         + "(Default: 'reaction')",
```

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/compound_rules.json` & `synrbl-0.0.6/synrbl/SynMCSImputer/compound_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/expand_rules.json` & `synrbl-0.0.6/synrbl/SynMCSImputer/expand_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/merge.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/merge_rules.json` & `synrbl-0.0.6/synrbl/SynMCSImputer/merge_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/model.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/rules.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/structure.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/utils.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/molcurator.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/mcs_process.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py` & `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynProcessor/check_carbon_balance.py` & `synrbl-0.0.6/synrbl/SynProcessor/check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynProcessor/rsmi_both_side_process.py` & `synrbl-0.0.6/synrbl/SynProcessor/rsmi_both_side_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynProcessor/rsmi_comparator.py` & `synrbl-0.0.6/synrbl/SynProcessor/rsmi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynProcessor/rsmi_decomposer.py` & `synrbl-0.0.6/synrbl/SynProcessor/rsmi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynProcessor/rsmi_processing.py` & `synrbl-0.0.6/synrbl/SynProcessor/rsmi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/auto_extract_rules.py` & `synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/auto_extract_smiles.py` & `synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/rule_data_manager.py` & `synrbl-0.0.6/synrbl/SynRuleImputer/rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/rules_manager.json.gz` & `synrbl-0.0.6/synrbl/SynRuleImputer/rules_manager.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/synthetic_rule_constraint.py` & `synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/synthetic_rule_imputer.py` & `synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynRuleImputer/synthetic_rule_matcher.py` & `synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynUtils/chem_utils.py` & `synrbl-0.0.6/synrbl/SynUtils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynUtils/data_utils.py` & `synrbl-0.0.6/synrbl/SynUtils/data_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynUtils/functional_group_utils.py` & `synrbl-0.0.6/synrbl/SynUtils/functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynUtils/rsmi_utils.py` & `synrbl-0.0.6/synrbl/SynUtils/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynVis/mcs_visualizer.py` & `synrbl-0.0.6/synrbl/SynVis/mcs_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/synrbl/SynVis/reaction_visualizer.py` & `synrbl-0.0.6/synrbl/SynVis/reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/.gitignore` & `synrbl-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/LICENSE` & `synrbl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/README.md` & `synrbl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.5/pyproject.toml` & `synrbl-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synrbl"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
 	{name="Tieu Long Phan", email="long.tieu_phan@uni-leipzig.de"}, 
 	{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}
 	]
 description = "Synthesis Rebalancing Framework for Computational Chemistry"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `synrbl-0.0.5/PKG-INFO` & `synrbl-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: synrbl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Synthesis Rebalancing Framework for Computational Chemistry
 Project-URL: homepage, https://github.com/TieuLongPhan/SynRBL
 Project-URL: source, https://github.com/TieuLongPhan/SynRBL
 Project-URL: issues, https://github.com/TieuLongPhan/SynRBL/issues
 Author-email: Tieu Long Phan <long.tieu_phan@uni-leipzig.de>, Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

