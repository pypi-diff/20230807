# Comparing `tmp/aimodelshare-0.1.4.tar.gz` & `tmp/aimodelshare-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimodelshare-0.1.4.tar", last modified: Fri May  5 16:57:08 2023, max compression
+gzip compressed data, was "aimodelshare-0.1.5.tar", last modified: Mon Aug  7 09:03:59 2023, max compression
```

## Comparing `aimodelshare-0.1.4.tar` & `aimodelshare-0.1.5.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.028069 aimodelshare-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2501 2023-05-05 16:57:08.028069 aimodelshare-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.006068 aimodelshare-0.1.4/aimodelshare/
--rw-r--r--   0 root         (0) root         (0)     2014 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/README.md
--rw-r--r--   0 root         (0) root         (0)      539 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68708 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/aimsonnx.py
--rw-r--r--   0 root         (0) root         (0)    34889 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/api.py
--rw-r--r--   0 root         (0) root         (0)    15188 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/aws.py
--rw-r--r--   0 root         (0) root         (0)     6784 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/aws_client.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/base_image.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/bucketpolicy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.007068 aimodelshare-0.1.4/aimodelshare/color_mappings/
--rw-r--r--   0 root         (0) root         (0)     2728 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/color_mappings/color_mapping_keras.csv
--rw-r--r--   0 root         (0) root         (0)     1960 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/color_mappings/color_mapping_pytorch.csv
--rw-r--r--   0 root         (0) root         (0)     8758 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/containerisation.py
--rw-r--r--   0 root         (0) root         (0)    29609 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/containerization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.008068 aimodelshare-0.1.4/aimodelshare/containerization_templates/
--rw-r--r--   0 root         (0) root         (0)      181 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/containerization_templates/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)      687 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/containerization_templates/Dockerfile_PySpark.txt
--rw-r--r--   0 root         (0) root         (0)      532 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/containerization_templates/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/containerization_templates/lambda_function.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.008068 aimodelshare-0.1.4/aimodelshare/custom_approach/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/custom_approach/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/custom_approach/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/custom_eval_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.009068 aimodelshare-0.1.4/aimodelshare/data_sharing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.010068 aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)     3855 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)    22799 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/download_data.py
--rw-r--r--   0 root         (0) root         (0)    13964 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/share_data.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/data_sharing/utils.py
--rw-r--r--   0 root         (0) root         (0)    11045 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/deploy_custom_lambda.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.010068 aimodelshare-0.1.4/aimodelshare/documentation/
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.011068 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/_version.py
--rw-r--r--   0 root         (0) root         (0)     3099 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     6192 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      513 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:07.997067 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.013068 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css.map
--rw-r--r--   0 root         (0) root         (0)    43005 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)   133076 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map
--rw-r--r--   0 root         (0) root         (0)    35271 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css
--rw-r--r--   0 root         (0) root         (0)   161215 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.014068 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/
--rw-r--r--   0 root         (0) root         (0)     8468 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot
--rw-r--r--   0 root         (0) root         (0)     5922 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg
--rw-r--r--   0 root         (0) root         (0)     8300 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf
--rw-r--r--   0 root         (0) root         (0)     5168 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff
--rw-r--r--   0 root         (0) root         (0)     4344 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.014068 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     1948 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js
--rwxr-xr-x   0 root         (0) root         (0)      146 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/make.bat
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.015068 aimodelshare-0.1.4/aimodelshare/documentation/source/
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/about.rst
--rw-r--r--   0 root         (0) root         (0)     5598 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/advanced_features.rst
--rw-r--r--   0 root         (0) root         (0)     8528 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/competition.rst
--rw-r--r--   0 root         (0) root         (0)     2028 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/create_credentials.rst
--rw-r--r--   0 root         (0) root         (0)     8854 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/example_notebooks.rst
--rw-r--r--   0 root         (0) root         (0)     4727 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/functions.rst
--rw-r--r--   0 root         (0) root         (0)    14863 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/gettingstarted.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.017068 aimodelshare-0.1.4/aimodelshare/documentation/source/images/
--rw-r--r--   0 root         (0) root         (0)    15684 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds1.png
--rw-r--r--   0 root         (0) root         (0)    80398 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds2.png
--rw-r--r--   0 root         (0) root         (0)   201488 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds3.png
--rw-r--r--   0 root         (0) root         (0)   208089 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds4.png
--rw-r--r--   0 root         (0) root         (0)   123164 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds5.png
--rw-r--r--   0 root         (0) root         (0)    45191 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds_file_example.png
--rw-r--r--   0 root         (0) root         (0)    95857 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/images/predict_tab.png
--rw-r--r--   0 root         (0) root         (0)     2452 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/index.rst
--rw-r--r--   0 root         (0) root         (0)     6712 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/documentation/source/modelplayground.rst
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    59901 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/generatemodelapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.018069 aimodelshare-0.1.4/aimodelshare/iam/
--rw-r--r--   0 root         (0) root         (0)     3855 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/iam/codebuild_policy.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/iam/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/iam/lambda_policy.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/iam/lambda_trust_relationship.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.019069 aimodelshare-0.1.4/aimodelshare/json_templates/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/api_json.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.019069 aimodelshare-0.1.4/aimodelshare/json_templates/auth/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/auth/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/auth/role.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.020069 aimodelshare-0.1.4/aimodelshare/json_templates/eval/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/eval/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/eval/role.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.020069 aimodelshare-0.1.4/aimodelshare/json_templates/function/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/function/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/function/role.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/integration_response.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/lambda_policy_1.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/lambda_policy_2.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/lambda_role_1.txt
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/json_templates/lambda_role_2.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/leaderboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.023069 aimodelshare-0.1.4/aimodelshare/main/
--rw-r--r--   0 root         (0) root         (0)     4146 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/1.txt
--rw-r--r--   0 root         (0) root         (0)     3616 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/1B.txt
--rw-r--r--   0 root         (0) root         (0)     4609 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/2.txt
--rw-r--r--   0 root         (0) root         (0)     4110 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/3.txt
--rw-r--r--   0 root         (0) root         (0)     4260 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/4.txt
--rw-r--r--   0 root         (0) root         (0)     3522 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/5.txt
--rw-r--r--   0 root         (0) root         (0)     3518 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/6.txt
--rw-r--r--   0 root         (0) root         (0)     4377 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/7.txt
--rw-r--r--   0 root         (0) root         (0)     4513 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/8.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10942 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/authorization.txt
--rw-r--r--   0 root         (0) root         (0)     3081 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/eval_classification.txt
--rw-r--r--   0 root         (0) root         (0)    59775 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/eval_lambda.txt
--rw-r--r--   0 root         (0) root         (0)     3111 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/eval_regression.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/lambda_function.txt
--rw-r--r--   0 root         (0) root         (0)     4941 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/main/nst.txt
--rw-r--r--   0 root         (0) root         (0)    49899 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/model.py
--rw-r--r--   0 root         (0) root         (0)     4311 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/modeluser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.023069 aimodelshare-0.1.4/aimodelshare/placeholders/
--rw-r--r--   0 root         (0) root         (0)     3464 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/placeholders/model.onnx
--rw-r--r--   0 root         (0) root         (0)     2930 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/placeholders/preprocessor.zip
--rw-r--r--   0 root         (0) root         (0)    88269 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/playground.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/postprocessormodules.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/preprocessormodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.026069 aimodelshare-0.1.4/aimodelshare/pyspark/
--rw-r--r--   0 root         (0) root         (0)     6529 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/1.txt
--rw-r--r--   0 root         (0) root         (0)     6078 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/1B.txt
--rw-r--r--   0 root         (0) root         (0)     7055 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/2.txt
--rw-r--r--   0 root         (0) root         (0)     6596 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/3.txt
--rw-r--r--   0 root         (0) root         (0)     6377 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/4.txt
--rw-r--r--   0 root         (0) root         (0)     5988 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/5.txt
--rw-r--r--   0 root         (0) root         (0)     5980 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/6.txt
--rw-r--r--   0 root         (0) root         (0)     6819 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/7.txt
--rw-r--r--   0 root         (0) root         (0)     6906 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/8.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10589 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/authorization.txt
--rw-r--r--   0 root         (0) root         (0)     3081 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/eval_classification.txt
--rw-r--r--   0 root         (0) root         (0)    51474 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/eval_lambda.txt
--rw-r--r--   0 root         (0) root         (0)     3111 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/eval_regression.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/lambda_function.txt
--rw-r--r--   0 root         (0) root         (0)     7110 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/pyspark/nst.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.026069 aimodelshare-0.1.4/aimodelshare/python/
--rw-r--r--   0 root         (0) root         (0)     1949 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/python/my_preprocessor.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/readme.md
--rw-r--r--   0 root         (0) root         (0)     5793 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/reproducibility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.028069 aimodelshare-0.1.4/aimodelshare/sam/
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/Dockerfile_PySpark.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      625 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)     3855 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/codebuild_policies.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)     5181 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/codepipeline_policies.txt
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/codepipeline_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/spark-class.txt
--rw-r--r--   0 root         (0) root         (0)     1195 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/sam/template.txt
--rw-r--r--   0 root         (0) root         (0)     3109 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/tools.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/aimodelshare/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.007068 aimodelshare-0.1.4/aimodelshare.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2501 2023-05-05 16:57:07.000000 aimodelshare-0.1.4/aimodelshare.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6377 2023-05-05 16:57:07.000000 aimodelshare-0.1.4/aimodelshare.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 16:57:07.000000 aimodelshare-0.1.4/aimodelshare.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-05 16:57:07.000000 aimodelshare-0.1.4/aimodelshare.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-05 16:57:07.000000 aimodelshare-0.1.4/aimodelshare.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 16:57:08.029069 aimodelshare-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1318 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 16:57:08.028069 aimodelshare-0.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/tests/test_aimsonnx.py
--rw-r--r--   0 root         (0) root         (0)    12210 2023-05-05 16:56:59.000000 aimodelshare-0.1.4/tests/test_playground.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.196730 aimodelshare-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       35 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-08-07 09:03:59.196730 aimodelshare-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.169728 aimodelshare-0.1.5/aimodelshare/
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/README.md
+-rw-r--r--   0 root         (0) root         (0)      539 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69338 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/aimsonnx.py
+-rw-r--r--   0 root         (0) root         (0)    34935 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/api.py
+-rw-r--r--   0 root         (0) root         (0)    15188 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6784 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/aws_client.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/base_image.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/bucketpolicy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.171728 aimodelshare-0.1.5/aimodelshare/color_mappings/
+-rw-r--r--   0 root         (0) root         (0)     2728 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/color_mappings/color_mapping_keras.csv
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/color_mappings/color_mapping_pytorch.csv
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/containerisation.py
+-rw-r--r--   0 root         (0) root         (0)    29609 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/containerization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.171728 aimodelshare-0.1.5/aimodelshare/containerization_templates/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/containerization_templates/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)      687 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/containerization_templates/Dockerfile_PySpark.txt
+-rw-r--r--   0 root         (0) root         (0)      532 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/containerization_templates/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/containerization_templates/lambda_function.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.172728 aimodelshare-0.1.5/aimodelshare/custom_approach/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/custom_approach/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/custom_approach/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/custom_eval_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.173728 aimodelshare-0.1.5/aimodelshare/data_sharing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.174728 aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)    22799 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/download_data.py
+-rw-r--r--   0 root         (0) root         (0)    13964 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/share_data.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/data_sharing/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11045 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/deploy_custom_lambda.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.174728 aimodelshare-0.1.5/aimodelshare/documentation/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.176729 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/
+-rw-r--r--   0 root         (0) root         (0)      797 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/layout.html
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/search.html
+-rw-r--r--   0 root         (0) root         (0)      513 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.159727 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.179729 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 root         (0) root         (0)       71 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css.map
+-rw-r--r--   0 root         (0) root         (0)    43005 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)   133076 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map
+-rw-r--r--   0 root         (0) root         (0)    35271 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css
+-rw-r--r--   0 root         (0) root         (0)   161215 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.180729 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg
+-rw-r--r--   0 root         (0) root         (0)     8300 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf
+-rw-r--r--   0 root         (0) root         (0)     5168 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.180729 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/js/
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js
+-rwxr-xr-x   0 root         (0) root         (0)      146 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/theme.conf
+-rw-r--r--   0 root         (0) root         (0)      804 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/make.bat
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.182729 aimodelshare-0.1.5/aimodelshare/documentation/source/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/about.rst
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/advanced_features.rst
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/competition.rst
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/create_credentials.rst
+-rw-r--r--   0 root         (0) root         (0)     8854 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/example_notebooks.rst
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/functions.rst
+-rw-r--r--   0 root         (0) root         (0)    14863 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/gettingstarted.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.184729 aimodelshare-0.1.5/aimodelshare/documentation/source/images/
+-rw-r--r--   0 root         (0) root         (0)    15684 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds1.png
+-rw-r--r--   0 root         (0) root         (0)    80398 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds2.png
+-rw-r--r--   0 root         (0) root         (0)   201488 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds3.png
+-rw-r--r--   0 root         (0) root         (0)   208089 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds4.png
+-rw-r--r--   0 root         (0) root         (0)   123164 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds5.png
+-rw-r--r--   0 root         (0) root         (0)    45191 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds_file_example.png
+-rw-r--r--   0 root         (0) root         (0)    95857 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/images/predict_tab.png
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/documentation/source/modelplayground.rst
+-rw-r--r--   0 root         (0) root         (0)      318 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    59901 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/generatemodelapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.185729 aimodelshare-0.1.5/aimodelshare/iam/
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/iam/codebuild_policy.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/iam/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/iam/lambda_policy.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/iam/lambda_trust_relationship.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.186729 aimodelshare-0.1.5/aimodelshare/json_templates/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/api_json.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.187729 aimodelshare-0.1.5/aimodelshare/json_templates/auth/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/auth/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/auth/role.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.187729 aimodelshare-0.1.5/aimodelshare/json_templates/eval/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/eval/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/eval/role.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.187729 aimodelshare-0.1.5/aimodelshare/json_templates/function/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/function/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/function/role.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/integration_response.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/lambda_policy_1.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/lambda_policy_2.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/lambda_role_1.txt
+-rw-r--r--   0 root         (0) root         (0)      350 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/json_templates/lambda_role_2.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/leaderboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.190730 aimodelshare-0.1.5/aimodelshare/main/
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/1.txt
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/1B.txt
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/2.txt
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/3.txt
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/4.txt
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/5.txt
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/6.txt
+-rw-r--r--   0 root         (0) root         (0)     4377 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/7.txt
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/8.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10942 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/authorization.txt
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/eval_classification.txt
+-rw-r--r--   0 root         (0) root         (0)    60314 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/eval_lambda.txt
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/eval_regression.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/lambda_function.txt
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/main/nst.txt
+-rw-r--r--   0 root         (0) root         (0)    49899 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/model.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/modeluser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.190730 aimodelshare-0.1.5/aimodelshare/placeholders/
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/placeholders/model.onnx
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/placeholders/preprocessor.zip
+-rw-r--r--   0 root         (0) root         (0)    88713 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/playground.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/postprocessormodules.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/preprocessormodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.193730 aimodelshare-0.1.5/aimodelshare/pyspark/
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/1.txt
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/1B.txt
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/2.txt
+-rw-r--r--   0 root         (0) root         (0)     6596 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/3.txt
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/4.txt
+-rw-r--r--   0 root         (0) root         (0)     5988 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/5.txt
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/6.txt
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/7.txt
+-rw-r--r--   0 root         (0) root         (0)     6906 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/8.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10589 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/authorization.txt
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/eval_classification.txt
+-rw-r--r--   0 root         (0) root         (0)    51474 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/eval_lambda.txt
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/eval_regression.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/lambda_function.txt
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/pyspark/nst.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.193730 aimodelshare-0.1.5/aimodelshare/python/
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/python/my_preprocessor.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/readme.md
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/reproducibility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.195730 aimodelshare-0.1.5/aimodelshare/sam/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/Dockerfile_PySpark.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      625 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/codebuild_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/codepipeline_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      245 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/codepipeline_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/spark-class.txt
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/sam/template.txt
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/tools.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/aimodelshare/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.170728 aimodelshare-0.1.5/aimodelshare.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-08-07 09:03:58.000000 aimodelshare-0.1.5/aimodelshare.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-08-07 09:03:59.000000 aimodelshare-0.1.5/aimodelshare.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 09:03:58.000000 aimodelshare-0.1.5/aimodelshare.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2023-08-07 09:03:58.000000 aimodelshare-0.1.5/aimodelshare.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-07 09:03:58.000000 aimodelshare-0.1.5/aimodelshare.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-07 09:03:59.196730 aimodelshare-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 09:03:59.195730 aimodelshare-0.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/tests/test_aimsonnx.py
+-rw-r--r--   0 root         (0) root         (0)    24574 2023-08-07 09:03:47.000000 aimodelshare-0.1.5/tests/test_playground.py
```

### Comparing `aimodelshare-0.1.4/LICENSE` & `aimodelshare-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/PKG-INFO` & `aimodelshare-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: aimodelshare
-Version: 0.1.4
+Version: 0.1.5
 Summary: Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org
 Home-page: https://www.modelshare.org
 Author: Michael Parrott
 Author-email: mikedparrott@modelshare.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aimodelshare-0.1.4/README.md` & `aimodelshare-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/README.md` & `aimodelshare-0.1.5/aimodelshare/README.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/__init__.py` & `aimodelshare-0.1.5/aimodelshare/__init__.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/aimsonnx.py` & `aimodelshare-0.1.5/aimodelshare/aimsonnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 # data wrangling
 import pandas as pd
 import numpy as np
 
 # ml frameworks
-
 try:
     import sklearn
     from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
 except:
-    pass
+    print("Warning: Please install sklearn to enable sklearn features")
+
 try:
     import torch
 except:
-    pass
+    print("Warning: Please install pytorch to enable pytorch features")
+
 try:
     import xgboost
 except:
-    pass
+    print("Warning: Please install xgboost to enable xgboost features")
+
 try:
     import tensorflow as tf
     import keras
 except:
-    pass
+    print("Warning: Please install tensorflow/keras to enable tensorflow/keras features")
+
+try:
+    import pyspark
+    from pyspark.sql import SparkSession
+    from pyspark.ml import PipelineModel, Model
+    from pyspark.ml.tuning import CrossValidatorModel, TrainValidationSplitModel
+    from onnxmltools import convert_sparkml
+except:
+    print("Warning: Please install pyspark to enable pyspark features")
 
 
 # onnx modules
 import onnx
 import skl2onnx
 from skl2onnx import convert_sklearn
 import tf2onnx
@@ -1180,15 +1191,14 @@
             **OP_STYLE
         )
     )
     
     return pydot_graph
 
 
-
 def inspect_model(apiurl, version=None, naming_convention = None, submission_type="competition"):
     if all(["username" in os.environ, 
            "password" in os.environ]):
         pass
     else:
         return print("'Inspect Model' unsuccessful. Please provide credentials with set_credentials().")
 
@@ -1578,17 +1588,17 @@
     module = models_modules_dict[model_type]
     model_class = getattr(importlib.import_module(module), model_type)
     return model_class
 
 def _get_pyspark_modules():
     try:
         if pyspark is None:
-            raise("Error: Please install pyspark to enable pyspark features")
+            raise Exception("Error: Please install pyspark to enable pyspark features")
     except:
-        raise("Error: Please install pyspark to enable pyspark features")
+        raise Exception("Error: Please install pyspark to enable pyspark features")
 
     pyspark_modules = ['ml', 'ml.feature', 'ml.classification', 'ml.clustering', 'ml.regression']
 
     models_modules_dict = {}
 
     for i in pyspark_modules:
         models_list = [j for j in dir(eval('pyspark.'+i)) if callable(getattr(eval('pyspark.'+i), j))]
@@ -1599,17 +1609,17 @@
     
     return models_modules_dict
 
 
 def pyspark_model_from_string(model_type):
     try:
         if pyspark is None:
-            raise("Error: Please install pyspark to enable pyspark features")
+            raise Exception("Error: Please install pyspark to enable pyspark features")
     except:
-        raise("Error: Please install pyspark to enable pyspark features")
+        raise Exception("Error: Please install pyspark to enable pyspark features")
 
     models_modules_dict = _get_pyspark_modules()
     module = models_modules_dict[model_type]
     model_class = getattr(importlib.import_module(module), model_type)
     return model_class
```

### Comparing `aimodelshare-0.1.4/aimodelshare/api.py` & `aimodelshare-0.1.5/aimodelshare/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,16 @@
 
         with open(os.path.join(self.file_objects_folder_path, 'lambda_function.py'), 'w') as file:
             file.write(data)
         
         ###
         api_key = str(shortuuid.uuid())
 
-        t = Template(pkg_resources.read_text(main, 'eval_lambda.txt').replace("$apikey",api_key))
+        t = Template(pkg_resources.read_text(main, 'eval_lambda.txt').replace("$apikey",api_key).replace("$task_type",self.task_type))
+        
         data = t.substitute(bucket_name = self.bucket_name, unique_model_id = self.unique_model_id, task_type = self.task_type)
         with open(os.path.join(self.temp_dir, 'main.py'), 'w') as file:
             file.write(data)
         with ZipFile(os.path.join(self.temp_dir, 'archive2.zip'), 'a') as z:
             z.write(os.path.join(self.temp_dir, 'main.py'), 'main.py')
         self.aws_client.upload_file_to_s3(os.path.join(self.temp_dir, 'archive2.zip'), os.environ.get("BUCKET_NAME"), self.unique_model_id+"/"+'archiveeval.zip')
```

### Comparing `aimodelshare-0.1.4/aimodelshare/aws.py` & `aimodelshare-0.1.5/aimodelshare/aws.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/aws_client.py` & `aimodelshare-0.1.5/aimodelshare/aws_client.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/base_image.py` & `aimodelshare-0.1.5/aimodelshare/base_image.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/bucketpolicy.py` & `aimodelshare-0.1.5/aimodelshare/bucketpolicy.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/color_mappings/color_mapping_keras.csv` & `aimodelshare-0.1.5/aimodelshare/color_mappings/color_mapping_keras.csv`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/color_mappings/color_mapping_pytorch.csv` & `aimodelshare-0.1.5/aimodelshare/color_mappings/color_mapping_pytorch.csv`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/containerisation.py` & `aimodelshare-0.1.5/aimodelshare/containerisation.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/containerization.py` & `aimodelshare-0.1.5/aimodelshare/containerization.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/containerization_templates/Dockerfile_PySpark.txt` & `aimodelshare-0.1.5/aimodelshare/containerization_templates/Dockerfile_PySpark.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/containerization_templates/buildspec.txt` & `aimodelshare-0.1.5/aimodelshare/containerization_templates/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/containerization_templates/lambda_function.txt` & `aimodelshare-0.1.5/aimodelshare/containerization_templates/lambda_function.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/custom_eval_metrics.py` & `aimodelshare-0.1.5/aimodelshare/custom_eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt` & `aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt` & `aimodelshare-0.1.5/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/data_sharing/download_data.py` & `aimodelshare-0.1.5/aimodelshare/data_sharing/download_data.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/data_sharing/share_data.py` & `aimodelshare-0.1.5/aimodelshare/data_sharing/share_data.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/deploy_custom_lambda.py` & `aimodelshare-0.1.5/aimodelshare/deploy_custom_lambda.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/Makefile` & `aimodelshare-0.1.5/aimodelshare/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/__init__.py` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/layout.html` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/search.html` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/searchbox.html` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js` & `aimodelshare-0.1.5/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/make.bat` & `aimodelshare-0.1.5/aimodelshare/documentation/make.bat`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/about.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/about.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/advanced_features.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/advanced_features.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/competition.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/competition.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/conf.py` & `aimodelshare-0.1.5/aimodelshare/documentation/source/conf.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/create_credentials.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/create_credentials.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/example_notebooks.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/example_notebooks.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/functions.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/functions.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/gettingstarted.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds1.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds1.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds2.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds2.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds3.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds3.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds4.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds4.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds5.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds5.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/creds_file_example.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/creds_file_example.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/images/predict_tab.png` & `aimodelshare-0.1.5/aimodelshare/documentation/source/images/predict_tab.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/index.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/index.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/documentation/source/modelplayground.rst` & `aimodelshare-0.1.5/aimodelshare/documentation/source/modelplayground.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/generatemodelapi.py` & `aimodelshare-0.1.5/aimodelshare/generatemodelapi.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/iam/codebuild_policy.txt` & `aimodelshare-0.1.5/aimodelshare/iam/codebuild_policy.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/json_templates/api_json.txt` & `aimodelshare-0.1.5/aimodelshare/json_templates/api_json.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/leaderboard.py` & `aimodelshare-0.1.5/aimodelshare/leaderboard.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/1.txt` & `aimodelshare-0.1.5/aimodelshare/main/1.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/1B.txt` & `aimodelshare-0.1.5/aimodelshare/main/1B.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/2.txt` & `aimodelshare-0.1.5/aimodelshare/main/2.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/3.txt` & `aimodelshare-0.1.5/aimodelshare/main/3.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/4.txt` & `aimodelshare-0.1.5/aimodelshare/main/4.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/5.txt` & `aimodelshare-0.1.5/aimodelshare/main/5.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/6.txt` & `aimodelshare-0.1.5/aimodelshare/main/6.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/7.txt` & `aimodelshare-0.1.5/aimodelshare/main/7.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/8.txt` & `aimodelshare-0.1.5/aimodelshare/main/8.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/authorization.txt` & `aimodelshare-0.1.5/aimodelshare/main/authorization.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/eval_classification.txt` & `aimodelshare-0.1.5/aimodelshare/main/eval_classification.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/eval_lambda.txt` & `aimodelshare-0.1.5/aimodelshare/main/eval_lambda.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,28 @@
     if isinstance(body, six.string_types):
         body = json.loads(body)
     
     for key, value in body.items():
         if value == "None":
             body[key]=None
 
+
+    if body.get("return_task_type","ALL")  == "True" or body.get("return_task_type", "ALL") == "TRUE":
+        task_type="$task_type"
+        task_type_dict = {"statusCode": 200,
+        "headers": {
+        "Access-Control-Allow-Origin" : "*",
+        "Access-Control-Allow-Credentials": True,
+        "Allow" : "GET, OPTIONS, POST",
+        "Access-Control-Allow-Methods" : "GET, OPTIONS, POST",
+        "Access-Control-Allow-Headers" : "*"},
+        "body": json.dumps({"task_type":task_type})
+        }
+        return task_type_dict
+
     if body.get("exampledata", "ALL") == "True" or body.get("exampledata", "ALL") == "TRUE":
 
         exampledata=get_exampledata(example_data_filename = "exampledata.json")
         
         exdata_dict = {"statusCode": 200,
         "headers": {
         "Access-Control-Allow-Origin" : "*",
```

### Comparing `aimodelshare-0.1.4/aimodelshare/main/eval_regression.txt` & `aimodelshare-0.1.5/aimodelshare/main/eval_regression.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/main/nst.txt` & `aimodelshare-0.1.5/aimodelshare/main/nst.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/model.py` & `aimodelshare-0.1.5/aimodelshare/model.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/modeluser.py` & `aimodelshare-0.1.5/aimodelshare/modeluser.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/placeholders/model.onnx` & `aimodelshare-0.1.5/aimodelshare/placeholders/model.onnx`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/placeholders/preprocessor.zip` & `aimodelshare-0.1.5/aimodelshare/placeholders/preprocessor.zip`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/playground.py` & `aimodelshare-0.1.5/aimodelshare/playground.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,21 @@
         # confirm correct args are provided
         if playground_url == None and any([input_type == None, task_type == None, private == None]):
             raise ValueError(
                 "To instantiate a ModelPlayground instance, please provide either a playground_url or \n the input_type, task_type, and private arguments.")
 
         self.model_type = input_type
 
+        if task_type == None:
+            post_dict = {"return_task_type": "TRUE"}
+            headers = { 'Content-Type':'application/json', 'authorizationToken': os.environ.get("AWS_TOKEN"),} 
+            playground_url_eval=playground_url[:-1]+"eval"
+            response = requests.post(playground_url_eval,headers=headers,data=json.dumps(post_dict))
+            task_type = json.loads(response.text)['task_type']
+        
         if task_type == "classification":
             self.categorical = True
         elif task_type == "regression":
             self.categorical = False
         else:
             raise ValueError('Please set task_type argument to "classification" or "regression".')
 
@@ -782,15 +789,15 @@
             from aimodelshare.generatemodelapi import create_experiment
             create_experiment(apiurl=self.playground_url,
                               data_directory=data_directory,
                               y_test=eval_data,
                               eval_metric_filepath=eval_metric_filepath,
                               email_list=email_list,
                               public=public,
-                              public_private_split=public_private_split,
+                              public_private_split=0, #set to 0 because its an experiment
                               input_dict=exp_input_dict,
                               print_output=False)
 
         print("Check out your Model Playground page for more.")
 
         try:
             temp.close()
```

### Comparing `aimodelshare-0.1.4/aimodelshare/postprocessormodules.py` & `aimodelshare-0.1.5/aimodelshare/postprocessormodules.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/preprocessormodules.py` & `aimodelshare-0.1.5/aimodelshare/preprocessormodules.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/1.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/1.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/1B.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/1B.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/2.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/2.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/3.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/3.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/4.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/4.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/5.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/5.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/6.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/6.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/7.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/7.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/8.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/8.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/authorization.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/authorization.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/eval_classification.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/eval_classification.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/eval_lambda.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/eval_lambda.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/eval_regression.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/eval_regression.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/pyspark/nst.txt` & `aimodelshare-0.1.5/aimodelshare/pyspark/nst.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/python/my_preprocessor.py` & `aimodelshare-0.1.5/aimodelshare/python/my_preprocessor.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/readme.md` & `aimodelshare-0.1.5/aimodelshare/readme.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/reproducibility.py` & `aimodelshare-0.1.5/aimodelshare/reproducibility.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/sam/Dockerfile_PySpark.txt` & `aimodelshare-0.1.5/aimodelshare/sam/Dockerfile_PySpark.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/sam/buildspec.txt` & `aimodelshare-0.1.5/aimodelshare/sam/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/sam/codebuild_policies.txt` & `aimodelshare-0.1.5/aimodelshare/sam/codebuild_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/sam/codepipeline_policies.txt` & `aimodelshare-0.1.5/aimodelshare/sam/codepipeline_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/sam/template.txt` & `aimodelshare-0.1.5/aimodelshare/sam/template.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/tools.py` & `aimodelshare-0.1.5/aimodelshare/tools.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare/utils.py` & `aimodelshare-0.1.5/aimodelshare/utils.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/aimodelshare.egg-info/PKG-INFO` & `aimodelshare-0.1.5/aimodelshare.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: aimodelshare
-Version: 0.1.4
+Version: 0.1.5
 Summary: Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org
 Home-page: https://www.modelshare.org
 Author: Michael Parrott
 Author-email: mikedparrott@modelshare.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aimodelshare-0.1.4/aimodelshare.egg-info/SOURCES.txt` & `aimodelshare-0.1.5/aimodelshare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.4/setup.py` & `aimodelshare-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='aimodelshare', #TODO:update
-    version='0.1.4',        #TODO:update
+    version='0.1.5',        #TODO:update
     author="Michael Parrott",
     author_email="mikedparrott@modelshare.org",
     description="Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.modelshare.org",
     packages=setuptools.find_packages(),
```

