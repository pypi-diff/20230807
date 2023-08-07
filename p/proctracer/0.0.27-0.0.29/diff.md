# Comparing `tmp/proctracer-0.0.27.tar.gz` & `tmp/proctracer-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.27.tar", last modified: Fri Aug  4 15:52:26 2023, max compression
+gzip compressed data, was "proctracer-0.0.29.tar", last modified: Mon Aug  7 17:42:06 2023, max compression
```

## Comparing `proctracer-0.0.27.tar` & `proctracer-0.0.29.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:26.269425 proctracer-0.0.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-04 15:52:16.000000 proctracer-0.0.27/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 15:52:16.000000 proctracer-0.0.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 15:52:26.269425 proctracer-0.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-04 15:52:16.000000 proctracer-0.0.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:26.265426 proctracer-0.0.27/proctracer/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:26.269425 proctracer-0.0.27/proctracer/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/net_softnet_stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5385 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/proctracer.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 15:52:16.000000 proctracer-0.0.27/proctracer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:26.269425 proctracer-0.0.27/proctracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 15:52:26.000000 proctracer-0.0.27/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-04 15:52:26.000000 proctracer-0.0.27/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:52:26.000000 proctracer-0.0.27/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 15:52:26.000000 proctracer-0.0.27/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 15:52:26.000000 proctracer-0.0.27/proctracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 15:52:26.000000 proctracer-0.0.27/proctracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 15:52:26.269425 proctracer-0.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-08-04 15:52:16.000000 proctracer-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.713570 proctracer-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-07 17:41:54.000000 proctracer-0.0.29/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-07 17:41:54.000000 proctracer-0.0.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 17:42:06.713570 proctracer-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-07 17:41:54.000000 proctracer-0.0.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.705570 proctracer-0.0.29/proctracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.713570 proctracer-0.0.29/proctracer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_softnet_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5394 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/proctracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 17:41:54.000000 proctracer-0.0.29/proctracer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:42:06.709570 proctracer-0.0.29/proctracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-07 17:42:06.000000 proctracer-0.0.29/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-07 17:42:06.713570 proctracer-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-08-07 17:41:54.000000 proctracer-0.0.29/setup.py
```

### Comparing `proctracer-0.0.27/LICENSE.md` & `proctracer-0.0.29/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/PKG-INFO` & `proctracer-0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.27
+Version: 0.0.29
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.27/README.md` & `proctracer-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/proctracer/plugins/__init__.py` & `proctracer-0.0.29/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.29/proctracer/plugins/net_dev.plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
                 for i in pivot_table.columns:
                     axs[0].plot( pivot_table[[i]].dropna(), label="%s %s" % (i, value ) )
             
             if not pivot_table.columns.empty:
                 axs[0].legend(title="interface: [tx,rx]", fontsize='small', loc= 'upper right')
                 
             axs[0].set_ylabel('Byte-Rate [1/s]')
+            axs[0].set_xticklabels([])
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
             axs[0].set_ylim(0,None)
 
             ######### Packets
             for value in ['rx-packets-per-sec', 'tx-packets-per-sec']:
                 pivot_table = self.data_frame.pivot_table(index='time', columns=[self.key], values=value)
```

### Comparing `proctracer-0.0.27/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.29/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,34 +56,37 @@
             #x=self.data_frame[["InErrors","RcvbufErrors"]].div(self.data_frame.InDatagrams, axis=0) # relative count wrt. start time
             x=self.data_frame[["InErrorRate"]] # 
 
             axs[1].plot( x *100.0, label= "InErrorRate")
             axs[1].legend()
                 
             axs[1].set_ylabel('Ratio [%]')
+            axs[1].set_xticklabels([])
             axs[1].grid()
             axs[1].set_xlim(0,maxT)
             axs[1].set_ylim(0,None)
 
             ######### Ratio 2
             x=self.data_frame[["SndbufErrors"]].div(self.data_frame.OutDatagrams, axis=0) # relative count wrt. start time
 
             axs[2].plot( x *100.0 , label= "SndbufErrors")
             axs[2].legend()
                 
             axs[2].set_ylabel('Ratio [%]')
+            axs[2].set_xlabel("Time t [s]")
             axs[2].grid()
             axs[2].set_xlim(0,maxT)
             axs[2].set_ylim(0,None)
 
             ######### Counts
             self.data_frame -= self.data_frame.iloc[0].values.squeeze() # relative count wrt. start time
             
             axs[0].plot( self.data_frame , label= self.data_frame.columns)
             axs[0].legend()
                 
             axs[0].set_ylabel('Datagrams [count]')
+            axs[0].set_xticklabels([])
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
             axs[0].set_ylim(0,None)
 
         pdf.savefig(fig)
```

### Comparing `proctracer-0.0.27/proctracer/plugins/net_softnet_stat.plugin.py` & `proctracer-0.0.29/proctracer/plugins/net_udpX.plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,159 @@
 from matplotlib import pyplot as plt
 
 from plugin_proc_tracer_base import ProcTracerBase
 
-class net_softnet_stat(ProcTracerBase):
+class net_udp4(ProcTracerBase):
 
     def __init__(self,config_yaml):
         super().__init__(
             config_yaml=config_yaml,
-            file='/proc/net/softnet_stat',
-            key='cpu',
-            header_in='packet_process packet_drop time_squeeze -c4- -c5- -c6- -c7- -c8- cpu_collision received_rps flow_limit_count softnet_backlog_len cpu',
+            file='/proc/net/udp',
+            key='inode',
+            header_in='sl local_address rem_address st tx_queue:rx_queue tr:tm->when retrnsmt uid timeout inode ref pointer drops',
+            first_line=1,
             patterns=''
             )
-    '''
-    https://insights-core.readthedocs.io/en/latest/shared_parsers_catalog/softnet_stat.html
-    Column-01: packet_process: Packet processed by each CPU.
-    Column-02: packet_drop: Packets dropped.
-    Column-03: time_squeeze: net_rx_action.
-    Column-09: cpu_collision: collision occur while obtaining device lock while transmitting.
-    Column-10: received_rps: number of times cpu woken up received_rps.
-    Column-11: flow_limit_count: number of times reached flow limit count.
-    Column-12: softnet_backlog_len: Backlog status
-    Column-13: index: core id owning this softnet_data
-    '''
-    
+        
+    def convert_hex_socket(self, hex_socket):
+        h_addr, h_port = hex_socket.split(':')
+        h_addr_list = ["".join(x) for x in zip(*[iter(str(h_addr))]*2)]
+        d_addr_list = [int(x, 16) for x in h_addr_list]
+        d_addr = ".".join(str(x) for x in (d_addr_list[::-1]))
+        d_port = str(int(h_port, 16))
+        return "{}:{}".format(d_addr, d_port)
+
     def mapper(self, sample):
         new_sample={}
         for k,entry in sample.items():
-
-            k=int(entry['cpu'],16)
             
+            h_tx_queue, h_rx_queue = entry['tx_queue:rx_queue'].split(":")
+
             new_sample[k] = {
                 self.key : k,
                 'time': entry['time'],
-                'packet_process' : int(entry['packet_process'],16),
-                'packet_drop': int(entry['packet_drop'],16),
-                'time_squeeze': int(entry['time_squeeze'],16),
-                'cpu_collision' : int(entry['cpu_collision'],16),
-                'received_rps' : int(entry['received_rps'],16),
-                'flow_limit_count': int(entry['flow_limit_count'],16),
-                'softnet_backlog_len' : int(entry['softnet_backlog_len'],16),
-                'packet_drop-per-sec' : 0.0
-                }
+                'socket': "%s -> %s (inode:%s)" % ( self.convert_hex_socket(entry['local_address']),  self.convert_hex_socket(entry['rem_address']), entry['inode'] ) ,
+                'tx_queue': int(h_tx_queue,16),
+                'rx_queue': int(h_rx_queue,16),
+                'drops': int(entry['drops']),
+                'drops-per-sec': 0.0 ,
+                 }
 
             if k in self.sample_old:
-                new_sample[k]['packet_drop-per-sec'] = 1.0*( new_sample[k]['packet_drop'] - self.sample_old[k]['packet_drop'] ) / ( new_sample[k]['time'] - self.sample_old[k]['time'] )
-                if new_sample[k]['packet_drop-per-sec'] < 0:
-                    new_sample[k]['packet_drop-per-sec']=0
+                new_sample[k]['drops-per-sec'] = 1.0*( new_sample[k]['drops'] - self.sample_old[k]['drops'] ) / ( new_sample[k]['time'] - self.sample_old[k]['time'] )
+                if new_sample[k]['drops-per-sec'] < 0:
+                    new_sample[k]['drops-per-sec']=0
                     
         return new_sample
 
     def add_diagrams(self, pdf, maxT):
 
         plt.clf()
         # Creating figure
         cm = 1/2.54                                         # centimeters in inches
         fig, axs = plt.subplots(3, dpi=72, figsize=(29.7*cm,21.0*cm))   # for landscape DIN A4
 
         fig.suptitle('%s' % self.file )
 
+        #get current kernel parameter
+        kernel_parameter={'/proc/sys/net/ipv4/udp_mem': "N/A",    
+                '/proc/sys/net/ipv4/udp_rmem_min': "N/A",
+                '/proc/sys/net/ipv4/udp_wmem_min': "N/A",
+                '/proc/sys/net/core/rmem_default': "N/A",
+                '/proc/sys/net/core/rmem_max': "N/A",
+                '/proc/sys/net/core/wmem_default': "N/A",
+                '/proc/sys/net/core/wmem_max': "N/A",
+                '/proc/sys/net/core/netdev_max_backlog': "N/A",
+                }
+        
+        kernel_parameter_note=""
+        for k,_ in kernel_parameter.items():
+            result = self.proc_reader(k)
+            if result:
+                kernel_parameter[k] = ' '.join(result.split())
+            
+            kernel_parameter_note+= "%s: %s\n" % (k,kernel_parameter[k])
+        
+        axs[1].annotate(kernel_parameter_note, fontsize='xx-small', xy = (0, 0), xycoords='axes fraction')
+
         if not self.data_frame.empty:
             
             pivot_table=[]
             
-            ######### 
+            ######### Queue Size
             maxV=0
-            for value in 'packet_process'.split():
-                pivot_table = self.data_frame.pivot_table(index='time', columns=['cpu'], values=value)
-                pivot_table -= pivot_table.iloc[0].values.squeeze() # relative count wrt. start time
+            for value in 'rx_queue tx_queue'.split():
+                pivot_table = self.data_frame.pivot_table(index='time', columns=['socket'], values=value)
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
                 
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for i in pivot_table.columns:
                     axs[0].plot( pivot_table[[i]].dropna(), label="%s , %s" % (i, value ) )
                 
             if not pivot_table.columns.empty:
                 axs[0].legend(fontsize='xx-small', loc= 'upper right')
                  
-            axs[0].set_ylabel('Packets [count]')
+            axs[0].set_ylabel('Size of tx/rx Queues')
+            axs[0].set_xticklabels([])
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
             axs[0].set_ylim(0,maxV*1.05+0.01)
 
-            ######### 
+            ######### Drops
             maxV=0
-            for value in ['packet_drop']:
-                pivot_table = self.data_frame.pivot_table(index='time', columns=['cpu'], values=value)
-                pivot_table -= pivot_table.iloc[0].values.squeeze() # relative count wrt. start time
+            for value in ['drops']:
+                pivot_table = self.data_frame.pivot_table(index='time', columns=['socket'], values=value)
+                #pivot_table -= pivot_table.iloc[0].values.squeeze() # relative count wrt. start time
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
                 
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for i in pivot_table.columns:
                     axs[1].plot( pivot_table[[i]].dropna(), label=i )
             
             if not pivot_table.columns.empty:
                 axs[1].legend(fontsize='xx-small', loc= 'upper right')
             
             axs[1].set_ylabel('Packet Drops [count]')
+            axs[1].set_xticklabels([])
             axs[1].grid()
             axs[1].set_xlim(0,maxT)
             axs[1].set_ylim(0,maxV*1.05+0.01)
             
-            #########
+            ######### Drop-Rate
             maxV=0
-            for value in ['flow_limit_count', 'softnet_backlog_len']:
-                pivot_table = self.data_frame.pivot_table(index='time', columns=['cpu'], values=value)
+            for value in ['drops-per-sec']:
+                pivot_table = self.data_frame.pivot_table(index='time', columns=['socket'], values=value)
                 pivot_table = pivot_table.loc[:, (pivot_table > 0).any()]
                 maxV=max(maxV, pivot_table.max(axis=1).max(axis=0))
                 
                 for i in pivot_table.columns:
                     axs[2].plot( pivot_table[[i]].dropna(), label=i )
 
             if not pivot_table.columns.empty:
                 axs[2].legend(fontsize='xx-small', loc= 'upper right')
 
             axs[2].set_xlabel('Time t [s]')
-            axs[2].set_ylabel('Counts / Length ')
+            axs[2].set_ylabel('Packet Drop Rate [1/s]')
             axs[2].grid()
             axs[2].set_xlim(0,maxT)
             axs[2].set_ylim(0,maxV*1.05+0.01)
 
-        pdf.savefig(fig)
+        pdf.savefig(fig)
+
+
+class net_udp6(net_udp4):
+
+    def __init__(self,config_yaml):
+        super().__init__(config_yaml=config_yaml)
+        self.file='/proc/net/udp6'
+
+    def convert_hex_socket(self, hex_socket):
+        h_addr, h_port = hex_socket.split(':')
+        h_addr_list = ["".join(x) for x in zip(*[iter(str(h_addr))]*2)]
+        h_addr_list = h_addr_list[:-4] + h_addr_list[:-5:-1] #reversed last 8 byte
+        h_addr = ''.join(h_addr_list)
+        h_addr_list = ["".join(x) for x in zip(*[iter(str(h_addr))]*4)]
+        d_addr = ":".join(str(x).lower() for x in (h_addr_list))
+        d_port = str(int(h_port, 16))
+        return "{}:{}".format(d_addr, d_port)
```

### Comparing `proctracer-0.0.27/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.29/proctracer/plugins/pid_stat.plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,15 @@
 
                 if i not in self.new_pid_map:
                     continue
 
                 axs[0].plot( pivot_table_1[[i]].dropna() * 100.0, label="%s/%s/%s : %s" % (i,self.new_pid_map[i]['ppid'],self.new_pid_map[i]['pgrp'], self.new_pid_map[i]['cmdline'][0:99] ) )
                 axs[0].set_ylabel("Process Load [%]")
                 axs[0].legend(title="pid/ppid/pgrp: cmdline", fontsize='xx-small', loc= 'upper right')
+                axs[0].set_xticklabels([])
                 axs[0].grid()
                 axs[0].set_xlim(0,maxT)
                 axs[0].set_ylim(0,105.0)
 
                 MB_per_page =  0.000001 * PAGESIZE
 
                 axs[1].plot( pivot_table_2[[i]].dropna() * MB_per_page, label="%s/%s/%s : %s" % (i,self.new_pid_map[i]['ppid'],self.new_pid_map[i]['pgrp'], self.new_pid_map[i]['cmdline'][0:99] ) )
```

### Comparing `proctracer-0.0.27/proctracer/plugins/plugin_base.py` & `proctracer-0.0.29/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.29/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.29/proctracer/plugins/pressure_X.plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             pivot_table = self.data_frame.pivot_table(index='time', columns=[self.key])
 
             x=pivot_table.xs(axis=1, level=1, key="some")
             
             axs[0].plot(x, label= (x.columns if len(x.columns)>1 else x.columns[0]) )
             axs[0].legend(title="some", fontsize='small', loc= 'upper right')
             axs[0].set_ylabel('Some Stall Time [%]')
+            axs[0].set_xticklabels([])
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
             axs[0].set_ylim(0,105.0)
 
             x=pivot_table.xs(axis=1, level=1, key="full")
 
             axs[1].plot(x, label=(x.columns if len(x.columns)>1 else x.columns[0]))
```

### Comparing `proctracer-0.0.27/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.29/proctracer/plugins/stat.plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
             pivot_table = self.data_frame.pivot_table(index='time', columns=[self.key], values='load')
 
             ######### Overall
             axs[0].plot( pivot_table[['cpu']].dropna() *100, label='cpu' )
             axs[0].legend(fontsize='small', loc= 'upper right')
             axs[0].set_ylabel('CPU Load [%]')
+            axs[0].set_xticklabels([])
             axs[0].grid()
             axs[0].set_xlim(0,maxT)
             axs[0].set_ylim(0,105.0)
 
             ######### Isolated
             for i in pivot_table.columns:
                 if i != 'cpu':
```

### Comparing `proctracer-0.0.27/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.29/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/proctracer/proctracer.py` & `proctracer-0.0.29/proctracer/proctracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             f.write("%s" % " ".join(options.string))
             
             
 if __name__ == '__main__':
     main()
 
 '''
-benchmark: python3 -m cProfile -s tottime ./proctracer.py
+benchmark: python3 -m cProfile -s tottime ./proctracer.py -f start
 
 iperf -u -sS
 iperf -u -c 0.0.0.0 -t 60 -b 50G
 
 iperf -u -s -V
 iperf -u -c :: -t 60 -b 50G
 '''
```

### Comparing `proctracer-0.0.27/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.29/proctracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.27
+Version: 0.0.29
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.27/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.29/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.27/setup.py` & `proctracer-0.0.29/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 # Always prefer setuptools over distutils
 from setuptools import find_packages, setup
 
 import os
 import re
+import subprocess
 from os import path
 
 
 # The tests utils are used by conan-package-tools
 here = path.abspath(path.dirname(__file__))
 excluded_test_packages = ["proctracer.test.{}*".format(d)
                          for d in os.listdir(os.path.join(here, "proctracer/test"))
@@ -29,16 +30,24 @@
 
 
 def load_version():
     """ Loads a file content """
     filename = os.path.abspath(os.path.join(os.path.dirname(os.path.abspath(__file__)),
                                             "proctracer", "__init__.py"))
     with open(filename, "rt") as version_file:
-        conan_init = version_file.read()
-        version = re.search(r"__version__ = '([0-9a-z.-]+)'", conan_init).group(1)
+        pkg_init = version_file.read()
+        version = re.search(r"__version__ = '([0-9a-z.-]+)'", pkg_init).group(1)
+        
+        tag = subprocess.check_output('git tag --points-at HEAD'.split())
+        subprocess.check_output('git fetch --depth=100000'.split())
+        counter = subprocess.check_output('git rev-list --count HEAD'.split())
+        
+        if not tag:
+            version="%s.dev%s" % (version, int(counter) )
+        
         return version
 
 
 def generate_long_description_file():
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md')) as f:
         long_description = f.read()
```

