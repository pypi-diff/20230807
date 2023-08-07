# Comparing `tmp/p2pfl-0.1.6.tar.gz` & `tmp/p2pfl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2pfl-0.1.6.tar", last modified: Sat Aug 20 17:55:39 2022, max compression
+gzip compressed data, was "p2pfl-0.1.7.tar", last modified: Sun Aug 21 11:42:12 2022, max compression
```

## Comparing `p2pfl-0.1.6.tar` & `p2pfl-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.559924 p2pfl-0.1.6/
--rw-r--r--   0 pedro      (501) staff       (20)    35149 2022-08-20 16:15:23.000000 p2pfl-0.1.6/LICENSE.md
--rw-r--r--   0 pedro      (501) staff       (20)      842 2022-08-20 17:55:39.559100 p2pfl-0.1.6/PKG-INFO
--rw-r--r--   0 pedro      (501) staff       (20)      538 2022-08-20 17:14:35.000000 p2pfl-0.1.6/README.md
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.547229 p2pfl-0.1.6/p2pfl/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)    13505 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/base_node.py
--rw-r--r--   0 pedro      (501) staff       (20)     3021 2022-08-20 16:38:21.000000 p2pfl-0.1.6/p2pfl/command.py
--rw-r--r--   0 pedro      (501) staff       (20)    21302 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/communication_protocol.py
--rw-r--r--   0 pedro      (501) staff       (20)     4720 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/encrypter.py
--rw-r--r--   0 pedro      (501) staff       (20)     3254 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/gossiper.py
--rw-r--r--   0 pedro      (501) staff       (20)     2901 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/heartbeater.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.551664 p2pfl-0.1.6/p2pfl/learning/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/__init__.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.553587 p2pfl-0.1.6/p2pfl/learning/agregators/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/agregators/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     7305 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/agregators/agregator.py
--rw-r--r--   0 pedro      (501) staff       (20)     1249 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/agregators/fedavg.py
--rw-r--r--   0 pedro      (501) staff       (20)      254 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/exceptions.py
--rw-r--r--   0 pedro      (501) staff       (20)     3579 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/learner.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.555520 p2pfl-0.1.6/p2pfl/learning/pytorch/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     4406 2022-08-20 16:39:05.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/lightninglearner.py
--rw-r--r--   0 pedro      (501) staff       (20)     3457 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/logger.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.556748 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     3846 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/mnistfederated_dm.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.557849 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/models/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/models/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     2738 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/models/cnn.py
--rw-r--r--   0 pedro      (501) staff       (20)     2340 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/models/mlp.py
--rw-r--r--   0 pedro      (501) staff       (20)    26224 2022-08-20 16:36:32.000000 p2pfl-0.1.6/p2pfl/node.py
--rw-r--r--   0 pedro      (501) staff       (20)    12772 2022-08-20 16:35:11.000000 p2pfl-0.1.6/p2pfl/node_connection.py
--rw-r--r--   0 pedro      (501) staff       (20)     2765 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/settings.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.558426 p2pfl-0.1.6/p2pfl/utils/
--rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/utils/__init__.py
--rw-r--r--   0 pedro      (501) staff       (20)     3528 2022-08-20 16:15:23.000000 p2pfl-0.1.6/p2pfl/utils/observer.py
-drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-20 17:55:39.550012 p2pfl-0.1.6/p2pfl.egg-info/
--rw-r--r--   0 pedro      (501) staff       (20)      842 2022-08-20 17:55:39.000000 p2pfl-0.1.6/p2pfl.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (501) staff       (20)      998 2022-08-20 17:55:39.000000 p2pfl-0.1.6/p2pfl.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (501) staff       (20)        1 2022-08-20 17:55:39.000000 p2pfl-0.1.6/p2pfl.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (501) staff       (20)       69 2022-08-20 17:55:39.000000 p2pfl-0.1.6/p2pfl.egg-info/requires.txt
--rw-r--r--   0 pedro      (501) staff       (20)        6 2022-08-20 17:55:39.000000 p2pfl-0.1.6/p2pfl.egg-info/top_level.txt
--rw-r--r--   0 pedro      (501) staff       (20)       38 2022-08-20 17:55:39.560016 p2pfl-0.1.6/setup.cfg
--rw-r--r--   0 pedro      (501) staff       (20)     1178 2022-08-20 17:55:01.000000 p2pfl-0.1.6/setup.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.896981 p2pfl-0.1.7/
+-rw-r--r--   0 pedro      (501) staff       (20)    35149 2022-08-21 10:44:02.000000 p2pfl-0.1.7/LICENSE.md
+-rw-r--r--   0 pedro      (501) staff       (20)      843 2022-08-21 11:42:12.896301 p2pfl-0.1.7/PKG-INFO
+-rw-r--r--   0 pedro      (501) staff       (20)      539 2022-08-21 10:44:02.000000 p2pfl-0.1.7/README.md
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.883494 p2pfl-0.1.7/p2pfl/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)    13478 2022-08-21 11:40:34.000000 p2pfl-0.1.7/p2pfl/base_node.py
+-rw-r--r--   0 pedro      (501) staff       (20)     3024 2022-08-21 11:11:32.000000 p2pfl-0.1.7/p2pfl/command.py
+-rw-r--r--   0 pedro      (501) staff       (20)    21318 2022-08-21 11:42:03.000000 p2pfl-0.1.7/p2pfl/communication_protocol.py
+-rw-r--r--   0 pedro      (501) staff       (20)     4720 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/encrypter.py
+-rw-r--r--   0 pedro      (501) staff       (20)     3254 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/gossiper.py
+-rw-r--r--   0 pedro      (501) staff       (20)     2901 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/heartbeater.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.888553 p2pfl-0.1.7/p2pfl/learning/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/__init__.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.890989 p2pfl-0.1.7/p2pfl/learning/aggregators/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/aggregators/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)     7364 2022-08-21 11:19:26.000000 p2pfl-0.1.7/p2pfl/learning/aggregators/aggregator.py
+-rw-r--r--   0 pedro      (501) staff       (20)     1256 2022-08-21 11:15:43.000000 p2pfl-0.1.7/p2pfl/learning/aggregators/fedavg.py
+-rw-r--r--   0 pedro      (501) staff       (20)      254 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/exceptions.py
+-rw-r--r--   0 pedro      (501) staff       (20)     3579 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/learner.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.892212 p2pfl-0.1.7/p2pfl/learning/pytorch/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)     4406 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/lightninglearner.py
+-rw-r--r--   0 pedro      (501) staff       (20)     3457 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/logger.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.893190 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)     3846 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/mnistfederated_dm.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.894368 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/models/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/models/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)     2738 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/models/cnn.py
+-rw-r--r--   0 pedro      (501) staff       (20)     2340 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/models/mlp.py
+-rw-r--r--   0 pedro      (501) staff       (20)    26297 2022-08-21 11:39:38.000000 p2pfl-0.1.7/p2pfl/node.py
+-rw-r--r--   0 pedro      (501) staff       (20)    12787 2022-08-21 11:13:00.000000 p2pfl-0.1.7/p2pfl/node_connection.py
+-rw-r--r--   0 pedro      (501) staff       (20)     2500 2022-08-21 11:09:36.000000 p2pfl-0.1.7/p2pfl/settings.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.895019 p2pfl-0.1.7/p2pfl/utils/
+-rw-r--r--   0 pedro      (501) staff       (20)        0 2022-08-21 10:44:02.000000 p2pfl-0.1.7/p2pfl/utils/__init__.py
+-rw-r--r--   0 pedro      (501) staff       (20)     3534 2022-08-21 11:38:38.000000 p2pfl-0.1.7/p2pfl/utils/observer.py
+drwxr-xr-x   0 pedro      (501) staff       (20)        0 2022-08-21 11:42:12.887469 p2pfl-0.1.7/p2pfl.egg-info/
+-rw-r--r--   0 pedro      (501) staff       (20)      843 2022-08-21 11:42:12.000000 p2pfl-0.1.7/p2pfl.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (501) staff       (20)     1002 2022-08-21 11:42:12.000000 p2pfl-0.1.7/p2pfl.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (501) staff       (20)        1 2022-08-21 11:42:12.000000 p2pfl-0.1.7/p2pfl.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (501) staff       (20)       69 2022-08-21 11:42:12.000000 p2pfl-0.1.7/p2pfl.egg-info/requires.txt
+-rw-r--r--   0 pedro      (501) staff       (20)        6 2022-08-21 11:42:12.000000 p2pfl-0.1.7/p2pfl.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (501) staff       (20)       38 2022-08-21 11:42:12.897115 p2pfl-0.1.7/setup.cfg
+-rw-r--r--   0 pedro      (501) staff       (20)     1178 2022-08-21 11:27:32.000000 p2pfl-0.1.7/setup.py
```

### Comparing `p2pfl-0.1.6/LICENSE.md` & `p2pfl-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/PKG-INFO` & `p2pfl-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pfl
-Version: 0.1.6
+Version: 0.1.7
 Summary: p2p Federated Learning framework
 Home-page: https://pguijas.github.io/federated_learning_p2p/
 Author: Pedro Guijas
 Author-email: pguijas@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -28,7 +28,8 @@
 
 ## Important
 
 Carefully with number of open files at high scale experiments.
 
 If fails, try to change the number of open files. `ulimit -n {VALUE}`
 
+
```

### Comparing `p2pfl-0.1.6/README.md` & `p2pfl-0.1.7/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 pip install p2pfl
 ```
 
 ## Important
 
 Carefully with number of open files at high scale experiments.
 
-If fails, try to change the number of open files. `ulimit -n {VALUE}`
+If fails, try to change the number of open files. `ulimit -n {VALUE}`
```

### Comparing `p2pfl-0.1.6/p2pfl/base_node.py` & `p2pfl-0.1.7/p2pfl/base_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         host (str): The host of the node.
         port (int): The port of the node.
         simulation (bool): If False, communication will be encrypted.
 
     Attributes:
         host (str): The host of the node.
         port (int): The port of the node.
-        simulation (bool): If the node is in simulation mode or not. Basically a simulation nodes don't have encryption and metrics aren't sended to network nodes.
+        simulation (bool): If the node is in simulation mode or not. Basically, simulation nodes don't have encryption and metrics aren't sent to network nodes.
         heartbeater (Heartbeater): The heartbeater of the node.
         gossiper (Gossiper): The gossiper of the node.
     """
 
     #####################
     #     Node Init     #
     #####################
@@ -46,16 +46,16 @@
         if port==None:
             self.__node_socket.bind((host, 0)) # gets a random free port
             self.port = self.__node_socket.getsockname()[1]
         else:
             self.__node_socket.bind((host, port))
         self.__node_socket.listen(50) # no more than 50 connections at queue
         
-        # Neightbors
-        self.__neightbors = [] # private to avoid concurrency issues
+        # Neighbors
+        self.__neighbors = [] # private to avoid concurrency issues
         self.__nei_lock = threading.Lock()
 
         # Logging
         logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 
         # Heartbeater and Gossiper
         self.gossiper = None 
@@ -85,15 +85,15 @@
 
         Note that a node is a thread, so an instance can only be started once.
         """
         # Main Loop
         super().start()
         # Heartbeater and Gossiper
         self.heartbeater = Heartbeater(self.get_name())
-        self.gossiper = Gossiper(self.get_name(),self.__neightbors) # thread safe, only read
+        self.gossiper = Gossiper(self.get_name(),self.__neighbors) # thread safe, only read
         self.heartbeater.add_observer(self)
         self.gossiper.add_observer(self)
         self.heartbeater.start()
         self.gossiper.start()
     
     def stop(self): 
         """
@@ -108,15 +108,15 @@
 
     ########################
     #   Main Thread Loop   #
     ########################
 
     def run(self):
         """
-        Main loop of the node, when a node is running, this method is beeing executed. It will listen for new connections and process them.
+        Main loop of the node, when a node is running, this method is being executed. It will listen for new connections and process them.
         """
         # Process new connections loop
         logging.info('({}) Node started'.format(self.get_name()))
         while not self._terminate_flag.is_set(): 
             try:
                 (ns, _) = self.__node_socket.accept()
                 msg = ns.recv(Settings.BLOCK_SIZE)
@@ -131,15 +131,15 @@
                 logging.exception(e)
        
         # Stop Heartbeater and Gossiper
         self.heartbeater.stop()
         self.gossiper.stop()
 
         # Stop Node
-        logging.info('({}) Stopping node. Disconnecting from {} nodos'.format(self.get_name(), len(self.__neightbors))) 
+        logging.info('({}) Stopping node. Disconnecting from {} nodos'.format(self.get_name(), len(self.__neighbors))) 
         nei_copy_list = self.get_neighbors()
         for n in nei_copy_list:
             n.stop()
         self.__node_socket.close()
 
 
     def __process_new_connection(self, node_socket, h, p, full, force):
@@ -162,20 +162,20 @@
                     node_socket.sendall(rsa.get_key())
                     rsa.load_pair_public_key(node_socket.recv(len(rsa.get_key())))
 
                     # Symmetric
                     aes_cipher = AESCipher()
                     node_socket.sendall(aes_cipher.get_key())
 
-                # Add neightboor
+                # Add neighboor
                 if result == 0:
                     logging.info('{} Connection accepted with {}:{}'.format(self.get_name(),h,p))
                     nc = NodeConnection(self.get_name(),node_socket,(h,p),aes_cipher)
                     nc.add_observer(self)
-                    self.__neightbors.append(nc)
+                    self.__neighbors.append(nc)
                     nc.start(force=force)
                     
                     if full:
                         self.broadcast(CommunicationProtocol.build_connect_to_msg(h,p),exc=[nc],thread_safe=False)
             else:
                 node_socket.close()
             
@@ -200,21 +200,21 @@
             return s
         else:
             s.close()
             return None
 
     def connect_to(self, h, p, full=False, force=False):
         """"
-        Connects a node to other.
+        Connects a node to another.
         
         Args:
             h (str): The host of the node.
             p (int): The port of the node.
             full (bool): If True, the node will be connected to the entire network.
-            force (bool): If True, the the node will be connected even though it should not be.
+            force (bool): If True, the node will be connected even though it should not be.
 
         Returns:
             node: The node that has been connected to.
         """
         if full:
             full = "1"
         else:
@@ -241,19 +241,19 @@
                     # Asymetric
                     rsa = RSACipher()
                     rsa.load_pair_public_key(s.recv(len(rsa.get_key())))
                     s.sendall(rsa.get_key())
                     # Symetric
                     aes_cipher = AESCipher(key=s.recv(AESCipher.key_len()))
 
-                # Add socket to neightbors
+                # Add socket to neighbors
                 logging.info("{} Connected to {}:{}".format(self.get_name(),h,p))
                 nc = NodeConnection(self.get_name(),s,(h,p),aes_cipher)
                 nc.add_observer(self)
-                self.__neightbors.append(nc)
+                self.__neighbors.append(nc)
                 nc.start(force=force)
                 self.__nei_lock.release()
                 return nc
         
             else:
                 logging.info("{} Already connected to {}:{}".format(self.get_name(),h,p))
                 self.__nei_lock.release()
@@ -276,57 +276,57 @@
             h (str): The host of the node.
             p (int): The port of the node.
         """
         self.get_neighbor(h,p).stop()
             
     def get_neighbor(self, h, p, thread_safe=True):
         """
-        Get a ``NodeConnection`` from the neightbors list.
+        Get a ``NodeConnection`` from the neighbors list.
 
         Args:
             h (str): The host of the node.
             p (int): The port of the node.
 
         Returns:
             NodeConnection: The connection with the node.
         """
         if thread_safe:
             self.__nei_lock.acquire()
 
         return_node = None    
-        for n in self.__neightbors:
+        for n in self.__neighbors:
             if n.get_addr() == (h,p):
                 return_node = n
                 break
             
         if thread_safe:
             self.__nei_lock.release()
         
         return return_node
 
     def get_neighbors(self):
         """
         Returns:
-            list: The neightbors of the node.
+            list: The neighbors of the node.
         """
         self.__nei_lock.acquire()
-        n = self.__neightbors.copy()
+        n = self.__neighbors.copy()
         self.__nei_lock.release()
         return n
 
     def rm_neighbor(self,n):
         """
-        Removes a neightboor from the neightbors list.
+        Removes a neighboor from the neighbors list.
 
         Args:
-            n (NodeConnection): The neightboor to be removed.
+            n (NodeConnection): The neighboor to be removed.
         """
         self.__nei_lock.acquire()
         try:
-            self.__neightbors.remove(n)
+            self.__neighbors.remove(n)
             n.stop()
         except:
             pass
         self.__nei_lock.release()
 
     def get_network_nodes(self):
         """
@@ -337,26 +337,26 @@
       
     ##########################
     #     Msg management     #
     ##########################
 
     def broadcast(self, msg, exc=[], thread_safe=True):
         """
-        Broadcasts a message to all the neightbors.
+        Broadcasts a message to all the neighbors.
 
         Args:
             msg (str): The message to be broadcasted.
-            exc (list): The neightbors to be excluded.
-            thread_safe (bool): If True, the broadcast will access the neightbors list in a thread safe mode.
+            exc (list): The neighbors to be excluded.
+            thread_safe (bool): If True, the broadcast will access the neighbors list in a thread safe mode.
 
         """
         if thread_safe:
             self.__nei_lock.acquire()
 
-        for n in self.__neightbors:
+        for n in self.__neighbors:
             if not (n in exc):
                 n.send(msg)
 
         if thread_safe:
             self.__nei_lock.release()
         
     ###########################
@@ -386,15 +386,15 @@
 
         elif event == Events.GOSSIP_BROADCAST_EVENT:
             self.broadcast(obj[0],exc=obj[1]) 
             
         elif event == Events.PROCESSED_MESSAGES_EVENT:
             node, msgs = obj
             # Comunicate to connections the new messages processed
-            for nc in self.__neightbors:
+            for nc in self.__neighbors:
                 if nc != node:
                     nc.add_processed_messages(list(msgs.keys()))
             # Gossip the new messages
             self.gossiper.add_messages(list(msgs.values()),node)
 
         elif event == Events.BEAT_RECEIVED_EVENT:
             self.heartbeater.add_node(obj)
```

### Comparing `p2pfl-0.1.6/p2pfl/command.py` & `p2pfl-0.1.7/p2pfl/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,20 +86,20 @@
 class Vote_train_set_cmd(Command):
     """
     Command that should be executed as a response to a **vote** message.
     """
     def execute(self, node, votes):
         self.node_connection.notify_train_set_votes(node, votes)
 
-class Models_agregated_cmd(Command):
+class Models_aggregated_cmd(Command):
     """
-    Command that should be executed as a response to a **models_agregated** message.
+    Command that should be executed as a response to a **models_aggregated** message.
     """
     def execute(self,node_list):
-        self.node_connection.add_models_agregated(node_list)
+        self.node_connection.add_models_aggregated(node_list)
 
 class Model_initialized_cmd(Command):
     """
     Command that should be executed as a response to a **model_initialized** message.
     """
     def execute(self):
         self.node_connection.set_model_initialized(True)
```

### Comparing `p2pfl-0.1.6/p2pfl/communication_protocol.py` & `p2pfl-0.1.7/p2pfl/communication_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ###############################
 #    CommunicationProtocol    # --> Invoker of Command Patern
 ###############################
 
 class CommunicationProtocol:
     """
-    Manages the meaning of node communication messages. Some messages contains a hash at end, it is used as a unique identifier for the message, 
+    Manages the meaning of node communication messages. Some messages contain a hash at end, it is used as a unique identifier for the message, 
     this kind of messages are gossiped to the entire network.
     
     The valid messages can be classified into gossiped and non-gossiped:
         Gossiped messages: 
             - BEAT <node> <HASH> 
             - START_LEARNING <rounds> <epoches> <HASH>
             - STOP_LEARNING <HASH>
@@ -23,15 +23,15 @@
 
         Non Gossiped messages (communication over only 2 nodes):
             - CONNECT <ip> <port> <full> <force>
             - CONNECT_TO <ip> <port>
             - STOP 
             - PARAMS <data> \PARAMS
             - MODELS_READY <round> 
-            - MODELS_AGREGATED <node>* MODELS_AGREGATED_CLOSE
+            - MODELS_AGGREGATED <node>* MODELS_AGGREGATED_CLOSE
             - MODEL_INITIALIZED
 
     Furthermore, all messages consists of encoded text (utf-8), with the exception of the `PARAMS` message, which contains serialized binaries.
 
     Non-static methods are used to process the different messages. Static methods are used to build messages and process only the `CONNECT` message (handshake). 
     
     Args:
@@ -86,21 +86,21 @@
     """
     Vote train set message header.
     """
     VOTE_TRAIN_SET_CLOSE = "\VOTE_TRAIN_SET"
     """
     Vote train set message closing.
     """
-    MODELS_AGREGATED = "MODELS_AGREGATED"    
+    MODELS_AGGREGATED = "MODELS_AGGREGATED"    
     """
-    Models agregated message header.
+    Models aggregated message header.
     """
-    MODELS_AGREGATED_CLOSE = "\MODELS_AGREGATED" 
+    MODELS_AGGREGATED_CLOSE = "\MODELS_AGGREGATED" 
     """
-    Models agregated message closing.
+    Models aggregated message closing.
     """
     MODEL_INITIALIZED = "MODEL_INITIALIZED" 
     """
     Model initialized message header.
     """
     
     ############################################
@@ -297,29 +297,29 @@
                             break
 
                     except Exception as e:
                         logging.exception(e)
                         error = True
                         break
                     
-                # Models Agregated
-                elif message[0] == CommunicationProtocol.MODELS_AGREGATED:
+                # Models Aggregated
+                elif message[0] == CommunicationProtocol.MODELS_AGGREGATED:
                     try:
                         # Divide messages and check length of message
-                        close_pos = message.index(CommunicationProtocol.MODELS_AGREGATED_CLOSE)
+                        close_pos = message.index(CommunicationProtocol.MODELS_AGGREGATED_CLOSE)
                         content = message[1:close_pos]
                         message = message[close_pos+1:]
 
                         # Get Nodes
                         nodes=[]
                         for n in content:
                             nodes.append(n)
 
                         # Exec
-                        if not self.__exec(CommunicationProtocol.MODELS_AGREGATED, None, None, nodes):
+                        if not self.__exec(CommunicationProtocol.MODELS_AGGREGATED, None, None, nodes):
                             error = True
                             break
 
                     except Exception as e:
                         logging.exception(e)
                         error = True
                         break
@@ -516,26 +516,26 @@
             A encoded vote train set message.
         """
         aux = ""
         for v in votes:
             aux = aux + " " + v[0]+ " " + str(v[1])
         return CommunicationProtocol.generate_hased_message(CommunicationProtocol.VOTE_TRAIN_SET + " " + node + aux + " " + CommunicationProtocol.VOTE_TRAIN_SET_CLOSE)
         
-    def build_models_agregated_msg(nodes):
+    def build_models_aggregated_msg(nodes):
         """
         Args:
-            nodes: List of strings to indicate agregated nodes.
+            nodes: List of strings to indicate aggregated nodes.
         
         Returns:
-            A encoded models agregated message.
+            A encoded models aggregated message.
         """
         aux = ""
         for n in nodes:
             aux = aux + " " + n
-        return (CommunicationProtocol.MODELS_AGREGATED + aux + " " + CommunicationProtocol.MODELS_AGREGATED_CLOSE + "\n").encode("utf-8")
+        return (CommunicationProtocol.MODELS_AGGREGATED + aux + " " + CommunicationProtocol.MODELS_AGGREGATED_CLOSE + "\n").encode("utf-8")
 
     def build_model_initialized_msg():
         """
         Returns:
             A encoded model inicialized message.
         """
         return (CommunicationProtocol.MODEL_INITIALIZED + "\n").encode("utf-8")
```

### Comparing `p2pfl-0.1.6/p2pfl/encrypter.py` & `p2pfl-0.1.7/p2pfl/encrypter.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/gossiper.py` & `p2pfl-0.1.7/p2pfl/gossiper.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/heartbeater.py` & `p2pfl-0.1.7/p2pfl/heartbeater.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/learning/agregators/agregator.py` & `p2pfl-0.1.7/p2pfl/learning/aggregators/aggregator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
 import threading
 import logging
 from p2pfl.settings import Settings
 from p2pfl.utils.observer import Events, Observable
    
-class Agregator(threading.Thread, Observable):
+class Aggregator(threading.Thread, Observable):
     """
-    Class to manage the agregation of models. Its a thread so, agregation will be done in background if all models was added or timeouts have gone. 
-    Also its a observable so, it will notify the node when the agregation was done.
+    Class to manage the aggregation of models. Its a thread so, aggregation will be done in background if all models was added or timeouts have gone. 
+    Also its a observable so, it will notify the node when the aggregation was done.
 
     Args:
         node_name: (str): String with the name of the node.
     """
     def __init__(self, node_name="unknown"):
         self.node_name = node_name
-        threading.Thread.__init__(self, name = "agregator-" + node_name)
+        threading.Thread.__init__(self, name = "aggregator-" + node_name)
         self.daemon = True
         Observable.__init__(self)
         self.__train_set = []
-        self.__waiting_agregated_model = False
-        self.__agregated_waited_model = False
+        self.__waiting_aggregated_model = False
+        self.__aggregated_waited_model = False
         self.__models = {}
         self.__lock = threading.Lock()
-        self.__agregation_lock = threading.Lock()
-        self.__agregation_lock.acquire()
+        self.__aggregation_lock = threading.Lock()
+        self.__aggregation_lock.acquire()
         self.__thread_executed = False
 
     def run(self):
         """
-        Wait for the agregation to be done or timeout. Then agregate the models and notify.
+        Wait for the aggregation to be done or timeout. Then aggregate the models and notify.
         """
         self.__thread_executed = True
 
         # Wait for all models to be added or TIMEOUT
-        self.__agregation_lock.acquire(timeout=Settings.AGREGATION_TIMEOUT) 
+        self.__aggregation_lock.acquire(timeout=Settings.AGGREGATION_TIMEOUT) 
         
-        # Check if node still running (could happen if agregation thread was a residual thread)
+        # Check if node still running (could happen if aggregation thread was a residual thread)
         if self.__train_set == []:
-            logging.info("({}) Shutting Down Agregator Process".format(self.node_name))
-            self.notify(Events.AGREGATION_FINISHED_EVENT,None) # To avoid residual trainning-thread
+            logging.info("({}) Shutting Down Aggregator Process".format(self.node_name))
+            self.notify(Events.AGGREGATION_FINISHED_EVENT,None) # To avoid residual trainning-thread
             return
         
-        # Start agregation
-        n_model_agregated = sum([len(nodes.split()) for nodes in list(self.__models.keys())])
-        if n_model_agregated != len(self.__train_set):
-            logging.info("({}) Agregating models, timeout reached. Missing models: {}".format(self.node_name,set(self.__train_set)-set(self.__models.keys())))
+        # Start aggregation
+        n_model_aggregated = sum([len(nodes.split()) for nodes in list(self.__models.keys())])
+        if n_model_aggregated != len(self.__train_set):
+            logging.info("({}) Aggregating models, timeout reached. Missing models: {}".format(self.node_name,set(self.__train_set)-set(self.__models.keys())))
         else:
-            logging.info("({}) Agregating models.".format(self.node_name))
+            logging.info("({}) Aggregating models.".format(self.node_name))
 
         # Notify node
-        self.notify(Events.AGREGATION_FINISHED_EVENT,self.agregate(self.__models)) 
+        self.notify(Events.AGGREGATION_FINISHED_EVENT,self.aggregate(self.__models)) 
 
-    def agregate(self,models): 
+    def aggregate(self,models): 
         """
-        Agregate the models.
+        Aggregate the models.
         """
         print("Not implemented")
             
-    def set_nodes_to_agregate(self, l):
+    def set_nodes_to_aggregate(self, l):
         """
-        List with the name of nodes to agregate.
+        List with the name of nodes to aggregate.
 
         Args:
-            l: List of nodes to agregate. Empty for no agregation.
+            l: List of nodes to aggregate. Empty for no aggregation.
         """
         self.__train_set = l
 
-    def set_waiting_agregated_model(self):
+    def set_waiting_aggregated_model(self):
         """
-        Indicates that the node is waiting for an agregation. It won't participate in agregation process.
+        Indicates that the node is waiting for an aggregation. It won't participate in aggregation process.
         """
-        self.__waiting_agregated_model = True
+        self.__waiting_aggregated_model = True
 
     def add_model(self, model, nodes, weight):
         """
         Add a model. The first model to be added starts the `run` method (timeout).
 
         Args:
             model: Model to add.
             nodes: Nodes that colaborated to get the model.
             weight: Number of samples used to get the model.
         """
-        if self.__waiting_agregated_model and not self.__agregated_waited_model:
-            logging.info("({}) Recived an agregated model.".format(self.node_name))
-            self.__agregated_waited_model = True
-            self.notify(Events.AGREGATION_FINISHED_EVENT,model) 
+        if self.__waiting_aggregated_model and not self.__aggregated_waited_model:
+            logging.info("({}) Recived an aggregated model.".format(self.node_name))
+            self.__aggregated_waited_model = True
+            self.notify(Events.AGGREGATION_FINISHED_EVENT,model) 
         else:
             if nodes is not None:
                 self.__lock.acquire()
 
-                # Start agregation timeout
+                # Start aggregation timeout
                 if self.__train_set != [] and not self.__thread_executed:
                     self.start()  
 
                 # Get a list of nodes added
                 models_added = [n.split() for n in list(self.__models.keys())] 
                 models_added = [element for sublist in models_added for element in sublist] # Flatten list
                 
-                # Check if agregation is needed
+                # Check if aggregation is needed
                 if len(self.__train_set)>len(models_added):
                     # Check if all nodes are in the train_set 
                     if all([n in self.__train_set for n in nodes]): 
-                        # Check if all nodes are not agregated                    
+                        # Check if all nodes are not aggregated                    
                         if all([n not in models_added for n in nodes]):
-                            # Agregar modelo
+                            # Aggregate model
                             self.__models[" ".join(nodes)] = ((model, weight))
                             logging.info("({}) Model added ({}/{}) from {}".format(self.node_name, str(len(models_added)+len(nodes)), str(len(self.__train_set)), str(nodes)))
                             # Check if all models have been added
-                            self.check_and_run_agregation()
+                            self.check_and_run_aggregation()
                             # Build response 
                             response = models_added + nodes
                             # Unloock
                             self.__lock.release()
                             
                             return response
                         else:
@@ -120,58 +120,58 @@
                         self.__lock.release()
                         logging.debug("({}) Can't add a model from a node ({}) that is not in the training test.".format(self.node_name, nodes))                
                 else:
                     self.__lock.release()
 
         return None
                 
-    def get_partial_agregation(self,except_nodes):
+    def get_partial_aggregation(self,except_nodes):
         """
-        Get the partial agregation of the models.
+        Get the partial aggregation of the models.
 
         Args:
             except_nodes: Nodes to exclude.
 
         Returns:
-            (model, nodes, weight): Model, nodes and number of samples for the partial agregation.
+            (model, nodes, weight): Model, nodes and number of samples for the partial aggregation.
         """
         dict_aux = {}
-        nodes_agregated = []
-        agregation_weight = 0
+        nodes_aggregated = []
+        aggregation_weight = 0
         models = self.__models.copy()
         for n,(m,s) in list(models.items()):
             splited_nodes = n.split() 
             if all([n not in except_nodes for n in splited_nodes]):
                 dict_aux[n] = (m,s)
-                nodes_agregated += splited_nodes
-                agregation_weight += s
+                nodes_aggregated += splited_nodes
+                aggregation_weight += s
         
-        # If there are no models to agregate
+        # If there are no models to aggregate
         if len(dict_aux) == 0:
             return None,None,None
 
-        return (self.agregate(dict_aux), nodes_agregated, agregation_weight)
+        return (self.aggregate(dict_aux), nodes_aggregated, aggregation_weight)
             
-    def check_and_run_agregation(self,force=False):
+    def check_and_run_aggregation(self,force=False):
         """
-        Check if all models have been added and start agregation if so.
+        Check if all models have been added and start aggregation if so.
 
         Args:
-            force: If true, agregation will be started even if not all models have been added.
+            force: If true, aggregation will be started even if not all models have been added.
         """
         models_added = [nodes.split() for nodes in list(self.__models.keys())] 
         models_added = [element for sublist in models_added for element in sublist] # Flatten list
         # Try Unloock
         try:
             if (force or len(models_added)>=len(self.__train_set)) and self.__train_set!=[]: 
-                self.__agregation_lock.release()
+                self.__aggregation_lock.release()
         except:
             pass
 
     def clear(self):
         """
-        Clear all for a new agregation.
+        Clear all for a new aggregation.
         """
         observers = self.get_observers()
         self.__init__(node_name=self.node_name)
         for o in observers:
             self.add_observer(o)
```

### Comparing `p2pfl-0.1.6/p2pfl/learning/agregators/fedavg.py` & `p2pfl-0.1.7/p2pfl/learning/aggregators/fedavg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import logging
 import torch
-from p2pfl.learning.agregators.agregator import Agregator
+from p2pfl.learning.aggregators.aggregator import Aggregator
    
-class FedAvg(Agregator):
+class FedAvg(Aggregator):
     """
     Federated Averaging (FedAvg) [McMahan et al., 2016]
     Paper: https://arxiv.org/abs/1602.05629
     """
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-    def agregate(self,models): 
+    def aggregate(self,models): 
         """
         Ponderated average of the models.
 
         Args:
             models: Dictionary with the models (node: model,num_samples).
         """
 
-        # Check if there are models to agregate
+        # Check if there are models to aggregate
         if len(models)==0:
-            logging.error("({}) Trying to agregate models when there is no models".format(self.node_name))
+            logging.error("({}) Trying to aggregate models when there is no models".format(self.node_name))
             return None
 
         models = list(models.values())
         
         # Total Samples
         total_samples = sum([y for _,y in models])
```

### Comparing `p2pfl-0.1.6/p2pfl/learning/learner.py` & `p2pfl-0.1.7/p2pfl/learning/learner.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/learning/pytorch/lightninglearner.py` & `p2pfl-0.1.7/p2pfl/learning/pytorch/lightninglearner.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/learning/pytorch/logger.py` & `p2pfl-0.1.7/p2pfl/learning/pytorch/logger.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/mnistfederated_dm.py` & `p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/mnistfederated_dm.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/models/cnn.py` & `p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/models/cnn.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/learning/pytorch/mnist_examples/models/mlp.py` & `p2pfl-0.1.7/p2pfl/learning/pytorch/mnist_examples/models/mlp.py`

 * *Files identical despite different names*

### Comparing `p2pfl-0.1.6/p2pfl/node.py` & `p2pfl-0.1.7/p2pfl/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 import logging
 import time
 from p2pfl.base_node import BaseNode
 from p2pfl.command import *
 from p2pfl.communication_protocol import CommunicationProtocol
 from p2pfl.settings import Settings
-from p2pfl.learning.agregators.fedavg import FedAvg
+from p2pfl.learning.aggregators.fedavg import FedAvg
 from p2pfl.learning.exceptions import DecodingParamsError, ModelNotMatchingError
 from p2pfl.learning.pytorch.lightninglearner import LightningLearner
 from p2pfl.utils.observer import Events, Observer
 
 class Node(BaseNode):
     """
     Class based on a base node that allows **p2p Federated Learning**. 
@@ -19,74 +19,74 @@
     Metrics will be saved under a folder with the name of the node.
             
     Args:
         model: Model to be learned. Carefull, model should be compatible with data and the learner.
         data: Dataset to be used in the learning process. Carefull, model should be compatible with data and the learner.
         host (str): Host where the node will be listening.
         port (int): Port where the node will be listening.
-        learner: Learner to be used in the learning process. Default: LightningLearner.
-        agregator (Agregator): Agregator to be used in the learning process. Default: FedAvg.
+        learner (NodeLearner): Learner to be used in the learning process. Default: LightningLearner.
+        aggregator (Aggregator): Aggregator to be used in the learning process. Default: FedAvg.
         simulation (bool): If False, node will share metrics and communication will be encrypted. Default: True.
 
     Attributes:
         round (int): Round of the learning process.
         totalrounds (int): Total number of rounds of the learning process.
-        learner (Learner): Learner to be used in the learning process.
-        agregator (Agregator): Agregator to be used in the learning process.
+        learner (NodeLearner): Learner to be used in the learning process.
+        aggregator (Aggregator): Aggregator to be used in the learning process.
     """
 
     #####################
     #     Node Init     #
     #####################
 
-    def __init__(self, model, data, host="127.0.0.1", port=None, learner=LightningLearner, agregator=FedAvg, simulation=True):
+    def __init__(self, model, data, host="127.0.0.1", port=None, learner=LightningLearner, aggregator=FedAvg, simulation=True):
         # Super init
         BaseNode.__init__(self,host,port, simulation)
         Observer.__init__(self)
 
         # Learning
         self.round = None 
         self.totalrounds = None 
         self.__model_initialized = False
         self.__initial_neighbors = []
         self.__start_thread_lock = threading.Lock()
 
         # Learner
         self.learner = learner(model, data, log_name=self.get_name()) 
 
-        # Agregator
-        self.agregator = agregator( node_name = self.get_name() )
-        self.agregator.add_observer(self)
+        # Aggregator
+        self.aggregator = aggregator( node_name = self.get_name() )
+        self.aggregator.add_observer(self)
 
         # Train Set Votes
         self.__train_set = []
         self.__train_set_votes = {}
         self.__train_set_votes_lock = threading.Lock()
 
         # Locks
         self.__wait_votes_ready_lock = threading.Lock()
-        self.__finish_agregation_lock = threading.Lock()
-        self.__finish_agregation_lock.acquire()
+        self.__finish_aggregation_lock = threading.Lock()
+        self.__finish_aggregation_lock.acquire()
         self.__wait_init_model_lock = threading.Lock()
         self.__wait_init_model_lock.acquire()
 
     #########################
     #    Node Management    #
     #########################
 
     def connect_to(self, h, p, full=False, force=False):
         """"
-        Connects a node to other. If learning is running connections are not allowed (it should be forced).
+        Connects a node to another. If learning is running connections are not allowed (it should be forced).
         Carefull, if connection is forced with a new node, it will produce timeouts in the network.
     
         Args:
             h (str): The host of the node.
             p (int): The port of the node.
             full (bool): If True, the node will be connected to the entire network.
-            force (bool): If True, the the node will be connected even though it should not be.
+            force (bool): If True, the node will be connected even though it should not be.
 
         Returns:
             node: The node that has been connected to.
         """
         # Check if learning is running
         if self.round is not None and not force:
             logging.info("({}) Cant connect to other nodes when learning is running.".format(self.get_name()))
@@ -212,46 +212,46 @@
         """
         logging.info("({}) Stopping learning".format(self.get_name()))
         # Rounds
         self.round = None
         self.totalrounds = None
         # Leraner
         self.learner.interrupt_fit()
-        # Agregator
-        self.agregator.check_and_run_agregation(force=True)  
-        self.agregator.set_nodes_to_agregate([])
-        self.agregator.clear()
+        # Aggregator
+        self.aggregator.check_and_run_aggregation(force=True)  
+        self.aggregator.set_nodes_to_aggregate([])
+        self.aggregator.clear()
         # Try to free wait locks
         try:
             self.__wait_votes_ready_lock.release()
         except:
             pass
 
     ####################################
-    #         Model Agregation         #
+    #         Model Aggregation         #
     ####################################
 
     def add_model(self,m): 
         """
-        Add a model. If the model isn't inicializated, the recieved model is used for it. Otherwise, the model is agregated using the **agregator**.
+        Add a model. If the model isn't inicializated, the recieved model is used for it. Otherwise, the model is aggregated using the **aggregator**.
 
         Args:
             m: Encoded model. Contains model and their contributors
         """
         # Check if Learning is running
         if self.round is not None:
             try:
                 if self.__model_initialized:
-                    # Add model to agregator
+                    # Add model to aggregator
                     decoded_model, contributors, weight = self.learner.decode_parameters(m)
                     if self.learner.check_parameters(decoded_model):
-                        models_added = self.agregator.add_model(decoded_model,contributors,weight)
+                        models_added = self.aggregator.add_model(decoded_model,contributors,weight)
                         if models_added is not None:
                             # CAREFULL RARE BUG at MACBOOCK: When CPU is high, only new nodes will be sent.
-                            self.broadcast(CommunicationProtocol.build_models_agregated_msg(models_added))
+                            self.broadcast(CommunicationProtocol.build_models_aggregated_msg(models_added))
                     else:
                         raise ModelNotMatchingError("Not matching models")
                 else:
                     # Initialize model
                     model, _, _ = self.learner.decode_parameters(m)
                     self.learner.set_parameters(model)
                     self.__model_initialized = True
@@ -286,35 +286,35 @@
 
         # Determine if node is in the train set
         is_train_set = self.get_name() in self.__train_set
         if is_train_set:
 
             # Full connect train set
             if self.round is not None:
-                self.__connect_and_set_agregator()
+                self.__connect_and_set_aggregator()
 
             # Evaluate and send metrics
             if self.round is not None:
                 self.__evaluate()
 
             # Train
             if self.round is not None:
                 self.__train()
             
-            # Agregate Model
+            # Aggregate Model
             if self.round is not None:
-                self.agregator.add_model(self.learner.get_parameters(),[self.get_name()],self.learner.get_num_samples()[0])
-                self.broadcast(CommunicationProtocol.build_models_agregated_msg([self.get_name()])) # Notify agregation
-                self.__gossip_model_agregation()
+                self.aggregator.add_model(self.learner.get_parameters(),[self.get_name()],self.learner.get_num_samples()[0])
+                self.broadcast(CommunicationProtocol.build_models_aggregated_msg([self.get_name()])) # Notify aggregation
+                self.__gossip_model_aggregation()
         else: 
 
-            # Set Models To Agregate 
-            self.agregator.set_waiting_agregated_model()
+            # Set Models To Aggregate 
+            self.aggregator.set_waiting_aggregated_model()
 
-        # Gossip agregated model (also syncrhonizes nodes)
+        # Gossip aggregated model (also syncrhonizes nodes)
         if self.round is not None:
             self.__gossip_model_difusion()
 
         # Finish round
         if self.round is not None:
             self.__on_round_finished()
 
@@ -368,15 +368,15 @@
             self.__train_set_votes_lock.release()
                 
             # Determine if all votes are received
             votes_ready = set(candidates) == set(nc_votes.keys())
             if votes_ready or timeout:
 
                 if timeout and not votes_ready:
-                    logging.info("({}) Timeout for vote agregation. Missing votes from {}".format(self.get_name(), set(candidates) - set(nc_votes.keys())))
+                    logging.info("({}) Timeout for vote aggregation. Missing votes from {}".format(self.get_name(), set(candidates) - set(nc_votes.keys())))
 
                 results = {}
                 for node_vote in list(nc_votes.values()):
                     for i in range(len(node_vote)):
                         k = list(node_vote.keys())[i]
                         v = list(node_vote.values())[i]
                         if k in results:
@@ -410,17 +410,17 @@
                 
         logging.info("{} Train set of {} nodes: {}".format(self.get_name(),len(self.__train_set),self.__train_set))
 
     ##########################
     #    Connect Trainset    #
     ##########################
 
-    def __connect_and_set_agregator(self):
-        # Set Models To Agregate 
-        self.agregator.set_nodes_to_agregate(self.__train_set)
+    def __connect_and_set_aggregator(self):
+        # Set Models To Aggregate 
+        self.aggregator.set_nodes_to_aggregate(self.__train_set)
 
         # Connect Train Set Nodes
         for node in self.__train_set :
             if node != self.get_name():
                 h,p = node.split(":")
                 if p.isdigit():
                     nc = self.get_neighbor(h,int(p))
@@ -468,20 +468,20 @@
 
     def __on_round_finished(self):
         # Remove trainset connections
         for nc in self.get_neighbors():
             if nc not in self.__initial_neighbors:
                 self.rm_neighbor(nc)
         # Set Next Round
-        self.agregator.clear()
+        self.aggregator.clear()
         self.learner.finalize_round() # revisar x si esto pueiera quedar mejor
         self.round = self.round + 1
-        # Clear node agregation
+        # Clear node aggregation
         for nc in self.get_neighbors():
-            nc.clear_models_agregated()
+            nc.clear_models_aggregated()
 
         # Next Step or Finish
         logging.info("({}) Round {} of {} finished.".format(self.get_name(),self.round,self.totalrounds))
         if self.round < self.totalrounds:
             self.__train_step()  
         else:
             # At end, all nodes compute metrics
@@ -492,34 +492,34 @@
             self.__model_initialized = False
             logging.info("({}) Training finished!!.".format(self.get_name(),self.round,self.totalrounds))
 
     #########################
     #    Model Gossiping    #
     #########################
 
-    def __gossip_model_agregation(self):
+    def __gossip_model_aggregation(self):
         # Anonymous functions
-        candidate_condition = lambda nc: nc.get_name() in self.__train_set and len(nc.get_models_agregated())<len(self.__train_set)
-        status_function = lambda nc: ( nc.get_name(),len(nc.get_models_agregated()) )
-        model_function = lambda nc: self.agregator.get_partial_agregation(nc.get_models_agregated())
+        candidate_condition = lambda nc: nc.get_name() in self.__train_set and len(nc.get_models_aggregated())<len(self.__train_set)
+        status_function = lambda nc: ( nc.get_name(),len(nc.get_models_aggregated()) )
+        model_function = lambda nc: self.aggregator.get_partial_aggregation(nc.get_models_aggregated())
 
         # Gossip
         self.__gossip_model(candidate_condition,status_function,model_function)
          
     def __gossip_model_difusion(self,initialization=False):
-        # Wait a model (init or agregated)
+        # Wait a model (init or aggregated)
         if initialization:
             logging.info("({}) Waiting initialization.".format(self.get_name()))
             self.__wait_init_model_lock.acquire()
             logging.info("({}) Gossiping model initialization.".format(self.get_name(), len(self.get_neighbors())))
             candidate_condition = lambda nc: not nc.get_model_initialized()
         else:
             logging.info("({}) Waiting aregation.".format(self.get_name()))
-            self.__finish_agregation_lock.acquire()
-            logging.info("({}) Gossiping agregated model.".format(self.get_name(), len(self.get_neighbors())))
+            self.__finish_aggregation_lock.acquire()
+            logging.info("({}) Gossiping aggregated model.".format(self.get_name(), len(self.get_neighbors())))
             candidate_condition = lambda nc: nc.get_model_ready_status()<self.round
 
         # Anonymous functions
         status_function = lambda nc: nc.get_name()
         model_function = lambda _: (self.learner.get_parameters(),None, None) # At diffusion, contributors are not relevant
         
         # Gossip
@@ -543,37 +543,37 @@
             nei = [nc for nc in self.get_neighbors() if candidate_condition(nc)]
 
             # Determine end of gossip
             if nei == []:
                 logging.info("({}) Gossip finished.".format(self.get_name()))
                 return
 
-            # Save state of neightbors. If nodes are not responding gossip will stop
+            # Save state of neighbors. If nodes are not responding gossip will stop
             if len(last_x_status) != Settings.GOSSIP_EXIT_ON_X_EQUAL_ROUNDS:
                 last_x_status.append([status_function(nc) for nc in nei])
             else:
                 last_x_status[j] = str([status_function(nc) for nc in nei])
                 j = (j+1)%Settings.GOSSIP_EXIT_ON_X_EQUAL_ROUNDS
 
                 # Check if las messages are the same
                 for i in range(len(last_x_status)-1):
                     if last_x_status[i] != last_x_status[i+1]:
                         break
                     logging.info("({}) Gossiping exited for {} equal reounds.".format(self.get_name(), Settings.GOSSIP_EXIT_ON_X_EQUAL_ROUNDS))
                     return
 
-            # Select a random subset of neightbors
+            # Select a random subset of neighbors
             samples = min(Settings.GOSSIP_MODELS_PER_ROUND,len(nei))
             nei = random.sample(nei, samples)
 
-            # Generate and Send Model Partial Agregations (model, node_contributors)
+            # Generate and Send Model Partial Aggregations (model, node_contributors)
             for nc in nei:
                 model,contributors,weights = model_function(nc)
 
-                # Send Partial Agregation
+                # Send Partial Aggregation
                 if model is not None:
                     logging.info("({}) Gossiping model to {}.".format(self.get_name(), nc.get_name()))
                     encoded_model = self.learner.encode_parameters(params=model, contributors=contributors, weight=weights)
                     encoded_msgs = CommunicationProtocol.build_params_msg(encoded_model)
                     # Send Fragments
                     for msg in encoded_msgs:
                         nc.send(msg)
@@ -600,25 +600,25 @@
         if event == Events.NODE_CONNECTED_EVENT:
             n, force = obj
             if self.round is not None and not force:
                 logging.info("({}) Cant connect to other nodes when learning is running. (however, other nodes can be connected to the node.)".format(self.get_name()))
                 n.stop()
                 return
                 
-        elif event == Events.AGREGATION_FINISHED_EVENT:
+        elif event == Events.AGGREGATION_FINISHED_EVENT:
             # Set parameters and communate it to the training process
             if obj is not None:
                 self.learner.set_parameters(obj)
-                # Share that agregation is done
+                # Share that aggregation is done
                 self.broadcast(CommunicationProtocol.build_models_ready_msg(self.round))
             else:
-                logging.error("({}) Agregation finished with no parameters".format(self.get_name()))
+                logging.error("({}) Aggregation finished with no parameters".format(self.get_name()))
                 self.stop()
             try:
-                self.__finish_agregation_lock.release()
+                self.__finish_aggregation_lock.release()
             except:
                 pass
 
         elif event == Events.START_LEARNING_EVENT:
             self.__start_learning_thread(obj[0],obj[1])
 
         elif event == Events.STOP_LEARNING_EVENT:
```

### Comparing `p2pfl-0.1.6/p2pfl/node_connection.py` & `p2pfl-0.1.7/p2pfl/node_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,27 +47,27 @@
 
         # Atributes
         self.__addr = addr
         self.__param_bufffer = b""
         self.__model_ready = -1
         self.__aes_cipher = aes_cipher
         self.__model_initialized = False
-        self.__models_agregated = []
+        self.__models_aggregated = []
         # Communication Protocol
         self.comm_protocol = CommunicationProtocol({
             CommunicationProtocol.BEAT: Beat_cmd(self),
             CommunicationProtocol.STOP: Stop_cmd(self),
             CommunicationProtocol.CONN_TO: Conn_to_cmd(self),
             CommunicationProtocol.START_LEARNING: Start_learning_cmd(self),
             CommunicationProtocol.STOP_LEARNING: Stop_learning_cmd(self),
             CommunicationProtocol.PARAMS: Params_cmd(self),
             CommunicationProtocol.MODELS_READY: Models_Ready_cmd(self),
             CommunicationProtocol.METRICS: Metrics_cmd(self),
             CommunicationProtocol.VOTE_TRAIN_SET: Vote_train_set_cmd(self),
-            CommunicationProtocol.MODELS_AGREGATED: Models_agregated_cmd(self),
+            CommunicationProtocol.MODELS_AGGREGATED: Models_aggregated_cmd(self),
             CommunicationProtocol.MODEL_INITIALIZED: Model_initialized_cmd(self),
         })
 
     ############## 
     #    Name    # 
     ##############
 
@@ -237,37 +237,37 @@
         """
         Returns:
             The model initialized.
         """
         return self.__model_initialized
 
     ##########################
-    #    Models Agregated    #
+    #    Models Aggregated    #
     ##########################
 
-    def add_models_agregated(self,models):
+    def add_models_aggregated(self,models):
         """
-        Add the models agregated.
+        Add the models aggregated.
         
         Args:
-            models: Models agregated.
+            models: Models aggregated.
         """
-        self.__models_agregated = list(set(models+self.__models_agregated))
+        self.__models_aggregated = list(set(models+self.__models_aggregated))
 
-    def clear_models_agregated(self):
+    def clear_models_aggregated(self):
         """
-        Clear models agregated.
+        Clear models aggregated.
         """
-        self.__models_agregated = []
-    def get_models_agregated(self):
+        self.__models_aggregated = []
+    def get_models_aggregated(self):
         """
         Returns:
-            The models agregated.
+            The models aggregated.
         """
-        return self.__models_agregated
+        return self.__models_aggregated
     
     #######################
     #    Params Buffer    #
     #######################
 
     def add_param_segment(self,data):
         """
```

### Comparing `p2pfl-0.1.6/p2pfl/settings.py` & `p2pfl-0.1.7/p2pfl/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     Timeout (seconds) for a node to be considered dead.
     """
     VOTE_TIMEOUT = 60
     """
     Timeout (seconds) for a node to wait for a vote.
     """
-    AGREGATION_TIMEOUT = 60
+    AGGREGATION_TIMEOUT = 60
     """
     Timeout (seconds) for a node to wait for other models. Timeout stars when the first model is added.
     """
 
     # HEARTBEATER
     HEARTBEAT_PERIOD = 4
     """
@@ -87,12 +87,8 @@
     GOSSIP_MODELS_FREC = 1
     """
     Frequency of gossiping models (times by second).
     """
     GOSSIP_MODELS_PER_ROUND = 2
     """
     Amount of gossip models per round.
-    """
-    FRAGMENTS_DELAY = 0.0
-    """
-    Delay (seconds) to wait before sending a fragment. This is a very important value, if the node is too slow and the buffer isn't big enough, the node will send fragments too fast and the other node will not receive them.
     """
```

### Comparing `p2pfl-0.1.6/p2pfl/utils/observer.py` & `p2pfl-0.1.7/p2pfl/utils/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     """
     Used to notify that beats must be sent.
     """
     END_CONNECTION_EVENT            = "END_CONNECTION_EVENT"
     """
     Used to notify that a connection has been closed. (arg: NodeConnection)
     """
-    AGREGATION_FINISHED_EVENT       = "AGREGATION_FINISHED_EVENT"
+    AGGREGATION_FINISHED_EVENT       = "AGGREGATION_FINISHED_EVENT"
     """
-    Used to notify that the agregation was done. (arg: model or None)
+    Used to notify that the aggregation was done. (arg: model or None)
     """
     CONN_TO_EVENT                   = "CONN_TO_EVENT"
     """
-    Used to notify when a node must connect to other. (arg: (host,port))
+    Used to notify when a node must connect to an other. (arg: (host,port))
     """
     START_LEARNING_EVENT            = "START_LEARNING_EVENT"
     """
     Used to notify when the learning process starts. (arg: (rounds,epochs))
     """
     STOP_LEARNING_EVENT             = "STOP_LEARNING_EVENT"
     """
```

### Comparing `p2pfl-0.1.6/p2pfl.egg-info/PKG-INFO` & `p2pfl-0.1.7/p2pfl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2pfl
-Version: 0.1.6
+Version: 0.1.7
 Summary: p2p Federated Learning framework
 Home-page: https://pguijas.github.io/federated_learning_p2p/
 Author: Pedro Guijas
 Author-email: pguijas@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -28,7 +28,8 @@
 
 ## Important
 
 Carefully with number of open files at high scale experiments.
 
 If fails, try to change the number of open files. `ulimit -n {VALUE}`
 
+
```

### Comparing `p2pfl-0.1.6/p2pfl.egg-info/SOURCES.txt` & `p2pfl-0.1.7/p2pfl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 p2pfl.egg-info/SOURCES.txt
 p2pfl.egg-info/dependency_links.txt
 p2pfl.egg-info/requires.txt
 p2pfl.egg-info/top_level.txt
 p2pfl/learning/__init__.py
 p2pfl/learning/exceptions.py
 p2pfl/learning/learner.py
-p2pfl/learning/agregators/__init__.py
-p2pfl/learning/agregators/agregator.py
-p2pfl/learning/agregators/fedavg.py
+p2pfl/learning/aggregators/__init__.py
+p2pfl/learning/aggregators/aggregator.py
+p2pfl/learning/aggregators/fedavg.py
 p2pfl/learning/pytorch/__init__.py
 p2pfl/learning/pytorch/lightninglearner.py
 p2pfl/learning/pytorch/logger.py
 p2pfl/learning/pytorch/mnist_examples/__init__.py
 p2pfl/learning/pytorch/mnist_examples/mnistfederated_dm.py
 p2pfl/learning/pytorch/mnist_examples/models/__init__.py
 p2pfl/learning/pytorch/mnist_examples/models/cnn.py
```

### Comparing `p2pfl-0.1.6/setup.py` & `p2pfl-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 HERE = Path(__file__).parent
 
 PACKAGE_NAME = 'p2pfl' 
-VERSION = '0.1.6' 
+VERSION = '0.1.7' 
 AUTHOR = 'Pedro Guijas' 
 AUTHOR_EMAIL = 'pguijas@gmail.com' 
 URL = 'https://pguijas.github.io/federated_learning_p2p/' 
 DESCRIPTION = 'p2p Federated Learning framework' 
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = "text/markdown"
 LICENSE = 'MIT'
```

