# Comparing `tmp/torchenhanced-0.1.4.tar.gz` & `tmp/torchenhanced-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchenhanced-0.1.4.tar", last modified: Sun Jul 23 16:16:22 2023, max compression
+gzip compressed data, was "torchenhanced-0.1.5.tar", last modified: Mon Aug  7 12:05:02 2023, max compression
```

## Comparing `torchenhanced-0.1.4.tar` & `torchenhanced-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 16:16:22.538648 torchenhanced-0.1.4/
--rw-rw-rw-   0        0        0       87 2023-07-23 00:32:41.000000 torchenhanced-0.1.4/.gitignore
--rw-rw-rw-   0        0        0      665 2023-07-23 16:16:22.537647 torchenhanced-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-05-29 21:44:08.000000 torchenhanced-0.1.4/README.md
--rw-rw-rw-   0        0        0      862 2023-07-23 00:32:41.000000 torchenhanced-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 16:16:22.538648 torchenhanced-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-23 16:16:22.504647 torchenhanced-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-23 16:16:22.515647 torchenhanced-0.1.4/src/torchenhanced/
--rw-rw-rw-   0        0        0     3716 2023-06-20 22:11:53.000000 torchenhanced-0.1.4/src/torchenhanced/CosineWarmup.py
--rw-rw-rw-   0        0        0       84 2023-06-20 22:11:53.000000 torchenhanced-0.1.4/src/torchenhanced/__init__.py
--rw-rw-rw-   0        0        0    20042 2023-07-23 16:14:24.000000 torchenhanced-0.1.4/src/torchenhanced/mlearning.py
-drwxrwxrwx   0        0        0        0 2023-07-23 16:16:22.535647 torchenhanced-0.1.4/src/torchenhanced/util/
--rw-rw-rw-   0        0        0      103 2023-06-20 22:11:53.000000 torchenhanced-0.1.4/src/torchenhanced/util/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-06-20 22:11:53.000000 torchenhanced-0.1.4/src/torchenhanced/util/color_compression.py
--rw-rw-rw-   0        0        0      721 2023-07-23 00:32:41.000000 torchenhanced-0.1.4/src/torchenhanced/util/files.py
--rw-rw-rw-   0        0        0     1335 2023-06-20 22:11:53.000000 torchenhanced-0.1.4/src/torchenhanced/util/misc.py
--rw-rw-rw-   0        0        0     2618 2023-06-20 22:11:53.000000 torchenhanced-0.1.4/src/torchenhanced/util/visualize.py
-drwxrwxrwx   0        0        0        0 2023-07-23 16:16:22.532647 torchenhanced-0.1.4/src/torchenhanced.egg-info/
--rw-rw-rw-   0        0        0      665 2023-07-23 16:16:22.000000 torchenhanced-0.1.4/src/torchenhanced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-07-23 16:16:22.000000 torchenhanced-0.1.4/src/torchenhanced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 16:16:22.000000 torchenhanced-0.1.4/src/torchenhanced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-23 16:16:22.000000 torchenhanced-0.1.4/src/torchenhanced.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-23 16:16:22.000000 torchenhanced-0.1.4/src/torchenhanced.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 16:16:22.536647 torchenhanced-0.1.4/tests/
--rw-rw-rw-   0        0        0     2445 2023-07-23 16:06:40.000000 torchenhanced-0.1.4/tests/test_Trainer.py
--rw-rw-rw-   0        0        0     2217 2023-07-23 00:32:41.000000 torchenhanced-0.1.4/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:05:02.867409 torchenhanced-0.1.5/
+-rw-rw-rw-   0        0        0       97 2023-08-07 11:38:07.000000 torchenhanced-0.1.5/.gitignore
+-rw-rw-rw-   0        0        0      665 2023-08-07 12:05:02.864411 torchenhanced-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-06-14 09:27:16.000000 torchenhanced-0.1.5/README.md
+-rw-rw-rw-   0        0        0      862 2023-08-07 10:56:17.000000 torchenhanced-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 12:05:02.868408 torchenhanced-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 12:05:02.769471 torchenhanced-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 12:05:02.788522 torchenhanced-0.1.5/src/torchenhanced/
+-rw-rw-rw-   0        0        0     3716 2023-06-14 09:28:57.000000 torchenhanced-0.1.5/src/torchenhanced/CosineWarmup.py
+-rw-rw-rw-   0        0        0    19703 2023-08-07 11:58:41.000000 torchenhanced-0.1.5/src/torchenhanced/Trainer.py
+-rw-rw-rw-   0        0        0      112 2023-08-07 11:01:49.000000 torchenhanced-0.1.5/src/torchenhanced/__init__.py
+-rw-rw-rw-   0        0        0     1944 2023-08-07 11:01:35.000000 torchenhanced-0.1.5/src/torchenhanced/modules.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:05:02.839413 torchenhanced-0.1.5/src/torchenhanced/util/
+-rw-rw-rw-   0        0        0      103 2023-06-14 09:27:16.000000 torchenhanced-0.1.5/src/torchenhanced/util/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-06-14 09:27:16.000000 torchenhanced-0.1.5/src/torchenhanced/util/color_compression.py
+-rw-rw-rw-   0        0        0      721 2023-08-07 10:56:17.000000 torchenhanced-0.1.5/src/torchenhanced/util/files.py
+-rw-rw-rw-   0        0        0     1335 2023-06-14 09:27:16.000000 torchenhanced-0.1.5/src/torchenhanced/util/misc.py
+-rw-rw-rw-   0        0        0     2618 2023-06-14 09:27:16.000000 torchenhanced-0.1.5/src/torchenhanced/util/visualize.py
+drwxrwxrwx   0        0        0        0 2023-08-07 12:05:02.830417 torchenhanced-0.1.5/src/torchenhanced.egg-info/
+-rw-rw-rw-   0        0        0      665 2023-08-07 12:05:02.000000 torchenhanced-0.1.5/src/torchenhanced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-08-07 12:05:02.000000 torchenhanced-0.1.5/src/torchenhanced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 12:05:02.000000 torchenhanced-0.1.5/src/torchenhanced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-07 12:05:02.000000 torchenhanced-0.1.5/src/torchenhanced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 12:05:02.000000 torchenhanced-0.1.5/src/torchenhanced.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 12:05:02.863410 torchenhanced-0.1.5/tests/
+-rw-rw-rw-   0        0        0     2965 2023-08-07 11:59:14.000000 torchenhanced-0.1.5/tests/test_Trainer.py
+-rw-rw-rw-   0        0        0     2217 2023-08-07 10:56:17.000000 torchenhanced-0.1.5/tests/test_util.py
```

### Comparing `torchenhanced-0.1.4/PKG-INFO` & `torchenhanced-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchenhanced
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrappers for pytorch stuff I use on the daily
 Author-email: Vassilis Papadopoulos <frotaur@hotmail.co.uk>
 License: MIT License
 Project-URL: Homepage, https://github.com/frotaur/torchenhanced
 Project-URL: Bug Tracker, https://github.com/frotaur/torchenhanced/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchenhanced-0.1.4/pyproject.toml` & `torchenhanced-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.1.4/src/torchenhanced/CosineWarmup.py` & `torchenhanced-0.1.5/src/torchenhanced/CosineWarmup.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.1.4/src/torchenhanced/mlearning.py` & `torchenhanced-0.1.5/src/torchenhanced/Trainer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,14 @@
 import torch.nn as nn
 import torch, wandb, os
 import torch.optim.lr_scheduler as lrsched
 from torch.optim import Optimizer
 from datetime import datetime
 from tqdm import tqdm
-
-
-class DevModule(nn.Module):
-    """
-        Extremely small wrapper for nn.Module.
-        Simply adds a method device() that returns
-        the current device the module is on. Changes if
-        self.to(...) is called.
-
-        args :
-        config : Dictionary that contains the key:value pairs needed to 
-        instantiate the model (essentially the arguments of the __init__ method).
-    """
-    def __init__(self):
-        super().__init__()
-
-        self.register_buffer('_devtens',torch.empty(0))
-
-    @property
-    def device(self):
-        return self._devtens.device
-
-    @property
-    def paranum(self):
-        return sum(p.numel() for p in self.parameters())
-    
-    @property
-    def config(self):
-        """
-            Returns a json-serializable dict containing the config of the model.
-            Essentially a key-value dictionary of the init arguments of the model.
-            Should be redefined in sub-classes.
-        """
-        return self._config
-
-
-class ConfigModule(DevModule):
-    """
-        Same as DevModule, but with a config property that
-        stores the necessary data to reconstruct the model.
-        Use preferably over DevModule, especially with use with Trainer.
-
-        args :
-        config : Dictionary that contains the key:value pairs needed to 
-        instantiate the model (i.e. the argument values of the __init__ method)
-    """
-    def __init__(self, config:dict):
-        super().__init__()
-
-        self._config = config
-        self._config['name'] = self.__class__.__name__
-
-    @property
-    def config(self):
-        """
-            Returns a json-serializable dict containing the config of the model.
-            Essentially a key-value dictionary of the init arguments of the model.
-            Should be redefined in sub-classes.
-        """
-        return self._config
+from .modules import DevModule, ConfigModule
 
 
 class Trainer(DevModule):
     """
         Mother class used to train models, exposing a host of useful functions.
         Should be subclassed to be used, and the following methods should be redefined :
             - process_batch, mandatory
@@ -82,40 +23,40 @@
         Parameters :
         model : Model to be trained
         optim : Optimizer to be used. ! Must be initialized
         with the model parameters ! Default : AdamW with 1e-3 lr.
         scheduler : Scheduler to be used. Can be provided only if using
         non-default optimizer. Must be initialized with aforementioned 
         optimizer. Default : warmup for 4 epochs from 1e-6.
-        model_save_loc : str or None(default), folder in which to save the raw model weights
-        state_save_loc : str or None(default), folder in which to save the training state, 
-        used to resume training.
+        state_save_loc : str or None(default), folder in which to store data 
+        pertaining to training, such as the training state, wandb folder and model weights.
         device : torch.device, device on which to train the model
         run_name : str, for wandb and saves, name of the training session
         project_name : str, name of the project in which the run belongs
     """
 
     def __init__(self, model : nn.Module, optim :Optimizer =None, scheduler : lrsched._LRScheduler =None, 
-                 model_save_loc=None,state_save_loc=None,device:str ='cpu', run_name :str = None, 
-                 project_name :str = None):
+                 state_save_loc=None,device:str ='cpu', run_name :str = None,project_name :str = None):
         super().__init__()
         
         self.to(device)
         self.model = model.to(device)
 
-        if(model_save_loc is None) :
-            self.model_save_loc = os.path.join('.',f"{self.model.__class__.__name__}_weights")
-        else :
-            self.model_save_loc = os.path.join(model_save_loc,f"{self.model.__class__.__name__}_weights")
         
         if(state_save_loc is None) :
-            self.state_save_loc = os.path.join('.',f"{self.model.__class__.__name__}_state")
+            self.data_fold = os.path.join('.',project_name)
+            self.state_save_loc = os.path.join(self.data_fold,"state")
+            self.model_save_loc = os.path.join(self.data_fold,"weights")
         else :
-            self.state_save_loc = os.path.join(state_save_loc,f"{self.model.__class__.__name__}_state")
+            self.data_fold = os.path.join(state_save_loc,project_name)#
+            
+            self.state_save_loc = os.path.join(state_save_loc,project_name,"state")
+            self.model_save_loc = os.path.join(state_save_loc,project_name,"weights")
         
+        os.makedirs(self.data_fold,exist_ok=True)
         if(optim is None):
             self.optim = torch.optim.AdamW(self.model.parameters(),lr=1e-3)
         else :
             self.optim = optim
 
         if(scheduler is None):
             self.scheduler = lrsched.LinearLR(self.optim,start_factor=0.05,total_iters=4)
@@ -147,39 +88,14 @@
             Changes the learning rate of the optimizer.
             Might clash with scheduler ?
         """
 
         for g in self.optim.param_groups:
             g['lr'] = new_lr
         
-    @staticmethod
-    def config_from_state(state_path: str):
-        """
-            Given the path to a trainer state, returns a tuple (config, weights)
-            for the saved model. The model can then be initialized by using config 
-            as its __init__ arguments, and load the state_dict from weights.
-
-            params : 
-            state_path : path of the saved trainer state
-
-            returns: 3-uple
-            model_name : str, the saved model class name
-            config : dict, the saved model config
-            weights : torch.state_dict, the model's state_dict
-
-        """
-        if(not os.path.exists(state_path)):
-            raise ValueError(f'Path {state_path} not found, can\'t load config from it')
-
-        state_dict = torch.load(state_path)
-        config = state_dict['model_config']
-        model_name = state_dict['name']
-        weights = state_dict['model']
-
-        return model_name,config,weights
 
     def load_state(self,state_path : str):
         """
             Loads trainer minimal trainer state (model,session_hash,optim,scheduler).
 
             params : 
             state_path : str, location of the sought-out state_dict
@@ -195,14 +111,16 @@
         self.model.load_state_dict(state_dict['model'])
         self.session_hash = state_dict['session']
         self.optim.load_state_dict(state_dict['optim'])
         self.scheduler.load_state_dict(state_dict['scheduler'])
         self.run_id = state_dict['run_id']
         # Maybe I need to load also the run_name, we'll see
 
+        print('LOAD OF SUCCESSFUL !')
+
 
     def save_state(self,unique:bool=False):
         """
             Saves trainer state.
             Params : 
             state_dict : dict, contains at least the following key-values:
                 - 'model' : contains model.state_dict
@@ -231,54 +149,95 @@
             ,model=self.model.state_dict(),session=self.session_hash,model_config=model_config,
             name=self.model.__class__.__name__, run_id=self.run_id)
 
         name = self.run_name
         if (unique):
             name=name+'_'+datetime.now().strftime('%H-%M_%d_%m')
 
+        name = name + '.state'
         saveloc = os.path.join(self.state_save_loc,name)
         torch.save(state,saveloc)
 
         print('Saved training state')
 
 
-    def save_model(self, name:str=None):
+    @staticmethod
+    def save_model_from_state(state_path:str,save_dir:str='.',name:str=None):
         """
-            Saves model weights onto trainer model_save_loc. Not necessarily useful since all the info
-            is contained in the saved state, but is sometimes practical.
+            Extract model weights and configuration, and saves two files in the specified directory,
+            the weights (.pt) and a .config file containing the model configuration, which can be loaded
+            as a dictionary with torch.load.
+
+            Args :
+            state_path : path to the trainer state
+            save_dir : directory in which to save the model
+            name : name of the model, if None, will be model_name_date.pt
         """
+        namu, config, weights = Trainer.config_from_state(state_path,device='cpu')
+
         if (name is None):
-            name=f"{self.model.__class__.__name__}_{datetime.now().strftime('%H-%M_%d_%m')}.pt"
-        os.makedirs(self.model_save_loc,exist_ok=True)
-        saveloc = os.path.join(self.model_save_loc,name)
+            name=f"{namu}_{datetime.now().strftime('%H-%M_%d_%m')}"
+        name=name+'.pt'
+        os.makedirs(save_dir,exist_ok=True)
+        saveloc = os.path.join(save_dir,name)
         
-        torch.save(self.model.state_dict(), saveloc)
-        try :
-            torch.save(self.model.config, os.path.join(self.model_save_loc,name[:-3]+'.config'))
-        except Exception as e:
-            print(f'''Problem when trying to get configuration of model : {e}. Make sure model.config
-                  is defined.''')
-            raise e
+        torch.save(weights, saveloc)
+
+        torch.save(config, os.path.join(save_dir,name[:-3]+'.config'))
 
-        print(f'Saved checkpoint : {name}')
+        print(f'Saved weights of {name} at {save_dir}/{name}  !')
+
+
+    @staticmethod
+    def config_from_state(state_path: str, device: str=None):
+        """
+            Given the path to a trainer state, returns a tuple (config, weights)
+            for the saved model. The model can then be initialized by using config 
+            as its __init__ arguments, and load the state_dict from weights.
+
+            args : 
+            state_path : path of the saved trainer state
+            device : device on which to load. Default one if None specified
+
+            returns: 3-uple
+            model_name : str, the saved model class name
+            config : dict, the saved model config
+            weights : torch.state_dict, the model's state_dict
+
+        """
+        if(not os.path.exists(state_path)):
+            raise ValueError(f'Path {state_path} not found, can\'t load config from it')
+        
+        if(device is None):
+            state_dict = torch.load(state_path)
+        else :
+            state_dict = torch.load(state_path,map_location=device)
+
+        config = state_dict['model_config']
+        model_name = state_dict['name']
+        weights = state_dict['model']
+
+        return model_name,config,weights
 
 
     def process_batch(self,batch_data,data_dict : dict,**kwargs):
         """
             Redefine this in sub-classes. Should return the loss, as well as 
             the data_dict (potentially updated). Can do logging and other things 
             optionally. Loss is automatically logged, so no need to worry about it. 
 
             params:
             batch_data : whatever is returned by the dataloader
             data_dict : Dictionary containing necessary data, mainly
             for logging. Always contains the following key-values :
                 - stepnum : total number of steps (minibatches) so far
                 - batchnum : current batch number
-                - batch_log : batch interval in which we should log
+                - batch_log : batch interval in which we should log (DEPRECATED)
+                - step_log : number of steps (minibatches) interval in which we should log 
+                (REPLACES deprecated batch_log)
                 - totbatch : total number of batches.
             data_dict can be modified to store running values, or any other value that might
             be important later. If data_dict is updated, this will persist through the next iteration
             and call of process_batch.
 
             Returns : 2-uple, (loss, data_dict)
         """
@@ -293,27 +252,29 @@
             Loss is automatically logged, so no need to worry about it. 
 
             params:
             batch_data : whatever is returned by the dataloader
             data_dict : Dictionary containing necessary data, mainly
             for logging. Always contains the following key-values :
                 - batchnum : current validation mini-batch number
-                - batch_log : batch interval in which we should log (used for training batch-level logging)
+                - batch_log : batch interval in which we should log (DEPRECATED)
+                - step_log : number of steps (minibatches) interval in which we should log 
+                (REPLACES deprecated batch_log)
                 - totbatch : total number of validation minibatches.
                 - epoch : current epoch
             data_dict can be modified to store running values, or any other value that might
             be important later. If data_dict is updated, this will persist through the next iteration
             and call of process_batch.
 
             Returns : 2-uple, (loss, data_dict)
         """
         raise NotImplementedError('process_batch_valid should be implemented in Trainer sub-class')
 
 
-    def get_loaders(self,batch_size):
+    def get_loaders(self,batch_size, num_workers=0):
         """
             Builds the dataloader needed for training and validation.
             Should be re-implemented in subclass.
 
             Params :
             batch_size
 
@@ -324,99 +285,111 @@
 
     def epoch_log(self,data_dict):
         """
             To be (optionally) implemented in sub-class. Does the logging 
             at the epoch level, is called every epoch. Data_dict has (at least) key-values :
                 - stepnum : total number of steps (minibatches) so far
                 - batchnum : current batch number
-                - batch_log : batch interval in which we should log
+                - batch_log : batch interval in which we should log (DEPRECATED)
+                - step_log : number of steps (minibatches) interval in which we should log 
+                (REPLACES deprecated batch_log)
                 - totbatch : total number of batches.
                 - epoch : current epoch
             And any number of additional values, depending on what process_batch does.
         """
         pass
 
     def valid_log(self,data_dict):
         """
             To be (optionally) implemented in sub-class. Does the logging 
             at the epoch level, is called every epoch. Data_dict has (at least) key-values :
                 - stepnum : total number of steps (minibatches) so far
                 - batchnum : current batch number
-                - batch_log : batch interval in which we should log
+                - batch_log : batch interval in which we should log (DEPRECATED)
+                - step_log : number of steps (minibatches) interval in which we should log 
+                (REPLACES deprecated batch_log)
                 - totbatch : total number of batches.
                 - epoch : current epoch
             And any number of additional values, depending on what process_batch does.
         """
         pass
 
     def train_epochs(self,epochs : int,*,batch_sched:bool=False,save_every:int=50,
-                     batch_log:int=None,batch_size:int=32,aggregate:int=1,
-                     load_from:str=None,unique:bool=False,**kwargs):
+                     step_log:int=None,batch_log:int=None,batch_size:int=32,num_workers:int=0,
+                     aggregate:int=1, load_from:str=None,unique:bool=False,**kwargs):
         """
             Trains for specified epoch number. This method trains the model in a basic way,
             and does very basic logging. At the minimum, it requires process_batch and 
             process_batch_valid to be overriden, and other logging methods are optionals.
 
             data_dict can be used to carry info from one batch to another inside the same epoch,
             and can be used by process_batch* functions for logging of advanced quantities.
             Params :
             epochs : number of epochs to train for
             batch_sched : if True, scheduler steps (by a lower amount) between each batch.
             Not that this use is deprecated, so it is recommended to keep False. For now, 
             necessary for some Pytorch schedulers (cosine annealing).
             save_every : saves trainer state every 'save_every' epochs
-            batch_log : If not none, will also log every batch_log batches, in addition to each epoch
+            step_log : If not none, will also log every step_log minibatches, in addition to each epoch
+            batch_log : same as step_log, DEPRECATED
             batch_size : batch size
+            num_workers : number of workers in dataloader
             aggregate : how many batches to aggregate (effective batch_size is aggreg*batch_size)
             load_from : path to a trainer state_dict. Loads the state
                 of the trainer from file, then continues training the specified
                 number of epochs.
             unique : if True, do not overwrites previous save states.
         """
         # Initiate logging
         wandb.init(name=self.run_name,project=self.project_name,config=self.run_config,
-                   id = self.run_id,resume='allow')
+                   id = self.run_id,resume='allow',dir=self.data_fold)
         
         if(os.path.isfile(str(load_from))):
             # Loads the trainer state
             self.load_state(load_from)
+        else :
+            print('Specified "load_from" directory non-existent; continuining with model from scratch.')
         
-        train_loader,valid_loader = self.get_loaders(batch_size)
+        train_loader,valid_loader = self.get_loaders(batch_size,num_workers=num_workers)
         self.model.train()
         epoch=self.scheduler.last_epoch
         print('Number of batches/epoch : ',len(train_loader))
         data_dict={}
-        data_dict['batch_log']=batch_log
+
+        if(step_log is None):
+            step_log=batch_log # FOR BACKWARD COMPATIBILITY, TO BE DEPRECATED
+        data_dict['batch_log']=step_log
+        data_dict['step_log']=step_log
         totbatch = len(train_loader)
-        
+        step_loss=[]
         for ep_incr in tqdm(range(epochs)):
-            epoch_loss,batch_log_loss,batchnum,n_aggreg=[[],[],0,0]
+            epoch_loss,batchnum,n_aggreg=[[],0,0]
             
             data_dict=self._reset_data_dict(data_dict)
             data_dict['epoch']=epoch
             data_dict['totbatch']=totbatch
             for batchnum,batch_data in tqdm(enumerate(train_loader),total=totbatch) :
                 n_aggreg+=1
                 # Process the batch according to the model.
                 data_dict['batchnum']=batchnum
                 data_dict['stepnum']=(epoch)*totbatch+batchnum
 
                 loss, data_dict = self.process_batch(batch_data,data_dict)
                 
                 epoch_loss.append(loss.item())
-                batch_log_loss.append(loss.item())
+                step_loss.append(loss.item())
 
                 loss=loss/aggregate # Rescale loss if aggregating.
                 loss.backward()
                 torch.nn.utils.clip_grad_norm_(self.model.parameters(), 1.)
 
                 
-                if(batchnum%batch_log==batch_log-1):
-                    wandb.log({'batchloss/train':sum(batch_log_loss)/len(batch_log_loss)})
-                    batch_log_loss=[]
+                if(data_dict['stepnum']%step_log==step_log-1):
+                    wandb.log({'steploss/train':sum(step_loss)/len(step_loss)},commit=False)
+                    step_loss=[]
 
                 if(n_aggreg%aggregate==aggregate-1):
                     n_aggreg=0
                     self.optim.step()
                     self.optim.zero_grad()
                 if(batch_sched):
                     self.scheduler.step(epoch+batchnum/totbatch)
@@ -454,14 +427,14 @@
                 self.save_state(unique=unique)
 
         wandb.finish()
 
     def _reset_data_dict(self,data_dict):
         keys = list(data_dict.keys())
         for k in keys:
-            if k not in ['epoch','batch_log'] :
+            if k not in ['epoch','batch_log', 'step_log'] :
                 del data_dict[k]
         # Probably useless to return
         return data_dict
     
     # def __del__(self):
     #     wandb.finish()
```

### Comparing `torchenhanced-0.1.4/src/torchenhanced/util/color_compression.py` & `torchenhanced-0.1.5/src/torchenhanced/util/color_compression.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.1.4/src/torchenhanced/util/files.py` & `torchenhanced-0.1.5/src/torchenhanced/util/files.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.1.4/src/torchenhanced/util/misc.py` & `torchenhanced-0.1.5/src/torchenhanced/util/misc.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.1.4/src/torchenhanced/util/visualize.py` & `torchenhanced-0.1.5/src/torchenhanced/util/visualize.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.1.4/src/torchenhanced.egg-info/PKG-INFO` & `torchenhanced-0.1.5/src/torchenhanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchenhanced
-Version: 0.1.4
+Version: 0.1.5
 Summary: Wrappers for pytorch stuff I use on the daily
 Author-email: Vassilis Papadopoulos <frotaur@hotmail.co.uk>
 License: MIT License
 Project-URL: Homepage, https://github.com/frotaur/torchenhanced
 Project-URL: Bug Tracker, https://github.com/frotaur/torchenhanced/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchenhanced-0.1.4/src/torchenhanced.egg-info/SOURCES.txt` & `torchenhanced-0.1.5/src/torchenhanced.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 README.md
 pyproject.toml
 src/torchenhanced/CosineWarmup.py
+src/torchenhanced/Trainer.py
 src/torchenhanced/__init__.py
-src/torchenhanced/mlearning.py
+src/torchenhanced/modules.py
 src/torchenhanced.egg-info/PKG-INFO
 src/torchenhanced.egg-info/SOURCES.txt
 src/torchenhanced.egg-info/dependency_links.txt
 src/torchenhanced.egg-info/requires.txt
 src/torchenhanced.egg-info/top_level.txt
 src/torchenhanced/util/__init__.py
 src/torchenhanced/util/color_compression.py
```

### Comparing `torchenhanced-0.1.4/tests/test_util.py` & `torchenhanced-0.1.5/tests/test_util.py`

 * *Files identical despite different names*

