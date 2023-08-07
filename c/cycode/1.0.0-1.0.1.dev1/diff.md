# Comparing `tmp/cycode-1.0.0.tar.gz` & `tmp/cycode-1.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-1.0.0.tar", max compression
+gzip compressed data, was "cycode-1.0.1.dev1.tar", max compression
```

## Comparing `cycode-1.0.0.tar` & `cycode-1.0.1.dev1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0    33099 2023-07-30 08:05:46.108893 cycode-1.0.0/README.md
--rw-r--r--   0        0        0      109 2023-07-30 08:06:03.940979 cycode-1.0.0/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     3003 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4727 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1588 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    54675 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      466 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5819 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1792 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2042 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      983 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     3004 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5927 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7805 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/main.py
--rw-r--r--   0        0        0     1584 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1973 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0      786 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/printer_base.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.108893 cycode-1.0.0/cycode/cli/printers/tables/__init__.py
--rw-r--r--   0        0        0     5853 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/sca_table_printer.py
--rw-r--r--   0        0        0     2281 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table.py
--rw-r--r--   0        0        0      480 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table_models.py
--rw-r--r--   0        0        0     5471 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table_printer.py
--rw-r--r--   0        0        0     2025 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/tables/table_printer_base.py
--rw-r--r--   0        0        0    10099 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      630 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4741 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     7202 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1954 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6687 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0      211 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/enum_utils.py
--rw-r--r--   0        0        0     2339 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0     7619 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/progress_bar.py
--rw-r--r--   0        0        0     2782 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/scan_batch.py
--rw-r--r--   0        0        0      334 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      978 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     2034 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2748 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      934 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0     1011 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       56 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1749 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2664 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      120 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      228 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3954 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      640 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1848 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0    10005 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6407 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1086 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1254 2023-07-30 08:05:46.112893 cycode-1.0.0/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0     3476 2023-07-30 08:06:03.936979 cycode-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    34635 1970-01-01 00:00:00.000000 cycode-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    33844 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/README.md
+-rw-r--r--   0        0        0      114 2023-08-07 10:20:58.740058 cycode-1.0.1.dev1/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     3003 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4727 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1588 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    56324 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      466 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5819 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     2061 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2042 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      983 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     3004 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5927 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     1857 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/helpers/tf_content_generator.py
+-rw-r--r--   0        0        0     7805 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/main.py
+-rw-r--r--   0        0        0     1845 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0     2078 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1973 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0      786 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/printer_base.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/tables/__init__.py
+-rw-r--r--   0        0        0     5853 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/tables/sca_table_printer.py
+-rw-r--r--   0        0        0     2281 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/tables/table.py
+-rw-r--r--   0        0        0      480 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/tables/table_models.py
+-rw-r--r--   0        0        0     5471 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/tables/table_printer.py
+-rw-r--r--   0        0        0     2025 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/tables/table_printer_base.py
+-rw-r--r--   0        0        0    10099 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      630 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4741 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     7202 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1954 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6687 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0      211 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/enum_utils.py
+-rw-r--r--   0        0        0     2764 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0     7619 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/progress_bar.py
+-rw-r--r--   0        0        0     2782 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/scan_batch.py
+-rw-r--r--   0        0        0      334 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      978 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     2034 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2748 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      934 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0     1011 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       56 2023-08-07 10:20:41.831845 cycode-1.0.1.dev1/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1749 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2664 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      120 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      228 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3954 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      640 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1848 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0    10005 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6407 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1086 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1254 2023-08-07 10:20:41.835845 cycode-1.0.1.dev1/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0     3481 2023-08-07 10:20:58.736058 cycode-1.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0    35385 1970-01-01 00:00:00.000000 cycode-1.0.1.dev1/PKG-INFO
```

### Comparing `cycode-1.0.0/README.md` & `cycode-1.0.1.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         1. [Branch Option](#branch-option)
     2. [Monitor Option](#monitor-option)
     3. [Report Option](#report-option)
     4. [Package Vulnerabilities Scan](#package-vulnerabilities-option)
         1. [License Compliance Option](#license-compliance-option)
         2. [Severity Threshold](#severity-threshold)
     5. [Path Scan](#path-scan)
+        1. [Terraform Plan Scan](#terraform-plan-scan)
     6. [Commit History Scan](#commit-history-scan)
         1. [Commit Range Option](#commit-range-option)
     7. [Pre-Commit Scan](#pre-commit-scan)
 5. [Scan Results](#scan-results)
     1. [Show/Hide Secrets](#showhide-secrets)
     2. [Soft Fail](#soft-fail)
     3. [Example Scan Results](#example-scan-results)
@@ -417,14 +418,44 @@
 
 `cycode scan path {{path}}`
 
 For example, consider a scenario in which you want to scan the directory located at `~/home/git/codebase`. You could then execute the following:
 
 `cycode scan path ~/home/git/codebase`
 
+
+### Terraform Plan Scan
+
+Cycode CLI supports Terraform plan scanning (supporting Terraform 0.12 and later)
+
+Terraform plan file must be in JSON format (having `.json` extension)
+
+
+_How to generate a Terraform plan from Terraform configuration file?_
+    
+1. Initialize a working directory that contains Terraform configuration file:
+
+    `terraform init`
+
+
+2. Create Terraform execution plan and save the binary output:
+
+    `terraform plan -out={tfplan_output}`
+
+
+3. Convert the binary output file into readable JSON:
+
+    `terraform show -json {tfplan_output} > {tfplan}.json`
+
+
+4. Scan your `{tfplan}.json` with Cycode CLI:
+
+    `cycode scan -t iac path ~/PATH/TO/YOUR/{tfplan}.json`
+
+
 ## Commit History Scan
 
 A commit history scan is limited to a local repository’s previous commits, focused on finding any secrets within the commit history, instead of examining the repository’s current state.
 
 To execute a commit history scan, execute the following:
 
 `cycode scan commit_history {{path}}`
```

### Comparing `cycode-1.0.0/cycode/cli/auth/auth_command.py` & `cycode-1.0.1.dev1/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/auth/auth_manager.py` & `cycode-1.0.1.dev1/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/ci_integrations.py` & `cycode-1.0.1.dev1/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/code_scanner.py` & `cycode-1.0.1.dev1/cycode/cli/code_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 import click
 from git import NULL_TREE, InvalidGitRepositoryError, Repo
 
 from cycode.cli import consts
 from cycode.cli.ci_integrations import get_commit_range
 from cycode.cli.config import configuration_manager
 from cycode.cli.exceptions import custom_exceptions
-from cycode.cli.helpers import sca_code_scanner
+from cycode.cli.helpers import sca_code_scanner, tf_content_generator
 from cycode.cli.models import CliError, CliErrors, Document, DocumentDetections, LocalScanResult, Severity
 from cycode.cli.printers import ConsolePrinter
 from cycode.cli.user_settings.config_file_manager import ConfigFileManager
 from cycode.cli.utils import scan_utils
 from cycode.cli.utils.path_utils import (
+    change_filename_extension,
     get_file_content,
     get_file_size,
     get_path_by_os,
     get_relevant_files_in_path,
     is_binary_file,
     is_sub_path,
+    load_json,
 )
 from cycode.cli.utils.progress_bar import ProgressBarSection
 from cycode.cli.utils.progress_bar import logger as progress_bar_logger
 from cycode.cli.utils.scan_batch import run_parallel_batched_scan
 from cycode.cli.utils.scan_utils import set_issue_detected
 from cycode.cli.utils.string_utils import get_content_size, is_binary_content
 from cycode.cli.utils.task_timer import TimeoutAfter
@@ -324,26 +326,30 @@
 def scan_disk_files(context: click.Context, path: str, files_to_scan: List[str]) -> None:
     scan_parameters = get_scan_parameters(context, path)
     scan_type = context.obj['scan_type']
     progress_bar = context.obj['progress_bar']
 
     is_git_diff = False
 
-    documents: List[Document] = []
-    for file in files_to_scan:
-        progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
+    try:
+        documents: List[Document] = []
+        for file in files_to_scan:
+            progress_bar.update(ProgressBarSection.PREPARE_LOCAL_FILES)
 
-        content = get_file_content(file)
-        if not content:
-            continue
+            content = get_file_content(file)
+            if not content:
+                continue
 
-        documents.append(Document(file, content, is_git_diff))
+            documents.append(_generate_document(file, scan_type, content, is_git_diff))
 
-    perform_pre_scan_documents_actions(context, scan_type, documents, is_git_diff)
-    scan_documents(context, documents, is_git_diff=is_git_diff, scan_parameters=scan_parameters)
+        perform_pre_scan_documents_actions(context, scan_type, documents, is_git_diff)
+        scan_documents(context, documents, is_git_diff=is_git_diff, scan_parameters=scan_parameters)
+
+    except Exception as e:
+        _handle_exception(context, e)
 
 
 def set_issue_detected_by_scan_results(context: click.Context, scan_results: List[LocalScanResult]) -> None:
     set_issue_detected(context, any(scan_result.issue_detected for scan_result in scan_results))
 
 
 def _get_scan_documents_thread_func(
@@ -570,15 +576,15 @@
     )
 
 
 def perform_pre_scan_documents_actions(
     context: click.Context, scan_type: str, documents_to_scan: List[Document], is_git_diff: bool = False
 ) -> None:
     if scan_type == consts.SCA_SCAN_TYPE:
-        logger.debug('Perform pre scan document actions')
+        logger.debug('Perform pre scan document add_dependencies_tree_document action')
         sca_code_scanner.add_dependencies_tree_document(context, documents_to_scan, is_git_diff)
 
 
 def zip_documents_to_scan(scan_type: str, zip_file: InMemoryZip, documents: List[Document]) -> InMemoryZip:
     start_zip_creation_time = time.time()
 
     for index, document in enumerate(documents):
@@ -1095,14 +1101,45 @@
 
     if scan_type == consts.SCA_SCAN_TYPE:
         return filename.endswith(consts.SCA_CONFIGURATION_SCAN_SUPPORTED_FILES)
 
     return not filename.endswith(consts.SECRET_SCAN_FILE_EXTENSIONS_TO_IGNORE)
 
 
+def _generate_document(file: str, scan_type: str, content: str, is_git_diff: bool) -> Document:
+    if _is_iac(scan_type) and _is_tfplan_file(file, content):
+        return _handle_tfplan_file(file, content, is_git_diff)
+    return Document(file, content, is_git_diff)
+
+
+def _handle_tfplan_file(file: str, content: str, is_git_diff: bool) -> Document:
+    document_name = _generate_tfplan_document_name(file)
+    tf_content = tf_content_generator.generate_tf_content_from_tfplan(file, content)
+    return Document(document_name, tf_content, is_git_diff)
+
+
+def _generate_tfplan_document_name(path: str) -> str:
+    document_name = change_filename_extension(path, 'tf')
+    timestamp = int(time.time())
+    return f'{timestamp}-{document_name}'
+
+
+def _is_iac(scan_type: str) -> bool:
+    return scan_type == consts.INFRA_CONFIGURATION_SCAN_TYPE
+
+
+def _is_tfplan_file(file: str, content: str) -> bool:
+    if not file.endswith('.json'):
+        return False
+    tf_plan = load_json(content)
+    if not isinstance(tf_plan, dict):
+        return False
+    return 'resource_changes' in tf_plan
+
+
 def _does_file_exceed_max_size_limit(filename: str) -> bool:
     return get_file_size(filename) > consts.FILE_MAX_SIZE_LIMIT_IN_BYTES
 
 
 def _does_document_exceed_max_size_limit(content: str) -> bool:
     return get_content_size(content) > consts.FILE_MAX_SIZE_LIMIT_IN_BYTES
 
@@ -1153,14 +1190,22 @@
         custom_exceptions.ZipTooLargeError: CliError(
             soft_fail=True,
             code='zip_too_large_error',
             message='The path you attempted to scan exceeds the current maximum scanning size cap (10MB). '
             'Please try ignoring irrelevant paths using the `cycode ignore --by-path` command '
             'and execute the scan again',
         ),
+        custom_exceptions.TfplanKeyError: CliError(
+            soft_fail=True,
+            code='key_error',
+            message=f'\n{e!s}\n'
+            'A crucial field is missing in your terraform plan file. '
+            'Please make sure that your file is well formed '
+            'and execute the scan again',
+        ),
         InvalidGitRepositoryError: CliError(
             soft_fail=False,
             code='invalid_git_error',
             message='The path you supplied does not correlate to a git repository. '
             'If you still wish to scan this path, use: `cycode scan path <path>`',
         ),
     }
```

### Comparing `cycode-1.0.0/cycode/cli/consts.py` & `cycode-1.0.1.dev1/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-1.0.1.dev1/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-1.0.1.dev1/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-1.0.1.dev1/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/helpers/sca_code_scanner.py` & `cycode-1.0.1.dev1/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/main.py` & `cycode-1.0.1.dev1/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/models.py` & `cycode-1.0.1.dev1/cycode/cli/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import dataclass
 from enum import Enum
 from typing import Dict, List, NamedTuple, Optional, Type
 
 from cycode.cyclient.models import Detection
 
 
 class Document:
@@ -59,7 +60,18 @@
 class LocalScanResult(NamedTuple):
     scan_id: str
     report_url: Optional[str]
     document_detections: List[DocumentDetections]
     issue_detected: bool
     detections_count: int
     relevant_detections_count: int
+
+
+@dataclass
+class ResourceChange:
+    resource_type: str
+    name: str
+    actions: List[str]
+    values: Dict[str, str]
+
+    def __repr__(self) -> str:
+        return f'resource_type: {self.resource_type}, name: {self.name}'
```

### Comparing `cycode-1.0.0/cycode/cli/printers/console_printer.py` & `cycode-1.0.1.dev1/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/json_printer.py` & `cycode-1.0.1.dev1/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/printer_base.py` & `cycode-1.0.1.dev1/cycode/cli/printers/printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/tables/sca_table_printer.py` & `cycode-1.0.1.dev1/cycode/cli/printers/tables/sca_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/tables/table.py` & `cycode-1.0.1.dev1/cycode/cli/printers/tables/table.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/tables/table_printer.py` & `cycode-1.0.1.dev1/cycode/cli/printers/tables/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/tables/table_printer_base.py` & `cycode-1.0.1.dev1/cycode/cli/printers/tables/table_printer_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/printers/text_printer.py` & `cycode-1.0.1.dev1/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/user_settings/base_file_manager.py` & `cycode-1.0.1.dev1/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/user_settings/config_file_manager.py` & `cycode-1.0.1.dev1/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/user_settings/configuration_manager.py` & `cycode-1.0.1.dev1/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/user_settings/credentials_manager.py` & `cycode-1.0.1.dev1/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/user_settings/user_settings_commands.py` & `cycode-1.0.1.dev1/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/utils/path_utils.py` & `cycode-1.0.1.dev1/cycode/cli/utils/path_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 from functools import lru_cache
 from typing import AnyStr, Iterable, List, Optional
 
 import pathspec
 from binaryornot.check import is_binary
 
@@ -67,17 +68,33 @@
     return os.path.exists(path)
 
 
 def get_file_dir(path: str) -> str:
     return os.path.dirname(path)
 
 
+def get_immediate_subdirectories(path: str) -> List[str]:
+    return [f.name for f in os.scandir(path) if f.is_dir()]
+
+
 def join_paths(path: str, filename: str) -> str:
     return os.path.join(path, filename)
 
 
 def get_file_content(file_path: str) -> Optional[AnyStr]:
     try:
         with open(file_path, 'r', encoding='UTF-8') as f:
             return f.read()
     except (FileNotFoundError, UnicodeDecodeError):
         return None
+
+
+def load_json(txt: str) -> Optional[dict]:
+    try:
+        return json.loads(txt)
+    except json.JSONDecodeError:
+        return None
+
+
+def change_filename_extension(filename: str, extension: str) -> str:
+    base_name, _ = os.path.splitext(filename)
+    return f'{base_name}.{extension}'
```

### Comparing `cycode-1.0.0/cycode/cli/utils/progress_bar.py` & `cycode-1.0.1.dev1/cycode/cli/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/utils/scan_batch.py` & `cycode-1.0.1.dev1/cycode/cli/utils/scan_batch.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/utils/shell_executor.py` & `cycode-1.0.1.dev1/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/utils/string_utils.py` & `cycode-1.0.1.dev1/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/utils/task_timer.py` & `cycode-1.0.1.dev1/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/utils/yaml_utils.py` & `cycode-1.0.1.dev1/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cli/zip_file.py` & `cycode-1.0.1.dev1/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/auth_client.py` & `cycode-1.0.1.dev1/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/config.py` & `cycode-1.0.1.dev1/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/cycode_client_base.py` & `cycode-1.0.1.dev1/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/cycode_dev_based_client.py` & `cycode-1.0.1.dev1/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/cycode_token_based_client.py` & `cycode-1.0.1.dev1/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/models.py` & `cycode-1.0.1.dev1/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/scan_client.py` & `cycode-1.0.1.dev1/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-1.0.1.dev1/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-1.0.1.dev1/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-1.0.0/pyproject.toml` & `cycode-1.0.1.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "1.0.0" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "1.0.1.dev1" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning."
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-1.0.0/PKG-INFO` & `cycode-1.0.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 1.0.0
+Version: 1.0.1.dev1
 Summary: Boost security in your dev lifecycle via SAST, SCA, Secrets & IaC scanning.
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
@@ -58,14 +58,15 @@
         1. [Branch Option](#branch-option)
     2. [Monitor Option](#monitor-option)
     3. [Report Option](#report-option)
     4. [Package Vulnerabilities Scan](#package-vulnerabilities-option)
         1. [License Compliance Option](#license-compliance-option)
         2. [Severity Threshold](#severity-threshold)
     5. [Path Scan](#path-scan)
+        1. [Terraform Plan Scan](#terraform-plan-scan)
     6. [Commit History Scan](#commit-history-scan)
         1. [Commit Range Option](#commit-range-option)
     7. [Pre-Commit Scan](#pre-commit-scan)
 5. [Scan Results](#scan-results)
     1. [Show/Hide Secrets](#showhide-secrets)
     2. [Soft Fail](#soft-fail)
     3. [Example Scan Results](#example-scan-results)
@@ -454,14 +455,44 @@
 
 `cycode scan path {{path}}`
 
 For example, consider a scenario in which you want to scan the directory located at `~/home/git/codebase`. You could then execute the following:
 
 `cycode scan path ~/home/git/codebase`
 
+
+### Terraform Plan Scan
+
+Cycode CLI supports Terraform plan scanning (supporting Terraform 0.12 and later)
+
+Terraform plan file must be in JSON format (having `.json` extension)
+
+
+_How to generate a Terraform plan from Terraform configuration file?_
+    
+1. Initialize a working directory that contains Terraform configuration file:
+
+    `terraform init`
+
+
+2. Create Terraform execution plan and save the binary output:
+
+    `terraform plan -out={tfplan_output}`
+
+
+3. Convert the binary output file into readable JSON:
+
+    `terraform show -json {tfplan_output} > {tfplan}.json`
+
+
+4. Scan your `{tfplan}.json` with Cycode CLI:
+
+    `cycode scan -t iac path ~/PATH/TO/YOUR/{tfplan}.json`
+
+
 ## Commit History Scan
 
 A commit history scan is limited to a local repository’s previous commits, focused on finding any secrets within the commit history, instead of examining the repository’s current state.
 
 To execute a commit history scan, execute the following:
 
 `cycode scan commit_history {{path}}`
```

