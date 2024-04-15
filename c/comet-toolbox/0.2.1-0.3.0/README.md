# Comparing `tmp/comet_toolbox-0.2.1.tar.gz` & `tmp/comet_toolbox-0.3.0.tar.gz`

## Comparing `comet_toolbox-0.2.1.tar` & `comet_toolbox-0.3.0.tar`

### file list

```diff
@@ -1,230 +1,229 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/.gitattributes
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/simulation.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/__init__.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/cifti.py
--rwxr-xr-x   0        0        0     3968 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/data.py
--rw-r--r--   0        0        0    24483 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/graph.py
--rw-r--r--   0        0        0    69570 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/gui.py
--rwxr-xr-x   0        0        0    44939 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/methods.py
--rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/multiverse.py
--rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/simulation.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/simulation.txt
--rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/single_state.txt
--rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
--rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/atlas/README.md
--rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
--rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/img/badge.svg
--rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/img/content.drawio
--rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/img/content.png
--rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/img/gui.png
--rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/src/comet/resources/img/logo.png
--rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_analysis.ipynb
--rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_dfc.ipynb
--rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_graph.ipynb
--rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_multiverse.ipynb
--rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_data/abide_50008.txt
--rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_data/aomic_multi.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_data/simulation.txt
--rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/example_data/xcpd.tsv
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_1.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_10.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_11.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_12.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_13.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_14.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_15.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_16.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_17.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_18.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_19.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_2.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_20.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_21.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_22.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_23.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_24.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_25.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_26.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_27.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_28.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_29.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_3.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_30.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_31.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_32.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_33.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_34.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_35.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_36.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_37.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_38.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_39.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_4.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_40.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_41.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_42.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_43.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_44.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_45.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_46.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_47.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_48.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_49.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_5.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_50.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_51.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_52.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_53.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_54.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_55.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_56.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_57.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_58.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_59.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_6.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_60.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_61.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_62.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_63.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_64.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_65.py
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_66.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_67.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_68.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_69.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_7.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_70.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_71.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_72.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_73.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_74.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_75.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_76.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_77.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_78.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_79.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_8.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_80.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_81.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_82.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_83.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_84.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_85.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_86.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_87.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_88.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_89.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_9.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_90.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_91.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_92.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_93.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_94.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_95.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/universe_96.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/pipelines.csv
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_1.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_10.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_11.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_12.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_13.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_14.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_15.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_16.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_17.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_18.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_19.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_2.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_20.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_21.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_22.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_23.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_24.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_25.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_26.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_27.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_28.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_29.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_3.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_30.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_31.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_32.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_33.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_34.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_35.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_36.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_37.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_38.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_39.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_4.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_40.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_41.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_42.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_43.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_44.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_45.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_46.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_47.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_48.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_49.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_5.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_50.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_51.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_52.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_53.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_54.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_55.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_56.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_57.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_58.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_59.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_6.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_60.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_61.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_62.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_63.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_64.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_65.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_66.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_67.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_68.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_69.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_7.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_70.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_71.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_72.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_73.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_74.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_75.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_76.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_77.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_78.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_79.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_8.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_80.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_81.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_82.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_83.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_84.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_85.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_86.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_87.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_88.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_89.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_9.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_90.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_91.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_92.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_93.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_94.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_95.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/tutorials/multiverse/results/universe_96.pkl
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/LICENSE
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/README.md
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 comet_toolbox-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/.gitattributes
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/__init__.py
+-rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/cifti.py
+-rwxr-xr-x   0        0        0     3968 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/data.py
+-rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/graph.py
+-rw-r--r--   0        0        0   105766 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/gui.py
+-rwxr-xr-x   0        0        0    44939 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/methods.py
+-rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/multiverse.py
+-rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/simulation.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/simulation.txt
+-rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/single_state.txt
+-rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
+-rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/README.md
+-rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
+-rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
+-rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/badge.svg
+-rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/content.drawio
+-rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/content.png
+-rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/gui.png
+-rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/src/comet/resources/img/logo.png
+-rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_analysis.ipynb
+-rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_dfc.ipynb
+-rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_graph.ipynb
+-rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_multiverse.ipynb
+-rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/abide_50008.txt
+-rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/aomic_multi.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/simulation.txt
+-rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/example_data/xcpd.tsv
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_1.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_10.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_11.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_12.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_13.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_14.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_15.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_16.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_17.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_18.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_19.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_2.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_20.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_21.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_22.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_23.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_24.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_25.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_26.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_27.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_28.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_29.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_3.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_30.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_31.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_32.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_33.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_34.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_35.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_36.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_37.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_38.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_39.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_4.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_40.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_41.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_42.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_43.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_44.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_45.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_46.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_47.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_48.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_49.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_5.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_50.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_51.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_52.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_53.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_54.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_55.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_56.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_57.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_58.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_59.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_6.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_60.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_61.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_62.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_63.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_64.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_65.py
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_66.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_67.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_68.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_69.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_7.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_70.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_71.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_72.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_73.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_74.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_75.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_76.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_77.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_78.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_79.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_8.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_80.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_81.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_82.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_83.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_84.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_85.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_86.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_87.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_88.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_89.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_9.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_90.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_91.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_92.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_93.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_94.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_95.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/universe_96.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/pipelines.csv
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_1.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_10.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_11.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_12.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_13.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_14.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_15.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_16.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_17.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_18.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_19.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_2.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_20.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_21.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_22.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_23.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_24.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_25.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_26.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_27.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_28.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_29.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_3.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_30.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_31.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_32.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_33.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_34.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_35.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_36.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_37.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_38.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_39.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_4.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_40.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_41.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_42.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_43.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_44.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_45.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_46.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_47.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_48.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_49.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_5.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_50.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_51.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_52.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_53.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_54.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_55.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_56.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_57.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_58.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_59.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_6.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_60.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_61.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_62.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_63.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_64.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_65.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_66.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_67.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_68.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_69.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_7.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_70.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_71.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_72.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_73.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_74.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_75.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_76.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_77.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_78.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_79.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_8.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_80.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_81.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_82.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_83.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_84.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_85.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_86.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_87.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_88.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_89.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_9.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_90.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_91.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_92.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_93.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_94.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_95.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/tutorials/multiverse/results/universe_96.pkl
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/README.md
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 comet_toolbox-0.3.0/PKG-INFO
```

### Comparing `comet_toolbox-0.2.1/simulation.txt` & `comet_toolbox-0.3.0/src/comet/resources/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/cifti.py` & `comet_toolbox-0.3.0/src/comet/cifti.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/data.py` & `comet_toolbox-0.3.0/src/comet/data.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/graph.py` & `comet_toolbox-0.3.0/src/comet/graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import bct
 import numpy as np
 from numba import jit
+from typing import Literal
 
-def handle_negative_weights(W, type="absolute", copy=True):
+def handle_negative_weights(W: np.ndarray, 
+                            type: Literal["absolute", "discard"] = "absolute", 
+                            copy: bool = True) -> np.ndarray:
     '''Handle negative weights in a connectivity/adjacency matrix
 
     Connectivity methods can produce negative estimates, which can be handled in different ways before graph analysis.
 
     Parameters
     ----------
     W : PxP np.ndarray
@@ -31,15 +35,19 @@
         W = np.abs(W)
     elif type == "discard":
         W[W < 0] = 0
     else:
         raise NotImplementedError("Options are: *absolute* or *discard*")
     return W
 
-def threshold(W, type="absolute", threshold=None, density=None, copy=True):
+def threshold(W: np.ndarray, 
+              type: Literal["absolute", "density"] = "absolute", 
+              threshold: float = None, 
+              density: float = None, 
+              copy: bool = True) -> np.ndarray:
     '''Thresholding of connectivity/adjacency matrix
     
     Performs absolute or density-based thresholding
 
     Parameters
     ----------
     W : PxP np.ndarray
@@ -73,30 +81,31 @@
     '''
     if copy:
         W = W.copy()
 
     if type == "absolute":
         W[W < threshold] = 0
     elif type == "density":
-        assert density > 0 and density < 1, "Error: Density must be between 0 and 1"
+        assert density >= 0 and density <= 1, "Error: Density must be between 0 and 1"
         assert np.allclose(W, W.T), "Error: Matrix is not symmetric"
         
         W[np.tril_indices(len(W))] = 0 # set lower triangle to zero
         triu_indices = np.triu_indices_from(W, k=1) # get upper triangle indices
         sorted_indices = np.argsort(W[triu_indices])[::-1] # sort upper triangle by indices
         cutoff_idx = int(np.round((len(sorted_indices) * density) + 1e-10)) # find cutoff index, add small constant to round .5 to 1
         keep_mask = np.zeros_like(W, dtype=bool)
         keep_mask[triu_indices[0][sorted_indices[:cutoff_idx]], triu_indices[1][sorted_indices[:cutoff_idx]]] = True # set values larger than cutoff to True
         W[~keep_mask] = 0
         W = W + W.T # restore symmetry
     else:
         raise NotImplementedError("Thresholding must be of type *absolute* or *density*")
     return W
 
-def binarise(W, copy=True):
+def binarise(W: np.ndarray, 
+             copy: bool = True) -> np.ndarray:
     '''Binarise connectivity/adjacency matrix
 
     Parameters
     ----------
     W : PxP np.ndarray
         adjacency/connectivity matrix
 
@@ -111,15 +120,16 @@
     '''
     if copy:
         W = W.copy()
 
     W[W != 0] = 1
     return W
 
-def normalise(W, copy=True):
+def normalise(W: np.ndarray, 
+              copy: bool = True) -> np.ndarray:
     '''Normalise connectivity/adjacency matrix
 
     Parameters
     ----------
     W : PxP np.ndarray
         adjacency/connectivity matrix
 
@@ -135,15 +145,16 @@
     if copy:
         W = W.copy()
 
     assert np.max(np.abs(W)) > 0, "Error: Matrix contains only zeros"
     W /= np.max(np.abs(W))
     return W
 
-def invert(W, copy=True):
+def invert(W: np.ndarray, 
+           copy: bool = True) -> np.ndarray:
     '''Invert connectivity/adjacency matrix
 
     Element wise inversion W such that each value W[i,j] will be 1 / W[i,j] (internode strengths internode distances)
 
     Parameters
     ----------
     W : PxP np.ndarray
@@ -161,15 +172,17 @@
     if copy:
         W = W.copy()
 
     W_safe = np.where(W == 0, np.inf, W)
     W = 1 / W_safe
     return W
 
-def logtransform(W, epsilon=1e-10, copy=True):
+def logtransform(W: np.ndarray, 
+                 epsilon: float = 1e-10, 
+                 copy: bool = True) -> np.ndarray:
     '''Log transform of connectivity/adjacency matrix
 
     Element wise log transform of W such that each value W[i,j] will be -log(W[i,j]
 
     Parameters
     ----------
     W : PxP np.ndarray
@@ -193,15 +206,16 @@
 
     if np.logical_or(W > 1, W <= 0).any():
         raise ValueError("Connections must be between (0,1] to use logtransform")
     W_safe = np.clip(W, a_min=epsilon, a_max=None) # clip very small values for numeric stability
     W = -np.log(W_safe)
     return W
 
-def symmetrise(W, copy=True):
+def symmetrise(W: np.ndarray, 
+               copy: bool = True) -> np.ndarray:
     '''Symmetrise connectivity/adjacency matrix
 
     Symmetrise W such that each value W[i,j] will be W[j,i]
 
     Parameters
     ----------
     W : PxP np.ndarray
@@ -225,19 +239,23 @@
         W = np.logical_or(W, W.T).astype(float)
     else:
         W_mean = (np.triu(W, k=1) + np.tril(W, k=-1)) / 2
         W = W_mean + W_mean.T + np.diag(np.diag(W))
     
     return W
 
-def randomise(G):
+def randomise(G: np.ndarray,
+              copy: bool = True) -> np.ndarray:
     '''
     Randomly rewire edges of a adjacency/connectivity matrix. Based on the small_world_propensity implementation
     which just randomizes the matrix: https://github.com/rkdan/small_world_propensity
     '''
+    if copy:
+        G = G.copy()
+    
     num_nodes = G.shape[0]
     G_rand = np.zeros((num_nodes, num_nodes))
     mask = np.triu(np.ones((num_nodes, num_nodes)), 1)
 
     # Find the indices where mask > 0 in column-major order
     grab_indices = np.column_stack(np.nonzero(mask.T))
 
@@ -250,15 +268,15 @@
     for i in range(num_nodes - 1):
         for j in range(i + 1, num_nodes):
             G_rand[i, j] = randomized_edges[edge]
             G_rand[j, i] = randomized_edges[edge]
             edge += 1
     return G_rand
 
-def regular_matrix(G, r):
+def regular_matrix(G: np.ndarray, r: float) -> np.ndarray:
     n = G.shape[0]
     G_upper = np.triu(G)  # Keep only the upper triangular part
     B = np.sort(G_upper.flatten(order="F"))[::-1]  # Flatten and sort including zeros
 
     # Calculate padding and reshape B to match the second function
     num_els = np.ceil(len(B) / (2 * n))
     num_zeros = int(2 * n * num_els - n * n)
@@ -277,15 +295,17 @@
             y_coord = (i + z + 1) % n
             M[i, y_coord] = B_matrix[a, z]
             M[y_coord, i] = B_matrix[a, z]
             B_matrix[a, z] = 0  # Remove the used weight
 
     return M
 
-def avg_shortest_path(G, include_diagonal=False, include_infinite=False):
+def avg_shortest_path(G: np.ndarray, 
+                      include_diagonal: bool = False, 
+                      include_infinite: bool = False) -> float:
     '''
     Average shortest path length calculated from the distance matrix.
     '''
     is_binary = np.all(np.logical_or(np.isclose(G, 0), np.isclose(G, 1)))
     if is_binary:
         D = distance_bin(G, inv=False)
     else:
@@ -300,40 +320,42 @@
     if not include_infinite:
         D[np.isinf(D)] = np.nan
 
     Dv = D[~np.isnan(D)]
     l = np.mean(Dv)
     return l
 
-def transitivity(A):
+def transitivity(A: np.ndarray) -> np.ndarray:
     '''Transitivity is the ratio of triangles to triplets in the network (classical version of the clustering coefficient).
-    Only for undirected matrices (binary/weighted). Adapted from the bytpy implementation: https://github.com/aestrivex/bctpy
+    Only for undirected matrices (binary/weighted). Adapted from the bctpy implementation: https://github.com/aestrivex/bctpy
     '''
     is_binary = np.all(np.logical_or(np.isclose(A, 0), np.isclose(A, 1)))
     
     if is_binary:
         tri3 = np.trace(np.dot(A, np.dot(A, A)))
         tri2 = np.sum(np.dot(A, A)) - np.trace(np.dot(A, A))
         return tri3 / tri2
     else:
         K = np.sum(np.logical_not(A == 0), axis=1)
         ws = np.cbrt(A)
         cyc3 = np.diag(np.dot(ws, np.dot(ws, ws)))
         return np.sum(cyc3, axis=0) / np.sum(K * (K - 1), axis=0)
 
-def clustering_onella(W):
+def clustering_onella(W: np.ndarray) -> np.ndarray:
     K = np.where(W > 0, 1, 0).sum(axis=1)
     W2 = W / W.max()
     cyc3 = np.diagonal(np.linalg.matrix_power(W2 ** (1/3), 3))
     K = np.where(cyc3 == 0, np.inf, K)
     C = cyc3 / (K * K-1)
 
     return C.mean()
 
-def postproc(W, diag=0, copy=True):
+def postproc(W: np.ndarray, 
+             diag: float = 0, 
+             copy: bool = True) -> np.ndarray:
     '''Postprocessing of connectivity/adjacency matrix
     
     Ensures W is symmetric, sets diagonal to diag, removes NaNs and infinities, and ensures exact binarity
 
     Parameters
     ----------
     W : PxP np.ndarray
@@ -357,15 +379,21 @@
 
     assert np.allclose(W, W.T), "Error: Matrix is not symmetrical"
     np.fill_diagonal(W, diag)
     np.nan_to_num(W, nan=0.0, posinf=0.0, neginf=0.0, copy=False)
     W = np.round(W, decimals=5) # This should ensure exact binarity if floating point inaccuracies occur
     return W
 
-def efficiency_wei(Gw, local=False):
+def efficiency(G: np.ndarray, 
+               weighted: bool = True,
+               local: bool = False) -> np.ndarray:
+    return efficiency_wei(G, local=local) if weighted else efficiency_bin(G, local=local)
+
+def efficiency_wei(Gw: np.ndarray, 
+                   local: bool=False) -> np.ndarray:
     '''Efficiency for weighted networks
     
     Based on the bctpy implelementation by Roan LaPlante: https://github.com/aestrivex/bctpy
     Global efficiency is the average of inverse shortest path length, and is inversely related to the characteristic path length.
     Local efficiency is the global efficiency computed on the neighborhood of the node, and is related to the clustering coefficient.
     
     Parameters
@@ -428,15 +456,16 @@
                 E[u] = numer / denom  # local efficiency
     else:
         e = distance_wei(Gl, inv=True)
         E = np.sum(e) / (n * n - n)
 
     return E
 
-def efficiency_bin(G, local=False):    
+def efficiency_bin(G: np.ndarray, 
+                   local: bool=False) -> np.ndarray:    
     '''Efficiency for binary networks
     
     Based on the bctpy implelementation by Roan LaPlante: https://github.com/aestrivex/bctpy
     Global efficiency is the average of inverse shortest path length, and is inversely related to the characteristic path length.
     Local efficiency is the global efficiency computed on the neighborhood of the node, and is related to the clustering coefficient.
     
     Parameters
@@ -488,15 +517,16 @@
                 E[u] = numer / denom  # local efficiency
     else:
         e = distance_bin(G, inv=True)
         E = np.sum(e) / (n * n - n)
     
     return E
 
-def small_world_sigma(G, nrand=10):
+def small_world_sigma(G: np.ndarray,
+                      nrand: int = 10) -> np.ndarray:
     '''Small-worldness sigma for undirected networks (binary or weighted)
         
     Small worldness sigma is calculated as the ratio of the clustering coefficient and the characteristic path length 
     of the real network to the average clustering coefficient and characteristic path length of the random networks.
 
     Parameters
     ----------
@@ -527,15 +557,15 @@
     L = avg_shortest_path(G)
     Cr = np.mean(randMetrics["C"])
     Lr = np.mean(randMetrics["L"])
 
     sigma = (C / Cr) / (L / Lr)
     return sigma
 
-def small_world_propensity(G):
+def small_world_propensity(G: np.ndarray) -> np.ndarray:
     assert np.allclose(G, G.T), "Error: Matrix is not symmetrical"
     G = G / np.max(G)
     n = G.shape[0]  # Number of nodes
 
     # Compute the average degree of the unweighted network (approximate radius)
     num_connections = np.count_nonzero(G)
     avg_deg_unw = num_connections / n
@@ -581,18 +611,18 @@
           "rngL", round(rand_path, 3),
           "ΔC", round(delta_C, 3),
           "ΔL", round(delta_L, 3),
           "α", round(alpha, 3),
           "δ", round(delta, 3),
           "SWP", round(SWP, 3))"""
 
-    return SWP, delta_C, delta_L
+    return SWP, delta_C, delta_L, alpha, delta
 
 @jit(nopython=True)
-def matching_ind_und(G):
+def matching_ind_und(G: np.ndarray) -> np.ndarray:
     '''Matching index for undirected networks
     
     Based on the MATLAB implementation by Stuart Oldham: https://github.com/StuartJO/FasterMatchingIndex
     Matching index is a measure of similarity between two nodes' connectivity profiles (excluding their mutual connection, should it exist).
 
     Parameters
     ----------
@@ -625,15 +655,15 @@
     denominator = np.where((degsum <= 2) & (nei != 1), 1.0, degsum - 2 * G)
     M = np.where(denominator != 0, (nei * 2) / denominator, 0.0)
     for i in range(n):
         M[i, i] = 0.0
     return M
 
 @jit(nopython=True)
-def distance_wei(G, inv=False):
+def distance_wei(G: np.ndarray, inv: bool = False) -> np.ndarray:
     '''(Inverse) distance matrix for weighted networks
     
     Based on the bctpy implelementation by Roan LaPlante: https://github.com/aestrivex/bctpy
     Significantly improved performance due to numba JIT compilation
     
     Parameters
     ----------
@@ -686,15 +716,15 @@
     if inv:
         D = 1 / D
         np.fill_diagonal(D, 0)
     
     return D
 
 @jit(nopython=True)
-def distance_bin(G, inv=False):
+def distance_bin(G: np.ndarray, inv: bool = False) -> np.ndarray:
     '''(Inverse) distance matrix for binary networks
     
     Based on the bctpy implelementation by Roan LaPlante: https://github.com/aestrivex/bctpy
     Significantly improved performance due to numba JIT compilation
     
     Parameters
     ----------
@@ -731,7 +761,90 @@
 
     np.fill_diagonal(D, 1)
     if inv:
         D = 1 / D
         np.fill_diagonal(D, 0)
     
     return D
+
+# BCT wrapper functions with type hinting (GUI needs to know the parameter types)
+def backbone_wu(CIJ: np.ndarray, 
+                avgdeg: int = 0,
+                verbose: bool = False) -> tuple[np.ndarray, np.ndarray]:
+    res = bct.backbone_wu(CIJ, avgdeg, verbose)
+    res_dict = {"Connection matrix of the minimum spanning tree of CIJ": res[0], 
+               f"Connection matrix of the minimum spanning tree plus strongest connections up to some average degree <avgdeg>": res[1]}
+    return res_dict
+
+def betweenness(G: np.ndarray,
+                weighted: bool = True) -> np.ndarray:
+    res = bct.betweenness_wei(G) if weighted else bct.betweenness_bin(G)
+    res_dict = {"Nodal betweenness centrality (weighted)": res} if weighted else {"Nodal betweenness centrality (binary)": res}
+    return res_dict
+
+def clustering_coef(G: np.ndarray,
+                       weighted: bool = True) -> np.ndarray:
+    res = bct.clustering_coef_wu(G) if weighted else bct.clustering_coef_bu(G)
+    res_dict = {"Nodal clustering coefficient (weighted)": res} if weighted else {"Nodal clustering coefficient (binary)": res}
+    return res_dict
+
+def degrees_und(CIJ: np.ndarray) -> np.ndarray:
+    res = bct.degrees_und(CIJ)
+    res_dict = {"Nodal degree": res}
+    return res_dict
+
+def density_und(CIJ: np.ndarray) -> tuple[float, int, int]:
+    res = bct.density_und(CIJ)
+    res_dict = {"Density": res[0], "Number of vertices": res[1], "Number of edges": res[2]}
+    return res_dict
+
+def eigenvector_centrality_und(CIJ: np.ndarray) -> np.ndarray:
+    res = bct.eigenvector_centrality_und(CIJ)
+    res_dict = {"Nodal eigenvector centrality": res}
+    return res_dict
+
+def gateway_coef_sign(CIJ: np.ndarray,
+                      ci: Literal["louvain"] = "louvain",
+                      centrality_type: Literal["degree", "betweenness"] = "degree", ) -> tuple[np.ndarray, np.ndarray]:
+    ci, q = bct.community_louvain(CIJ)
+    res = bct.gateway_coef_sign(CIJ, ci, centrality_type)
+    res_dict = {"Gateway coefficient for positive weights": res[0], "Gateway coefficient for negative weights": res[1]}
+    return res_dict
+
+def pagerank_centrality(A: np.ndarray,
+                        d: float = 0.85,
+                        falff: Literal["byesian prior"] = "byesian prior") -> np.ndarray:
+    res = bct.pagerank_centrality(A, d, None)
+    res_dict = {"Nodal pageranking vectors": res}
+    return res_dict
+
+def participation_coef(CIJ: np.ndarray,
+                       ci: Literal["louvain"] = "louvain",
+                       sparse: bool = False,
+                       degree: Literal["undirected"] = "undirected") -> np.ndarray:
+    ci, q = bct.community_louvain(CIJ)
+    res = bct.participation_coef_sparse(CIJ, ci, degree) if sparse else bct.participation_coef(CIJ, ci, degree)
+    res_dict = {"Nodal participation coefficient (sparse)": res} if sparse else {"Nodal participation coefficient": res}
+    return res_dict
+
+def participation_coef_sign(CIJ: np.ndarray,
+                            ci: Literal["louvain"] = "louvain",) -> tuple[np.ndarray, np.ndarray]:
+    ci, q = bct.community_louvain(CIJ)
+    res = bct.participation_coef_sign(CIJ, ci)
+    res_dict = {"Nodal participation coefficient from positive weights": res[0], "Nodal participation coefficient from negative weights": res[1]}
+    return res_dict
+
+"""
+def rich_club(CIJ: np.ndarray,
+                 weighted: bool=True,
+                 klevel: int = None) -> np.ndarray:
+    res = bct.rich_club_wu(CIJ, klevel) if weighted else bct.rich_club_bu(CIJ, klevel)
+    print("rich club", type(res))
+    print(res)
+    res_dict = {"Rich club coefficient vectors (weighted)": res} if weighted else {"Rich club coefficient vectors (binary)": res}
+    return res_dict"""
+
+def transitivity(CIJ: np.ndarray,
+                 weighted: bool=True) -> float:
+    res = bct.transitivity_wu(CIJ) if weighted else bct.transitivity_bu(CIJ)
+    res_dict = {"Global transitivity (weighted)": res} if weighted else {"Global transitivity (binary)": res}
+    return res_dict
```

### Comparing `comet_toolbox-0.2.1/src/comet/gui.py` & `comet_toolbox-0.3.0/src/comet/gui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import re
 import sys
 import copy
 import pickle
 import inspect
 import numpy as np
 import pandas as pd
 import nibabel as nib
-from typing import Any, Dict
 from scipy.io import loadmat, savemat
 from dataclasses import dataclass, field
 from importlib import resources as pkg_resources
+from typing import Any, Dict, get_type_hints, get_origin, get_args, Literal, Union
 
 # Plotting imports
 from matplotlib.image import imread
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.figure import Figure
 from matplotlib.ticker import FuncFormatter
@@ -20,22 +21,23 @@
 
 # Qt imports
 import qdarkstyle
 from PyQt6.QtCore import Qt, QPoint, QThread, pyqtSignal, QObject
 from PyQt6.QtGui import QEnterEvent, QFontMetrics
 from PyQt6.QtWidgets import QApplication, QMainWindow, QPushButton, QVBoxLayout, QHBoxLayout, \
     QSlider, QToolTip, QWidget, QLabel, QFileDialog, QComboBox, QLineEdit, QSizePolicy, \
-    QSpacerItem, QCheckBox, QTabWidget, QMessageBox, QSpinBox, QDoubleSpinBox
+    QSpacerItem, QCheckBox, QTabWidget, QSpinBox, QDoubleSpinBox, QTextEdit
 
 # Comet imports and state-based dFC methods from pydfc
-from . import cifti, methods
+from . import cifti, methods, graph
 import pydfc
+import bct
 
 class Worker(QObject):
-    # Worker class for dFC calculation (runs in a separate thread)
+    # Worker class for calculations (runs in a separate thread)
     finished = pyqtSignal()
     error = pyqtSignal(str)
     result = pyqtSignal(object)
 
     def __init__(self, calculationFunc, parameters):
         super().__init__()
         self.calculationFunc = calculationFunc
@@ -74,14 +76,20 @@
     dfc_name:     str        = field(default=None)         # method class name
     dfc_params:   Dict       = field(default_factory=dict) # input parameters
     dfc_data:     np.ndarray = field(default=None)         # dfc data
     dfc_states:   Dict       = field(default_factory=dict) # dfc states
     dfc_state_tc: np.ndarray = field(default=None)         # dfc state time course
     dfc_edge_ts:  np.ndarray = field(default=None)         # dfc edge time series
 
+    # Graph variables
+    graph_file:   str        = field(default=None)         # graph file name
+    graph_raw:    np.ndarray = field(default=None)         # raw input data for graph (dFC matrix)
+    graph_data:   np.ndarray = field(default=None)         # working data for graph (while processing)
+    graph_out:    Any = field(default=None)                # output graph measure data
+
     # Misc variables
     cifti_data:   np.ndarray = field(default=None)         # input cifti data (for .dtseries files)
     roi_names:    np.ndarray = field(default=None)         # input roi data (for .tsv files)
 
     def clear_dfc_data(self):
         self.dfc_params   = {}
         self.dfc_data     = None
@@ -140,14 +148,15 @@
         self.init_flag = True
 
         self.data = Data()
         self.data_storage = DataStorage()
 
         self.currentSliderValue = 0
         self.currentTabIndex = 0
+        self.graphStepCounter = 1
 
         self.param_names = {
             "self":                 "self", 
             "time_series":          "Time series",
             "windowsize":           "Window size",
             "shape":                "Window shape",
             "std":                  "Window sigma",
@@ -205,15 +214,15 @@
         topLayout = QVBoxLayout()
         self.topTabWidget = QTabWidget()
         topLayout.addWidget(self.topTabWidget)
 
         # Setup the individual tabs
         self.connectivityTab()
         self.graphTab()
-        self.multiverseTab()
+        #self.multiverseTab()
 
         # Set main window layout to the top-level layout
         centralWidget = QWidget()
         centralWidget.setLayout(topLayout)
         self.setCentralWidget(centralWidget)
 
     def initFromData(self, init_dfc_data=None, init_dfc_instance=None):
@@ -286,260 +295,513 @@
 
         for param_name in init_signature.parameters:
             self.data.dfc_params[param_name] = getattr(init_dfc_instance, param_name, None)
         
         self.setParameters(disable=True)
 
     def connectivityTab(self):
-            connectivityTab = QWidget()
-            connectivityLayout = QHBoxLayout()
-            connectivityTab.setLayout(connectivityLayout)
-
-            ###############################
-            #  Left section for settings  #
-            ###############################
-            self.leftLayout = QVBoxLayout()
-
-            # Create button and label for file loading
-            self.fileButton = QPushButton('Load File')
-            self.fileNameLabel = QLabel('No file loaded')
-            self.leftLayout.addWidget(self.fileButton)
-            self.leftLayout.addWidget(self.fileNameLabel)
-            self.fileButton.clicked.connect(self.loadFile)
-
-            # Create a checkbox for reshaping the data
-            self.transposeCheckbox = QCheckBox("Transpose data (time has to be the first dimension)")
-            self.leftLayout.addWidget(self.transposeCheckbox)
-            self.transposeCheckbox.setEnabled(False)
-
-            # Connect the checkbox to a method
-            self.transposeCheckbox.stateChanged.connect(self.onTransposeChecked)
-
-            # Add spacer for an empty line
-            self.leftLayout.addItem(QSpacerItem(0, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed))
-
-            # Method label and combobox
-            self.methodLabel = QLabel("Dynamic functional connectivity method:")
-            
-            # Checkboxes for method types
-            self.continuousCheckBox = QCheckBox("Continuous")
-            self.stateBasedCheckBox = QCheckBox("State-based")
-            self.staticCheckBox = QCheckBox("Static")
-
-            checkboxLayout = QHBoxLayout()
-            checkboxLayout.addWidget(self.continuousCheckBox)
-            checkboxLayout.addWidget(self.stateBasedCheckBox)
-            checkboxLayout.addWidget(self.staticCheckBox)
-            checkboxLayout.setSpacing(10)
-            checkboxLayout.addStretch()
-
-            # Connect the stateChanged signal of checkboxes to the slot
-            self.continuousCheckBox.stateChanged.connect(self.updateMethodComboBox)
-            self.stateBasedCheckBox.stateChanged.connect(self.updateMethodComboBox)
-            self.staticCheckBox.stateChanged.connect(self.updateMethodComboBox)
-            
-            self.methodComboBox = QComboBox()
-            self.leftLayout.addWidget(self.methodLabel)
-            self.leftLayout.addLayout(checkboxLayout)
-            self.leftLayout.addWidget(self.methodComboBox)
-
-            # Get all the dFC methods and names
-            self.class_info = {
-                obj.name: name  # Map human-readable name to class name
-                for name, obj in inspect.getmembers(methods)
-                if inspect.isclass(obj) and obj.__module__ == methods.__name__ and name != "ConnectivityMethod"
-            }
-
-            # Create a layout for dynamic textboxes
-            self.parameterLayout = QVBoxLayout()
-
-            # Create a container widget for the parameter layout
-            self.parameterContainer = QWidget()  # Use an instance attribute to access it later
-            self.parameterContainer.setLayout(self.parameterLayout)
-            self.parameterContainer.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Expanding)
+        connectivityTab = QWidget()
+        connectivityLayout = QHBoxLayout()
+        connectivityTab.setLayout(connectivityLayout)
+
+        ###############################
+        #  Left section for settings  #
+        ###############################
+        self.leftLayout = QVBoxLayout()
+
+        # Create button and label for file loading
+        self.fileButton = QPushButton('Load File')
+        self.fileNameLabel = QLabel('No file loaded')
+        self.leftLayout.addWidget(self.fileButton)
+        self.leftLayout.addWidget(self.fileNameLabel)
+        self.fileButton.clicked.connect(self.loadConnectivityFile)
+
+        # Create a checkbox for reshaping the data
+        self.transposeCheckbox = QCheckBox("Transpose data (time has to be the first dimension)")
+        self.leftLayout.addWidget(self.transposeCheckbox)
+        self.transposeCheckbox.setEnabled(False)
+
+        # Connect the checkbox to a method
+        self.transposeCheckbox.stateChanged.connect(self.onTransposeChecked)
+
+        # Add spacer for an empty line
+        self.leftLayout.addItem(QSpacerItem(0, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed))
+
+        # Method label and combobox
+        self.methodLabel = QLabel("Dynamic functional connectivity method:")
+        
+        # Checkboxes for method types
+        self.continuousCheckBox = QCheckBox("Continuous")
+        self.stateBasedCheckBox = QCheckBox("State-based")
+        self.staticCheckBox = QCheckBox("Static")
+
+        checkboxLayout = QHBoxLayout()
+        checkboxLayout.addWidget(self.continuousCheckBox)
+        checkboxLayout.addWidget(self.stateBasedCheckBox)
+        checkboxLayout.addWidget(self.staticCheckBox)
+        checkboxLayout.setSpacing(10)
+        checkboxLayout.addStretch()
+
+        # Connect the stateChanged signal of checkboxes to the slot
+        self.continuousCheckBox.stateChanged.connect(self.updateMethodComboBox)
+        self.stateBasedCheckBox.stateChanged.connect(self.updateMethodComboBox)
+        self.staticCheckBox.stateChanged.connect(self.updateMethodComboBox)
+        
+        self.methodComboBox = QComboBox()
+        self.leftLayout.addWidget(self.methodLabel)
+        self.leftLayout.addLayout(checkboxLayout)
+        self.leftLayout.addWidget(self.methodComboBox)
+
+        # Get all the dFC methods and names
+        self.class_info = {
+            obj.name: name  # Map human-readable name to class name
+            for name, obj in inspect.getmembers(methods)
+            if inspect.isclass(obj) and obj.__module__ == methods.__name__ and name != "ConnectivityMethod"
+        }
 
-            # Add the container widget to the left layout directly below the combobox
-            self.leftLayout.addWidget(self.parameterContainer)
-            
-            # Initial population of the combobox, this does the entire initialization
-            self.updateMethodComboBox()
+        # Create a layout for dynamic textboxes
+        self.parameterLayout = QVBoxLayout()
 
-            # Add parameter textbox for time_series
-            self.time_series_textbox = QLineEdit()
-            self.time_series_textbox.setReadOnly(True) # read only as based on the loaded file
-
-            # Set up the atlas combobox
-            self.atlasComboBox = QComboBox()
-            self.atlasComboBox.addItems(["Glasser MMP", "Schaefer Kong 200", "Schaefer Tian 254"])
-            self.atlasComboBox.currentIndexChanged.connect(self.onAtlasSelected)
-
-            # Add a stretch after the parameter layout container
-            self.leftLayout.addStretch()
-
-            # Calculate connectivity and save button
-            buttonsLayout = QHBoxLayout()
-
-            # Calculate connectivity button
-            self.calculateButton = QPushButton('Calculate Connectivity')
-            self.calculateButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
-            buttonsLayout.addWidget(self.calculateButton, 2)  # 2/3 of the space
-            self.calculateButton.clicked.connect(self.onCalculateButton)
-
-            # Create the "Save" button
-            self.saveButton = QPushButton('Save')
-            self.saveButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
-            buttonsLayout.addWidget(self.saveButton, 1)  # 1/3 of the space
-            self.saveButton.clicked.connect(self.saveFile)
-
-            # Add the buttons layout to the left layout
-            self.leftLayout.addLayout(buttonsLayout)
-
-            # Memory buttons
-            self.keepInMemoryCheckbox = QCheckBox("Keep in memory")
-            self.keepInMemoryCheckbox.stateChanged.connect(self.onKeepInMemoryChecked)
-            self.clearMemoryButton = QPushButton("Clear Memory")
-            self.clearMemoryButton.clicked.connect(self.onClearMemory)
-
-            buttonLayout = QHBoxLayout()
-            buttonLayout.addWidget(self.keepInMemoryCheckbox)
-            buttonLayout.addWidget(self.clearMemoryButton)
-
-            # Assuming you have a QVBoxLayout named 'leftLayout'
-            self.leftLayout.addLayout(buttonLayout)
-
-            # Calculation info textbox
-            self.calculatingLabel = QLabel('No data calculated yet')
-            self.leftLayout.addWidget(self.calculatingLabel)
-            
-            ################################
-            #  Right section for plotting  #
-            ################################
-            rightLayout = QVBoxLayout()
-            self.tabWidget = QTabWidget()
-            
-            # Tab 1: Imshow plot
-            imshowTab = QWidget()
-            imshowLayout = QVBoxLayout()
-            imshowTab.setLayout(imshowLayout)
-
-            self.figure = Figure()
-            self.canvas = FigureCanvas(self.figure)
-            self.figure.patch.set_facecolor('#E0E0E0')
-            imshowLayout.addWidget(self.canvas)
-            self.tabWidget.addTab(imshowTab, "Connectivity")
-
-            # Tab 2: Time series/course plot
-            timeSeriesTab = QWidget()
-            timeSeriesLayout = QVBoxLayout()
-            timeSeriesTab.setLayout(timeSeriesLayout)
-
-            self.timeSeriesFigure = Figure()
-            self.timeSeriesCanvas = FigureCanvas(self.timeSeriesFigure)
-            self.timeSeriesFigure.patch.set_facecolor('#E0E0E0')
-            timeSeriesLayout.addWidget(self.timeSeriesCanvas)
-            self.tabWidget.addTab(timeSeriesTab, "Time course")
-
-            rightLayout.addWidget(self.tabWidget)
-
-            # Tab 3: Distribution plot
-            distributionTab = QWidget()
-            distributionLayout = QVBoxLayout()
-            distributionTab.setLayout(distributionLayout)
-
-            self.distributionFigure = Figure()
-            self.distributionCanvas = FigureCanvas(self.distributionFigure)
-            self.distributionFigure.patch.set_facecolor('#E0E0E0')
-            distributionLayout.addWidget(self.distributionCanvas)
-            self.tabWidget.addTab(distributionTab, "Distribution")
-
-            # Method for doing things if the tab is changed
-            self.tabWidget.currentChanged.connect(self.onTabChanged)
-
-            # Slider
-            self.slider = QSlider(Qt.Orientation.Horizontal)
-            self.slider.setMinimum(0)  # Set the minimum value of the slider
-            self.slider.setMaximum(0)  
-            self.slider.valueChanged.connect(self.onSliderValueChanged)
-            rightLayout.addWidget(self.slider)
-
-            # Navigation buttons layout
-            navButtonLayout = QHBoxLayout()
-            navButtonLayout.addStretch(1)  # Spacer to the left of the buttons
-
-            # Creating navigation buttons
-            self.backLargeButton = QPushButton("<<")
-            self.backButton = QPushButton("<")
-            self.positionLabel = QLabel('no data available')
-            self.forwardButton = QPushButton(">")
-            self.forwardLargeButton = QPushButton(">>")
-
-            # Buttons that interact with the slider
-            navButtonLayout.addWidget(self.backLargeButton)
-            navButtonLayout.addWidget(self.backButton)
-            navButtonLayout.addWidget(self.positionLabel)
-            navButtonLayout.addWidget(self.forwardButton)
-            navButtonLayout.addWidget(self.forwardLargeButton)
-
-            self.backLargeButton.clicked.connect(self.onSliderButtonClicked)
-            self.backButton.clicked.connect(self.onSliderButtonClicked)
-            self.forwardButton.clicked.connect(self.onSliderButtonClicked)
-            self.forwardLargeButton.clicked.connect(self.onSliderButtonClicked)
-
-            navButtonLayout.addStretch(1) # Spacer to the right of the buttons
-            rightLayout.addLayout(navButtonLayout)
-
-            # UI elements for dFC time series plotting
-            self.rowSelector = QSpinBox()
-            self.rowSelector.setMaximum(0)
-            self.rowSelector.valueChanged.connect(self.plotTimeSeries)
-
-            self.colSelector = QSpinBox()
-            self.colSelector.setMaximum(0)
-            self.colSelector.valueChanged.connect(self.plotTimeSeries)
-
-            self.timeSeriesSelectorLayout = QHBoxLayout()
-            self.timeSeriesSelectorLayout.addWidget(QLabel("Brain region 1 (row):"))
-            self.timeSeriesSelectorLayout.addWidget(self.rowSelector)
-            self.timeSeriesSelectorLayout.addWidget(QLabel("Brain region 2 (column):"))
-            self.timeSeriesSelectorLayout.addWidget(self.colSelector)
+        # Create a container widget for the parameter layout
+        self.parameterContainer = QWidget()  # Use an instance attribute to access it later
+        self.parameterContainer.setLayout(self.parameterLayout)
+        self.parameterContainer.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Expanding)
+
+        # Add the container widget to the left layout directly below the combobox
+        self.leftLayout.addWidget(self.parameterContainer)
+        
+        # Initial population of the combobox, this does the entire initialization
+        self.updateMethodComboBox()
+
+        # Add parameter textbox for time_series
+        self.time_series_textbox = QLineEdit()
+        self.time_series_textbox.setReadOnly(True) # read only as based on the loaded file
+
+        # Set up the atlas combobox
+        self.atlasComboBox = QComboBox()
+        self.atlasComboBox.addItems(["Glasser MMP", "Schaefer Kong 200", "Schaefer Tian 254"])
+        self.atlasComboBox.currentIndexChanged.connect(self.onAtlasSelected)
+
+        # Add a stretch after the parameter layout container
+        self.leftLayout.addStretch()
+
+        # Calculate connectivity and save button
+        buttonsLayout = QHBoxLayout()
+
+        # Calculate connectivity button
+        self.calculateButton = QPushButton('Calculate Connectivity')
+        self.calculateButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
+        buttonsLayout.addWidget(self.calculateButton, 2)  # 2/3 of the space
+        self.calculateButton.clicked.connect(self.onCalculateButton)
+
+        # Create the "Save" button
+        self.saveButton = QPushButton('Save')
+        self.saveButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
+        buttonsLayout.addWidget(self.saveButton, 1)  # 1/3 of the space
+        self.saveButton.clicked.connect(self.saveConnectivityFile)
+
+        # Add the buttons layout to the left layout
+        self.leftLayout.addLayout(buttonsLayout)
+
+        # Memory buttons
+        self.keepInMemoryCheckbox = QCheckBox("Keep in memory")
+        self.keepInMemoryCheckbox.stateChanged.connect(self.onKeepInMemoryChecked)
+        self.clearMemoryButton = QPushButton("Clear Memory")
+        self.clearMemoryButton.clicked.connect(self.onClearMemory)
+
+        buttonLayout = QHBoxLayout()
+        buttonLayout.addWidget(self.keepInMemoryCheckbox)
+        buttonLayout.addWidget(self.clearMemoryButton)
+
+        # Assuming you have a QVBoxLayout named 'leftLayout'
+        self.leftLayout.addLayout(buttonLayout)
+
+        # Calculation info textbox
+        self.calculatingLabel = QLabel('No data calculated yet')
+        self.leftLayout.addWidget(self.calculatingLabel)
+        
+        ################################
+        #  Right section for plotting  #
+        ################################
+        rightLayout = QVBoxLayout()
+        self.tabWidget = QTabWidget()
+        
+        # Tab 1: Imshow plot
+        imshowTab = QWidget()
+        imshowLayout = QVBoxLayout()
+        imshowTab.setLayout(imshowLayout)
+
+        self.figure = Figure()
+        self.canvas = FigureCanvas(self.figure)
+        self.figure.patch.set_facecolor('#E0E0E0')
+        imshowLayout.addWidget(self.canvas)
+        self.tabWidget.addTab(imshowTab, "Connectivity")
+
+        # Tab 2: Time series/course plot
+        timeSeriesTab = QWidget()
+        timeSeriesLayout = QVBoxLayout()
+        timeSeriesTab.setLayout(timeSeriesLayout)
+
+        self.timeSeriesFigure = Figure()
+        self.timeSeriesCanvas = FigureCanvas(self.timeSeriesFigure)
+        self.timeSeriesFigure.patch.set_facecolor('#E0E0E0')
+        timeSeriesLayout.addWidget(self.timeSeriesCanvas)
+        self.tabWidget.addTab(timeSeriesTab, "Time course")
+
+        rightLayout.addWidget(self.tabWidget)
+
+        # Tab 3: Distribution plot
+        distributionTab = QWidget()
+        distributionLayout = QVBoxLayout()
+        distributionTab.setLayout(distributionLayout)
+
+        self.distributionFigure = Figure()
+        self.distributionCanvas = FigureCanvas(self.distributionFigure)
+        self.distributionFigure.patch.set_facecolor('#E0E0E0')
+        distributionLayout.addWidget(self.distributionCanvas)
+        self.tabWidget.addTab(distributionTab, "Distribution")
+
+        # Method for doing things if the tab is changed
+        self.tabWidget.currentChanged.connect(self.onTabChanged)
+
+        # Slider
+        self.slider = QSlider(Qt.Orientation.Horizontal)
+        self.slider.setMinimum(0)  # Set the minimum value of the slider
+        self.slider.setMaximum(0)  
+        self.slider.valueChanged.connect(self.onSliderValueChanged)
+        rightLayout.addWidget(self.slider)
+
+        # Navigation buttons layout
+        navButtonLayout = QHBoxLayout()
+        navButtonLayout.addStretch(1)  # Spacer to the left of the buttons
+
+        # Creating navigation buttons
+        self.backLargeButton = QPushButton("<<")
+        self.backButton = QPushButton("<")
+        self.positionLabel = QLabel('no data available')
+        self.forwardButton = QPushButton(">")
+        self.forwardLargeButton = QPushButton(">>")
+
+        # Buttons that interact with the slider
+        navButtonLayout.addWidget(self.backLargeButton)
+        navButtonLayout.addWidget(self.backButton)
+        navButtonLayout.addWidget(self.positionLabel)
+        navButtonLayout.addWidget(self.forwardButton)
+        navButtonLayout.addWidget(self.forwardLargeButton)
+
+        self.backLargeButton.clicked.connect(self.onSliderButtonClicked)
+        self.backButton.clicked.connect(self.onSliderButtonClicked)
+        self.forwardButton.clicked.connect(self.onSliderButtonClicked)
+        self.forwardLargeButton.clicked.connect(self.onSliderButtonClicked)
+
+        navButtonLayout.addStretch(1) # Spacer to the right of the buttons
+        rightLayout.addLayout(navButtonLayout)
+
+        # UI elements for dFC time series plotting
+        self.rowSelector = QSpinBox()
+        self.rowSelector.setMaximum(0)
+        self.rowSelector.valueChanged.connect(self.plotTimeSeries)
+
+        self.colSelector = QSpinBox()
+        self.colSelector.setMaximum(0)
+        self.colSelector.valueChanged.connect(self.plotTimeSeries)
+
+        self.timeSeriesSelectorLayout = QHBoxLayout()
+        self.timeSeriesSelectorLayout.addWidget(QLabel("Brain region 1 (row):"))
+        self.timeSeriesSelectorLayout.addWidget(self.rowSelector)
+        self.timeSeriesSelectorLayout.addWidget(QLabel("Brain region 2 (column):"))
+        self.timeSeriesSelectorLayout.addWidget(self.colSelector)
 
-            timeSeriesLayout.addLayout(self.timeSeriesSelectorLayout)
+        timeSeriesLayout.addLayout(self.timeSeriesSelectorLayout)
 
-            # Set checkboxes to default values
-            self.continuousCheckBox.setChecked(True)
-            self.stateBasedCheckBox.setChecked(True)
-            self.staticCheckBox.setChecked(True)
+        # Set checkboxes to default values
+        self.continuousCheckBox.setChecked(True)
+        self.stateBasedCheckBox.setChecked(True)
+        self.staticCheckBox.setChecked(True)
 
-            #####################
-            #  Combine layouts  #
-            #####################
-            connectivityLayout.addLayout(self.leftLayout, 1)
-            connectivityLayout.addLayout(rightLayout, 2)
-            self.topTabWidget.addTab(connectivityTab, "Connectivity Analysis")
+        #####################
+        #  Combine layouts  #
+        #####################
+        connectivityLayout.addLayout(self.leftLayout, 1)
+        connectivityLayout.addLayout(rightLayout, 2)
+        self.topTabWidget.addTab(connectivityTab, "Connectivity Analysis")
 
     def graphTab(self):
         graphTab = QWidget()
-        graphLayout = QVBoxLayout()
+        graphLayout = QVBoxLayout()  # Main layout for the tab
         graphTab.setLayout(graphLayout)
+        
+        ###############################
+        #  Left section for settings  #
+        ###############################
+        leftLayout = QVBoxLayout()
+
+        # Calculate connectivity and save button
+        buttonsLayout = QHBoxLayout()
+
+        self.loadGraphFileButton = QPushButton('Load File')
+        self.loadGraphFileButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
+        buttonsLayout.addWidget(self.loadGraphFileButton, 1)
+        self.loadGraphFileButton.clicked.connect(self.loadGraphFile)
+
+        self.takeCurrentButton = QPushButton('From current dFC')
+        self.takeCurrentButton.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
+        buttonsLayout.addWidget(self.takeCurrentButton, 1)
+        self.takeCurrentButton.clicked.connect(self.takeCurrentData)
+        
+        self.graphFileNameLabel = QLabel('No file loaded')
+
+        leftLayout.addLayout(buttonsLayout)
+        leftLayout.addWidget(self.graphFileNameLabel)
+        leftLayout.addItem(QSpacerItem(0, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed))
+
+        # Graph analysis options
+        graphTabLabel = QLabel("Graph analysis options:")
+        leftLayout.addWidget(graphTabLabel)
+
+        # Checkboxes for method types
+        self.preprocessingCheckBox = QCheckBox("Preprocessing")
+        self.graphCheckBox = QCheckBox("Comet")
+        self.BCTCheckBox = QCheckBox("BCT")
+
+        # Populate the combo box with options
+        self.graphOptions = {
+            "handle_negative_weights":      "PREP Negative weights",
+            "threshold":                    "PREP Threshold",
+            "binarise":                     "PREP Binarise",
+            "normalise":                    "PREP Normalise",
+            "invert":                       "PREP Invert",
+            "logtransform":                 "PREP Log-transform",
+            "symmetrise":                   "PREP Symmetrise",
+            "randomise":                    "PREP Randomise",
+            "postproc":                     "PREP Post-processing",
+            
+            "efficiency":                   "COMET Efficiency",
+            "matching_ind_und":             "COMET Matching index",
+            "small_world_propensity":       "COMET Small world propensity",
+
+            "backbone_wu":                  "BCT Backbone (weighted)",
+            "betweenness":                  "BCT Betweenness centrality",
+            "clustering_coef":              "BCT Clustering coefficient",
+            "degrees_und":                  "BCT Degrees",
+            "density_und":                  "BCT Density",
+            "eigenvector_centrality_und":   "BCT Eigenvector centrality",
+            "gateway_coef_sign":            "BCT Gateway coefficient (sign)",
+            "pagerank_centrality":          "BCT Pagerank centrality",
+            "participation_coef":           "BCT Participation coef",
+            "participation_coef_sign":      "BCT Participation coef (sign)",
+            "transitivity":                 "BCT Transitivity",
+        }
+ 
+        self.reverse_graphOptions = {v: k for k, v in self.graphOptions.items()}
 
-        # Add Graph Analysis tab to the top level tab widget
+        # Checkboxes for function types
+        checkboxLayout = QHBoxLayout()
+        checkboxLayout.addWidget(self.preprocessingCheckBox)
+        checkboxLayout.addWidget(self.graphCheckBox)
+        checkboxLayout.addWidget(self.BCTCheckBox)
+        checkboxLayout.setSpacing(10)
+        checkboxLayout.addStretch()
+
+        # Init checkbox states
+        self.preprocessingCheckBox.setChecked(False)
+        self.graphCheckBox.setChecked(False)
+        self.BCTCheckBox.setChecked(True)
+        leftLayout.addLayout(checkboxLayout)
+            
+        # Create the combo box for selecting the graph analysis type
+        self.graphAnalysisComboBox = QComboBox()
+        leftLayout.addWidget(self.graphAnalysisComboBox)
+
+        self.graphAnalysisComboBox.currentIndexChanged.connect(self.onGraphCombobox)
+        self.graphParameterLayout = QVBoxLayout()
+
+        # Connect the stateChanged signal of checkboxes to the slot
+        self.preprocessingCheckBox.stateChanged.connect(self.updateGraphComboBox)
+        self.graphCheckBox.stateChanged.connect(self.updateGraphComboBox)
+        self.BCTCheckBox.stateChanged.connect(self.updateGraphComboBox)
+        
+        self.updateGraphComboBox()
+
+        # Create a container widget for the parameter layout
+        parameterContainer = QWidget()  # Use an instance attribute to access it later
+        parameterContainer.setLayout(self.graphParameterLayout)
+        parameterContainer.setSizePolicy(QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Expanding)
+
+        # Add the container widget to the left layout directly below the combobox
+        leftLayout.addWidget(parameterContainer)
+
+        # Stretch empty space
+        leftLayout.addStretch()
+
+        # Create a layout for the buttons
+        buttonsLayout = QHBoxLayout()
+
+        # Create the "Add option" button
+        addOptionButton = QPushButton('Add current option')
+        buttonsLayout.addWidget(addOptionButton, 1) # The second parameter is the stretch factor
+        addOptionButton.clicked.connect(self.onAddGraphOption)
+
+        # Create the "Save" button
+        saveButton = QPushButton('Clear options')
+        buttonsLayout.addWidget(saveButton, 1)
+        saveButton.clicked.connect(self.onClearGraphOptions)
+
+        # Add the buttons layout to the left layout
+        leftLayout.addLayout(buttonsLayout)
+
+        self.optionsTextbox = QTextEdit()
+        self.optionsTextbox.setReadOnly(True) # Make the textbox read-only
+        leftLayout.addWidget(self.optionsTextbox)
+
+        # "Save" button
+        saveButton = QPushButton('Save')
+        leftLayout.addWidget(saveButton)
+        saveButton.clicked.connect(self.saveGraphFile)
+
+
+        ################################
+        #  Right section for plotting  #
+        ################################
+        rightLayout = QVBoxLayout()
+        
+        # Different plotting tabs
+        graphTabWidget = QTabWidget()
+
+        # Tab 1: Adjacency matrix plot
+        matrixTab = QWidget()
+        matrixLayout = QVBoxLayout()
+        matrixTab.setLayout(matrixLayout)
+
+        self.matrixFigure = Figure()
+        self.matrixCanvas = FigureCanvas(self.matrixFigure)
+        self.matrixFigure.patch.set_facecolor('#E0E0E0')
+        matrixLayout.addWidget(self.matrixCanvas)
+        graphTabWidget.addTab(matrixTab, "Adjacency Matrix")
+       
+        # Draw default plot (logo)
+        self.plotLogo(self.matrixFigure)
+        self.matrixCanvas.draw()
+
+        # Tab 2: Graph measures plot
+        measureTab = QWidget()
+        measureLayout = QVBoxLayout()
+        measureTab.setLayout(measureLayout)
+
+        # Widget for the plot
+        plotWidget = QWidget()  # Create a widget to hold the plot
+        plotLayout = QVBoxLayout()  # Use QVBoxLayout for the plot widget
+        plotWidget.setLayout(plotLayout)
+
+        # Add the graph canvas to the plot layout
+        self.graphFigure = Figure()
+        self.graphCanvas = FigureCanvas(self.graphFigure)
+        self.graphFigure.patch.set_facecolor('#E0E0E0')
+        plotLayout.addWidget(self.graphCanvas)
+
+        # Widget for the textbox
+        self.graphTextbox = QTextEdit()
+        self.graphTextbox.setReadOnly(True)
+
+        # Add the plot widget and the textbox to the measure layout
+        measureLayout.addWidget(plotWidget, 2)
+        measureLayout.addWidget(self.graphTextbox, 1)
+        graphTabWidget.addTab(measureTab, "Graph Measure")
+
+        # Draw default plot (e.g., logo)
+        self.plotLogo(self.graphFigure)
+        self.graphCanvas.draw()
+
+        # Add widgets to the right layout
+        rightLayout.addWidget(graphTabWidget)
+
+        #####################
+        #  Combine layouts  #
+        #####################
+        mainLayout = QHBoxLayout()
+        mainLayout.addLayout(leftLayout, 1)
+        mainLayout.addLayout(rightLayout, 2)
+        graphLayout.addLayout(mainLayout)
+
+        # Add the tab to the top level tab widget
         self.topTabWidget.addTab(graphTab, "Graph Analysis")
 
     def multiverseTab(self):
         multiverseTab = QWidget()
-        multiverseLayout = QVBoxLayout()
+        multiverseLayout = QVBoxLayout()  # Main layout for the tab
         multiverseTab.setLayout(multiverseLayout)
+        
+        ###############################
+        #  Left section for settings  #
+        ###############################
+        leftLayout = QVBoxLayout()
+
+        # Section for defining decision points
+        decisionPointLabel = QLabel('Define Decision Points:')
+        leftLayout.addWidget(decisionPointLabel)
+
+        # Container for dynamic input fields based on decision type
+        self.decisionFieldsContainer = QVBoxLayout()
+        self.decisionTypeDropdown = QComboBox()
+        self.decisionTypeDropdown.addItems(['Select Decision Type', 'strings', 'numbers', 'booleans', 'dfc_measures', 'graph_measures'])
+        self.decisionTypeDropdown.currentIndexChanged.connect(self.updateDecisionFields)  # Implement this method
+        leftLayout.addWidget(self.decisionTypeDropdown)
+        leftLayout.addLayout(self.decisionFieldsContainer)
+
+        addDecisionButton = QPushButton('Add Decision Point')
+        addDecisionButton.clicked.connect(self.addDecisionPoint)  # Implement this method
+        leftLayout.addWidget(addDecisionButton)
+
+        # Section for defining invalid paths
+        invalidPathsLabel = QLabel('Define Invalid Paths:')
+        self.invalidPathsEditor = QTextEdit()
+        leftLayout.addWidget(invalidPathsLabel)
+        leftLayout.addWidget(self.invalidPathsEditor)
+
+        leftLayout.addStretch()
+
+        ################################
+        #  Right section for plotting  #
+        ################################
+        rightLayout = QVBoxLayout()
+        
+        # Different plotting tabs
+        multiverseTabWidget = QTabWidget()
+
+        # Tab 1: Imshow plot
+        imshowTab = QWidget()
+        imshowLayout = QVBoxLayout()
+        imshowTab.setLayout(imshowLayout)
+
+        self.multiverseFigure = Figure()
+        self.multiverseCanvas = FigureCanvas(self.multiverseFigure)
+        self.multiverseFigure.patch.set_facecolor('#E0E0E0')
+        imshowLayout.addWidget(self.multiverseCanvas)
+        multiverseTabWidget.addTab(imshowTab, "Imshow Plot")
+        rightLayout.addWidget(multiverseTabWidget)
+
+        # Draw default plot (logo)
+        self.plotLogo(self.multiverseFigure)
+        self.multiverseCanvas.draw()
+
+        #####################
+        #  Combine layouts  #
+        #####################
+        mainLayout = QHBoxLayout()
+        mainLayout.addLayout(leftLayout, 1)
+        mainLayout.addLayout(rightLayout, 2)
+        multiverseLayout.addLayout(mainLayout)
 
-        # Add Multiverse Analysis tab to the top level tab widget
         self.topTabWidget.addTab(multiverseTab, "Multiverse Analysis")
-    
+
     """
-    I/O functions
+    I/O and data related functions
     """
-    def loadFile(self):
+    # dFC functions
+    def loadConnectivityFile(self):
         fileFilter = "All Supported Files (*.mat *.txt *.npy *.pkl *.tsv *.dtseries.nii *.ptseries.nii);;MAT files (*.mat);;Text files (*.txt);;NumPy files (*.npy);;Pickle files (*.pkl);;TSV files (*.tsv);;CIFTI files (*.dtseries.nii *.ptseries.nii)"
         file_path, _ = QFileDialog.getOpenFileName(self, "Load File", "", fileFilter)
         file_name = file_path.split('/')[-1]
         self.data.file_name = file_name
         self.getParameters() # Get current UI parameters
 
         if not file_path:
@@ -645,15 +907,15 @@
         # Reset and enable the GUI elements
         self.methodComboBox.setEnabled(True)
         self.methodComboBox.setEnabled(True)
         self.calculateButton.setEnabled(True)
         self.clearMemoryButton.setEnabled(True)
         self.keepInMemoryCheckbox.setEnabled(True)
 
-    def saveFile(self):
+    def saveConnectivityFile(self):
         if self.data.dfc_data is None:
             print("No dFC data available to save.")
             return
 
         # Open a file dialog to specify where to save the file
         filePath, _ = QFileDialog.getSaveFileName(self, "Save File", "", "MAT Files (*.mat)")
 
@@ -707,18 +969,173 @@
         else:
             # Transpose it back to original
             self.data.file_data = self.data.file_data.transpose()
 
         # Update the labels
         self.fileNameLabel.setText(f"Loaded {self.time_series_textbox.text()} with shape: {self.data.file_data.shape}")
         self.time_series_textbox.setText(self.data.file_name)
- 
+
+    # Graph functions
+    def loadGraphFile(self):
+        fileFilter = "All Supported Files (*.mat *.txt *.npy *.pkl *.tsv *.dtseries.nii *.ptseries.nii);;MAT files (*.mat);;Text files (*.txt);;NumPy files (*.npy);;Pickle files (*.pkl);;TSV files (*.tsv);;CIFTI files (*.dtseries.nii *.ptseries.nii)"
+        file_path, _ = QFileDialog.getOpenFileName(self, "Load File", "", fileFilter)
+        file_name = file_path.split('/')[-1]
+        self.data.graph_file = file_name
+
+        if not file_path:
+            return  # Early exit if no file is selected
+
+        if file_path.endswith('.mat'):
+            data_dict = loadmat(file_path)
+            try:
+                self.data.graph_data = data_dict["graph_data"] # Try to load graph_data (saving files with comet will create this field)
+            except:
+                self.data.graph_data = data_dict[list(data_dict.keys())[-1]] # Else get the last item in the file (which is the data if there is only one field)
+
+        elif file_path.endswith('.txt'):
+            self.data.graph_data = np.loadtxt(file_path)
+        
+        elif file_path.endswith('.npy'):
+            self.data.graph_data = np.load(file_path)
+      
+        else:
+            self.data.graph_data = None
+            self.time_series_textbox.setText("Unsupported file format")
+
+        self.data.graph_raw = self.data.graph_data
+        self.graphFileNameLabel.setText(f"Loaded {self.data.graph_file} with shape {self.data.graph_data.shape}")
+        
+        self.plotGraph()
+        self.onGraphCombobox()
+
+    def saveGraphFile(self):
+        if self.data.graph_data is None:
+            print("No graph data available to save.")
+            return
+
+        # Open a file dialog to specify where to save the file
+        filePath, _ = QFileDialog.getSaveFileName(self, "Save File", "", "MAT Files (*.mat)")
+
+        if filePath:
+            # Ensure the file has the correct extension
+            if not filePath.endswith('.mat'):
+                filePath += '.mat'
+            
+            # Save the the current data object to a .mat file
+            try:
+                data_dict = {}
+                for field in [f for f in self.data.__dataclass_fields__ if f.startswith('graph_')]:
+                    value = getattr(self.data, field)
+                    
+                    if isinstance(value, np.ndarray):
+                        data_dict[field] = value
+                    elif isinstance(value, dict):
+                        # Ensure all dict values are appropriately converted
+                        converted_dict = {}
+                        for k, v in value.items():
+                            if isinstance(v, np.ndarray):
+                                converted_dict[k] = v
+                            elif v is None:
+                                converted_dict[k] = np.array([])
+                                print(f"Converted None to empty array for dict key: {k}")
+                            else:
+                                converted_dict[k] = v
+                        data_dict[field] = converted_dict
+                    elif value is None:
+                        data_dict[field] = np.array([])
+                        print(f"Converted None to empty array for field: {field}")
+                    elif field == 'dfc_instance':
+                        pass
+                    else:
+                        data_dict[field] = value
+
+                savemat(filePath, data_dict)
+            
+            except Exception as e:
+                print(f"Error saving data: {e}")
+            
+            return
+
+    def takeCurrentData(self):
+        if self.data.dfc_data is None:
+            print("No current dFC data available.")
+            return
+        
+        self.data.graph_data = self.data.dfc_data[:,:,self.currentSliderValue]
+        self.data.graph_raw = self.data.graph_data
+        
+        print(f"Used current dFC data with shape {self.data.graph_data.shape}")
+        self.graphFileNameLabel.setText(f"Used current dFC data with shape {self.data.graph_data.shape}")
+        self.data.graph_file = f"dfC from {self.data.file_name}" #with {self.data.dfc_name} at t={self.currentSliderValue}"
+        self.plotGraph()
+        self.onGraphCombobox()
+
+    """
+    multiverse functions
     """
-    dFC functions
+    def updateDecisionFields(self):
+        # First, clear existing fields in the decisionFieldsContainer layout
+        for i in reversed(range(self.decisionFieldsContainer.count())): 
+            self.decisionFieldsContainer.itemAt(i).widget().deleteLater()
+
+        # Check which decision type is selected and create corresponding input fields
+        decision_type = self.decisionTypeDropdown.currentText()
+        if decision_type == "strings" or decision_type == "numbers":
+            inputField = QLineEdit()
+            self.decisionFieldsContainer.addWidget(QLabel(f"Enter {decision_type}:"))
+            self.decisionFieldsContainer.addWidget(inputField)
+        elif decision_type == "booleans":
+            inputField = QComboBox()
+            inputField.addItems(["True", "False"])
+            self.decisionFieldsContainer.addWidget(QLabel("Select boolean value:"))
+            self.decisionFieldsContainer.addWidget(inputField)
+        elif decision_type in ["dfc_measures", "graph_measures"]:
+            # For complex types like dfc_measures, you might need multiple fields
+            nameField = QLineEdit()
+            connectivityField = QLineEdit()
+            inputDataField = QLineEdit()
+            self.decisionFieldsContainer.addWidget(QLabel("Name:"))
+            self.decisionFieldsContainer.addWidget(nameField)
+            self.decisionFieldsContainer.addWidget(QLabel("Connectivity:"))
+            self.decisionFieldsContainer.addWidget(connectivityField)
+            self.decisionFieldsContainer.addWidget(QLabel("Input Data:"))
+            self.decisionFieldsContainer.addWidget(inputDataField)
+            # Add more fields as needed for args etc.
+        # Add more decision types as needed
+
+    def addDecisionPoint(self):
+        decision_type = self.decisionTypeDropdown.currentText()
+        decision_data = {}
+
+        if decision_type == "strings" or decision_type == "numbers":
+            value = self.decisionFieldsContainer.itemAt(1).widget().text()  # Assuming the second widget is the input field
+            decision_data[decision_type] = [value]  # Wrap value in a list to mimic the structure
+        elif decision_type == "booleans":
+            value = self.decisionFieldsContainer.itemAt(1).widget().currentText()
+            decision_data[decision_type] = [value == "True"]  # Convert to boolean
+        elif decision_type in ["dfc_measures", "graph_measures"]:
+            # Assuming the first, third, and fifth widgets are the input fields
+            name = self.decisionFieldsContainer.itemAt(1).widget().text()
+            connectivity = self.decisionFieldsContainer.itemAt(3).widget().text()
+            input_data = self.decisionFieldsContainer.itemAt(5).widget().text()
+            # Collect more fields as needed and construct the decision data
+            decision_data[decision_type] = [{
+                "name": name,
+                "connectivity": connectivity,
+                "input_data": input_data,
+                # Include "args" and other fields as needed
+            }]
+
+        print("Added decision point:", decision_data)
+        # Here, instead of printing, you would add decision_data to your forking_paths structure
+
     """
+    dFC/graph functions
+    """
+    # dFC functions
     def onMethodCombobox(self, methodName=None):
         # Clear old variables and data
         self.clearParameters(self.parameterLayout)
 
         # Return if no methods are available
         if methodName == None or methodName == "Use checkboxes to get available methods":
             return
@@ -754,15 +1171,15 @@
             self.positionLabel.setText(position_text)
             self.slider.setValue(self.slider.value())
         
         # If connectivity data does not exist we reset the figure and slider to prepare for a new calculation
         # This also indicates to the user that this data was not yet calculated/saved
         else:
             self.figure.clear()
-            self.plotLogo()
+            self.plotLogo(self.figure)
             self.canvas.draw()
             self.distributionFigure.clear()
             self.distributionCanvas.draw()
             self.timeSeriesFigure.clear()
             self.timeSeriesCanvas.draw()
 
             position_text = f"no data available"
@@ -781,16 +1198,16 @@
                     return True 
             if self.staticCheckBox.isChecked() and className.startswith("STATIC"):
                     return True
             return False
 
         class_mappings = {
             'CONT': [
-                'Sliding Window', 'Jackknife Correlation', 'Dynamic Conditional Correlation', 
-                'Flexible Least Squares', 'Spatial Distance', 'Multiplication of Temporal Derivatives', 
+                'Sliding Window', 'Jackknife Correlation', 'Flexible Least Squares', 'Spatial Distance', 
+                'Multiplication of Temporal Derivatives', 'Dynamic Conditional Correlation', 
                 'Phase Synchronization', 'Leading Eigenvector Dynamics', 'Wavelet Coherence', 'Edge-centric Connectivity'
             ],
             'STATE': [
                 'Sliding Window Clustering', 'Co-activation patterns', 'Discrete Hidden Markov Model', 
                 'Continuous Hidden Markov Model', 'Windowless'
             ],
             'STATIC': [
@@ -919,18 +1336,57 @@
             "Schaefer Kong 200": "schaefer_kong",
             "Schaefer Tian 254": "schaefer_tian"
         }
         atlas_name = atlas_map.get(atlas_name, None)
 
         self.data.file_data = cifti.parcellate(self.data.cifti_data, atlas=atlas_name)
         self.fileNameLabel.setText(f"Loaded and parcellated {self.data.file_name} with shape {self.data.file_data.shape}")
-       
+
+    # Graph functios
+    def onGraphCombobox(self):
+        self.setGraphParameters()
+
+    def updateGraphComboBox(self):
+        def shouldIncludeFunc(funcName):
+            if self.preprocessingCheckBox.isChecked() and funcName.startswith("PREP"):
+                return True
+            if self.graphCheckBox.isChecked() and funcName.startswith("COMET"):
+                return True
+            if self.BCTCheckBox.isChecked() and funcName.startswith("BCT"):
+                return True
+            return False
+
+        # Disconnect existing connections to avoid multiple calls
+        try:
+            self.graphAnalysisComboBox.currentTextChanged.disconnect(self.onGraphCombobox)
+        except TypeError:
+            pass
+
+        # Clear the combobox
+        self.graphAnalysisComboBox.clear()
+
+        # Filter options based on the checkboxes
+        filtered_options = {name: desc for name, desc in self.graphOptions.items() if shouldIncludeFunc(desc)}
+
+        for analysis_function, pretty_name in filtered_options.items():
+            self.graphAnalysisComboBox.addItem(pretty_name, analysis_function)
+
+        # Reconnect the signal
+        self.graphAnalysisComboBox.currentTextChanged.connect(self.onGraphCombobox)
+
+        # Trigger the onGraphCombobox for the initial setup if there are any options
+        if filtered_options:
+            self.onGraphCombobox()
+
+        return
+
     """
     Parameters
     """
+    # dFC functions
     def initParameters(self, class_instance):
         # Now the parameter labels and boxes are set up    
         labels = []
 
         # Calculate the maximum label width (just a visual thing)
         max_label_width = 0
         init_signature = inspect.signature(class_instance.__init__)
@@ -1160,18 +1616,189 @@
                     widget.deleteLater()  # Schedule the widget for deletion
             elif item.layout():  # If the item is a layout
                 self.clearParameters(item.layout())  # Recursively clear the layout
                 item.layout().deleteLater()  # Delete the layout itself
             elif item.spacerItem():  # If the item is a spacer
                 # No need to delete spacer items; they are automatically handled by Qt
                 pass
+    
+    # Graph functions
+    def setGraphParameters(self):
+        # Clear parameters
+        self.clearParameters(self.graphParameterLayout)
+        
+        # Retrieve the selected function from the graph module
+        if self.graphAnalysisComboBox.currentData() == None:
+            return
+
+        func = getattr(graph, self.graphAnalysisComboBox.currentData())
+        
+        # Retrieve the signature of the function
+        func_signature = inspect.signature(func)
+        type_hints = get_type_hints(func)
+
+        # Calculate the maximum label width
+        max_label_width = 0
+        font_metrics = QFontMetrics(self.font())
+        for name, param in func_signature.parameters.items():
+            if name not in ['self', 'args', 'kwargs']:  # Skip unwanted parameters
+                label_width = font_metrics.boundingRect(f"{name}:").width()
+                max_label_width = max(max_label_width, label_width)
+
+        is_first_parameter = True  # Flag to identify the first parameter
+
+        # Iterate over parameters in the function signature
+        temp_widgets = {}
+        for name, param in func_signature.parameters.items():
+
+            if name not in ['self', 'copy', 'args', 'kwargs']:  # Skip unwanted parameters
+                # Horizontal layout for each parameter
+                param_layout = QHBoxLayout()
+                param_type = type_hints.get(name)
+                param_default = 1 if isinstance(param.default, inspect._empty) else param.default
+                
+                if param_default == None:
+                    if param_type == bool:
+                        param_default = False
+                    elif param_type == int or param_type == float:
+                        param_default = 1
+                    else:
+                        param_default = "empty"
+
+
+                # Create a label for the parameter and set its fixed width
+                param_label = QLabel(f"{name}:")
+                param_label.setFixedWidth(max_label_width + 20)  # Add some padding
+                param_layout.addWidget(param_label)
+
+                # For the first parameter, set its value based on the data source and lock it
+                if is_first_parameter:
+                    param_widget = QLineEdit("as shown in plot" if self.data.graph_file else "")
+                    param_widget.setReadOnly(True)  # Make the widget read-only
+                    is_first_parameter = False  # Update the flag so this block runs only for the first parameter
+                else:
+                    # Bool
+                    if param_type == bool:
+                        param_widget = QComboBox()
+                        param_widget.addItems(["False", "True"])
+                        param_widget.setCurrentIndex(int(param_default))
+                    # Int                  
+                    elif param_type == int:
+                        param_widget = QSpinBox()
+                        param_widget.setValue(param_default)
+                        param_widget.setMaximum(10000)
+                        param_widget.setMinimum(-10000)
+                        param_widget.setSingleStep(param_default)
+                    # Float 
+                    elif param_type == float:    
+                        param_widget = QDoubleSpinBox()
+                        if name == "threshold":
+                            param_widget.setValue(0.0)
+                        else:
+                            param_widget.setValue(param_default)
+                        param_widget.setMaximum(1.0)
+                        param_widget.setMinimum(0.0)
+                        param_widget.setSingleStep(0.01)
+                    # String
+                    elif get_origin(type_hints.get(name)) is Literal:
+                        options = type_hints.get(name).__args__ 
+                        param_widget = QComboBox()
+                        param_widget.addItems([str(option) for option in options])
+                    # Fallback
+                    else:
+                        param_widget = QLineEdit(str(param.default) if param.default != inspect.Parameter.empty else "")
+
+                temp_widgets[name] = (param_label, param_widget)
+                param_layout.addWidget(param_widget)
+                self.graphParameterLayout.addLayout(param_layout)
+
+        # Adjust visibility based on 'type' parameter
+        type_widget = None
+        if 'type' in temp_widgets:
+            _, type_widget = temp_widgets['type']
+
+        if type_widget:
+            # Function to update parameter visibility
+            def updateVisibility():
+                selected_type = type_widget.currentText()
+                if selected_type == 'absolute':
+                    if 'threshold' in temp_widgets:
+                        temp_widgets['threshold'][0].show()
+                        temp_widgets['threshold'][1].show()
+                    if 'density' in temp_widgets:
+                        temp_widgets['density'][0].hide()
+                        temp_widgets['density'][1].hide()
+                elif selected_type == 'density':
+                    if 'threshold' in temp_widgets:
+                        temp_widgets['threshold'][0].hide()
+                        temp_widgets['threshold'][1].hide()
+                    if 'density' in temp_widgets:
+                        temp_widgets['density'][0].show()
+                        temp_widgets['density'][1].show()
+            
+            # Connect the signal from the type_widget to the updateVisibility function
+            type_widget.currentIndexChanged.connect(updateVisibility)
+            updateVisibility()
+
+        self.graphParameterLayout.addStretch()
+
+    def getGraphOptions(self):
+        # Initialize a dictionary to hold parameter names and their values
+        params_dict = {}
+
+        # Iterate over all layout items in the graphParameterLayout
+        for i in range(self.graphParameterLayout.count()):
+            layout_item = self.graphParameterLayout.itemAt(i)
+
+            # Check if the layout item is a QHBoxLayout (as each parameter is in its own QHBoxLayout)
+            if isinstance(layout_item, QHBoxLayout):
+                param_layout = layout_item.layout()
+
+                # The parameter name is in the QLabel, and the value is in the second widget (QLineEdit, QComboBox, etc.)
+                if param_layout.count() >= 2:
+                    # Extract the parameter name from the QLabel
+                    param_name_label = param_layout.itemAt(0).widget()
+                    if isinstance(param_name_label, QLabel):
+                        param_name = param_name_label.text().rstrip(':')  # Remove the colon at the end
+
+                        # Extract the parameter value from the appropriate widget type
+                        param_widget = param_layout.itemAt(1).widget()
+                        if isinstance(param_widget, QLineEdit):
+                            param_value = param_widget.text()
+                        elif isinstance(param_widget, QComboBox):
+                            param_value = param_widget.currentText()
+                        elif isinstance(param_widget, QSpinBox) or isinstance(param_widget, QDoubleSpinBox):
+                            param_value = param_widget.value()
+
+                        # Convert to appropriate boolean type (LineEdit ad ComboBox return strings))
+                        if param_value == "True":
+                            param_value = True
+                        elif param_value == "False":
+                            param_value = False
+
+                        # Add the parameter name and value to the dictionary
+                        params_dict[param_name] = param_value
+
+        # Retrieve the currently selected option in the graphAnalysisComboBox
+        current_option = self.graphAnalysisComboBox.currentText()
+
+        # Return the current option and its parameters
+        return current_option, params_dict
+
+    def onClearGraphOptions(self):
+        self.data.graph_data = self.data.graph_raw
+        self.plotGraph()
+        self.optionsTextbox.clear()
+        self.graphTextbox.clear()
+        self.graphStepCounter = 1
 
     """
-    dFC calculation
+    Calculation
     """
+    # dFC functions
     def onCalculateButton(self):
         # Check if ts_data is available
         if self.data.file_data is None:
             self.calculatingLabel.setText(f"Error. No time series data has been loaded.")
             return
         
         # Get the current parameters from the UI for the upcoming calculation
@@ -1274,19 +1901,98 @@
 
     def handleError(self, error):
         # Handles errors in the worker thread
         print(f"Error occurred: {error}")
         self.calculateButton.setEnabled(True)
         self.data.clear_dfc_data()
         self.positionLabel.setText("no data available")
-        self.plotLogo()
+        self.plotLogo(self.figure)
+        self.canvas.draw()
+
+    # Graph functions
+    def onAddGraphOption(self):
+
+        # Start worker thread for graph calculations
+        self.workerThread = QThread()
+        self.worker = Worker(self.calculateGraph, None)
+        self.worker.moveToThread(self.workerThread)
+
+        self.worker.finished.connect(self.workerThread.quit)
+        self.worker.result.connect(self.handleGraphResult)  # Ensure you have a slot to handle results
+        self.worker.error.connect(self.handleGraphError)  # And error handling
+
+        self.workerThread.started.connect(self.worker.run)
+        self.workerThread.start()
+
+    def calculateGraph(self, unused):
+        option, params = self.getGraphOptions()
+
+        # Get the function
+        func_name = self.reverse_graphOptions[option]
+        func = getattr(graph, func_name)
+
+        option_name = re.sub(r'^\S+\s+', '', option) # regex to remove the PREP/GRAPH part
+        self.optionsTextbox.append(f"{self.graphStepCounter}. {option_name}: calculating, please wait...")
+
+        first_param_name = next(iter(params))
+        graph_params = {first_param_name: self.data.graph_data}
+        graph_params.update({k: v for k, v in params.items() if k != first_param_name})
+
+        graph_data = func(**graph_params)
+        return f'graph_{option.split()[0].lower()}', graph_data, option_name, graph_params
+
+    def handleGraphResult(self, result):
+        output = result[0]
+        data   = result[1]
+        option = result[2]
+        params = result[3]
+
+        print(f"Finished calculation for {option}, output data: {type(data)}.")
+
+        # Update self.data.graph_data or self.data.graph_out based on the result
+        if output == 'graph_prep':
+            self.data.graph_data = data
+            self.plotGraph()
+        else:
+            self.data.graph_out = data
+            self.plotMeasure(option)
+
+        # Output step and options to textbox, remove unused parameters
+        if option == 'Threshold':
+            if params.get('type') == 'absolute':
+                filtered_params = {k: v for k, v in params.items() if k != 'density'}
+            elif params.get('type') == 'density':
+                filtered_params = {k: v for k, v in params.items() if k != 'threshold'}
+        else:
+            filtered_params = params
+
+        filtered_params = {k: v for k, v in list(filtered_params.items())[1:]}
+
+        # Update the textbox with the current step and options
+        current_text = self.optionsTextbox.toPlainText()
+        lines = current_text.split('\n')
+
+        if len(lines) > 1:
+            lines[-1] = f"{self.graphStepCounter}. {option}: {filtered_params}"
+        else:
+            lines = [f"{self.graphStepCounter}. {option}: {filtered_params}"]
+
+        updated_text = '\n'.join(lines)
+        self.optionsTextbox.setPlainText(updated_text)
+
+        self.graphStepCounter += 1
+
+    def handleGraphError(self, error):
+        # Handles errors in the worker thread
+        print(f"Error occurred: {error}")
 
     """
     Memory functions
     """
+    # dFC functions
     def onKeepInMemoryChecked(self, state):
         if state == 2 and self.data.dfc_data is not None:
             self.data_storage.add_data(self.data)
                 
     def onClearMemory(self):
         self.data_storage = DataStorage()
         
@@ -1298,14 +2004,15 @@
         self.calculatingLabel.setText(f"Cleared memory")
         print("Cleared memory")
         return
 
     """
     Plotting functions
     """
+    # dFC functions
     def plotConnectivity(self):
         current_data = self.data.dfc_data
         
         if current_data is None:
             print("No calculated data available for plotting")
             return
 
@@ -1317,14 +2024,17 @@
             vmax = np.max(np.abs(current_slice))
             self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
         except:
             current_slice = current_data[:, :, 0] if len(current_data.shape) == 3 else current_data
             vmax = np.max(np.abs(current_slice))
             self.im = ax.imshow(current_slice, cmap='coolwarm', vmin=-vmax, vmax=vmax)
 
+        ax.set_xlabel("ROI")
+        ax.set_ylabel("ROI")
+
         # Create the colorbar
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.15)
         cbar = self.figure.colorbar(self.im, cax=cax)
         cbar.ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
 
         self.slider.setMaximum(current_data.shape[2] - 1 if len(current_data.shape) == 3 else 0)
@@ -1347,17 +2057,17 @@
         self.colSelector.show()
 
         if current_data is not None and row < current_data.shape[0] and col < current_data.shape[1] and self.data.dfc_edge_ts is None and self.data.dfc_state_tc is None:    
             self.timeSeriesFigure.clear()
             ax = self.timeSeriesFigure.add_subplot(111)
             time_series = current_data[row, col, :] if len(current_data.shape) == 3 else current_data[row, col]
             ax.set_title(f"dFC time course between region {row} and {col}.")
-            
+            ax.set_xlabel("time (TRs)")
+            ax.set_ylabel("dFC strength")
             ax.plot(time_series)
-            self.timeSeriesCanvas.draw()
 
         elif self.data.dfc_state_tc is not None:
             self.timeSeriesFigure.clear()
 
             time_series = self.data.dfc_state_tc
             num_states = len(self.data.dfc_states)
 
@@ -1379,16 +2089,14 @@
             for col, (state, matrix) in enumerate(self.data.dfc_states.items()):
                 ax_state = self.timeSeriesFigure.add_subplot(gs[2, col])
                 ax_state.imshow(matrix, cmap='coolwarm', aspect=1)
                 ax_state.set_title(f"State {col+1}")
                 ax_state.set_xticks([])
                 ax_state.set_yticks([]) 
 
-            self.timeSeriesFigure.canvas.draw()
-
         elif self.data.dfc_edge_ts is not None:
             self.timeSeriesFigure.clear()
             gs = gridspec.GridSpec(3, 1, self.timeSeriesFigure, height_ratios=[2, 0.5, 1]) # GridSpec with 3 rows and 1 column
 
             # The first subplot occupies the 1st row
             ax1 = self.timeSeriesFigure.add_subplot(gs[:1, 0])
             ax1.imshow(self.data.dfc_edge_ts.T, cmap='coolwarm', aspect='auto', vmin=-1*self.data.dfc_params["vlim"], vmax=self.data.dfc_params["vlim"])
@@ -1400,21 +2108,24 @@
             ax2 = self.timeSeriesFigure.add_subplot(gs[2, 0])
             mean_edge_values = np.mean(self.data.dfc_edge_ts.T, axis=0)
             ax2.plot(mean_edge_values)
             ax2.set_xlim(0, len(mean_edge_values) - 1)
             ax2.set_title("Mean time series")
             ax2.set_xlabel("Time (TRs)")
             ax2.set_ylabel("Mean Edge Value")
-            
-            self.timeSeriesFigure.canvas.draw()
         
         else:
             # Clear the plot if the data is not available
             self.timeSeriesFigure.clear()
-            self.timeSeriesCanvas.draw()
+
+        self.timeSeriesFigure.set_facecolor('#E0E0E0')
+        self.timeSeriesFigure.tight_layout()
+        self.timeSeriesCanvas.draw()
+
+        return
 
     def plotDistribution(self):
         current_data = self.data.dfc_data
 
         if current_data is None or not hasattr(self, 'distributionFigure'):
             self.distributionFigure.clear()
             return
@@ -1422,29 +2133,22 @@
         # Clear the current distribution plot
         self.distributionFigure.clear()
 
         # Assuming you want to plot the distribution of values in the current slice
         current_slice = current_data[:, :, self.slider.value()] if len(current_data.shape) == 3 else current_data
         ax = self.distributionFigure.add_subplot(111)
         ax.hist(current_slice.flatten(), bins=50)  # number of bins
+        ax.set_xlabel("dFC values")
+        ax.set_ylabel("frequency")
 
+        self.distributionFigure.set_facecolor('#E0E0E0')
+        self.distributionFigure.tight_layout()
         self.distributionCanvas.draw()
 
-    def plotLogo(self):
-        with pkg_resources.path("comet.resources.img", "logo.png") as file_path:
-            logo = imread(file_path)
-
-        self.figure.clear()
-        ax = self.figure.add_subplot(111)
-        ax.set_axis_off()
-        self.im = ax.imshow(logo)
-
-        self.figure.set_facecolor('#f4f1f6')
-        self.figure.tight_layout()
-        self.canvas.draw()
+        return
 
     def updateTimeSeriesPlot(self, center):
         if self.data.dfc_data is None:
             return
 
         max_index = self.data.dfc_data.shape[2] - 1 if len(self.data.dfc_data.shape) == 3 else 0
         width = 101
@@ -1460,25 +2164,29 @@
         row = self.rowSelector.value()
         col = self.colSelector.value()
         time_series_slice = self.dfc_data['data'][row, col, start:end]
 
         self.timeSeriesFigure.clear()
         ax = self.timeSeriesFigure.add_subplot(111)
         ax.plot(range(start, end), time_series_slice)
+        
+        self.timeSeriesFigure.tight_layout()
         self.timeSeriesCanvas.draw()
+        
+        return
 
     def onTabChanged(self):
         self.currentTabIndex = self.tabWidget.currentIndex()
         # index 0: Connectivity plot
         # index 1: Time series plot
         # index 2: Distribution plot
         # index 3: Graph analysis
 
         if self.data.dfc_data is None:
-            self.plotLogo()
+            self.plotLogo(self.figure)
             self.canvas.draw()
             self.distributionFigure.clear()
             self.distributionCanvas.draw()
             self.timeSeriesFigure.clear()
             self.timeSeriesCanvas.draw()
             self.backLargeButton.hide()
             self.backButton.hide()
@@ -1596,14 +2304,145 @@
         self.currentSliderValue = max(0, min(self.slider.value() + delta, self.slider.maximum()))
         self.slider.setValue(self.currentSliderValue)
         self.slider.update()
         
         self.plotConnectivity()
         self.plotDistribution()
 
+    # Graph functions
+    def plotGraph(self):
+        current_data = self.data.graph_data
+        
+        if current_data is None:
+            print("No data available for plotting")
+            return
+
+        self.matrixFigure.clear()
+        ax = self.matrixFigure.add_subplot(111)
+
+        vmax = np.max(np.abs(current_data))
+        self.im = ax.imshow(current_data, cmap='coolwarm', vmin=-vmax, vmax=vmax)
+        ax.set_xlabel("ROI")
+        ax.set_ylabel("ROI")
+
+        # Create the colorbar
+        divider = make_axes_locatable(ax)
+        cax = divider.append_axes("right", size="5%", pad=0.15)
+        cbar = self.matrixFigure.colorbar(self.im, cax=cax)
+        cbar.ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
+    
+        self.matrixFigure.set_facecolor('#E0E0E0')
+        self.matrixFigure.tight_layout()
+        self.matrixCanvas.draw()
+
+    def plotMeasure(self, measure):
+        self.graphFigure.clear()
+        ax = self.graphFigure.add_subplot(111)
+        
+        # Check type of the graph output data
+        if isinstance(self.data.graph_out, (np.ndarray, np.float64)):
+            if self.data.graph_out.ndim == 0:
+                # If graph_out is a single value (0D array)
+                self.graphTextbox.append(f"{measure}: {self.data.graph_out.item()}")
+            elif self.data.graph_out.ndim == 1:
+                # For a 1D array, plot a vertical lollipop plot
+                ax.stem(self.data.graph_out, linefmt="#19232d", markerfmt='o', basefmt=" ")
+                ax.set_xlabel("ROI")
+                ax.set_ylabel(measure)
+
+                # Calculate mean and variance, and update the textbox
+                mean_val = np.mean(self.data.graph_out)
+                var_val = np.var(self.data.graph_out)
+                self.graphTextbox.append(f"{measure} (mean: {mean_val:.2f}, variance: {var_val:.2f})")
+            
+            elif self.data.graph_out.ndim == 2:
+                # For a 2D array, use imshow
+                vmax = np.max(np.abs(self.data.graph_out))
+                im = ax.imshow(self.data.graph_out, cmap='coolwarm', vmin=-vmax, vmax=vmax)
+
+                # Create the colorbar
+                divider = make_axes_locatable(ax)
+                cax = divider.append_axes("right", size="5%", pad=0.15)
+                self.graphFigure.colorbar(im, cax=cax).ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
+            else:
+                self.graphTextbox.append("3D graph data not currently supported for plotting.")
+        
+        elif isinstance(self.data.graph_out, dict):
+            # Setup data for output
+            output_string = f"{measure}: "
+            output_arrays = []
+            for key, value in self.data.graph_out.items():
+                if isinstance(value, (int, float)):
+                    output_string += f"{key}: {value:.2f}, "
+                    self.plotLogo(self.graphFigure)
+
+                elif isinstance(value, np.ndarray):
+                    output_arrays.append((key, value))
+
+            # Print the output string
+            self.graphTextbox.append(output_string.strip(', '))  # Remove the trailing comma
+
+            # Plot the output arrays
+            if output_arrays:
+                self.graphFigure.clear()
+                n_subplots = len(output_arrays)
+
+                for i, (key, value) in enumerate(output_arrays):
+                    ax = self.graphFigure.add_subplot(1, n_subplots, i + 1)
+                    vmax = np.max(np.abs(value))
+                    if value.ndim == 1:
+                        # For a 1D vector, plot a vertical lollipop plot
+                        ax.stem(value, linefmt="#19232d", markerfmt='o', basefmt=" ")
+                        ax.set_xlabel("ROI")
+                        ax.set_ylabel(measure)
+
+                        # Calculate mean and variance, and update the textbox
+                        mean_val = np.mean(value)
+                        var_val = np.var(value)
+                        self.graphTextbox.append(f"{measure} (mean: {mean_val:.2f}, variance: {var_val:.2f})")
+                        
+                    elif value.ndim == 2:
+                        # For a 2D array, use imshow
+                        im = ax.imshow(value, cmap='coolwarm', vmin=-vmax, vmax=vmax)
+                        ax.set_title(key)
+    
+                        # Create the colorbar
+                        divider = make_axes_locatable(ax)
+                        cax = divider.append_axes("right", size="5%", pad=0.15)
+                        cbar = self.graphFigure.colorbar(im, cax=cax)
+                        cbar.ax.yaxis.set_major_formatter(FuncFormatter(lambda x, _: f'{x:.1f}'))
+  
+                    else:
+                        self.graphTextbox.append("Graph output data is not in expected format.")
+
+                    ax.set_title(key)
+        
+        else:
+            self.graphTextbox.append("Graph output data is not in expected format.")
+
+        # Draw the plot
+        self.graphFigure.set_facecolor('#E0E0E0')
+        self.graphFigure.tight_layout()
+        self.graphCanvas.draw()
+        
+        return
+    
+    # Shared functions
+    def plotLogo(self, figure=None):
+        with pkg_resources.path("comet.resources.img", "logo.png") as file_path:
+            logo = imread(file_path)
+
+        figure.clear()
+        ax = figure.add_subplot(111)
+        ax.set_axis_off()
+        ax.imshow(logo)
+
+        figure.set_facecolor('#f4f1f6')
+        figure.tight_layout()
+
 """
 Run the application
 """
 def run(dfc_data=None, method=None):
     app = QApplication(sys.argv)
 
     # Set global stylesheet for tooltips
@@ -1611,14 +2450,21 @@
         QToolTip {
             background-color: #E0E0E0;
             border: 1px solid black;
         }
     """)
     ex = App(init_dfc_data=dfc_data, init_dfc_instance=method)
     ex.setStyleSheet(qdarkstyle.load_stylesheet_pyqt6())
+
+    default_width = ex.width()
+    default_height = ex.height()
+    new_width = int(default_width * 1.8)
+    new_height = int(default_height * 1.5)
+    ex.resize(new_width, new_height)
+
     ex.show()
 
     try:
         sys.exit(app.exec())
     except SystemExit as e:
         print(f"GUI closed with status {e}")
```

### Comparing `comet_toolbox-0.2.1/src/comet/methods.py` & `comet_toolbox-0.3.0/src/comet/methods.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/multiverse.py` & `comet_toolbox-0.3.0/src/comet/multiverse.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/simulation.pkl` & `comet_toolbox-0.3.0/src/comet/resources/simulation.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/simulation.txt` & `comet_toolbox-0.3.0/tutorials/example_data/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/single_state.txt` & `comet_toolbox-0.3.0/src/comet/resources/single_state.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii` & `comet_toolbox-0.3.0/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/atlas/README.md` & `comet_toolbox-0.3.0/src/comet/resources/atlas/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii` & `comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii` & `comet_toolbox-0.3.0/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat` & `comet_toolbox-0.3.0/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/img/badge.svg` & `comet_toolbox-0.3.0/src/comet/resources/img/badge.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/img/content.drawio` & `comet_toolbox-0.3.0/src/comet/resources/img/content.drawio`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/img/content.png` & `comet_toolbox-0.3.0/src/comet/resources/img/content.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/img/gui.png` & `comet_toolbox-0.3.0/src/comet/resources/img/gui.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/src/comet/resources/img/logo.png` & `comet_toolbox-0.3.0/src/comet/resources/img/logo.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_analysis.ipynb` & `comet_toolbox-0.3.0/tutorials/example_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_dfc.ipynb` & `comet_toolbox-0.3.0/tutorials/example_dfc.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_graph.ipynb` & `comet_toolbox-0.3.0/tutorials/example_graph.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_multiverse.ipynb` & `comet_toolbox-0.3.0/tutorials/example_multiverse.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_data/abide_50008.txt` & `comet_toolbox-0.3.0/tutorials/example_data/abide_50008.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_data/aomic_multi.pkl` & `comet_toolbox-0.3.0/tutorials/example_data/aomic_multi.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/example_data/xcpd.tsv` & `comet_toolbox-0.3.0/tutorials/example_data/xcpd.tsv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_1.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_1.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_10.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_10.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_11.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_11.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_12.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_12.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_13.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_13.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_14.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_14.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_15.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_15.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_16.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_16.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_17.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_17.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_18.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_18.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_19.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_19.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_2.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_2.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_20.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_20.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_21.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_21.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_22.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_22.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_23.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_23.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_24.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_24.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_25.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_25.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_26.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_26.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_27.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_27.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_28.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_28.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_29.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_29.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_3.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_3.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_30.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_30.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_31.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_31.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_32.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_32.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_33.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_33.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_34.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_34.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_35.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_35.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_36.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_36.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_37.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_37.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_38.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_38.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_39.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_39.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_4.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_4.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_40.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_40.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_41.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_41.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_42.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_42.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_43.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_43.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_44.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_44.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_45.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_45.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_46.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_46.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_47.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_47.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_48.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_48.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_49.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_49.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_5.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_5.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_50.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_50.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_51.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_51.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_52.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_52.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_53.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_53.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_54.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_54.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_55.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_55.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_56.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_56.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_57.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_57.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_58.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_58.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_59.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_59.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_6.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_6.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_60.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_60.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_61.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_61.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_62.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_62.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_63.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_63.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_64.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_64.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_65.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_65.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_66.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_66.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_67.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_67.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_68.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_68.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_69.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_69.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_7.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_7.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_70.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_70.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_71.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_71.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_72.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_72.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_73.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_73.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_74.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_74.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_75.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_75.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_76.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_76.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_77.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_77.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_78.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_78.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_79.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_79.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_8.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_8.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_80.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_80.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_81.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_81.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_82.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_82.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_83.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_83.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_84.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_84.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_85.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_85.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_86.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_86.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_87.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_87.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_88.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_88.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_89.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_89.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_9.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_9.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_90.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_90.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_91.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_91.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_92.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_92.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_93.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_93.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_94.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_94.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_95.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_95.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/universe_96.py` & `comet_toolbox-0.3.0/tutorials/multiverse/universe_96.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/results/forking_paths.pkl` & `comet_toolbox-0.3.0/tutorials/multiverse/results/forking_paths.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.3.0/tutorials/multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/tutorials/multiverse/results/pipelines.csv` & `comet_toolbox-0.3.0/tutorials/multiverse/results/pipelines.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/.gitignore` & `comet_toolbox-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/LICENSE` & `comet_toolbox-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.2.1/README.md` & `comet_toolbox-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 ## Comet - A dynamic functional connectivity toolbox for multiverse analysis
 [![DOI](src/comet/resources/img/badge.svg)](https://doi.org/10.1101/2024.01.21.576546)
 
 **Important notes:**
 
 * This package is at an early stage of development, with frequent changes being made. If you intend to use this package at this stage, I kindly ask that you contact me via the email address in the [pyproject.toml](https://github.com/mibur1/dfc-multiverse/blob/main/pyproject.toml) file.
 * Many features are not yet tested, so there will be bugs (the question is just how many). A comprehensive testing suite and documentation will be added in the near future
-* The GUI still has many bugs, so using the scripting API is recommended for now
 
 ### Current Features
 
 ![Features_image](src/comet/resources/img/content.png)
 
 ### Installation
```

### Comparing `comet_toolbox-0.2.1/pyproject.toml` & `comet_toolbox-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comet-toolbox"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   {name="Micha Burkhardt", email="micha.burkhardt@uol.de"},
 ]
 description = "Dynamic functional connectivity toolbox for multiverse analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `comet_toolbox-0.2.1/PKG-INFO` & `comet_toolbox-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: comet-toolbox
-Version: 0.2.1
+Version: 0.3.0
 Summary: Dynamic functional connectivity toolbox for multiverse analysis
 Project-URL: Homepage, https://github.com/mibur1/dfc-multiverse
 Project-URL: Issues, https://github.com/mibur1/dfc-multiverse/issues
 Author-email: Micha Burkhardt <micha.burkhardt@uol.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,14 @@
 ## Comet - A dynamic functional connectivity toolbox for multiverse analysis
 [![DOI](src/comet/resources/img/badge.svg)](https://doi.org/10.1101/2024.01.21.576546)
 
 **Important notes:**
 
 * This package is at an early stage of development, with frequent changes being made. If you intend to use this package at this stage, I kindly ask that you contact me via the email address in the [pyproject.toml](https://github.com/mibur1/dfc-multiverse/blob/main/pyproject.toml) file.
 * Many features are not yet tested, so there will be bugs (the question is just how many). A comprehensive testing suite and documentation will be added in the near future
-* The GUI still has many bugs, so using the scripting API is recommended for now
 
 ### Current Features
 
 ![Features_image](src/comet/resources/img/content.png)
 
 ### Installation
```

