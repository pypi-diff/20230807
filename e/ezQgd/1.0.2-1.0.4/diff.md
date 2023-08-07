# Comparing `tmp/ezQgd-1.0.2-py3-none-any.whl.zip` & `tmp/ezQgd-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17672 bytes, number of entries: 13
--rw-r--r--  2.0 unx    35259 b- defN 23-Jul-11 15:38 ezQgd.py
+Zip file size: 17922 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    36856 b- defN 23-Aug-07 08:03 ezQgd.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:52 qasmtoqcis/__init__.py
 -rw-r--r--  2.0 unx     3973 b- defN 23-Jul-11 05:52 qasmtoqcis/const.py
 -rw-r--r--  2.0 unx     7400 b- defN 23-Jul-11 05:52 qasmtoqcis/qasm.py
 -rw-r--r--  2.0 unx    11185 b- defN 23-Jul-11 05:52 qasmtoqcis/qasm_to_qcis.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:52 qcistoqasm/__init__.py
 -rw-r--r--  2.0 unx      409 b- defN 23-Jul-11 05:52 qcistoqasm/const.py
 -rw-r--r--  2.0 unx     2612 b- defN 23-Jul-11 05:52 qcistoqasm/qcis.py
 -rw-r--r--  2.0 unx     2216 b- defN 23-Jul-11 05:52 qcistoqasm/qcis_to_qasm.py
--rw-r--r--  2.0 unx      872 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      975 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/RECORD
-13 files, 65021 bytes uncompressed, 16066 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx      930 b- defN 23-Aug-07 08:08 ezQgd-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 08:08 ezQgd-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-Aug-07 08:08 ezQgd-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      975 b- defN 23-Aug-07 08:08 ezQgd-1.0.4.dist-info/RECORD
+13 files, 66676 bytes uncompressed, 16316 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: qcistoqasm/qcis.py
 Comment: 
 
 Filename: qcistoqasm/qcis_to_qasm.py
 Comment: 
 
-Filename: ezQgd-1.0.2.dist-info/METADATA
+Filename: ezQgd-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ezQgd-1.0.2.dist-info/WHEEL
+Filename: ezQgd-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ezQgd-1.0.2.dist-info/top_level.txt
+Filename: ezQgd-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ezQgd-1.0.2.dist-info/RECORD
+Filename: ezQgd-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ezQgd.py

```diff
@@ -1,904 +1,909 @@
-# -*- coding: utf-8 -*-
-import json
-import requests
-import re
-import os
-import shutil
-import traceback
-from time import time, sleep
-import random
-import datetime
-import numpy as np
-from qasmtoqcis.qasm_to_qcis import QasmToQcis
-from qcistoqasm.qcis_to_qasm import QcisToQasm
-from isqmap import transpile
-from sabreMapper.sabre_mapper import SabreMapper
-from typing import List, Optional, Dict, Union
-
-
-class Account():
-
-    def __init__(
-            self, 
-            login_key: Optional[str]=None, 
-            machine_name: Optional[str]=None
-        ):
-        """accout initialization
-
-        Args:
-            login_key: 
-                API Token under personal center on the web. Defaults to None.. Defaults to None.
-            machine_name: 
-                name of quantum computer. Defaults to None.
-
-        Raises:
-            Exception: throw an exception when login fails
-        """
-        self.qasmtoqcis = QasmToQcis()
-        self.qcistoqasm = QcisToQasm()
-        self.login_key = login_key
-        self.token = None
-        self.machine_name = machine_name
-        self.base_url = 'https://quantumctek-cloud.com/agency/'  # 生产环境url
-        self.base_login_url = 'https://quantumctek-cloud.com/api-uaa/oauth/token' # 生产环境登录url
-        self.login = self.log_in()
-        if self.login == 0:
-            raise Exception('登录失败')
-        else:
-            print('登录成功')
-
-    def log_in(self):
-        """
-        Authenticate username and password and return user credit
-
-        Returns
-            int: log in state, 1 means pass authentication, 0 means failed
-
-        """
-        data = {
-            'grant_type': 'openId',
-            'openId': self.login_key,
-            'account_type': 'member'
-        }
-        headers = {"Authorization": "Basic d2ViQXBwOndlYkFwcA=="}
-        res = requests.post(url=self.base_login_url, headers=headers, data=data)
-        status_code = res.status_code
-        if status_code != 200:
-            print('登录接口请求失败')
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code', -1)
-        msg = result.get('msg', '登录失败')
-        if code != 0:
-            print(f'登录失败：{msg}')
-            return 0
-        token = result.get('data').get('access_token')
-        self.token = token
-        return 1
-
-    def create_experiment(
-            self, 
-            exp_name: str, 
-            remark: Optional[str]="测试"
-        ):
-        """create a new experiment, the new one is the experiment set ID.
-
-        Args:
-            exp_name: new experiment collection Name.
-            remark: experimental remarks. Defaults to 测试.
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, success returns the experimental set id
-        """
-        url = f'{self.base_url}/service/sdk/api/experiment/save'
-        data = {"name": exp_name,
-                "remark": remark}
-        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-        res = requests.post(url, json=data, headers=headers)
-        status_code = res.status_code
-        if status_code != 200:
-            print(f'创建实验接口请求失败, code:{status_code}')
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code', -1)
-        msg = result.get('message', '创建实验失败')
-        if code != 0:
-            print(f'创建实验失败：{msg}')
-            return 0
-        lab_id = result.get('data').get('lab_id')
-        return lab_id
-
-    def save_experiment(
-            self, 
-            lab_id: str, 
-            exp_data: str, 
-            name: Optional[str]="detailtest", 
-            language: Optional[str]="qcis"
-        ):
-        """save the experiment and return the experiment ID.
-
-        Args:
-            lab_id: 
-                the result returned by the create_experiment interface, experimental set id
-            exp_data: 
-                experimental content, qics
-            name: experimental Details Name. Defaults to "detailtest".
-            language: Quantum computer language, including ['isq', 'quingo', 'qcis']. Defaults to "qcis".
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, success returns the experiment id.
-        """
-        language_list = ['isq', 'quingo', 'qcis']
-        if language not in language_list:
-            print(f'保存实验失败, 量子语言只能在{language_list}中选择')
-        exp_data = self.get_experiment_data(exp_data.upper())
-        url = self.base_url + '/service/sdk/api/experiment/detail/save'
-        data = {
-            "inputCode": exp_data, "lab_id": lab_id,
-            "languageCode": language, "name": name,
-            "source": "SDK", "computerCode": self.machine_name
-        }
-        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-        res = requests.post(url, json=data, headers=headers)
-        status_code = res.status_code
-        if status_code != 200:
-            print('保存实验接口请求失败')
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code', -1)
-        msg = result.get('message', '保存实验失败')
-        if code != 0:
-            print(f'保存实验失败：{msg}')
-            return 0
-        save_result = result.get('data').get('exp_id')
-        return save_result
-
-    def run_experiment(
-            self,
-            exp_id: str, 
-            num_shots: Optional[int]=12000,
-            is_verify: Optional[bool]=True
-        ):
-        """running the experiment returns the query result id.
-
-        Args:
-            exp_id: 
-                the result returned by the save_experiment interface, experimental id
-            num_shots: 
-                number of repetitions per experiment. Defaults to 12000.
-            is_verify:
-                Is the circuit verified.True verify, False do not verify. Defaults to True.
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, success returns the query id
-        """
-        data = {"exp_id": exp_id, "shots": num_shots, "is_verify": is_verify}
-        return self.handler_run_experiment_result(data)
-
-    def handler_run_experiment_result(
-            self, 
-            data
-        ):
-        url = self.base_url + '/service/sdk/api/experiment/temporary/save'
-        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-        res = requests.post(url, json=data, headers=headers)
-        status_code = res.status_code
-        if status_code != 200:
-            print('运行实验接口请求失败')
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code', -1)
-        msg = result.get('message', '运行实验失败')
-        if code != 0:
-            print(f'运行实验失败：{msg}')
-            return 0
-        run_result = result.get('data').get('query_ids')
-        return run_result
-
-    def submit_job(
-            self,
-            circuit: Optional[Union[List, str]]=None, 
-            exp_name: Optional[str]="exp0",
-            parameters: Optional[List[List]]=None, 
-            values: Optional[List[List]]=None,
-            num_shots: Optional[int]=12000,
-            lab_id: Optional[str]=None, 
-            exp_id: Optional[str]=None, 
-            version: Optional[str]="version01",
-            is_verify: Optional[bool]=True
-        ):
-        """submit experimental tasks
-
-        Args:
-            circuit: 
-                experimental content, qics. Defaults to None.
-            exp_name:
-                new experiment collection Name. Defaults to 'exp0'.
-            parameters: 
-                parameters that need to be assigned in the experimental content. Defaults to None.
-            values: 
-                The values corresponding to the parameters that need to be assigned in the experimental content. Defaults to None.
-            num_shots:
-                number of repetitions per experiment. Defaults to 12000.
-            lab_id: 
-                the result returned by the create_experiment interface, experimental set id. Defaults to None.
-            exp_id: 
-                the result returned by the save_experiment interface, experimental id. Defaults to None.
-            version: 
-                version description. Defaults to 'version01'.
-            is_verify:
-                Is the circuit verified.True verify, False do not verify. Defaults to True.
-
-            There are some parameter range limitations when using batch submission circiuts.
-                1. circuits length less than 50
-                   numshots maximum 100000
-                   the number of measurement qubits is less than 15
-                2. circuits length greater than 50 but less than 100
-                   numshots maximum 50000
-                   the number of measurement qubits is less than 30
-                3. circuits length greater than 100 but less than 300
-                   numshots maximum 10000
-                   the number of measurement bits is less than the number of all available qubits
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, success returns the query id.
-        """
-        if isinstance(circuit, str):
-            circuit = [circuit]
-        if len(circuit) > 1:
-            version = None
-        if circuit and parameters and values and len(parameters) == len(circuit) == len(values):
-            new_circuit = self.assign_parameters(circuit, parameters, values)
-            if not new_circuit:
-                print('无法为线路赋值，请检查线路，参数和参数值之后重试')
-                return 0
-        else:
-            new_circuit = circuit
-        data = {
-            "exp_id": exp_id,
-            "lab_id": lab_id,
-            "inputCode": new_circuit,
-            "languageCode": "qcis",
-            "name": exp_name,
-            "shots": num_shots,
-            "source": "SDK",
-            "computerCode": self.machine_name,
-            "experimentDetailName": version,
-            "is_verify": is_verify
-        }
-        return self.handler_run_experiment_result(data)
-
-    def query_experiment(
-            self,
-            query_id: Union[str, List[str]],
-            max_wait_time: Optional[int]=60
-        ):
-        """query experimental results
-
-        Args:
-            query_id: 
-                the result returned by the run_experiment interface, experimental set id
-            max_wait_time: 
-                maximum waiting time for querying experiments. Defaults to 60.
-
-            The maximum number of experimental result queries supported by the server is 50.
-            If there are more than 50, an error message will be displayed.
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, success returns the experimental result
-        """
-        if isinstance(query_id, str):
-            query_id = [query_id]
-        t0 = time()
-        while time()-t0 < max_wait_time:
-            try:
-                url = f'{self.base_url}/service/sdk/api/experiment/result/find/results'
-                headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-                data = {"query_ids": query_id}
-                res = requests.post(url, json=data, headers=headers)
-                status_code = res.status_code
-                if status_code != 200:
-                    print('查询接口请求失败')
-                    return 0
-                result = json.loads(res.text)
-                code = result.get('code', -1)
-                msg = result.get('message', '查询实验失败')
-                if code != 0:
-                    print(f'查询实验失败：{msg}')
-                query_exp = result.get('data').get('experimentResultModelList')
-                if query_exp:
-                    return query_exp
-            except:
-                continue
-            sleep_time = random.randint(
-                0, 15)*0.3+round(random.uniform(0, 1.5), 2)
-            print(f'查询实验结果请等待: {{:.2f}}秒'.format(sleep_time))
-            sleep(sleep_time)
-        print(f'查询实验结果失败')
-        return 0
-
-    def assign_parameters(
-            self,
-            circuits: List[str], 
-            parameters: List[List], 
-            values: List[List]
-        ):
-        """Check if the number of parameters, values match the circuit definition
-
-        Args:
-            circuit: 
-                string, QCIS circuit definition with or without parameter place holder
-            parameters: 
-                list or ndarray of strings, parameters to be filled
-            values: 
-                list or ndarray of floats, values to be assigned
-
-        Returns:
-            circuit: circuit with parameters replaced by values or empty string
-            empty string occurs when errors prevents parameters to be assigned
-        """
-        new_circuit = []
-        for circuit, parameter, value in zip(circuits, parameters, values):
-            circuit = circuit.upper()
-            p = re.compile(r'\{(\w+)\}')
-            circuit_parameters = p.findall(circuit)
-            if circuit_parameters:
-                # # 如果values为整数或浮点数，改为列表格式##########################################################
-                # if isinstance(values, (float, int)):
-                #     values = [values]
-                # # 如果parameters为字符格式，改为列表格式#########################################################
-                # if isinstance(parameters, str):
-                #     parameters = [parameters]
-                
-                # 将所有parameter变为大写， 否则set(parameters) != set(circuit_parameters) 不通过 ###############
-                parameters = [p.upper() for p in parameter]
-
-                if not value:
-                    error_message = f'线路含有参数{circuit_parameters}, 请提供相应的参数值'
-                    print(error_message)
-                    return ''
-
-                else:
-                    if len(circuit_parameters) != len(value):
-                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(value)}个参数值'
-                        print(error_message)
-                        return ''
-
-                    elif parameter and len(circuit_parameters) != len(parameter):
-                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(parameter)}个参数'
-                        print(error_message)
-                        return ''
-                    
-                    elif set(parameter) != set(circuit_parameters):
-                        error_message = '线路中的参数与您输入的参数名称不符'
-                        print(error_message)
-                    else:
-                        param_dic = {}
-                        ############################# 这个转化可以删了 #########################################
-                        #parameters_upper = [p.upper() for p in parameters]
-                        for p, v in zip(parameter, value):
-                            param_dic[p] = v
-                        expData = circuit.format(**param_dic)
-                        new_circuit.append(expData)
-            elif parameter or value:
-                error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
-                print(error_message)
-                return ''
-            else:
-                expData = circuit
-                new_circuit.append(expData)
-        return new_circuit
-
-    def get_experiment_data(
-            self, 
-            circuit: str
-        ):
-        """Parse circuit description and generate 
-           experiment script and extract number of measured qubits.
-
-        Args:
-            circuit: 
-                string, QCIS circuit
-
-        Returns:
-            expData: 
-                string, transformed circuit
-        """
-        # get gates from circuit
-        gates_list = circuit.split('\n')
-        gates_list_strip = [g.strip() for g in gates_list if g]
-        gates_list_strip = [g for g in gates_list_strip if g]
-
-        # transform circuit from QCIS to expData
-        expData = '\n'.join(gates_list_strip)
-        return expData
-
-    def set_machine(
-            self, 
-            machine_name: str
-        ):
-        """set the machine name.
-
-        Args:
-            machine_name: name of quantum computer.
-        """
-        self.machine_name = machine_name
-
-    def download_config(
-            self, 
-            down_file: Optional[bool]=True
-        ):
-        """download experimental parameters.
-
-        Args:
-            down_file: 
-                the parameter is True to write to the file, and False to directly return the experimental parameters. Defaults to True.
-
-        Returns:
-           Union[int, str]: 0 failed, not 0 successful, success returns the experimental parameters.
-        """
-        url = f'{self.base_url}/service/sdk/api/experiment/download/config/{self.machine_name}'
-        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-        res = requests.get(url, headers=headers)
-        status_code = res.status_code
-        if status_code != 200:
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code')
-        if code != 0:
-            msg = result.get('msg', '下载实验参数失败')
-            print(f'下载实验参数失败:{msg}')
-            return 0
-        data = result.get('data')
-        cur_time = self.current_time()
-        if down_file:
-            with open(f'./{self.machine_name}_config_param_{cur_time}.json', 'w') as f:
-                f.write(json.dumps(data))
-        return data
-
-    def convert_qasm_to_qcis(
-            self, 
-            qasm: str, 
-            qubit_map: Optional[Dict]=None
-        ):
-        """convert qasm to qcis.
-
-        Args:
-            qasm: 
-                qasm.
-            qubit_map: 
-                Number mapping in qasm, where the value is None, 
-                directly maps bits based on the format of number plus 1. Defaults to None.
-        Raises:
-            Exception: language conversion failed.
-
-        Returns:
-            str: simplified qcis.
-        """
-        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis(qasm, qubit_map=qubit_map)
-        simplity_qcis = self.qasmtoqcis.simplify(qcis_raw)
-        return simplity_qcis
-
-    def convert_qasm_to_qcis_from_file(
-            self, 
-            qasm_file: str, 
-            qubit_map: Optional[Dict]=None
-        ):
-        """Read qasm from file and convert it to qcis
-
-        Args:
-            qasm_file: 
-                qasm file.
-            qubit_map: 
-                Number mapping in qasm, where the value is None, 
-                directly maps bits based on the format of number plus 1. Defaults to None.
-
-        Raises:
-            Exception: language conversion failed.
-
-        Returns:
-            str: simplified qcis.
-        """
-        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis_from_file(qasm_file, qubit_map=qubit_map)
-        simplity_qcis = self.qasmtoqcis.simplify(qcis_raw)
-        return simplity_qcis
-    
-    def convert_qcis_to_qasm(
-            self, 
-            qcis: str
-        ):
-        """convert qcis to qasm.
-
-        Args:
-            qcis: qcis
-
-        Returns:
-            str: converted qasm.
-        """
-        qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis)
-        return qasm_circuit
-
-    def qcis_check_regular(
-            self, 
-            qcis_raw: str
-        ):
-        """qcis regular check,normal returns 1, abnormal returns 0
-
-        Args:
-            qcis_raw: qcis
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, successfully returned the input qics.
-        """
-        url = f'{self.base_url}service/sdk/api/experiment/qcis/rule/verify'
-        data = {
-            "computerCode": self.machine_name,
-            "qcis": qcis_raw
-        }
-        res = requests.post(url, json=data)
-        status_code = res.status_code
-        if status_code != 200:
-            print(f'qcis检验失败, code:{status_code}')
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code', -1)
-        msg = result.get('message', 'qcis检验失败')
-        if code != 0:
-            print(f'qcis检验失败: {msg}')
-            return 0
-        return qcis_raw
-
-    def simplify(
-            self, 
-            qcis_raw: str
-        ):
-        """simplification of qcis lines.
-
-        Args:
-            qcis_raw: qcis
-
-        Returns:
-            str: simplified qcis.
-        """
-        new_qcis_raw = self.qcis_check_regular(qcis_raw)
-        simplity_qcis = self.qasmtoqcis.simplify(new_qcis_raw)
-        return simplity_qcis
-    
-    def current_time(self):
-        """get the current time
-
-        Returns:
-            str: time string
-        """
-        timestamp = datetime.datetime.fromtimestamp(time())
-        str_time = timestamp.strftime('%Y%m%d%H%M%S')
-        return str_time
-
-    def readout_data_to_state_probabilities(
-            self, 
-            result
-        ):
-        state01 = result.get('resultStatus')
-        basis_list = []
-        basis_content = ''.join([''.join([str(s) for s in state]) for state in state01[1:]])
-        qubits_num = len(state01[0])  # 测量比特个数
-        for idx in range(qubits_num):
-            basis_result = basis_content[idx: len(basis_content): qubits_num]
-            basis_list.append([True if res == "1" else False for res in basis_result])
-        return basis_list
-
-    # 读取数据转换成量子态概率
-    def readout_data_to_state_probabilities_whole(
-            self, 
-            result: Dict
-        ):
-        """read data and convert it into a quantum state probability, all returns.
-
-        Args:
-            result: the results returned after query_experiment.
-
-        Returns:
-            Dict: probability
-        """
-        basis_list = self.readout_data_to_state_probabilities(result)
-        probabilities = self.original_onversion_whole(basis_list)
-        return probabilities
-    
-    def readout_data_to_state_probabilities_part(
-            self, 
-            result: Dict
-        ):
-        """read data and convert it into a quantum state probability, do not return with a probability of 0.
-
-        Args:
-            result: the results returned after query_experiment.
-
-        Returns:
-            Dict: probability
-        """
-        basis_list = self.readout_data_to_state_probabilities(result)
-        probabilities = self.original_onversion_part(basis_list)
-        return probabilities
-    
-    def original_onversion_whole(
-            self, 
-            state01
-        ):
-        #当state01为一维时转换成二维数据
-        if isinstance(state01[0], bool):
-            state01=[state01]
-        n = len(state01)  # 读取比特数
-        # 测量比特概率限制
-        # if n > MAX_QUBIT_NUM:
-        #     print(f'Number of qubits > {MAX_QUBIT_NUM}, cannot calculate probabilities.')
-        counts = [0] * (2 ** n)
-        state01_T = np.transpose(state01)  # 转置
-        numShots = len(state01_T)  # 测量重复次数
-        # 统计所有numShots 列
-        for num in range(numShots):
-            k = 0
-            for i in range(n):
-                k += state01_T[num][i] * (2 ** i)
-            counts[k] += 1
-        # 计算概率
-        # P=[counts[k]/numShots for k in range(2**n)]
-        P = {bin(k)[2:].zfill(n): counts[k]/numShots for k in range(2**n)}
-        return P
-    
-    def original_onversion_part(
-            self, 
-            state01
-        ):
-        #当state01为一维时转换成二维数据
-        if isinstance(state01[0], bool):
-            state01=[state01]
-        n = len(state01)  # 读取比特数
-        # 测量比特概率限制
-        # if n > MAX_QUBIT_NUM:
-        #     raise Exception(f'Number of qubits > {MAX_QUBIT_NUM}, cannot calculate probabilities.')
-        counts = {}
-        state01_T = np.transpose(state01)  # 转置
-        numShots = len(state01_T)  # 测量重复次数
-        # 统计所有numShots 列
-        for num in range(numShots):
-            k = 0
-            for i in range(n):
-                k += state01_T[num][i] * (2 ** i)
-            prob_state = bin(k)[2:].zfill(n)
-            if prob_state not in counts:
-                counts[prob_state] = 1
-            else:
-                counts[prob_state] += 1
-        # 计算概率
-        # P=[counts[k]/numShots for k in range(2**n)]
-        P = {k: v/numShots for k, v in counts.items()}
-        return P
-    
-    # 量子态概率矫正
-    def probability_calibration(
-            self, 
-            result: Dict, 
-            config_json: Optional[Dict]=None):
-        """correction of the measured probability of 01 quantum state.
-
-        Args:
-            result:
-                the results returned after query_experiment.
-            config_json: 
-                experimental parameters of quantum computer. 
-                config_json value is None, read the latest experimental parameters for calculation.
-                Defaults to None.
-
-        Raises:
-            Exception: cannot calibrate probability with fidelity.
-
-        Returns:
-            Dict: corrected probability.
-        """
-        CM_CACHE = {}
-        if config_json is None:
-            config_json = self.download_config(down_file=False)
-        qubit_num = [f'Q{i}' for i in result.get('resultStatus')[0]]
-        n = len(qubit_num)  # 测量比特个数
-        qubits = config_json['readout']['readoutArray']['|0> readout fidelity']['qubit_used']
-        readout_fidelity0 = config_json['readout']['readoutArray']['|0> readout fidelity']['param_list']
-        readout_fidelity1 = config_json['readout']['readoutArray']['|1> readout fidelity']['param_list']
-        iq2probFidelity = [[readout_fidelity0[qubits.index(q)], readout_fidelity1[qubits.index(q)]] for q in qubit_num]
-        P = self.readout_data_to_state_probabilities_whole(result)
-        Pm = list(P.values())
-        if not isinstance(iq2probFidelity[0], list):
-            iq2probFidelity=[iq2probFidelity]
-        f = tuple([float(fi) for fi in sum(iq2probFidelity, [])])
-        if f not in CM_CACHE:
-            inv_CM = 1
-            for k in iq2probFidelity[::-1]:
-                F00 = k[0]
-                F11 = k[1]
-                if F00 + F11 == 1:
-                    raise Exception(f'Cannot calibrate probability with fidelity: [{F00}, {F11}]')
-                inv_cm = np.array([[F11, F11 - 1], [F00 - 1, F00]]) / (F00 + F11 - 1)
-                inv_CM = np.kron(inv_CM, inv_cm)
-            CM_CACHE[f] = inv_CM
-        else:
-            inv_CM = CM_CACHE[f]
-        Pi = np.dot(inv_CM, (np.array(Pm, ndmin=2).T))
-        Pi = {bin(idx)[2:].zfill(n): k[0] for idx, k in enumerate(Pi)}
-        return Pi
-    
-    # 对矫正后的概率进行修正
-    def probability_correction(self, probabilities):
-        """correction of the measured probability of 01 quantum state.
-           If there is a probability greater than 1, change this item to 1; 
-           If there is anything less than 0, change the item to 0.
-
-        Args:
-            probabilities:
-               corrected probability.
-            
-        Returns:
-            Dict: corrected probability.
-        """
-        abnormal_fidelity_list = list(filter(lambda x: x < 0 or x > 1, probabilities.values()))
-        if not abnormal_fidelity_list:
-            return probabilities
-        for k, v in probabilities.items():
-            if v > 1:
-                probabilities[k] = 1
-            elif v < 0:
-                probabilities[k] = 0
-        fidelity_sum = sum(probabilities.values())
-        for k, v in probabilities.items():
-            probabilities[k] = v / fidelity_sum
-        return probabilities
-    
-    def qcis_mapping_isq(
-            self, 
-            qcis_circuit: str, 
-            initial_layout: Optional[Dict]=None,
-            objective: Optional[str]='size', 
-            seed: Optional[int]=None, 
-            use_post_opt: Optional[bool]=False
-        ):
-        """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
-           and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
-           described by the coupling_map, in the meanwhile reduces circuit depth.
-
-        Args:
-            qcis_circuit: qcis circuit
-            initial_layout: 
-                Initial position of virtual qubits on physical qubits.
-                If given, this is the initial state in search of virtual to physical qubit mapping
-                e.g.:
-                    {0:4, 1:1, 2:5, 3:2, 4:0, 5:3}. Defaults to None.
-            objective: 
-                size: min. # of added swaps
-                depth: min. depth
-                no_swap: try best to find an initial mapping requiring no swaps; raise 
-                an error if fail. Defaults to 'size'.
-            seed: 
-                Set random seed for the stochastic part of the tranpiler. Defaults to None.
-            use_post_opt: 
-                we provide a genetic alg. which utilizes exchange rules for
-                swaps to futher min. depth. Defaults to False.
-
-        raised:
-            TranspileError:
-                if graph specified by coupling map is disconnected.
-
-        Returns:
-            str: qcis string after transpilation
-        """
-        config_json = self.download_config(down_file=False)
-        try:
-            qasm_circuit = self.convert_qcis_to_qasm(qcis_circuit)
-            cur_time = self.current_time()
-            qpu_file = f'./{self.machine_name}_config_param_{cur_time}.json'
-            with open(qpu_file, 'w') as f:
-                f.write(json.dumps(config_json))
-            qasm_transpiled, _, _, _ = transpile(qasm_circuit,
-                                                qpu_file, 
-                                                initial_layout=initial_layout,
-                                                objective=objective,
-                                                seed=seed,
-                                                use_post_opt=use_post_opt)
-            simplity_qcis = self.convert_qasm_to_qcis(qasm_transpiled)
-            os.remove(qpu_file)
-            return simplity_qcis
-        except Exception as e:
-            print(e)
-            print(traceback.format_exc())
-            print('circuit mapping error, will submit using the original route')
-            os.remove(qpu_file)
-            return qcis_circuit
-    
-    def qcis_mapping_sabre(
-            self, 
-            qcis_circuit: str):
-        """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
-           and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
-           described by the coupling_map, in the meanwhile reduces circuit depth.
-
-        Args:
-            qcis_circuit: qcis circuit
-
-        Returns:
-            str : qcis after mapping
-        """       
-        config_json = self.download_config(down_file=False)
-        try:
-            # qcis转换成qasm并写入qasm_file中
-            qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis_circuit)
-            folder_path = 'temp'
-            if not os.path.exists(folder_path):
-                os.makedirs(folder_path)
-            qasm_file = f'{folder_path}/qasm.qasm'
-            with open(qasm_file, 'w') as f:
-                f.write(qasm_circuit)
-            sabre = SabreMapper()
-            # 组装chip_info_fn映射信息
-            chip_info_fn = {}
-            couplings = []
-            coupler_maps = config_json.get('overview').get('coupler_map')
-            coupler_used = config_json.get('twoQubitGate').get('czGate').get('gate error').get('qubit_used')
-            cz_gate_error = config_json.get('twoQubitGate').get('czGate').get('gate error').get('param_list')
-            for coupler, error in zip(coupler_used, cz_gate_error):
-                fidelity = 1- error
-                coupler_qubit_map = coupler_maps.get(coupler)
-                couplings.append({"fidelity": fidelity, "qubit pair": coupler_qubit_map})
-            chip_info_fn['couplings'] = couplings
-            qubit_used = config_json.get('qubit').get('singleQubit').get('gate error').get('qubit_used')
-            qubit_gate_error = config_json.get('qubit').get('singleQubit').get('gate error').get('param_list')
-            qubit_fidelity = {}
-            for qubit, error in zip(qubit_used, qubit_gate_error):
-                qubit_fidelity[qubit] = 1 - error
-            chip_info_fn['fidelity'] = qubit_fidelity
-            chip_info_fn['has multiple chips'] = False
-            chip_info_fn['qubits'] = qubit_used
-
-            chip_info_fn_file = f'{folder_path}/chip_info_fn.json'
-            mapped_qasm_fn_file = f'{folder_path}/mapped_qasm_fn.qasm'
-            qubit_mapping_fn_file = f'{folder_path}/qubit_mapping_fn.json'
-            with open(chip_info_fn_file, 'w') as f:
-                json.dump(chip_info_fn, f)
-            # 调用quMapper做mapping操作
-            success = sabre.map_schedule(qasm_file, chip_info_fn_file, mapped_qasm_fn_file, qubit_mapping_fn_file)
-            if success:
-                with open(qubit_mapping_fn_file, 'r') as f:
-                    qubit_mapping_fn = json.load(f)
-                qubit_map = qubit_mapping_fn.get('physical qubits idx')
-                # mapping成功，将转换后的qasm转为qcis，其中编号根据physical qubits idx做映射
-                simplity_qcis = self.convert_qasm_to_qcis_from_file(mapped_qasm_fn_file, qubit_map)
-                shutil.rmtree(folder_path)
-                return simplity_qcis
-        except Exception as e:
-            print(e)
-            print(traceback.format_exc())
-            print('circuit mapping error, will submit using the original route')
-            shutil.rmtree(folder_path)
-            return qcis_circuit
-
-    def get_experiment_circuit(
-            self,
-            exp_id: str):
-        """according to the exp_id obtained experimental circuit
-
-        Args:
-            exp_id: the result returned by the save_experiment interface, experimental id.
-
-        Returns:
-            Union[int, str]: 0 failed, not 0 successful, success returns the experimental circuit
-        """
-        url = f'{self.base_url}service/sdk/api/experiment/getQcis/by/{exp_id}'
-        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-        res = requests.get(url, headers=headers)
-        status_code = res.status_code
-        if status_code != 200:
-            return 0
-        result = json.loads(res.text)
-        code = result.get('code', -1)
-        msg = result.get('msg', '查询实验线路失败')
-        if code != 0:
-            print(f'查询实验线路: {msg}')
-            return 0
-        circuit = result.get('data').get('qcis')
+# -*- coding: utf-8 -*-
+import json
+import requests
+import re
+import os
+import shutil
+import traceback
+from time import time, sleep
+import random
+import datetime
+import numpy as np
+from qasm_to_qcis.qasm_to_qcis import QasmToQcis
+from qcis_to_qasm.qcis_to_qasm import QcisToQasm
+from isqmap import transpile
+from sabreMapper.sabre_mapper import SabreMapper
+from typing import List, Optional, Dict, Union
+
+
+class Account():
+
+    def __init__(
+            self, 
+            login_key: Optional[str]=None, 
+            machine_name: Optional[str]=None
+        ):
+        """accout initialization
+
+        Args:
+            login_key: 
+                API Token under personal center on the web. Defaults to None.. Defaults to None.
+            machine_name: 
+                name of quantum computer. Defaults to None.
+
+        Raises:
+            Exception: throw an exception when login fails
+        """
+        self.qasmtoqcis = QasmToQcis()
+        self.qcistoqasm = QcisToQasm()
+        self.login_key = login_key
+        self.token = None
+        self.machine_name = machine_name
+        self.base_url = 'https://quantumctek-cloud.com/agency/'  # 生产环境url
+        self.base_login_url = 'https://quantumctek-cloud.com/api-uaa/oauth/token' # 生产环境登录url
+        self.login = self.log_in()
+        if self.login == 0:
+            raise Exception('登录失败')
+        else:
+            print('登录成功')
+
+    def log_in(self):
+        """
+        Authenticate username and password and return user credit
+
+        Returns
+            int: log in state, 1 means pass authentication, 0 means failed
+
+        """
+        data = {
+            'grant_type': 'openId',
+            'openId': self.login_key,
+            'account_type': 'member'
+        }
+        headers = {"Authorization": "Basic d2ViQXBwOndlYkFwcA=="}
+        res = requests.post(url=self.base_login_url, headers=headers, data=data)
+        status_code = res.status_code
+        if status_code != 200:
+            print('登录接口请求失败')
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('msg', '登录失败')
+        if code != 0:
+            print(f'登录失败：{msg}')
+            return 0
+        token = result.get('data').get('access_token')
+        self.token = token
+        return 1
+
+    def create_experiment(
+            self, 
+            exp_name: str, 
+            remark: Optional[str]="测试"
+        ):
+        """create a new experiment, the new one is the experiment set ID.
+
+        Args:
+            exp_name: new experiment collection Name.
+            remark: experimental remarks. Defaults to 测试.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the experimental set id
+        """
+        url = f'{self.base_url}/service/sdk/api/experiment/save'
+        data = {"name": exp_name,
+                "remark": remark}
+        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+        res = requests.post(url, json=data, headers=headers)
+        status_code = res.status_code
+        if status_code != 200:
+            print(f'创建实验接口请求失败, code:{status_code}')
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('message', '创建实验失败')
+        if code != 0:
+            print(f'创建实验失败：{msg}')
+            return 0
+        lab_id = result.get('data').get('lab_id')
+        return lab_id
+
+    def save_experiment(
+            self, 
+            lab_id: str, 
+            exp_data: str, 
+            name: Optional[str]="detailtest", 
+            language: Optional[str]="qcis"
+        ):
+        """save the experiment and return the experiment ID.
+
+        Args:
+            lab_id: 
+                the result returned by the create_experiment interface, experimental set id
+            exp_data: 
+                experimental content, qics
+            name: experimental Details Name. Defaults to "detailtest".
+            language: Quantum computer language, including ['isq', 'quingo', 'qcis']. Defaults to "qcis".
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the experiment id.
+        """
+        language_list = ['isq', 'quingo', 'qcis']
+        if language not in language_list:
+            print(f'保存实验失败, 量子语言只能在{language_list}中选择')
+        exp_data = self.get_experiment_data(exp_data.upper())
+        url = self.base_url + '/service/sdk/api/experiment/detail/save'
+        data = {
+            "inputCode": exp_data, "lab_id": lab_id,
+            "languageCode": language, "name": name,
+            "source": "SDK", "computerCode": self.machine_name
+        }
+        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+        res = requests.post(url, json=data, headers=headers)
+        status_code = res.status_code
+        if status_code != 200:
+            print('保存实验接口请求失败')
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('message', '保存实验失败')
+        if code != 0:
+            print(f'保存实验失败：{msg}')
+            return 0
+        save_result = result.get('data').get('exp_id')
+        return save_result
+
+    def run_experiment(
+            self,
+            exp_id: str, 
+            num_shots: Optional[int]=12000,
+            is_verify: Optional[bool]=True
+        ):
+        """running the experiment returns the query result id.
+
+        Args:
+            exp_id: 
+                the result returned by the save_experiment interface, experimental id
+            num_shots: 
+                number of repetitions per experiment. Defaults to 12000.
+            is_verify:
+                Is the circuit verified.True verify, False do not verify. Defaults to True.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the query id
+        """
+        data = {"exp_id": exp_id, "shots": num_shots, "is_verify": is_verify}
+        return self.handler_run_experiment_result(data)
+
+    def handler_run_experiment_result(
+            self, 
+            data
+        ):
+        url = self.base_url + '/service/sdk/api/experiment/temporary/save'
+        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+        res = requests.post(url, json=data, headers=headers)
+        status_code = res.status_code
+        if status_code != 200:
+            print('运行实验接口请求失败')
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('message', '运行实验失败')
+        if code != 0:
+            print(f'运行实验失败：{msg}')
+            return 0
+        run_result = result.get('data').get('query_ids')
+        return run_result
+
+    def submit_job(
+            self,
+            circuit: Optional[Union[List, str]]=None, 
+            exp_name: Optional[str]="exp0",
+            parameters: Optional[List[List]]=None, 
+            values: Optional[List[List]]=None,
+            num_shots: Optional[int]=12000,
+            lab_id: Optional[str]=None, 
+            exp_id: Optional[str]=None, 
+            version: Optional[str]="version01",
+            is_verify: Optional[bool]=True
+        ):
+        """submit experimental tasks
+
+        Args:
+            circuit: 
+                experimental content, qics. Defaults to None.
+            exp_name:
+                new experiment collection Name. Defaults to 'exp0'.
+            parameters: 
+                parameters that need to be assigned in the experimental content. Defaults to None.
+            values: 
+                The values corresponding to the parameters that need to be assigned in the experimental content. Defaults to None.
+            num_shots:
+                number of repetitions per experiment. Defaults to 12000.
+            lab_id: 
+                the result returned by the create_experiment interface, experimental set id. Defaults to None.
+            exp_id: 
+                the result returned by the save_experiment interface, experimental id. Defaults to None.
+            version: 
+                version description. Defaults to 'version01'.
+            is_verify:
+                Is the circuit verified.True verify, False do not verify. Defaults to True.
+        description:
+                There are some parameter range limitations when using batch submission circiuts.
+                1. circuits length less than 50
+                   numshots maximum 100000
+                   the number of measurement qubits is less than 15
+                2. circuits length greater than 50 but less than 100
+                   numshots maximum 50000
+                   the number of measurement qubits is less than 30
+                3. circuits length greater than 100 but less than 600
+                   numshots maximum 10000
+                   the number of measurement bits is less than the number of all available qubits
+                4. When the circuit is none, the exp_id cannot be none and the lab_id needs to be none,
+                5. When the circuit is not none, when the circuit is multiple lines, the version and exp_id need to be none,
+                   and the line will be saved under the default collection if the lab_id or exp_name is not transmitted.
+                6. When the circuit is not none, when the circuit is a single line, exp_id need none,
+                   version does not transmit to generate the default, lab_id or exp_name does not transmit the line is saved under the default collection.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the query id.
+        """
+        if isinstance(circuit, str):
+            circuit = [circuit]
+        if len(circuit) > 1:
+            version = None
+        if circuit and parameters and values and len(parameters) == len(circuit) == len(values):
+            new_circuit = self.assign_parameters(circuit, parameters, values)
+            if not new_circuit:
+                print('无法为线路赋值，请检查线路，参数和参数值之后重试')
+                return 0
+        else:
+            new_circuit = circuit
+        data = {
+            "exp_id": exp_id,
+            "lab_id": lab_id,
+            "inputCode": new_circuit,
+            "languageCode": "qcis",
+            "name": exp_name,
+            "shots": num_shots,
+            "source": "SDK",
+            "computerCode": self.machine_name,
+            "experimentDetailName": version,
+            "is_verify": is_verify
+        }
+        return self.handler_run_experiment_result(data)
+
+    def query_experiment(
+            self,
+            query_id: Union[str, List[str]],
+            max_wait_time: Optional[int]=60
+        ):
+        """query experimental results
+
+        Args:
+            query_id: 
+                the result returned by the run_experiment interface, experimental set id
+            max_wait_time: 
+                maximum waiting time for querying experiments. Defaults to 60.
+        description:
+            The maximum number of experimental result queries supported by the server is 50.
+            If there are more than 50, an error message will be displayed.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the experimental result
+        """
+        if isinstance(query_id, str):
+            query_id = [query_id]
+        t0 = time()
+        while time()-t0 < max_wait_time:
+            try:
+                url = f'{self.base_url}/service/sdk/api/experiment/result/find/results'
+                headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+                data = {"query_ids": query_id}
+                res = requests.post(url, json=data, headers=headers)
+                status_code = res.status_code
+                if status_code != 200:
+                    print('查询接口请求失败')
+                    return 0
+                result = json.loads(res.text)
+                code = result.get('code', -1)
+                msg = result.get('message', '查询实验失败')
+                if code != 0:
+                    print(f'查询实验失败：{msg}')
+                query_exp = result.get('data').get('experimentResultModelList')
+                if query_exp:
+                    return query_exp
+            except:
+                continue
+            sleep_time = random.randint(
+                0, 15)*0.3+round(random.uniform(0, 1.5), 2)
+            print(f'查询实验结果请等待: {{:.2f}}秒'.format(sleep_time))
+            sleep(sleep_time)
+        print(f'查询实验结果失败')
+        return 0
+
+    def assign_parameters(
+            self,
+            circuits: List[str], 
+            parameters: List[List], 
+            values: List[List]
+        ):
+        """Check if the number of parameters, values match the circuit definition
+
+        Args:
+            circuits:
+                string, QCIS circuit definition with or without parameter place holder
+            parameters: 
+                list or ndarray of strings, parameters to be filled
+            values: 
+                list or ndarray of floats, values to be assigned
+
+        Returns:
+            circuit: circuit with parameters replaced by values or empty string
+            empty string occurs when errors prevents parameters to be assigned
+        """
+        new_circuit = []
+        for circuit, parameter, value in zip(circuits, parameters, values):
+            circuit = circuit.upper()
+            p = re.compile(r'\{(\w+)\}')
+            circuit_parameters = p.findall(circuit)
+            if circuit_parameters:
+                # # 如果values为整数或浮点数，改为列表格式##########################################################
+                # if isinstance(values, (float, int)):
+                #     values = [values]
+                # # 如果parameters为字符格式，改为列表格式#########################################################
+                # if isinstance(parameters, str):
+                #     parameters = [parameters]
+                
+                # 将所有parameter变为大写， 否则set(parameters) != set(circuit_parameters) 不通过 ###############
+                after_parameter = [p.upper() for p in parameter]
+
+                if not value:
+                    error_message = f'线路含有参数{circuit_parameters}, 请提供相应的参数值'
+                    print(error_message)
+                    return ''
+
+                else:
+                    if len(circuit_parameters) != len(value):
+                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(value)}个参数值'
+                        print(error_message)
+                        return ''
+
+                    elif after_parameter and len(circuit_parameters) != len(after_parameter):
+                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(after_parameter)}个参数'
+                        print(error_message)
+                        return ''
+                    
+                    elif set(after_parameter) != set(circuit_parameters):
+                        error_message = '线路中的参数与您输入的参数名称不符'
+                        print(error_message)
+                    else:
+                        param_dic = {}
+                        ############################# 这个转化可以删了 #########################################
+                        #parameters_upper = [p.upper() for p in parameters]
+                        for p, v in zip(after_parameter, value):
+                            param_dic[p] = v
+                        expData = circuit.format(**param_dic)
+                        new_circuit.append(expData)
+            elif parameter or value:
+                error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
+                print(error_message)
+                return ''
+            else:
+                expData = circuit
+                new_circuit.append(expData)
+        return new_circuit
+
+    def get_experiment_data(
+            self, 
+            circuit: str
+        ):
+        """Parse circuit description and generate 
+           experiment script and extract number of measured qubits.
+
+        Args:
+            circuit: 
+                string, QCIS circuit
+
+        Returns:
+            expData: 
+                string, transformed circuit
+        """
+        # get gates from circuit
+        gates_list = circuit.split('\n')
+        gates_list_strip = [g.strip() for g in gates_list if g]
+        gates_list_strip = [g for g in gates_list_strip if g]
+
+        # transform circuit from QCIS to expData
+        expData = '\n'.join(gates_list_strip)
+        return expData
+
+    def set_machine(
+            self, 
+            machine_name: str
+        ):
+        """set the machine name.
+
+        Args:
+            machine_name: name of quantum computer.
+        """
+        self.machine_name = machine_name
+
+    def download_config(
+            self, 
+            down_file: Optional[bool]=True
+        ):
+        """download experimental parameters.
+
+        Args:
+            down_file: 
+                the parameter is True to write to the file, and False to directly return the experimental parameters. Defaults to True.
+
+        Returns:
+           Union[int, str]: 0 failed, not 0 successful, success returns the experimental parameters.
+        """
+        url = f'{self.base_url}/service/sdk/api/experiment/download/config/{self.machine_name}'
+        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+        res = requests.get(url, headers=headers)
+        status_code = res.status_code
+        if status_code != 200:
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code')
+        if code != 0:
+            msg = result.get('msg', '下载实验参数失败')
+            print(f'下载实验参数失败:{msg}')
+            return 0
+        data = result.get('data')
+        cur_time = self.current_time()
+        if down_file:
+            with open(f'./{self.machine_name}_config_param_{cur_time}.json', 'w') as f:
+                f.write(json.dumps(data))
+        return data
+
+    def convert_qasm_to_qcis(
+            self, 
+            qasm: str, 
+            qubit_map: Optional[Dict]=None
+        ):
+        """convert qasm to qcis.
+
+        Args:
+            qasm: 
+                qasm.
+            qubit_map: 
+                Number mapping in qasm, where the value is None, 
+                directly maps bits based on the format of number plus 1. Defaults to None.
+        Raises:
+            Exception: language conversion failed.
+
+        Returns:
+            str: simplified qcis.
+        """
+        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis(qasm, qubit_map=qubit_map)
+        simplity_qcis = self.qasmtoqcis.simplify(qcis_raw)
+        return simplity_qcis
+
+    def convert_qasm_to_qcis_from_file(
+            self, 
+            qasm_file: str, 
+            qubit_map: Optional[Dict]=None
+        ):
+        """Read qasm from file and convert it to qcis
+
+        Args:
+            qasm_file: 
+                qasm file.
+            qubit_map: 
+                Number mapping in qasm, where the value is None, 
+                directly maps bits based on the format of number plus 1. Defaults to None.
+
+        Raises:
+            Exception: language conversion failed.
+
+        Returns:
+            str: simplified qcis.
+        """
+        qcis_raw = self.qasmtoqcis.convert_qasm_to_qcis_from_file(qasm_file, qubit_map=qubit_map)
+        simplity_qcis = self.qasmtoqcis.simplify(qcis_raw)
+        return simplity_qcis
+    
+    def convert_qcis_to_qasm(
+            self, 
+            qcis: str
+        ):
+        """convert qcis to qasm.
+
+        Args:
+            qcis: qcis
+
+        Returns:
+            str: converted qasm.
+        """
+        qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis)
+        return qasm_circuit
+
+    def qcis_check_regular(
+            self, 
+            qcis_raw: str
+        ):
+        """qcis regular check,normal returns 1, abnormal returns 0
+
+        Args:
+            qcis_raw: qcis
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, successfully returned the input qics.
+        """
+        url = f'{self.base_url}service/sdk/api/experiment/qcis/rule/verify'
+        data = {
+            "computerCode": self.machine_name,
+            "qcis": qcis_raw
+        }
+        res = requests.post(url, json=data)
+        status_code = res.status_code
+        if status_code != 200:
+            print(f'qcis检验失败, code:{status_code}')
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('message', 'qcis检验失败')
+        if code != 0:
+            print(f'qcis检验失败: {msg}')
+            return 0
+        return qcis_raw
+
+    def simplify(
+            self, 
+            qcis_raw: str
+        ):
+        """simplification of qcis lines.
+
+        Args:
+            qcis_raw: qcis
+
+        Returns:
+            str: simplified qcis.
+        """
+        new_qcis_raw = self.qcis_check_regular(qcis_raw)
+        simplity_qcis = self.qasmtoqcis.simplify(new_qcis_raw)
+        return simplity_qcis
+    
+    def current_time(self):
+        """get the current time
+
+        Returns:
+            str: time string
+        """
+        timestamp = datetime.datetime.fromtimestamp(time())
+        str_time = timestamp.strftime('%Y%m%d%H%M%S')
+        return str_time
+
+    def readout_data_to_state_probabilities(
+            self, 
+            result
+        ):
+        state01 = result.get('resultStatus')
+        basis_list = []
+        basis_content = ''.join([''.join([str(s) for s in state]) for state in state01[1:]])
+        qubits_num = len(state01[0])  # 测量比特个数
+        for idx in range(qubits_num):
+            basis_result = basis_content[idx: len(basis_content): qubits_num]
+            basis_list.append([True if res == "1" else False for res in basis_result])
+        return basis_list
+
+    # 读取数据转换成量子态概率
+    def readout_data_to_state_probabilities_whole(
+            self, 
+            result: Dict
+        ):
+        """read data and convert it into a quantum state probability, all returns.
+
+        Args:
+            result: the results returned after query_experiment.
+
+        Returns:
+            Dict: probability
+        """
+        basis_list = self.readout_data_to_state_probabilities(result)
+        probabilities = self.original_onversion_whole(basis_list)
+        return probabilities
+    
+    def readout_data_to_state_probabilities_part(
+            self, 
+            result: Dict
+        ):
+        """read data and convert it into a quantum state probability, do not return with a probability of 0.
+
+        Args:
+            result: the results returned after query_experiment.
+
+        Returns:
+            Dict: probability
+        """
+        basis_list = self.readout_data_to_state_probabilities(result)
+        probabilities = self.original_onversion_part(basis_list)
+        return probabilities
+    
+    def original_onversion_whole(
+            self, 
+            state01
+        ):
+        #当state01为一维时转换成二维数据
+        if isinstance(state01[0], bool):
+            state01=[state01]
+        n = len(state01)  # 读取比特数
+        # 测量比特概率限制
+        # if n > MAX_QUBIT_NUM:
+        #     print(f'Number of qubits > {MAX_QUBIT_NUM}, cannot calculate probabilities.')
+        counts = [0] * (2 ** n)
+        state01_T = np.transpose(state01)  # 转置
+        numShots = len(state01_T)  # 测量重复次数
+        # 统计所有numShots 列
+        for num in range(numShots):
+            k = 0
+            for i in range(n):
+                k += state01_T[num][i] * (2 ** i)
+            counts[k] += 1
+        # 计算概率
+        # P=[counts[k]/numShots for k in range(2**n)]
+        P = {bin(k)[2:].zfill(n): counts[k]/numShots for k in range(2**n)}
+        return P
+    
+    def original_onversion_part(
+            self, 
+            state01
+        ):
+        #当state01为一维时转换成二维数据
+        if isinstance(state01[0], bool):
+            state01=[state01]
+        n = len(state01)  # 读取比特数
+        # 测量比特概率限制
+        # if n > MAX_QUBIT_NUM:
+        #     raise Exception(f'Number of qubits > {MAX_QUBIT_NUM}, cannot calculate probabilities.')
+        counts = {}
+        state01_T = np.transpose(state01)  # 转置
+        numShots = len(state01_T)  # 测量重复次数
+        # 统计所有numShots 列
+        for num in range(numShots):
+            k = 0
+            for i in range(n):
+                k += state01_T[num][i] * (2 ** i)
+            prob_state = bin(k)[2:].zfill(n)
+            if prob_state not in counts:
+                counts[prob_state] = 1
+            else:
+                counts[prob_state] += 1
+        # 计算概率
+        # P=[counts[k]/numShots for k in range(2**n)]
+        P = {k: v/numShots for k, v in counts.items()}
+        return P
+    
+    # 量子态概率矫正
+    def probability_calibration(
+            self, 
+            result: Dict, 
+            config_json: Optional[Dict]=None):
+        """correction of the measured probability of 01 quantum state.
+
+        Args:
+            result:
+                the results returned after query_experiment.
+            config_json: 
+                experimental parameters of quantum computer. 
+                config_json value is None, read the latest experimental parameters for calculation.
+                Defaults to None.
+
+        Raises:
+            Exception: cannot calibrate probability with fidelity.
+
+        Returns:
+            Dict: corrected probability.
+        """
+        CM_CACHE = {}
+        if config_json is None:
+            config_json = self.download_config(down_file=False)
+        qubit_num = [f'Q{i}' for i in result.get('resultStatus')[0]]
+        n = len(qubit_num)  # 测量比特个数
+        qubits = config_json['readout']['readoutArray']['|0> readout fidelity']['qubit_used']
+        readout_fidelity0 = config_json['readout']['readoutArray']['|0> readout fidelity']['param_list']
+        readout_fidelity1 = config_json['readout']['readoutArray']['|1> readout fidelity']['param_list']
+        iq2probFidelity = [[readout_fidelity0[qubits.index(q)], readout_fidelity1[qubits.index(q)]] for q in qubit_num]
+        P = self.readout_data_to_state_probabilities_whole(result)
+        Pm = list(P.values())
+        if not isinstance(iq2probFidelity[0], list):
+            iq2probFidelity=[iq2probFidelity]
+        f = tuple([float(fi) for fi in sum(iq2probFidelity, [])])
+        if f not in CM_CACHE:
+            inv_CM = 1
+            for k in iq2probFidelity[::-1]:
+                F00 = k[0]
+                F11 = k[1]
+                if F00 + F11 == 1:
+                    raise Exception(f'Cannot calibrate probability with fidelity: [{F00}, {F11}]')
+                inv_cm = np.array([[F11, F11 - 1], [F00 - 1, F00]]) / (F00 + F11 - 1)
+                inv_CM = np.kron(inv_CM, inv_cm)
+            CM_CACHE[f] = inv_CM
+        else:
+            inv_CM = CM_CACHE[f]
+        Pi = np.dot(inv_CM, (np.array(Pm, ndmin=2).T))
+        Pi = {bin(idx)[2:].zfill(n): k[0] for idx, k in enumerate(Pi)}
+        return Pi
+    
+    # 对矫正后的概率进行修正
+    def probability_correction(self, probabilities):
+        """correction of the measured probability of 01 quantum state.
+           If there is a probability greater than 1, change this item to 1.
+           If there is anything less than 0, change the item to 0.
+
+        Args:
+            probabilities:
+               corrected probability.
+            
+        Returns:
+            Dict: corrected probability.
+        """
+        abnormal_fidelity_list = list(filter(lambda x: x < 0 or x > 1, probabilities.values()))
+        if not abnormal_fidelity_list:
+            return probabilities
+        for k, v in probabilities.items():
+            if v > 1:
+                probabilities[k] = 1
+            elif v < 0:
+                probabilities[k] = 0
+        fidelity_sum = sum(probabilities.values())
+        for k, v in probabilities.items():
+            probabilities[k] = v / fidelity_sum
+        return probabilities
+    
+    def qcis_mapping_isq(
+            self, 
+            qcis_circuit: str, 
+            initial_layout: Optional[Dict]=None,
+            objective: Optional[str]='size', 
+            seed: Optional[int]=None, 
+            use_post_opt: Optional[bool]=False
+        ):
+        """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
+           and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
+           described by the coupling_map, in the meanwhile reduces circuit depth.
+
+        Args:
+            qcis_circuit: qcis circuit
+            initial_layout: 
+                Initial position of virtual qubits on physical qubits.
+                If given, this is the initial state in search of virtual to physical qubit mapping
+                e.g.:
+                    {0:4, 1:1, 2:5, 3:2, 4:0, 5:3}. Defaults to None.
+            objective: 
+                size: min. # of added swaps
+                depth: min. depth
+                no_swap: try best to find an initial mapping requiring no swaps; raise 
+                an error if fail. Defaults to 'size'.
+            seed: 
+                Set random seed for the stochastic part of the tranpiler. Defaults to None.
+            use_post_opt: 
+                we provide a genetic alg. which utilizes exchange rules for
+                swaps to futher min. depth. Defaults to False.
+
+        raised:
+            TranspileError:
+                if graph specified by coupling map is disconnected.
+
+        Returns:
+            str: qcis string after transpilation
+        """
+        config_json = self.download_config(down_file=False)
+        try:
+            qasm_circuit = self.convert_qcis_to_qasm(qcis_circuit)
+            cur_time = self.current_time()
+            qpu_file = f'./{self.machine_name}_config_param_{cur_time}.json'
+            with open(qpu_file, 'w') as f:
+                f.write(json.dumps(config_json))
+            qasm_transpiled, _, _, _ = transpile(qasm_circuit,
+                                                qpu_file, 
+                                                initial_layout=initial_layout,
+                                                objective=objective,
+                                                seed=seed,
+                                                use_post_opt=use_post_opt)
+            simplity_qcis = self.convert_qasm_to_qcis(qasm_transpiled)
+            os.remove(qpu_file)
+            return simplity_qcis
+        except Exception as e:
+            print(e)
+            print(traceback.format_exc())
+            print('circuit mapping error, will submit using the original route')
+            os.remove(qpu_file)
+            return qcis_circuit
+    
+    def qcis_mapping_sabre(
+            self, 
+            qcis_circuit: str):
+        """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
+           and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
+           described by the coupling_map, in the meanwhile reduces circuit depth.
+
+        Args:
+            qcis_circuit: qcis circuit
+
+        Returns:
+            str : qcis after mapping
+        """       
+        config_json = self.download_config(down_file=False)
+        try:
+            # qcis转换成qasm并写入qasm_file中
+            qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis_circuit)
+            folder_path = 'temp'
+            if not os.path.exists(folder_path):
+                os.makedirs(folder_path)
+            qasm_file = f'{folder_path}/qasm.qasm'
+            with open(qasm_file, 'w') as f:
+                f.write(qasm_circuit)
+            sabre = SabreMapper()
+            # 组装chip_info_fn映射信息
+            chip_info_fn = {}
+            couplings = []
+            coupler_maps = config_json.get('overview').get('coupler_map')
+            coupler_used = config_json.get('twoQubitGate').get('czGate').get('gate error').get('qubit_used')
+            cz_gate_error = config_json.get('twoQubitGate').get('czGate').get('gate error').get('param_list')
+            for coupler, error in zip(coupler_used, cz_gate_error):
+                fidelity = 1- error
+                coupler_qubit_map = coupler_maps.get(coupler)
+                couplings.append({"fidelity": fidelity, "qubit pair": coupler_qubit_map})
+            chip_info_fn['couplings'] = couplings
+            qubit_used = config_json.get('qubit').get('singleQubit').get('gate error').get('qubit_used')
+            qubit_gate_error = config_json.get('qubit').get('singleQubit').get('gate error').get('param_list')
+            qubit_fidelity = {}
+            for qubit, error in zip(qubit_used, qubit_gate_error):
+                qubit_fidelity[qubit] = 1 - error
+            chip_info_fn['fidelity'] = qubit_fidelity
+            chip_info_fn['has multiple chips'] = False
+            chip_info_fn['qubits'] = qubit_used
+
+            chip_info_fn_file = f'{folder_path}/chip_info_fn.json'
+            mapped_qasm_fn_file = f'{folder_path}/mapped_qasm_fn.qasm'
+            qubit_mapping_fn_file = f'{folder_path}/qubit_mapping_fn.json'
+            with open(chip_info_fn_file, 'w') as f:
+                json.dump(chip_info_fn, f)
+            # 调用quMapper做mapping操作
+            success = sabre.map_schedule(qasm_file, chip_info_fn_file, mapped_qasm_fn_file, qubit_mapping_fn_file)
+            if success:
+                with open(qubit_mapping_fn_file, 'r') as f:
+                    qubit_mapping_fn = json.load(f)
+                qubit_map = qubit_mapping_fn.get('physical qubits idx')
+                # mapping成功，将转换后的qasm转为qcis，其中编号根据physical qubits idx做映射
+                simplity_qcis = self.convert_qasm_to_qcis_from_file(mapped_qasm_fn_file, qubit_map)
+                shutil.rmtree(folder_path)
+                return simplity_qcis
+        except Exception as e:
+            print(e)
+            print(traceback.format_exc())
+            print('circuit mapping error, will submit using the original route')
+            shutil.rmtree(folder_path)
+            return qcis_circuit
+
+    def get_experiment_circuit(
+            self,
+            exp_id: str):
+        """according to the exp_id obtained experimental circuit
+
+        Args:
+            exp_id: the result returned by the save_experiment interface, experimental id.
+
+        Returns:
+            Union[int, str]: 0 failed, not 0 successful, success returns the experimental circuit
+        """
+        url = f'{self.base_url}service/sdk/api/experiment/getQcis/by/{exp_id}'
+        headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
+        res = requests.get(url, headers=headers)
+        status_code = res.status_code
+        if status_code != 200:
+            return 0
+        result = json.loads(res.text)
+        code = result.get('code', -1)
+        msg = result.get('msg', '查询实验线路失败')
+        if code != 0:
+            print(f'查询实验线路: {msg}')
+            return 0
+        circuit = result.get('data').get('qcis')
         return circuit
```

## Comparing `ezQgd-1.0.2.dist-info/METADATA` & `ezQgd-1.0.4.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezQgd
-Version: 1.0.2
+Version: 1.0.4
 Summary: A SDK to use Quantum Computer @ quantumctek-cloud.com with QCIS.
 Home-page: https://quantumctek-cloud.com
 Author: Code42
 Author-email: support@quantumctek-cloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -19,11 +19,12 @@
 Requires-Dist: numpy
 Requires-Dist: requests
 Requires-Dist: isqmap
 Requires-Dist: sabreMapper
 
 
 # 国盾量子计算云平台量子编程教学(Readme版)
-# https://quantumctek-cloud.com
+# 官网：https://quantumctek-cloud.com
+# 说明书：https://docs.quantumctek-cloud.com
```

## Comparing `ezQgd-1.0.2.dist-info/RECORD` & `ezQgd-1.0.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ezQgd.py,sha256=7tZIDx1T0urunx-g77MUgWI3jXf2cW3QRMGUJaHFGnE,35259
+ezQgd.py,sha256=s4UoWR-96YL2TI9RFzS9n8NnQRlEuwNOOHHqlt7Spn4,36856
 qasmtoqcis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qasmtoqcis/const.py,sha256=AZTrt8AjrREnIHsK_VQrd_fEcB3TNBJqR1TiatsIurY,3973
 qasmtoqcis/qasm.py,sha256=Uu8zrTXpDCQok2lAeMCSChzjY6oE1xoV8LulgpAJSYc,7400
 qasmtoqcis/qasm_to_qcis.py,sha256=MSCwpWKtqcc5kY9tUgqg_0x30yi7J9v98_p89ikcKgI,11185
 qcistoqasm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qcistoqasm/const.py,sha256=jeuG0MbtqK3MxFlCC_eGwlsUO1nYp6B20KGztuJgmoc,409
 qcistoqasm/qcis.py,sha256=r5ae12O9ZFkCl3Bgw3ldyt2l451rESfZUC7P-qEaTL8,2612
 qcistoqasm/qcis_to_qasm.py,sha256=458xj6Z6rYhCD8918bc7TZZXLKcHhdJgPwQYCqOKIfM,2216
-ezQgd-1.0.2.dist-info/METADATA,sha256=_HtIoP6vfJH1pTt5q-mcYaA2ppfi7L7r0Z2AP82LDy4,872
-ezQgd-1.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-ezQgd-1.0.2.dist-info/top_level.txt,sha256=5SxS9D4ntYSuP5DotvN8wGdQVSZzRN2_NfaD7QO5U8o,28
-ezQgd-1.0.2.dist-info/RECORD,,
+ezQgd-1.0.4.dist-info/METADATA,sha256=k7DNFNp4tmSpds-ElMis4pRkQFxaYFCjSRQqm-ywnuE,930
+ezQgd-1.0.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+ezQgd-1.0.4.dist-info/top_level.txt,sha256=5SxS9D4ntYSuP5DotvN8wGdQVSZzRN2_NfaD7QO5U8o,28
+ezQgd-1.0.4.dist-info/RECORD,,
```

