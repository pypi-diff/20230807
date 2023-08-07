# Comparing `tmp/tibanna-3.3.1.tar.gz` & `tmp/tibanna-3.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibanna-3.3.1.tar", max compression
+gzip compressed data, was "tibanna-3.3.1b0.tar", max compression
```

## Comparing `tibanna-3.3.1.tar` & `tibanna-3.3.1b0.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rwxr-xr-x   0        0        0     1083 2021-02-24 22:20:32.790882 tibanna-3.3.1/LICENSE.txt
--rwxr-xr-x   0        0        0     2391 2022-04-12 18:14:11.086288 tibanna-3.3.1/README.md
--rwxr-xr-x   0        0        0        0 2021-02-24 22:20:32.794409 tibanna-3.3.1/awsf3/__init__.py
--rwxr-xr-x   0        0        0     5058 2022-03-22 14:50:29.279994 tibanna-3.3.1/awsf3/__main__.py
--rwxr-xr-x   0        0        0    12351 2023-03-20 16:18:32.417979 tibanna-3.3.1/awsf3/aws_run_workflow_generic.sh
--rw-r--r--   0        0        0     1000 2023-03-22 15:34:35.007839 tibanna-3.3.1/awsf3/cloudwatch_agent_config.json
--rw-r--r--   0        0        0     1003 2021-02-24 22:20:32.794931 tibanna-3.3.1/awsf3/log.py
--rw-r--r--   0        0        0     1629 2022-03-22 14:50:29.283309 tibanna-3.3.1/awsf3/spot_failure_detection.sh
--rwxr-xr-x   0        0        0    11814 2022-03-22 14:50:29.284914 tibanna-3.3.1/awsf3/target.py
--rw-r--r--   0        0        0    20670 2022-12-06 18:20:49.560464 tibanna-3.3.1/awsf3/utils.py
--rw-r--r--   0        0        0     1940 2023-04-12 16:25:00.555064 tibanna-3.3.1/pyproject.toml
--rwxr-xr-x   0        0        0      905 2021-02-24 22:20:33.102923 tibanna-3.3.1/tibanna/__init__.py
--rwxr-xr-x   0        0        0    32555 2022-12-06 18:20:49.647426 tibanna-3.3.1/tibanna/__main__.py
--rwxr-xr-x   0        0        0      717 2022-10-31 13:42:10.422020 tibanna-3.3.1/tibanna/_version.py
--rwxr-xr-x   0        0        0     8393 2023-03-16 18:26:02.672939 tibanna-3.3.1/tibanna/ami.py
--rwxr-xr-x   0        0        0    16648 2023-03-16 18:26:02.674092 tibanna-3.3.1/tibanna/awsem.py
--rwxr-xr-x   0        0        0      964 2021-02-24 22:20:33.120382 tibanna-3.3.1/tibanna/base.py
--rwxr-xr-x   0        0        0    12072 2023-03-22 15:34:35.011986 tibanna-3.3.1/tibanna/check_task.py
--rwxr-xr-x   0        0        0    59272 2022-12-06 18:20:49.670461 tibanna-3.3.1/tibanna/core.py
--rw-r--r--   0        0        0      680 2022-12-06 18:20:49.676312 tibanna-3.3.1/tibanna/create_ami_userdata
--rwxr-xr-x   0        0        0    56161 2023-03-22 15:34:35.012952 tibanna-3.3.1/tibanna/cw_utils.py
--rwxr-xr-x   0        0        0     3196 2021-02-24 22:20:33.137619 tibanna-3.3.1/tibanna/dd_utils.py
--rwxr-xr-x   0        0        0    53996 2023-03-22 15:34:35.014084 tibanna-3.3.1/tibanna/ec2_utils.py
--rwxr-xr-x   0        0        0     4326 2022-11-03 20:17:39.217693 tibanna-3.3.1/tibanna/exceptions.py
--rwxr-xr-x   0        0        0    30382 2022-12-06 18:20:49.689939 tibanna-3.3.1/tibanna/iam_utils.py
--rw-r--r--   0        0        0    12760 2023-03-16 18:26:02.674930 tibanna-3.3.1/tibanna/job.py
--rwxr-xr-x   0        0        0      111 2021-03-16 13:52:19.436482 tibanna-3.3.1/tibanna/lambdas/__init__.py
--rwxr-xr-x   0        0        0      522 2022-04-12 18:11:48.701463 tibanna-3.3.1/tibanna/lambdas/check_task_awsem.py
--rwxr-xr-x   0        0        0       68 2023-04-12 16:25:00.555651 tibanna-3.3.1/tibanna/lambdas/requirements.txt
--rwxr-xr-x   0        0        0      471 2022-04-12 18:11:48.711468 tibanna-3.3.1/tibanna/lambdas/run_task_awsem.py
--rwxr-xr-x   0        0        0      491 2022-04-12 18:11:48.719469 tibanna-3.3.1/tibanna/lambdas/update_cost_awsem.py
--rwxr-xr-x   0        0        0     2757 2021-02-24 22:20:33.153185 tibanna-3.3.1/tibanna/nnested_array.py
--rwxr-xr-x   0        0        0    19075 2022-12-06 18:20:49.706362 tibanna-3.3.1/tibanna/pricing_utils.py
--rwxr-xr-x   0        0        0     3215 2021-04-19 16:08:03.718285 tibanna-3.3.1/tibanna/run_task.py
--rwxr-xr-x   0        0        0     3418 2022-10-31 13:42:10.450245 tibanna-3.3.1/tibanna/stepfunction.py
--rwxr-xr-x   0        0        0     2469 2021-09-27 13:44:50.867418 tibanna-3.3.1/tibanna/stepfunction_cost_updater.py
--rw-r--r--   0        0        0    17156 2021-09-27 13:51:09.655388 tibanna-3.3.1/tibanna/top.py
--rwxr-xr-x   0        0        0     2203 2021-03-16 13:52:19.439863 tibanna-3.3.1/tibanna/update_cost.py
--rwxr-xr-x   0        0        0     6671 2022-03-22 14:50:29.302765 tibanna-3.3.1/tibanna/utils.py
--rwxr-xr-x   0        0        0     6290 2023-03-22 15:34:35.016604 tibanna-3.3.1/tibanna/vars.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 tibanna-3.3.1/setup.py
--rw-r--r--   0        0        0     3466 1970-01-01 00:00:00.000000 tibanna-3.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2021-02-24 22:20:32.790882 tibanna-3.3.1b0/LICENSE.txt
+-rwxr-xr-x   0        0        0     2391 2022-04-12 18:14:11.086288 tibanna-3.3.1b0/README.md
+-rwxr-xr-x   0        0        0        0 2021-02-24 22:20:32.794409 tibanna-3.3.1b0/awsf3/__init__.py
+-rwxr-xr-x   0        0        0     5058 2022-03-22 14:50:29.279994 tibanna-3.3.1b0/awsf3/__main__.py
+-rwxr-xr-x   0        0        0    12351 2023-03-20 16:18:32.417979 tibanna-3.3.1b0/awsf3/aws_run_workflow_generic.sh
+-rw-r--r--   0        0        0     1000 2023-03-22 15:34:35.007839 tibanna-3.3.1b0/awsf3/cloudwatch_agent_config.json
+-rw-r--r--   0        0        0     1003 2021-02-24 22:20:32.794931 tibanna-3.3.1b0/awsf3/log.py
+-rw-r--r--   0        0        0     1629 2022-03-22 14:50:29.283309 tibanna-3.3.1b0/awsf3/spot_failure_detection.sh
+-rwxr-xr-x   0        0        0    11814 2022-03-22 14:50:29.284914 tibanna-3.3.1b0/awsf3/target.py
+-rw-r--r--   0        0        0    20670 2022-12-06 18:20:49.560464 tibanna-3.3.1b0/awsf3/utils.py
+-rw-r--r--   0        0        0     1942 2023-08-07 19:20:23.060103 tibanna-3.3.1b0/pyproject.toml
+-rwxr-xr-x   0        0        0      905 2021-02-24 22:20:33.102923 tibanna-3.3.1b0/tibanna/__init__.py
+-rwxr-xr-x   0        0        0    32555 2022-12-06 18:20:49.647426 tibanna-3.3.1b0/tibanna/__main__.py
+-rwxr-xr-x   0        0        0      717 2022-10-31 13:42:10.422020 tibanna-3.3.1b0/tibanna/_version.py
+-rwxr-xr-x   0        0        0     8393 2023-03-16 18:26:02.672939 tibanna-3.3.1b0/tibanna/ami.py
+-rwxr-xr-x   0        0        0    16648 2023-03-16 18:26:02.674092 tibanna-3.3.1b0/tibanna/awsem.py
+-rwxr-xr-x   0        0        0      964 2021-02-24 22:20:33.120382 tibanna-3.3.1b0/tibanna/base.py
+-rwxr-xr-x   0        0        0    12072 2023-03-22 15:34:35.011986 tibanna-3.3.1b0/tibanna/check_task.py
+-rwxr-xr-x   0        0        0    60331 2023-08-07 19:14:42.865761 tibanna-3.3.1b0/tibanna/core.py
+-rw-r--r--   0        0        0      680 2022-12-06 18:20:49.676312 tibanna-3.3.1b0/tibanna/create_ami_userdata
+-rwxr-xr-x   0        0        0    56161 2023-07-24 19:16:28.026972 tibanna-3.3.1b0/tibanna/cw_utils.py
+-rwxr-xr-x   0        0        0     3196 2021-02-24 22:20:33.137619 tibanna-3.3.1b0/tibanna/dd_utils.py
+-rwxr-xr-x   0        0        0    53996 2023-03-22 15:34:35.014084 tibanna-3.3.1b0/tibanna/ec2_utils.py
+-rwxr-xr-x   0        0        0     4326 2022-11-03 20:17:39.217693 tibanna-3.3.1b0/tibanna/exceptions.py
+-rwxr-xr-x   0        0        0    30382 2022-12-06 18:20:49.689939 tibanna-3.3.1b0/tibanna/iam_utils.py
+-rw-r--r--   0        0        0    12760 2023-03-16 18:26:02.674930 tibanna-3.3.1b0/tibanna/job.py
+-rwxr-xr-x   0        0        0      111 2021-03-16 13:52:19.436482 tibanna-3.3.1b0/tibanna/lambdas/__init__.py
+-rwxr-xr-x   0        0        0      522 2022-04-12 18:11:48.701463 tibanna-3.3.1b0/tibanna/lambdas/check_task_awsem.py
+-rwxr-xr-x   0        0        0       68 2023-04-12 16:25:00.555651 tibanna-3.3.1b0/tibanna/lambdas/requirements.txt
+-rwxr-xr-x   0        0        0      471 2022-04-12 18:11:48.711468 tibanna-3.3.1b0/tibanna/lambdas/run_task_awsem.py
+-rwxr-xr-x   0        0        0      491 2022-04-12 18:11:48.719469 tibanna-3.3.1b0/tibanna/lambdas/update_cost_awsem.py
+-rwxr-xr-x   0        0        0     2757 2021-02-24 22:20:33.153185 tibanna-3.3.1b0/tibanna/nnested_array.py
+-rwxr-xr-x   0        0        0    19075 2023-08-07 19:14:40.095138 tibanna-3.3.1b0/tibanna/pricing_utils.py
+-rwxr-xr-x   0        0        0     3215 2021-04-19 16:08:03.718285 tibanna-3.3.1b0/tibanna/run_task.py
+-rwxr-xr-x   0        0        0     3418 2022-10-31 13:42:10.450245 tibanna-3.3.1b0/tibanna/stepfunction.py
+-rwxr-xr-x   0        0        0     2469 2021-09-27 13:44:50.867418 tibanna-3.3.1b0/tibanna/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0    17156 2021-09-27 13:51:09.655388 tibanna-3.3.1b0/tibanna/top.py
+-rwxr-xr-x   0        0        0     2203 2021-03-16 13:52:19.439863 tibanna-3.3.1b0/tibanna/update_cost.py
+-rwxr-xr-x   0        0        0     6671 2022-03-22 14:50:29.302765 tibanna-3.3.1b0/tibanna/utils.py
+-rwxr-xr-x   0        0        0     6290 2023-03-22 15:34:35.016604 tibanna-3.3.1b0/tibanna/vars.py
+-rw-r--r--   0        0        0     3468 1970-01-01 00:00:00.000000 tibanna-3.3.1b0/PKG-INFO
```

### Comparing `tibanna-3.3.1/LICENSE.txt` & `tibanna-3.3.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/README.md` & `tibanna-3.3.1b0/README.md`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/__main__.py` & `tibanna-3.3.1b0/awsf3/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/aws_run_workflow_generic.sh` & `tibanna-3.3.1b0/awsf3/aws_run_workflow_generic.sh`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/cloudwatch_agent_config.json` & `tibanna-3.3.1b0/awsf3/cloudwatch_agent_config.json`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/log.py` & `tibanna-3.3.1b0/awsf3/log.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/spot_failure_detection.sh` & `tibanna-3.3.1b0/awsf3/spot_failure_detection.sh`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/target.py` & `tibanna-3.3.1b0/awsf3/target.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/awsf3/utils.py` & `tibanna-3.3.1b0/awsf3/utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/pyproject.toml` & `tibanna-3.3.1b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibanna"
-version = "3.3.1"
+version = "3.3.1b0"
 description = "Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tibanna"]
 homepage = "http://github.com/4dn-dcic/tibanna"
 repository = "http://github.com/4dn-dcic/tibanna.git"
```

### Comparing `tibanna-3.3.1/tibanna/__init__.py` & `tibanna-3.3.1b0/tibanna/__init__.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/__main__.py` & `tibanna-3.3.1b0/tibanna/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/_version.py` & `tibanna-3.3.1b0/tibanna/_version.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/ami.py` & `tibanna-3.3.1b0/tibanna/ami.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/awsem.py` & `tibanna-3.3.1b0/tibanna/awsem.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/base.py` & `tibanna-3.3.1b0/tibanna/base.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/check_task.py` & `tibanna-3.3.1b0/tibanna/check_task.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/core.py` & `tibanna-3.3.1b0/tibanna/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,37 +387,39 @@
             raise Exception("n and job_id filters do not work together.")
         if sfn and job_ids:
             raise Exception("Please do not specify sfn when job_ids are specified.")
         if status and job_ids:
             raise Exception("Status filter cannot be specified when job_ids are specified.")
         if verbose:
             print("{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}".format('jobid', 'status', 'name',
-                                                                      'start_time', 'stop_time',
-                                                                      'instance_id', 'instance_type',
+                                                                      'execution_start_time', 'execution_stop_time',
+                                                                      'instance_id', 'instance_start_time', 'instance_type',
                                                                       'instance_status', 'ip', 'key',
                                                                       'password'))
         else:
-            print("{}\t{}\t{}\t{}\t{}".format('jobid', 'status', 'name', 'start_time', 'stop_time'))
+            print("{}\t{}\t{}\t{}\t{}".format('jobid', 'status', 'name', 'execution_start_time', 'execution_stop_time'))
         client = boto3.client('stepfunctions')
         ec2 = boto3.client('ec2')
 
-        def parse_exec_desc_and_ec2_desc(exec_arn, verbose):
+        def parse_exec_desc_and_ec2_desc(exec_arn, verbose, job_id=None):
             # collecting execution stats
             exec_desc = client.describe_execution(executionArn=exec_arn)
 
             # getting info from execution description
             exec_desc = client.describe_execution(executionArn=exec_arn)
             job_id = json.loads(exec_desc['input']).get('jobid', 'no jobid')
             status = exec_desc['status']
             name = exec_desc['name']
-            start_time = exec_desc['startDate'].strftime("%Y-%m-%d %H:%M")
+            execution_start_time_ts = exec_desc['startDate'].timestamp()
+            execution_start_time = datetime.fromtimestamp(execution_start_time_ts).strftime("%Y-%m-%d %H:%M")
             if 'stopDate' in exec_desc:
-                stop_time = exec_desc['stopDate'].strftime("%Y-%m-%d %H:%M")
+                execution_stop_time_ts = exec_desc['stopDate'].timestamp()
+                execution_stop_time = datetime.fromtimestamp(execution_stop_time_ts).strftime("%Y-%m-%d %H:%M")
             else:
-                stop_time = ''
+                execution_stop_time = ''
 
             # collect instance stats
             ec2_desc = ec2.describe_instances(Filters=[{'Name': 'tag:Name', 'Values': ['awsem-' + job_id]}])
 
             # getting info from ec2 description
             if ec2_desc['Reservations']:
                 ec2_desc_inst = ec2_desc['Reservations'][0]['Instances'][0]
@@ -436,31 +438,43 @@
                 instance_status = '-'
                 instance_id = '-'
                 instance_type = '-'
                 instance_ip = '-'
                 keyname = '-'
                 password = '-'
 
-            parsed_stat = (job_id, status, name, start_time, stop_time,
-                           instance_id, instance_type, instance_status,
+            instance_start_time = '-'
+            if verbose and job_id:
+                try:
+                    job = Job(exec_arn=exec_arn, job_id=job_id, sfn=self.default_stepfunction_name)
+                    # We use the creation date of <job_id>.job_started as proxy for the EC2 creation date
+                    res_s3 = boto3.client('s3').get_object(Bucket=job.log_bucket, Key=job.job_id + ".job_started")
+                    instance_start_time_ts = res_s3['LastModified'].timestamp()
+                    instance_start_time = datetime.fromtimestamp(instance_start_time_ts).strftime("%Y-%m-%d %H:%M")
+                except Exception as e:
+                    instance_start_time = 'NA'
+
+
+            parsed_stat = (job_id, status, name, execution_start_time, execution_stop_time,
+                           instance_id, instance_start_time, instance_type, instance_status,
                            instance_ip, keyname, password)
             if verbose:
                 print("{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}".format(*parsed_stat))
             else:
                 print("{}\t{}\t{}\t{}\t{}".format(*parsed_stat[0:5]))
 
         if job_ids:
             for job_id in job_ids:
                 dd_info = self.info(job_id)
                 if 'Execution Name' not in dd_info:
                     raise Exception("Cannot find execution name for job ID %s" % job_id)
                 if 'Step Function' not in dd_info:
                     raise Exception("Cannot find step function for job ID %s" % job_id)
                 exec_arn = EXECUTION_ARN(dd_info['Execution Name'], dd_info['Step Function'])
-                parse_exec_desc_and_ec2_desc(exec_arn, verbose)
+                parse_exec_desc_and_ec2_desc(exec_arn, verbose, job_id=job_id)
         else:
             if not sfn:
                 sfn = self.default_stepfunction_name
             args = {
                 'stateMachineArn': STEP_FUNCTION_ARN(sfn),
                 'maxResults': 100
             }
```

### Comparing `tibanna-3.3.1/tibanna/create_ami_userdata` & `tibanna-3.3.1b0/tibanna/create_ami_userdata`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/cw_utils.py` & `tibanna-3.3.1b0/tibanna/cw_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/dd_utils.py` & `tibanna-3.3.1b0/tibanna/dd_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/ec2_utils.py` & `tibanna-3.3.1b0/tibanna/ec2_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/exceptions.py` & `tibanna-3.3.1b0/tibanna/exceptions.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/iam_utils.py` & `tibanna-3.3.1b0/tibanna/iam_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/job.py` & `tibanna-3.3.1b0/tibanna/job.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/lambdas/check_task_awsem.py` & `tibanna-3.3.1b0/tibanna/lambdas/check_task_awsem.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/nnested_array.py` & `tibanna-3.3.1b0/tibanna/nnested_array.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/pricing_utils.py` & `tibanna-3.3.1b0/tibanna/pricing_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/run_task.py` & `tibanna-3.3.1b0/tibanna/run_task.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/stepfunction.py` & `tibanna-3.3.1b0/tibanna/stepfunction.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/stepfunction_cost_updater.py` & `tibanna-3.3.1b0/tibanna/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/top.py` & `tibanna-3.3.1b0/tibanna/top.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/update_cost.py` & `tibanna-3.3.1b0/tibanna/update_cost.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/utils.py` & `tibanna-3.3.1b0/tibanna/utils.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/tibanna/vars.py` & `tibanna-3.3.1b0/tibanna/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna-3.3.1/PKG-INFO` & `tibanna-3.3.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibanna
-Version: 3.3.1
+Version: 3.3.1b0
 Summary: Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.
 Home-page: http://github.com/4dn-dcic/tibanna
 License: MIT
 Keywords: tibanna
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.9
```

