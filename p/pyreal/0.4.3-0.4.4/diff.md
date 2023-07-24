# Comparing `tmp/pyreal-0.4.3.tar.gz` & `tmp/pyreal-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreal-0.4.3.tar", max compression
+gzip compressed data, was "pyreal-0.4.4.tar", max compression
```

## Comparing `pyreal-0.4.3.tar` & `pyreal-0.4.4.tar`

### file list

```diff
@@ -1,148 +1,150 @@
--rw-r--r--   0        0        0      165 2023-07-05 17:31:15.912947 pyreal-0.4.3/AUTHORS.rst
--rw-r--r--   0        0        0        9 2023-07-05 17:31:15.912947 pyreal-0.4.3/HISTORY.md
--rw-r--r--   0        0        0     1075 2023-07-05 17:31:15.912947 pyreal-0.4.3/LICENSE
--rw-r--r--   0        0        0     4242 2023-07-05 17:31:15.912947 pyreal-0.4.3/README.md
--rw-r--r--   0        0        0     1787 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      240 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/__init__.py
--rw-r--r--   0        0        0     3042 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/explainer_challenge.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/gfi/__init__.py
--rw-r--r--   0        0        0      436 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
--rw-r--r--   0        0        0      430 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/lfc/__init__.py
--rw-r--r--   0        0        0      439 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
--rw-r--r--   0        0        0      436 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
--rw-r--r--   0        0        0     1623 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/dataset.py
--rw-r--r--   0        0        0      610 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/download_datasets_script.py
--rw-r--r--   0        0        0     5213 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/main.py
--rw-r--r--   0        0        0    15073 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
--rw-r--r--   0        0        0     1652 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/adult_logistic_regression.pkl
--rw-r--r--   0        0        0     3108 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
--rw-r--r--   0        0        0     1244 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
--rw-r--r--   0        0        0      941 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
--rw-r--r--   0        0        0      892 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
--rw-r--r--   0        0        0      881 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/breast-w_logistic_regression.pkl
--rw-r--r--   0        0        0     1116 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/cmc_logistic_regression.pkl
--rw-r--r--   0        0        0    62681 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
--rw-r--r--   0        0        0     1180 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
--rw-r--r--   0        0        0     1300 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/credit-g_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/diabetes_logistic_regression.pkl
--rw-r--r--   0        0        0      873 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/electricity_logistic_regression.pkl
--rw-r--r--   0        0        0     4528 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
--rw-r--r--   0        0        0     3423 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
--rw-r--r--   0        0        0      948 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/ilpd_logistic_regression.pkl
--rw-r--r--   0        0        0   129793 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/isolet_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/jm1_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/kc1_logistic_regression.pkl
--rw-r--r--   0        0        0      977 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/kc2_logistic_regression.pkl
--rw-r--r--   0        0        0     1396 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
--rw-r--r--   0        0        0     4636 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/letter_logistic_regression.pkl
--rw-r--r--   0        0        0     4865 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/madelon_logistic_regression.pkl
--rw-r--r--   0        0        0    18351 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
--rw-r--r--   0        0        0     7151 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
--rw-r--r--   0        0        0     1551 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
--rw-r--r--   0        0        0     4831 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
--rw-r--r--   0        0        0    63793 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
--rw-r--r--   0        0        0     1807 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/nomao_logistic_regression.pkl
--rw-r--r--   0        0        0     6191 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/optdigits_logistic_regression.pkl
--rw-r--r--   0        0        0     1439 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
--rw-r--r--   0        0        0     1028 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pc1_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pc3_logistic_regression.pkl
--rw-r--r--   0        0        0     1159 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pc4_logistic_regression.pkl
--rw-r--r--   0        0        0     2351 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/pendigits_logistic_regression.pkl
--rw-r--r--   0        0        0      900 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/phoneme_logistic_regression.pkl
--rw-r--r--   0        0        0     1191 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
--rw-r--r--   0        0        0     2703 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/satimage_logistic_regression.pkl
--rw-r--r--   0        0        0    21553 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/semeion_logistic_regression.pkl
--rw-r--r--   0        0        0     1228 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/sick_logistic_regression.pkl
--rw-r--r--   0        0        0     1319 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/spambase_logistic_regression.pkl
--rw-r--r--   0        0        0     7738 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/splice_logistic_regression.pkl
--rw-r--r--   0        0        0     1025 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
--rw-r--r--   0        0        0     1444 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/vehicle_logistic_regression.pkl
--rw-r--r--   0        0        0     3384 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/vowel_logistic_regression.pkl
--rw-r--r--   0        0        0     1695 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
--rw-r--r--   0        0        0     1100 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/models/wdbc_logistic_regression.pkl
--rw-r--r--   0        0        0      145 2023-07-05 17:31:15.916947 pyreal-0.4.3/pyreal/benchmark/models.py
--rw-r--r--   0        0        0    10056 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10104 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
--rw-r--r--   0        0        0    10111 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
--rw-r--r--   0        0        0    10072 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0    10069 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
--rw-r--r--   0        0        0    10073 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
--rw-r--r--   0        0        0     1186 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/benchmark/task.py
--rw-r--r--   0        0        0     2315 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/__init__.py
--rw-r--r--   0        0        0    20704 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/base.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/__init__.py
--rw-r--r--   0        0        0     3338 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/base.py
--rw-r--r--   0        0        0     3019 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/decision_tree_explainer.py
--rw-r--r--   0        0        0     3448 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/dte/surrogate_decision_tree.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/example/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/example/base.py
--rw-r--r--   0        0        0     2819 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/example/similar_examples.py
--rw-r--r--   0        0        0     4883 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/generic_explainer.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/__init__.py
--rw-r--r--   0        0        0     4301 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/base.py
--rw-r--r--   0        0        0     2984 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/global_feature_importance.py
--rw-r--r--   0        0        0     2237 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/permutation_feature_importance.py
--rw-r--r--   0        0        0     3729 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/gfi/shap_feature_importance.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/__init__.py
--rw-r--r--   0        0        0     4990 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/base.py
--rw-r--r--   0        0        0     3135 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/local_feature_contribution.py
--rw-r--r--   0        0        0     4425 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/shap_feature_contribution.py
--rw-r--r--   0        0        0     3354 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/lfc/simple_counterfactual_contribution.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/__init__.py
--rw-r--r--   0        0        0     3625 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/base.py
--rw-r--r--   0        0        0     2796 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence.py
--rw-r--r--   0        0        0     1929 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence_explainer.py
--rw-r--r--   0        0        0      372 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/__init__.py
--rw-r--r--   0        0        0     4689 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/base.py
--rw-r--r--   0        0        0     5623 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
--rw-r--r--   0        0        0     5916 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/realapp/__init__.py
--rw-r--r--   0        0        0    26048 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/realapp/realapp.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/sample_applications/__init__.py
--rw-r--r--   0        0        0     8997 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/sample_applications/ames_housing.py
--rw-r--r--   0        0        0     1769 2023-07-05 17:31:15.920947 pyreal-0.4.3/pyreal/sample_applications/california_housing.py
--rw-r--r--   0        0        0   460673 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data.csv
--rw-r--r--   0        0        0    13637 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data_description.txt
--rw-r--r--   0        0        0     3431 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
--rw-r--r--   0        0        0    14681 2023-07-05 17:31:15.924947 pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
--rw-r--r--   0        0        0  1217129 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/california.csv
--rw-r--r--   0        0        0    68558 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_student/data.csv
--rw-r--r--   0        0        0     1514 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_student/students.csv
--rw-r--r--   0        0        0    60300 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/data_titanic/data.csv
--rw-r--r--   0        0        0     4570 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/student_performance.py
--rw-r--r--   0        0        0     3183 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/sample_applications/titanic.py
--rw-r--r--   0        0        0     1837 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/__init__.py
--rw-r--r--   0        0        0    17977 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/base.py
--rw-r--r--   0        0        0     5376 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/feature_select.py
--rw-r--r--   0        0        0     2726 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/impute.py
--rw-r--r--   0        0        0    18490 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/one_hot_encode.py
--rw-r--r--   0        0        0     2171 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/pad.py
--rw-r--r--   0        0        0     6565 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/sax.py
--rw-r--r--   0        0        0    16182 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/time_series_formatter.py
--rw-r--r--   0        0        0      469 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/type_cast.py
--rw-r--r--   0        0        0     2055 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/transformers/wrappers.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/__init__.py
--rw-r--r--   0        0        0     4137 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/base.py
--rw-r--r--   0        0        0      987 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/decision_tree.py
--rw-r--r--   0        0        0     2989 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/example_based.py
--rw-r--r--   0        0        0     5184 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/feature_based.py
--rw-r--r--   0        0        0     3084 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/feature_value_based.py
--rw-r--r--   0        0        0      646 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/types/explanations/time_series_saliency.py
--rw-r--r--   0        0        0        0 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/__init__.py
--rw-r--r--   0        0        0     7810 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/_plot_tree.py
--rw-r--r--   0        0        0     1968 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/dataloader.py
--rw-r--r--   0        0        0     1821 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/utils/model_utils.py
--rw-r--r--   0        0        0      520 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/__init__.py
--rw-r--r--   0        0        0    14256 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/feature_based_vis.py
--rw-r--r--   0        0        0     2576 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/time_series_vis.py
--rw-r--r--   0        0        0     2687 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/tree_vis.py
--rw-r--r--   0        0        0      870 2023-07-05 17:31:15.932947 pyreal-0.4.3/pyreal/visualize/visualize_config.py
--rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 pyreal-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-07-24 22:18:51.998880 pyreal-0.4.4/AUTHORS.rst
+-rw-r--r--   0        0        0        9 2023-07-24 22:18:51.998880 pyreal-0.4.4/HISTORY.md
+-rw-r--r--   0        0        0     1075 2023-07-24 22:18:51.998880 pyreal-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4528 2023-07-24 22:18:51.998880 pyreal-0.4.4/README.md
+-rw-r--r--   0        0        0     1787 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      240 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/__init__.py
+-rw-r--r--   0        0        0     3042 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/explainer_challenge.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/gfi/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/gfi/global_feature_importance_challenge.py
+-rw-r--r--   0        0        0      430 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/gfi/shap_feature_importance_challenge.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/lfc/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/lfc/local_feature_contribution_challenge.py
+-rw-r--r--   0        0        0      436 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/challenges/lfc/shap_feature_contribution_challenge.py
+-rw-r--r--   0        0        0     1623 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/dataset.py
+-rw-r--r--   0        0        0      610 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/download_datasets_script.py
+-rw-r--r--   0        0        0     5213 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/main.py
+-rw-r--r--   0        0        0    15073 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl
+-rw-r--r--   0        0        0     1652 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/adult_logistic_regression.pkl
+-rw-r--r--   0        0        0     3108 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl
+-rw-r--r--   0        0        0     1244 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl
+-rw-r--r--   0        0        0      941 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/balance-scale_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl
+-rw-r--r--   0        0        0      892 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl
+-rw-r--r--   0        0        0      881 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/breast-w_logistic_regression.pkl
+-rw-r--r--   0        0        0     1116 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/cmc_logistic_regression.pkl
+-rw-r--r--   0        0        0    62681 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/cnae-9_logistic_regression.pkl
+-rw-r--r--   0        0        0     1180 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/credit-approval_logistic_regression.pkl
+-rw-r--r--   0        0        0     1300 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/credit-g_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/diabetes_logistic_regression.pkl
+-rw-r--r--   0        0        0      873 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/electricity_logistic_regression.pkl
+-rw-r--r--   0        0        0     4528 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl
+-rw-r--r--   0        0        0     3423 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl
+-rw-r--r--   0        0        0      948 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models/ilpd_logistic_regression.pkl
+-rw-r--r--   0        0        0   129793 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/isolet_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/jm1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/kc1_logistic_regression.pkl
+-rw-r--r--   0        0        0      977 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/kc2_logistic_regression.pkl
+-rw-r--r--   0        0        0     1396 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl
+-rw-r--r--   0        0        0     4636 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/letter_logistic_regression.pkl
+-rw-r--r--   0        0        0     4865 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/madelon_logistic_regression.pkl
+-rw-r--r--   0        0        0    18351 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl
+-rw-r--r--   0        0        0     7151 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl
+-rw-r--r--   0        0        0     1551 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl
+-rw-r--r--   0        0        0     4831 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl
+-rw-r--r--   0        0        0    63793 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/mnist_784_logistic_regression.pkl
+-rw-r--r--   0        0        0     1807 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/nomao_logistic_regression.pkl
+-rw-r--r--   0        0        0     6191 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/optdigits_logistic_regression.pkl
+-rw-r--r--   0        0        0     1439 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl
+-rw-r--r--   0        0        0     1028 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/pc1_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/pc3_logistic_regression.pkl
+-rw-r--r--   0        0        0     1159 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/pc4_logistic_regression.pkl
+-rw-r--r--   0        0        0     2351 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/pendigits_logistic_regression.pkl
+-rw-r--r--   0        0        0      900 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/phoneme_logistic_regression.pkl
+-rw-r--r--   0        0        0     1191 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl
+-rw-r--r--   0        0        0     2703 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/satimage_logistic_regression.pkl
+-rw-r--r--   0        0        0    21553 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/semeion_logistic_regression.pkl
+-rw-r--r--   0        0        0     1228 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/sick_logistic_regression.pkl
+-rw-r--r--   0        0        0     1319 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/spambase_logistic_regression.pkl
+-rw-r--r--   0        0        0     7738 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/splice_logistic_regression.pkl
+-rw-r--r--   0        0        0     1025 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl
+-rw-r--r--   0        0        0     1444 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/vehicle_logistic_regression.pkl
+-rw-r--r--   0        0        0     3384 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/vowel_logistic_regression.pkl
+-rw-r--r--   0        0        0     1695 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl
+-rw-r--r--   0        0        0     1100 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/models/wdbc_logistic_regression.pkl
+-rw-r--r--   0        0        0      145 2023-07-24 22:18:52.002879 pyreal-0.4.4/pyreal/benchmark/models.py
+-rw-r--r--   0        0        0    10056 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10104 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge
+-rw-r--r--   0        0        0    10111 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge
+-rw-r--r--   0        0        0    10072 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10069 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge
+-rw-r--r--   0        0        0    10073 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge
+-rw-r--r--   0        0        0     1186 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/benchmark/task.py
+-rw-r--r--   0        0        0     2315 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/__init__.py
+-rw-r--r--   0        0        0    20704 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/dte/__init__.py
+-rw-r--r--   0        0        0     3338 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/dte/base.py
+-rw-r--r--   0        0        0     3019 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/dte/decision_tree_explainer.py
+-rw-r--r--   0        0        0     3448 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/dte/surrogate_decision_tree.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/example/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/example/base.py
+-rw-r--r--   0        0        0     2819 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/example/similar_examples.py
+-rw-r--r--   0        0        0     4883 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/generic_explainer.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/gfi/__init__.py
+-rw-r--r--   0        0        0     4301 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/gfi/base.py
+-rw-r--r--   0        0        0     2984 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/gfi/global_feature_importance.py
+-rw-r--r--   0        0        0     2237 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/gfi/permutation_feature_importance.py
+-rw-r--r--   0        0        0     3729 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/gfi/shap_feature_importance.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/lfc/__init__.py
+-rw-r--r--   0        0        0     4990 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/lfc/base.py
+-rw-r--r--   0        0        0     3135 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/lfc/local_feature_contribution.py
+-rw-r--r--   0        0        0     4425 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/lfc/shap_feature_contribution.py
+-rw-r--r--   0        0        0     3354 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/lfc/simple_counterfactual_contribution.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/pdp/__init__.py
+-rw-r--r--   0        0        0     3625 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/pdp/base.py
+-rw-r--r--   0        0        0     2965 2023-07-24 22:18:52.006879 pyreal-0.4.4/pyreal/explainers/pdp/partial_dependence.py
+-rw-r--r--   0        0        0     1987 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/explainers/pdp/partial_dependence_explainer.py
+-rw-r--r--   0        0        0      372 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/explainers/time_series/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/explainers/time_series/saliency/__init__.py
+-rw-r--r--   0        0        0     4689 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/explainers/time_series/saliency/base.py
+-rw-r--r--   0        0        0     5623 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py
+-rw-r--r--   0        0        0     5916 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/realapp/__init__.py
+-rw-r--r--   0        0        0    26048 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/realapp/realapp.py
+-rw-r--r--   0        0        0       71 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/__init__.py
+-rw-r--r--   0        0        0     8334 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/ames_housing.py
+-rw-r--r--   0        0        0      598 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/base.py
+-rw-r--r--   0        0        0     1769 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/california_housing.py
+-rw-r--r--   0        0        0   460673 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/data_ames_housing/data.csv
+-rw-r--r--   0        0        0    13637 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/data_ames_housing/data_description.txt
+-rw-r--r--   0        0        0     3431 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv
+-rw-r--r--   0        0        0    14681 2023-07-24 22:18:52.010880 pyreal-0.4.4/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv
+-rw-r--r--   0        0        0  1217129 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/sample_applications/data_cal_housing/california.csv
+-rw-r--r--   0        0        0    68558 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/sample_applications/data_student/data.csv
+-rw-r--r--   0        0        0     1514 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/sample_applications/data_student/students.csv
+-rw-r--r--   0        0        0    60300 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/sample_applications/data_titanic/data.csv
+-rw-r--r--   0        0        0     4264 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/sample_applications/student_performance.py
+-rw-r--r--   0        0        0     3331 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/sample_applications/titanic.py
+-rw-r--r--   0        0        0     1837 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/__init__.py
+-rw-r--r--   0        0        0    17977 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/base.py
+-rw-r--r--   0        0        0     5376 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/feature_select.py
+-rw-r--r--   0        0        0     2726 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/impute.py
+-rw-r--r--   0        0        0    18490 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/one_hot_encode.py
+-rw-r--r--   0        0        0     2171 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/pad.py
+-rw-r--r--   0        0        0     6565 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/sax.py
+-rw-r--r--   0        0        0    16182 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/time_series_formatter.py
+-rw-r--r--   0        0        0      469 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/type_cast.py
+-rw-r--r--   0        0        0     2055 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/transformers/wrappers.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/types/explanations/__init__.py
+-rw-r--r--   0        0        0     4137 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/types/explanations/base.py
+-rw-r--r--   0        0        0      987 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/types/explanations/decision_tree.py
+-rw-r--r--   0        0        0     2989 2023-07-24 22:18:52.018880 pyreal-0.4.4/pyreal/types/explanations/example_based.py
+-rw-r--r--   0        0        0     5184 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/types/explanations/feature_based.py
+-rw-r--r--   0        0        0     3084 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/types/explanations/feature_value_based.py
+-rw-r--r--   0        0        0      646 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/types/explanations/time_series_saliency.py
+-rw-r--r--   0        0        0        0 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/utils/__init__.py
+-rw-r--r--   0        0        0     7810 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/utils/_plot_tree.py
+-rw-r--r--   0        0        0     1968 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/utils/dataloader.py
+-rw-r--r--   0        0        0     1821 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/utils/model_utils.py
+-rw-r--r--   0        0        0      627 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/visualize/__init__.py
+-rw-r--r--   0        0        0    14325 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/visualize/feature_based_vis.py
+-rw-r--r--   0        0        0     2301 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/visualize/partial_dependence_vis.py
+-rw-r--r--   0        0        0     2576 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/visualize/time_series_vis.py
+-rw-r--r--   0        0        0     2687 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/visualize/tree_vis.py
+-rw-r--r--   0        0        0      870 2023-07-24 22:18:52.022879 pyreal-0.4.4/pyreal/visualize/visualize_config.py
+-rw-r--r--   0        0        0     5641 1970-01-01 00:00:00.000000 pyreal-0.4.4/PKG-INFO
```

### Comparing `pyreal-0.4.3/LICENSE` & `pyreal-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/README.md` & `pyreal-0.4.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt=“DAI-Lab” />
 <i>An open source project from Data to AI Lab at MIT.</i>
 </p>
 
 <!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
+
 [![PyPI Shield](https://img.shields.io/pypi/v/pyreal.svg)](https://pypi.python.org/pypi/pyreal)
+
 <!--[![Downloads](https://pepy.tech/badge/pyreal)](https://pepy.tech/project/pyreal)-->
 <!--[![Travis CI Shield](https://travis-ci.org/DAI-Lab/pyreal.svg?branch=stable)](https://travis-ci.org/DAI-Lab/pyreal)-->
 <!--[![Coverage Status](https://codecov.io/gh/DAI-Lab/pyreal/branch/stable/graph/badge.svg)](https://codecov.io/gh/DAI-Lab/pyreal)-->
+
 [![Build Action Status](https://github.com/DAI-Lab/pyreal/workflows/Test%20CI/badge.svg)](https://github.com/DAI-Lab/pyreal/actions)
+
 # Pyreal
 
 Library for generating useful and usable machine learning explanations.
 
-- License: MIT
-- Documentation: https://pyreal.gitbook.io/pyreal
-- API Documentation: https://sibyl-ml.dev/pyreal/api_reference/index.html
-- Homepage: https://sibyl-ml.dev/
+-   License: MIT
+-   Documentation: https://pyreal.gitbook.io/pyreal
+-   API Documentation: https://sibyl-ml.dev/pyreal/api_reference/index.html
+-   Homepage: https://sibyl-ml.dev/
 
 # Overview
 
 **Pyreal** wraps the complete machine learning explainability pipeline into RealApp objects, which seamlessly
 provide usable explanations in a low-code manner.
 
 # Install
@@ -38,14 +42,15 @@
 ```
 pip install pyreal
 ```
 
 This will pull and install the latest stable release from [PyPI](https://pypi.org/project/pyreal/).
 
 ## Install from source
+
 If you do not have **poetry** installed, please head to [poetry installation guide](https://python-poetry.org/docs/#installation)
 and install poetry according to the instructions.\
 Run the following command to make sure poetry is activated. You may need to close and reopen the terminal.
 
 ```
 poetry --version
 ```
@@ -69,47 +74,61 @@
 
 # Quickstart
 
 In this short tutorial we will guide you through a series of steps that will help you
 getting started with **Pyreal**. We will get an explanation for a prediction on whether a
 passenger on the Titanic would have survived.
 
- For a more detailed version of this tutorial, see [our documentation](https://dtail.gitbook.io/pyreal/getting-started/quickstart).
+For a more detailed version of this tutorial, see [our documentation](https://dtail.gitbook.io/pyreal/getting-started/quickstart).
 
 #### Load in the demo data and application
+
 ```
 >>> import pyreal.sample_applications.titanic as titanic
 
 >>> real_app = titanic.load_app()
 >>> sample_data = titanic.load_data(n_rows=300)
 
 ```
+
 #### Predict and produce explanation
+
 ```
 >>> predictions = real_app.predict(sample_data)
 
 >>> explanation = real_app.produce_feature_contributions(sample_data)
 
 ```
+
 #### Visualize explanation for one passenger
+
 ```
 passenger_id = 1
 plot_top_contributors(explanation[passenger_id], prediction=predictions[passenger_id], show=False)
 
 ```
 
 The output will be a bar plot showing the most contributing features, by absolute value.
 
 ![Quickstart](docs/images/titanic.png)
 
 We can see here that the input passenger's predicted chance of survival was greatly reduced
 because of their sex (male) and ticket class (3rd class).
 
+### Troubleshoot
+
+For macOS users, an error regarding `lightgbm` might arise when running the `titanic` tutorial due to lack of lightgbm installation.
+If this occurs, please run the following line in your terminal to install `lightgbm`.
+
+```
+brew install lightgbm
+```
+
 ### Terminology
+
 Pyreal introduces specific terms and naming schemes to refer to different feature spaces and
 transformations. The [Terminology User Guide](https://dtail.gitbook.io/pyreal/developing-applications/developer-terminology-guide) provides an introduction to these terms.
 
 # What's next?
 
 For more details about **Pyreal** and all its possibilities
-and features, please check the [documentation site](
-https://dtail.gitbook.io/pyreal/).
+and features, please check the [documentation site](https://dtail.gitbook.io/pyreal/).
```

### Comparing `pyreal-0.4.3/pyproject.toml` & `pyreal-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 maintainers = [
   "MIT Data To AI Lab <dailabmit@gmail.com>",
 ]
 
 description = "Library for evaluating and deploying human readable machine learning explanations."
 name = "pyreal"
-version = "0.4.3"
+version = "0.4.4"
 
 license = ""
 
 readme = "README.md"
 
 documentation = "https://sibyl-dev.github.io/pyreal"
 homepage = "https://sibyl-ml.dev/"
```

### Comparing `pyreal-0.4.3/pyreal/benchmark/challenges/explainer_challenge.py` & `pyreal-0.4.4/pyreal/benchmark/challenges/explainer_challenge.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/dataset.py` & `pyreal-0.4.4/pyreal/benchmark/dataset.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/download_datasets_script.py` & `pyreal-0.4.4/pyreal/benchmark/download_datasets_script.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/main.py` & `pyreal-0.4.4/pyreal/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/Bioresponse_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/PhishingWebsites_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/adult_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/adult_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/analcatdata_authorship_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/analcatdata_dmft_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/balance-scale_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/balance-scale_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/banknote-authentication_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/blood-transfusion-service-center_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/breast-w_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/breast-w_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/cmc_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/cmc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/cnae-9_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/cnae-9_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/credit-approval_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/credit-approval_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/credit-g_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/credit-g_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/diabetes_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/diabetes_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/electricity_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/electricity_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/eucalyptus_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/first-order-theorem-proving_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/ilpd_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/ilpd_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/isolet_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/isolet_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/jm1_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/jm1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/kc1_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/kc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/kc2_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/kc2_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/kr-vs-kp_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/letter_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/letter_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/madelon_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/madelon_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/mfeat-factors_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/mfeat-fourier_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/mfeat-karhunen_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/mfeat-morphological_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/mfeat-zernike_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/mnist_784_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/mnist_784_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/nomao_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/nomao_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/optdigits_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/optdigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/ozone-level-8hr_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/pc1_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/pc1_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/pc3_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/pc3_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/pc4_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/pc4_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/pendigits_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/pendigits_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/phoneme_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/phoneme_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/qsar-biodeg_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/satimage_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/satimage_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/semeion_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/semeion_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/sick_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/sick_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/spambase_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/spambase_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/splice_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/splice_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/tic-tac-toe_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/vehicle_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/vehicle_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/vowel_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/vowel_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/wall-robot-navigation_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/models/wdbc_logistic_regression.pkl` & `pyreal-0.4.4/pyreal/benchmark/models/wdbc_logistic_regression.pkl`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge` & `pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge` & `pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/LocalFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge` & `pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/ShapFeatureContributionChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge` & `pyreal-0.4.4/pyreal/benchmark/results/20210916-115944/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge` & `pyreal-0.4.4/pyreal/benchmark/results/20210924-133808/GlobalFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge` & `pyreal-0.4.4/pyreal/benchmark/results/20210924-133808/ShapFeatureImportanceChallenge`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/benchmark/task.py` & `pyreal-0.4.4/pyreal/benchmark/task.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/__init__.py` & `pyreal-0.4.4/pyreal/explainers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/base.py` & `pyreal-0.4.4/pyreal/explainers/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/dte/base.py` & `pyreal-0.4.4/pyreal/explainers/dte/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/dte/decision_tree_explainer.py` & `pyreal-0.4.4/pyreal/explainers/dte/decision_tree_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/dte/surrogate_decision_tree.py` & `pyreal-0.4.4/pyreal/explainers/dte/surrogate_decision_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/example/base.py` & `pyreal-0.4.4/pyreal/explainers/example/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/example/similar_examples.py` & `pyreal-0.4.4/pyreal/explainers/example/similar_examples.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/generic_explainer.py` & `pyreal-0.4.4/pyreal/explainers/generic_explainer.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/gfi/base.py` & `pyreal-0.4.4/pyreal/explainers/gfi/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/gfi/global_feature_importance.py` & `pyreal-0.4.4/pyreal/explainers/gfi/global_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/gfi/permutation_feature_importance.py` & `pyreal-0.4.4/pyreal/explainers/gfi/permutation_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/gfi/shap_feature_importance.py` & `pyreal-0.4.4/pyreal/explainers/gfi/shap_feature_importance.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/lfc/base.py` & `pyreal-0.4.4/pyreal/explainers/lfc/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/lfc/local_feature_contribution.py` & `pyreal-0.4.4/pyreal/explainers/lfc/local_feature_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/lfc/shap_feature_contribution.py` & `pyreal-0.4.4/pyreal/explainers/lfc/shap_feature_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/lfc/simple_counterfactual_contribution.py` & `pyreal-0.4.4/pyreal/explainers/lfc/simple_counterfactual_contribution.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/pdp/base.py` & `pyreal-0.4.4/pyreal/explainers/pdp/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence.py` & `pyreal-0.4.4/pyreal/explainers/pdp/partial_dependence.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         x_train_orig=None,
         grid_resolution=100,
         interpretable_features=True,
         **kwargs,
     ):
         self.features = features
         self.grid_resolution = grid_resolution
+        self.is_fitted = False
         super().__init__(model, x_train_orig, interpretable_features, **kwargs)
 
     def fit(self, x_train_orig=None, y_train=None):
         """
         Fit this explainer.
 
         Calculates the partial dependence values
@@ -62,15 +63,18 @@
             self.model,
             dataset,
             features=self.features,
             grid_resolution=self.grid_resolution,
         )
         self.pdp_values = explanation_results["average"]
         self.grid_points = explanation_results["values"]
+        self.is_fitted = True
         return self
 
     def get_pdp(self):
         """
         Produce the partial dependence explanation
 
         """
+        if not self.is_fitted:
+            raise RuntimeError("Must fit explainer before calling produce!")
         return PartialDependenceExplanation(self.features, self.pdp_values, self.grid_points)
```

### Comparing `pyreal-0.4.3/pyreal/explainers/pdp/partial_dependence_explainer.py` & `pyreal-0.4.4/pyreal/explainers/pdp/partial_dependence_explainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,19 @@
             If True, return explanations using the interpretable feature descriptions instead of
             default names
         **kwargs: see base Explainer args
     """
 
     def __init__(self, model, features, x_train_orig=None, grid_resolution=100, **kwargs):
         self.base_partial_dependence = PartialDependence(
-            model, features=features, x_train_orig=x_train_orig, grid_resolution=grid_resolution
+            model,
+            features=features,
+            x_train_orig=x_train_orig,
+            grid_resolution=grid_resolution,
+            **kwargs
         )
         super(PartialDependenceExplainer, self).__init__(model, x_train_orig, **kwargs)
 
     def get_pdp(self):
         """
         Gets the raw explanation
```

### Comparing `pyreal-0.4.3/pyreal/explainers/time_series/saliency/base.py` & `pyreal-0.4.4/pyreal/explainers/time_series/saliency/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py` & `pyreal-0.4.4/pyreal/explainers/time_series/saliency/univariate_lime_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py` & `pyreal-0.4.4/pyreal/explainers/time_series/saliency/univariate_occlusion_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/realapp/realapp.py` & `pyreal-0.4.4/pyreal/realapp/realapp.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/ames_housing.py` & `pyreal-0.4.4/pyreal/sample_applications/ames_housing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import pickle
 
 import pandas as pd
 from sklearn.linear_model import Ridge
 
 from pyreal import RealApp
 from pyreal.transformers import OneHotEncoder, Transformer, fit_transformers, run_transformers
 
@@ -120,50 +119,36 @@
     elif include_targets:
         return x_orig, y
     else:
         return x_orig
 
 
 def load_model():
-    if os.path.exists(MODEL_FILE):
-        return pickle.load(open(os.path.join(DATA_DIR, "model.pkl"), "rb"))
-    else:
-        transformers = load_transformers()
-        x_orig, y = load_data(include_targets=True)
-        x_orig = x_orig.drop("Id", axis="columns")
-        x_model = run_transformers(transformers, x_orig)
-        model = Ridge()
-        model.fit(x_model, y)
-
-        if not os.path.isdir(DATA_DIR):
-            os.mkdir(DATA_DIR)
-        with open(MODEL_FILE, "wb") as f:
-            pickle.dump(model, f)
-        return model
+    transformers = load_transformers()
+    x_orig, y = load_data(include_targets=True)
+    x_orig = x_orig.drop("Id", axis="columns")
+    x_model = run_transformers(transformers, x_orig)
+    model = Ridge()
+    model.fit(x_model, y)
+
+    return model
 
 
 def load_transformers():
-    if os.path.exists(TRANSFORMER_FILE):
-        return pickle.load(open(os.path.join(DATA_DIR, "transformers.pkl"), "rb"))
-    else:
-        x_orig, y = load_data(include_targets=True)
-        x_orig = x_orig.drop("Id", axis="columns")
-        ames_imputer = AmesHousingImputer()
-        x_imputed = fit_transformers(ames_imputer, x_orig)
-        object_columns = x_imputed.select_dtypes(include=["object"]).columns
-        onehotencoder = OneHotEncoder(object_columns)
-        fit_transformers(onehotencoder, x_imputed)
-
-        transformers = [ames_imputer, onehotencoder]
-
-        if not os.path.isdir(DATA_DIR):
-            os.mkdir(DATA_DIR)
-        with open(TRANSFORMER_FILE, "wb") as f:
-            pickle.dump(transformers, f)
-        return transformers
+    x_orig = load_data()
+    x_orig = x_orig.drop("Id", axis="columns")
+    ames_imputer = AmesHousingImputer()
+    x_imputed = fit_transformers(ames_imputer, x_orig)
+    object_columns = x_imputed.select_dtypes(include=["object"]).columns
+    onehotencoder = OneHotEncoder(object_columns)
+    fit_transformers(onehotencoder, x_imputed)
+
+    transformers = [ames_imputer, onehotencoder]
+
+    return transformers
 
 
 def load_app():
     x_train_orig, y = load_data(include_targets=True)
     model = load_model()
     transformers = load_transformers()
     feature_descriptions = load_feature_descriptions()
```

### Comparing `pyreal-0.4.3/pyreal/sample_applications/california_housing.py` & `pyreal-0.4.4/pyreal/sample_applications/california_housing.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_ames_housing/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/data_description.txt` & `pyreal-0.4.4/pyreal/sample_applications/data_ames_housing/data_description.txt`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_ames_housing/feature_descriptions.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_cal_housing/cal_cities_lat_long.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_cal_housing/california.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_cal_housing/california.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_student/data.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_student/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_student/students.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_student/students.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/data_titanic/data.csv` & `pyreal-0.4.4/pyreal/sample_applications/data_titanic/data.csv`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/sample_applications/student_performance.py` & `pyreal-0.4.4/pyreal/sample_applications/student_performance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import pickle
 
 import pandas as pd
 from lightgbm import LGBMClassifier
 from sklearn.preprocessing import StandardScaler
 
 from pyreal import RealApp
 from pyreal.transformers import (
@@ -88,28 +87,21 @@
 
 def load_students():
     x, _ = load_data(filename=STUDENTS_FILE)
     return x
 
 
 def load_model():
-    if os.path.exists(MODEL_FILE):
-        return pickle.load(open(os.path.join(DATA_DIR, "model.pkl"), "rb"))
-    else:
-        transformers = load_transformers()
-        x_orig, y = load_data()
-        x_model = run_transformers(transformers, x_orig)
-        model = LGBMClassifier()
-        model.fit(x_model, y)
-
-        if not os.path.isdir(DATA_DIR):
-            os.mkdir(DATA_DIR)
-        with open(MODEL_FILE, "wb") as f:
-            pickle.dump(model, f)
-        return model
+    transformers = load_transformers()
+    x_orig, y = load_data()
+    x_model = run_transformers(transformers, x_orig)
+    model = LGBMClassifier()
+    model.fit(x_model, y)
+
+    return model
 
 
 def load_transformers(x=None):
     if x is None:
         x, _ = load_data()
     onehotencoder = OneHotEncoder(
         ["school", "sex", "address", "Pstatus", "reason", "guardian", "Mjob", "Fjob"], model=True
```

### Comparing `pyreal-0.4.3/pyreal/sample_applications/titanic.py` & `pyreal-0.4.4/pyreal/sample_applications/titanic.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,47 +53,49 @@
         "Ticket": "Ticket Number",
         "Fare": "Passenger Fare",
         "Cabin": "Cabin Number",
         "Embarked": "Port of Embarkment",
     }
 
 
-def load_model():
-    if os.path.exists(MODEL_FILE):
+def load_model(save=False, use_saved=False):
+    if use_saved and os.path.exists(MODEL_FILE):
         return pickle.load(open(os.path.join(DATA_DIR, "model.pkl"), "rb"))
     else:
         transformers = load_transformers()
         x_orig, y = load_data(include_targets=True)
         x_model = run_transformers(transformers, x_orig)
         model = LGBMClassifier()
         model.fit(x_model, y)
 
-        if not os.path.isdir(DATA_DIR):
-            os.mkdir(DATA_DIR)
-        with open(MODEL_FILE, "wb") as f:
-            pickle.dump(model, f)
+        if save:
+            if not os.path.isdir(DATA_DIR):
+                os.mkdir(DATA_DIR)
+            with open(MODEL_FILE, "wb") as f:
+                pickle.dump(model, f)
         return model
 
 
-def load_transformers():
-    if os.path.exists(TRANSFORMER_FILE):
+def load_transformers(save=False, use_saved=False):
+    if use_saved and os.path.exists(TRANSFORMER_FILE):
         return pickle.load(open(os.path.join(DATA_DIR, "transformers.pkl"), "rb"))
     else:
         x_orig, y = load_data(include_targets=True)
         column_drop = ColumnDropTransformer(["PassengerId", "Name", "Ticket", "Cabin"])
         imputer = MultiTypeImputer()
         one_hot_encoder = OneHotEncoder(["Sex", "Embarked"])
 
         transformers = [column_drop, imputer, one_hot_encoder]
         fit_transformers(transformers, x_orig)
 
-        if not os.path.isdir(DATA_DIR):
-            os.mkdir(DATA_DIR)
-        with open(TRANSFORMER_FILE, "wb") as f:
-            pickle.dump(transformers, f)
+        if save:
+            if not os.path.isdir(DATA_DIR):
+                os.mkdir(DATA_DIR)
+            with open(TRANSFORMER_FILE, "wb") as f:
+                pickle.dump(transformers, f)
         return transformers
 
 
 def load_app():
     x_train_orig, y = load_data(include_targets=True)
     model = load_model()
     transformers = load_transformers()
```

### Comparing `pyreal-0.4.3/pyreal/transformers/__init__.py` & `pyreal-0.4.4/pyreal/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/base.py` & `pyreal-0.4.4/pyreal/transformers/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/feature_select.py` & `pyreal-0.4.4/pyreal/transformers/feature_select.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/impute.py` & `pyreal-0.4.4/pyreal/transformers/impute.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/one_hot_encode.py` & `pyreal-0.4.4/pyreal/transformers/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/pad.py` & `pyreal-0.4.4/pyreal/transformers/pad.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/sax.py` & `pyreal-0.4.4/pyreal/transformers/sax.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/time_series_formatter.py` & `pyreal-0.4.4/pyreal/transformers/time_series_formatter.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/transformers/wrappers.py` & `pyreal-0.4.4/pyreal/transformers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/types/explanations/base.py` & `pyreal-0.4.4/pyreal/types/explanations/base.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/types/explanations/decision_tree.py` & `pyreal-0.4.4/pyreal/types/explanations/decision_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/types/explanations/example_based.py` & `pyreal-0.4.4/pyreal/types/explanations/example_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/types/explanations/feature_based.py` & `pyreal-0.4.4/pyreal/types/explanations/feature_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/types/explanations/feature_value_based.py` & `pyreal-0.4.4/pyreal/types/explanations/feature_value_based.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/types/explanations/time_series_saliency.py` & `pyreal-0.4.4/pyreal/types/explanations/time_series_saliency.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/utils/_plot_tree.py` & `pyreal-0.4.4/pyreal/utils/_plot_tree.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/utils/dataloader.py` & `pyreal-0.4.4/pyreal/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/utils/model_utils.py` & `pyreal-0.4.4/pyreal/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/visualize/feature_based_vis.py` & `pyreal-0.4.4/pyreal/visualize/feature_based_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,14 +391,16 @@
         )
 
     plt.axhline(0, color="black", zorder=0)
     plt.xlabel("Values for %s" % feature)
     if legend_type == "continuous":
         norm = plt.Normalize(0, 1)
         sm = plt.cm.ScalarMappable(cmap=PALETTE_CMAP, norm=norm)
+        if discrete:
+            plt.xticks(rotation=45, ha="right")
         min_val = predictions.min()
         max_val = predictions.max()
         sm.set_array([])
         cbar = ax.figure.colorbar(sm)
         cbar.ax.get_yaxis().set_ticks([])
         cbar.ax.text(1.5, 0.05, ("%.2f" % min_val).rstrip("0").rstrip("."), ha="left", va="center")
         cbar.ax.text(1.5, 0.95, ("%.2f" % max_val).rstrip("0").rstrip("."), ha="left", va="center")
```

### Comparing `pyreal-0.4.3/pyreal/visualize/time_series_vis.py` & `pyreal-0.4.4/pyreal/visualize/time_series_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/visualize/tree_vis.py` & `pyreal-0.4.4/pyreal/visualize/tree_vis.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/pyreal/visualize/visualize_config.py` & `pyreal-0.4.4/pyreal/visualize/visualize_config.py`

 * *Files identical despite different names*

### Comparing `pyreal-0.4.3/PKG-INFO` & `pyreal-0.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreal
-Version: 0.4.3
+Version: 0.4.4
 Summary: Library for evaluating and deploying human readable machine learning explanations.
 Home-page: https://sibyl-ml.dev/
 Keywords: pyreal,Pyreal
 Author: Alexandra Zytek
 Author-email: zyteka@mit.edu
 Maintainer: MIT Data To AI Lab
 Maintainer-email: dailabmit@gmail.com
@@ -29,27 +29,31 @@
 
 <p align="left">
 <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt=“DAI-Lab” />
 <i>An open source project from Data to AI Lab at MIT.</i>
 </p>
 
 <!-- Uncomment these lines after releasing the package to PyPI for version and downloads badges -->
+
 [![PyPI Shield](https://img.shields.io/pypi/v/pyreal.svg)](https://pypi.python.org/pypi/pyreal)
+
 <!--[![Downloads](https://pepy.tech/badge/pyreal)](https://pepy.tech/project/pyreal)-->
 <!--[![Travis CI Shield](https://travis-ci.org/DAI-Lab/pyreal.svg?branch=stable)](https://travis-ci.org/DAI-Lab/pyreal)-->
 <!--[![Coverage Status](https://codecov.io/gh/DAI-Lab/pyreal/branch/stable/graph/badge.svg)](https://codecov.io/gh/DAI-Lab/pyreal)-->
+
 [![Build Action Status](https://github.com/DAI-Lab/pyreal/workflows/Test%20CI/badge.svg)](https://github.com/DAI-Lab/pyreal/actions)
+
 # Pyreal
 
 Library for generating useful and usable machine learning explanations.
 
-- License: MIT
-- Documentation: https://pyreal.gitbook.io/pyreal
-- API Documentation: https://sibyl-ml.dev/pyreal/api_reference/index.html
-- Homepage: https://sibyl-ml.dev/
+-   License: MIT
+-   Documentation: https://pyreal.gitbook.io/pyreal
+-   API Documentation: https://sibyl-ml.dev/pyreal/api_reference/index.html
+-   Homepage: https://sibyl-ml.dev/
 
 # Overview
 
 **Pyreal** wraps the complete machine learning explainability pipeline into RealApp objects, which seamlessly
 provide usable explanations in a low-code manner.
 
 # Install
@@ -67,14 +71,15 @@
 ```
 pip install pyreal
 ```
 
 This will pull and install the latest stable release from [PyPI](https://pypi.org/project/pyreal/).
 
 ## Install from source
+
 If you do not have **poetry** installed, please head to [poetry installation guide](https://python-poetry.org/docs/#installation)
 and install poetry according to the instructions.\
 Run the following command to make sure poetry is activated. You may need to close and reopen the terminal.
 
 ```
 poetry --version
 ```
@@ -98,48 +103,62 @@
 
 # Quickstart
 
 In this short tutorial we will guide you through a series of steps that will help you
 getting started with **Pyreal**. We will get an explanation for a prediction on whether a
 passenger on the Titanic would have survived.
 
- For a more detailed version of this tutorial, see [our documentation](https://dtail.gitbook.io/pyreal/getting-started/quickstart).
+For a more detailed version of this tutorial, see [our documentation](https://dtail.gitbook.io/pyreal/getting-started/quickstart).
 
 #### Load in the demo data and application
+
 ```
 >>> import pyreal.sample_applications.titanic as titanic
 
 >>> real_app = titanic.load_app()
 >>> sample_data = titanic.load_data(n_rows=300)
 
 ```
+
 #### Predict and produce explanation
+
 ```
 >>> predictions = real_app.predict(sample_data)
 
 >>> explanation = real_app.produce_feature_contributions(sample_data)
 
 ```
+
 #### Visualize explanation for one passenger
+
 ```
 passenger_id = 1
 plot_top_contributors(explanation[passenger_id], prediction=predictions[passenger_id], show=False)
 
 ```
 
 The output will be a bar plot showing the most contributing features, by absolute value.
 
 ![Quickstart](docs/images/titanic.png)
 
 We can see here that the input passenger's predicted chance of survival was greatly reduced
 because of their sex (male) and ticket class (3rd class).
 
+### Troubleshoot
+
+For macOS users, an error regarding `lightgbm` might arise when running the `titanic` tutorial due to lack of lightgbm installation.
+If this occurs, please run the following line in your terminal to install `lightgbm`.
+
+```
+brew install lightgbm
+```
+
 ### Terminology
+
 Pyreal introduces specific terms and naming schemes to refer to different feature spaces and
 transformations. The [Terminology User Guide](https://dtail.gitbook.io/pyreal/developing-applications/developer-terminology-guide) provides an introduction to these terms.
 
 # What's next?
 
 For more details about **Pyreal** and all its possibilities
-and features, please check the [documentation site](
-https://dtail.gitbook.io/pyreal/).
+and features, please check the [documentation site](https://dtail.gitbook.io/pyreal/).
```

