# Comparing `tmp/dcm_classifier-0.8.1.tar.gz` & `tmp/dcm_classifier-0.8.2.tar.gz`

## Comparing `dcm_classifier-0.8.1.tar` & `dcm_classifier-0.8.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.git
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/citations/EndNote_citation.enw
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/citations/RIS_citation.ris
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/citations/bib_citation.bib
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    18085 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32256 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/LICENSE
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/README.md
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.git
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/citations/EndNote_citation.enw
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/citations/RIS_citation.ris
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/citations/bib_citation.bib
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    18435 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32425 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2203268 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11603 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/LICENSE
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 dcm_classifier-0.8.2/PKG-INFO
```

### Comparing `dcm_classifier-0.8.1/.pre-commit-config.yaml` & `dcm_classifier-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/CONTRIBUTING.md` & `dcm_classifier-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.8.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/.github/workflows/push_to_main.yml` & `dcm_classifier-0.8.2/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/citations/bib_citation.bib` & `dcm_classifier-0.8.2/citations/bib_citation.bib`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/models/ova_rf_classifier.onnx` & `dcm_classifier-0.8.2/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/models/rf_classifier.onnx` & `dcm_classifier-0.8.2/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.8.2/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/classify_study.py` & `dcm_classifier-0.8.2/scripts/classify_study.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
                 current_dict["Acq.Plane"] = str(volume.get_acquisition_plane())
             except AttributeError:
                 current_dict["Acq.Plane"] = "None"
             try:
                 current_dict["Isotropic"] = str(volume.get_is_isotropic())
             except AttributeError:
                 current_dict["Isotropic"] = "None"
-
-            print(volume.get_modality_probabilities().to_string(index=False))
+            vol_probabilities = volume.get_modality_probabilities()
+            print(vol_probabilities.to_string(index=False))
             try:
                 current_dict["Bvalue"] = str(volume.get_volume_bvalue())
             except AttributeError:
                 current_dict["Bvalue"] = "None"
             try:
                 current_dict["SeriesDesc"] = volume.get_volume_series_description()
             except AttributeError:
```

### Comparing `dcm_classifier-0.8.1/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.8.2/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/create_training_sheet.py` & `dcm_classifier-0.8.2/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.8.2/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/modality_classifier_training.py` & `dcm_classifier-0.8.2/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.8.2/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/orientation_model_training.py` & `dcm_classifier-0.8.2/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.8.2/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/running_classifier.ipynb` & `dcm_classifier-0.8.2/scripts/running_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/todo_list` & `dcm_classifier-0.8.2/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/training_config.py` & `dcm_classifier-0.8.2/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/scripts/utilities.py` & `dcm_classifier-0.8.2/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.8.2/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.8.2/src/dcm_classifier/dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.8.2/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.8.2/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.8.2/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.8.2/src/dcm_classifier/image_type_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 )
 from pathlib import Path
 import warnings
 
 import numpy as np
 import pandas as pd
 
-from typing import Any, Optional
+from typing import Any
 
 
 imagetype_to_integer_mapping = {
     "t1w": 0,
     "gret2star": 1,
     "t2w": 2,
     "flair": 3,
@@ -366,14 +366,21 @@
                 volume.set_has_contrast(contrast)
 
                 modality, full_outputs = self.infer_modality(
                     feature_dict=volume.get_volume_dictionary()
                 )
                 volume.set_volume_modality(modality)
                 volume.set_modality_probabilities(pd.DataFrame(full_outputs, index=[0]))
+            else:
+                # if features are not validated, set values to defaults
+                volume.set_acquisition_plane("INVALID")
+                volume.set_is_isotropic(False)
+                volume.set_has_contrast(False)
+                volume.set_volume_modality("INVALID")
+                volume.set_modality_probabilities(pd.DataFrame())
 
         """
         Aggregates the modality and acquisition plane information from the volumes to the series level.
         """
         # if there is only a single volume in the series, the series modality and acquisition plane are set to the
         # volume's modality and acquisition plane
         if len(self.series.get_volume_list()) == 1:
```

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.8.2/src/dcm_classifier/study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.8.2/src/dcm_classifier/utility_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,14 @@
                 dicom_element = dicom_header_info[v]
 
             # This decoding of bvalues follows the NAMIC conventions defined at
             # https://www.na-mic.org/wiki/NAMIC_Wiki:DTI:DICOM_for_DWI_and_DTI
             # TODO: add testing for this
             if v == private_tags_map["GE"]:
                 large_number_modulo_for_GE = 100000
-                # value = dicom_element.value[0] % large_number_modulo_for_GE
                 # TODO: This is a hack to get around an error. Might be due to missing data in SickKids project
                 try:
                     value = dicom_element.value[0] % large_number_modulo_for_GE
                 except TypeError:
                     return -12345
             elif v == private_tags_map["Siemens_historical"]:
                 # This is not supported yet
@@ -198,23 +197,29 @@
                     pass
                 else:
                     print(
                         f"UNKNOWN CONVERSION OF VR={dicom_element.VR}: {type(dicom_element.value)} len={len(dicom_element.value)} ==> {value}"
                     )
                     return -12345
             # print(f"Found BValue at {v} for {k}, {value} of type {dicom_element.VR}")
+            if value is None:
+                # Field exists without value, USE DEFAULT
+                return -12345
             try:
                 result = float(value)
                 if result > 5000:
                     return -12345
             except ValueError:
                 print(
                     f"UNKNOWN CONVERSION OF VR={dicom_element.VR}: {type(dicom_element.value)} len={len(dicom_element.value)} ==> {dicom_element.value} to float"
                 )
                 return -12345
+            except Exception as e:
+                print(f"UNKNOWN IDENTIFICATION OF BVALUE: {e}")
+                return -12345
             if round_to_nearst_10:
                 result = round(result / 10.0) * 10
             return result
     return -12345
 
 
 def ensure_magnitude_of_1(vector: np.ndarray) -> bool:
```

### Comparing `dcm_classifier-0.8.1/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.8.2/src/dcm_classifier/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/conftest.py` & `dcm_classifier-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.8.2/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files 19% similar despite different names*

#### anonymized_testing_data.tar

##### file list

```diff
@@ -1,533 +1,534 @@
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149132 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149148 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149134 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149134 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111492 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234544 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234538 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    10135 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/flair.xml
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234548 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234540 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   234538 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832602 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653406 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653406 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653404 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653398 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653398 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653404 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    66394 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66382 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66384 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218166 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111704 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111694 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111694 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111696 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111700 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166946 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166948 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166956 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166952 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111492 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314416 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   149114 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149110 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149110 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149114 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    66392 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66388 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)    66396 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66394 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    66382 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/
--rw-r--r--   0 cavriley (2446225) users      (100)    13532 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/no_valid_fields.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64842 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64850 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/
--rw-r--r--   0 cavriley (2446225) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832220 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm
--rw-r--r--   0 cavriley (2446225) users      (100)   832220 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/all_fields_data/
--rw-r--r--   0 cavriley (2446225) users      (100)    64900 2024-03-28 15:09:01.000000 anonymized_testing_data/all_fields_data/all_fields_file.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/with_contrast/
--rw-r--r--   0 cavriley (2446225) users      (100)   437476 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
-drwxr-xr-x   0 cavriley (2446225) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/without_contrast/
--rw-r--r--   0 cavriley (2446225) users      (100)   132600 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    13532 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/no_valid_fields.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-04-15 18:16:35.000000 anonymized_testing_data/invalid_data/invalid_fields/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64842 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149116 2024-04-15 18:16:19.000000 anonymized_testing_data/invalid_data/invalid_fields/emptyBValue.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64850 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832220 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832220 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832640 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/without_contrast/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   132600 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/with_contrast/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   437476 2024-03-28 15:09:01.000000 anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218166 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218160 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218156 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   218162 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149148 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149142 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149134 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149134 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149132 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149150 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149136 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149146 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149140 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149138 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149144 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66382 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66396 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66394 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111706 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111704 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111694 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111702 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111694 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111696 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111700 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111698 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314416 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314422 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314418 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314412 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   314414 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149114 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149110 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149114 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149116 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149112 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149120 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   149110 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66392 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66388 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66390 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66382 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66384 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    66394 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166956 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166948 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166952 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166958 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166954 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166946 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   166950 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653406 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653406 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653398 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653400 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653404 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653408 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653402 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653410 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653398 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   653404 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64868 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64870 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64880 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64874 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64876 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64872 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64878 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111492 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234540 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234538 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234546 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234544 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234548 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    10135 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/flair.xml
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234538 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234550 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   234542 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111494 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111492 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111496 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111498 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111500 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   111502 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832602 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832592 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832598 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
+-rw-r--r--   0 mbrzus   (2269401) users      (100)   832596 2024-03-28 15:09:01.000000 anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
+drwxr-xr-x   0 mbrzus   (2269401) users      (100)        0 2024-03-28 15:09:01.000000 anonymized_testing_data/all_fields_data/
+-rw-r--r--   0 mbrzus   (2269401) users      (100)    64900 2024-03-28 15:09:01.000000 anonymized_testing_data/all_fields_data/all_fields_file.dcm
```

### Comparing `dcm_classifier-0.8.1/tests/testing_data/mock_data.txt` & `dcm_classifier-0.8.2/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.8.2/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.8.2/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.8.2/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.8.2/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.8.2/tests/unit_testing/test_utility_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     convert_array_to_min_max,
     sanitize_dicom_dataset,
     itk_read_from_dicomfn_list,
     is_integer,
     ensure_magnitude_of_1,
     convert_array_to_index_value,
     get_coded_dictionary_elements,
+    get_bvalue,
 )
 from dcm_classifier.dicom_config import required_DICOM_fields, optional_DICOM_fields
 from pathlib import Path
 
 relative_testing_data_path: Path = Path(__file__).parent.parent / "testing_data"
 current_file_path: Path = Path(__file__).parent
 inference_model_path = list(
-    current_file_path.parent.parent.rglob("models/rf_classifier.onnx")
+    current_file_path.parent.parent.rglob("models/ova_rf_classifier.onnx")
 )[0]
 
 
 def test_rglob_for_singular_result():
     single_file_dir = (
         relative_testing_data_path / "dummy_directory" / "dir_with_one_file"
     )
@@ -202,14 +203,27 @@
 
     f = pydicom.dcmread(vol[0])
     ds_dict = sanitize_dicom_dataset(f, required_DICOM_fields, optional_DICOM_fields)[0]
 
     assert ds_dict["PixelBandwidth"] == "INVALID_VALUE"
 
 
+def test_empty_bvalue():
+    assert dicom_file_dir.exists()
+    vol = list()
+    for file in dicom_file_dir.iterdir():
+        if "emptyBValue" in file.stem:
+            vol.append(file)
+
+    f = pydicom.dcmread(vol[0])
+    bval = get_bvalue(f)
+
+    assert bval == -12345
+
+
 def test_invalid_fields():
     file_dir = dicom_file_dir.parent
 
     assert file_dir.exists()
     vol = list()
     for file in file_dir.iterdir():
         if "no_valid" in file.stem:
```

### Comparing `dcm_classifier-0.8.1/.gitignore` & `dcm_classifier-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/LICENSE` & `dcm_classifier-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/README.md` & `dcm_classifier-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.1/pyproject.toml` & `dcm_classifier-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.8.1'
+version = '0.8.2'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
   { name="Cavan Riley", email="cavan-riley@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
```

### Comparing `dcm_classifier-0.8.1/PKG-INFO` & `dcm_classifier-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.8.1
+Version: 0.8.2
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>, Cavan Riley <cavan-riley@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: itk-core>=5.3.0
```

