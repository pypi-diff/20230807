# Comparing `tmp/secretflow_rayfed-0.1.1a4-py3-none-any.whl.zip` & `tmp/secretflow_rayfed-0.2.0a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,42 @@
-Zip file size: 34848 bytes, number of entries: 24
--rw-rw-r--  2.0 unx      853 b- defN 23-Jul-07 03:44 fed/__init__.py
--rw-rw-r--  2.0 unx    15277 b- defN 23-Jul-07 03:44 fed/api.py
+Zip file size: 58616 bytes, number of entries: 40
+-rw-rw-r--  2.0 unx      859 b- defN 23-Aug-04 07:48 fed/__init__.py
+-rw-rw-r--  2.0 unx    13964 b- defN 23-Aug-04 07:48 fed/api.py
 -rw-rw-r--  2.0 unx    15513 b- defN 23-Jul-07 03:44 fed/barriers.py
--rw-rw-r--  2.0 unx     3025 b- defN 23-Jul-07 03:44 fed/cleanup.py
--rw-rw-r--  2.0 unx     1745 b- defN 23-Jul-07 03:44 fed/config.py
+-rw-rw-r--  2.0 unx     3668 b- defN 23-Aug-04 07:48 fed/cleanup.py
+-rw-rw-r--  2.0 unx     6254 b- defN 23-Aug-04 07:48 fed/config.py
 -rw-rw-r--  2.0 unx     2877 b- defN 23-Mar-17 03:18 fed/fed_object.py
--rw-rw-r--  2.0 unx     4806 b- defN 23-Jul-07 03:44 fed/utils.py
+-rw-rw-r--  2.0 unx     7912 b- defN 23-Aug-04 07:48 fed/tree_util.py
+-rw-rw-r--  2.0 unx     7614 b- defN 23-Aug-04 07:48 fed/utils.py
 -rw-rw-r--  2.0 unx      581 b- defN 23-Mar-17 03:18 fed/_private/__init__.py
 -rw-rw-r--  2.0 unx      581 b- defN 23-Mar-17 03:18 fed/_private/api.py
--rw-rw-r--  2.0 unx     4487 b- defN 23-Jul-07 03:44 fed/_private/compatible_utils.py
--rw-rw-r--  2.0 unx     1227 b- defN 23-Jul-07 03:44 fed/_private/constants.py
--rw-rw-r--  2.0 unx     3837 b- defN 23-Mar-17 03:18 fed/_private/fed_actor.py
--rw-rw-r--  2.0 unx     3813 b- defN 23-Jul-07 03:44 fed/_private/fed_call_holder.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jul-07 03:44 fed/_private/global_context.py
+-rw-rw-r--  2.0 unx     5269 b- defN 23-Aug-04 07:48 fed/_private/compatible_utils.py
+-rw-rw-r--  2.0 unx     1078 b- defN 23-Aug-04 07:48 fed/_private/constants.py
+-rw-rw-r--  2.0 unx     3851 b- defN 23-Aug-04 07:48 fed/_private/fed_actor.py
+-rw-rw-r--  2.0 unx     3947 b- defN 23-Aug-04 07:48 fed/_private/fed_call_holder.py
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Aug-04 07:48 fed/_private/global_context.py
 -rw-rw-r--  2.0 unx     2859 b- defN 23-Jul-07 03:44 fed/_private/grpc_options.py
--rw-rw-r--  2.0 unx     2386 b- defN 23-Mar-17 03:18 fed/_private/serialization_utils.py
+-rw-rw-r--  2.0 unx     2559 b- defN 23-Aug-04 07:48 fed/_private/serialization_utils.py
 -rw-rw-r--  2.0 unx      581 b- defN 23-Mar-17 03:18 fed/grpc/__init__.py
 -rw-rw-r--  2.0 unx     5608 b- defN 23-Mar-17 03:18 fed/grpc/fed_pb2.py
 -rw-rw-r--  2.0 unx     2955 b- defN 23-Mar-17 03:18 fed/grpc/fed_pb2_grpc.py
--rw-rw-r--  2.0 unx    11356 b- defN 23-Jul-07 03:45 secretflow_rayfed-0.1.1a4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7213 b- defN 23-Jul-07 03:45 secretflow_rayfed-0.1.1a4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 03:45 secretflow_rayfed-0.1.1a4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 23-Jul-07 03:45 secretflow_rayfed-0.1.1a4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-07 03:45 secretflow_rayfed-0.1.1a4.dist-info/RECORD
-24 files, 94543 bytes uncompressed, 31748 bytes compressed:  66.4%
+-rw-rw-r--  2.0 unx      581 b- defN 23-Aug-07 07:25 fed/grpc/pb3/__init__.py
+-rw-rw-r--  2.0 unx     5608 b- defN 23-Aug-04 07:48 fed/grpc/pb3/fed_pb2.py
+-rw-rw-r--  2.0 unx     2959 b- defN 23-Aug-04 07:48 fed/grpc/pb3/fed_pb2_grpc.py
+-rw-rw-r--  2.0 unx      581 b- defN 23-Aug-07 07:25 fed/grpc/pb4/__init__.py
+-rw-rw-r--  2.0 unx     2113 b- defN 23-Aug-04 07:48 fed/grpc/pb4/fed_pb2.py
+-rw-rw-r--  2.0 unx     2980 b- defN 23-Aug-04 07:48 fed/grpc/pb4/fed_pb2_grpc.py
+-rw-rw-r--  2.0 unx      613 b- defN 23-Aug-04 07:48 fed/proxy/__init__.py
+-rw-rw-r--  2.0 unx    14523 b- defN 23-Aug-07 06:46 fed/proxy/barriers.py
+-rw-rw-r--  2.0 unx     2661 b- defN 23-Aug-04 07:48 fed/proxy/base_proxy.py
+-rw-rw-r--  2.0 unx      581 b- defN 23-Aug-04 08:25 fed/proxy/brpc_link/__init__.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Aug-04 07:55 fed/proxy/brpc_link/link.py
+-rw-rw-r--  2.0 unx     2114 b- defN 23-Aug-04 07:55 fed/proxy/brpc_link/link_config.py
+-rw-rw-r--  2.0 unx      581 b- defN 23-Aug-04 07:48 fed/proxy/grpc/__init__.py
+-rw-rw-r--  2.0 unx     2569 b- defN 23-Aug-04 07:48 fed/proxy/grpc/grpc_options.py
+-rw-rw-r--  2.0 unx    12361 b- defN 23-Aug-04 07:48 fed/proxy/grpc/grpc_proxy.py
+-rw-rw-r--  2.0 unx    11356 b- defN 23-Aug-07 07:26 secretflow_rayfed-0.2.0a0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7308 b- defN 23-Aug-07 07:26 secretflow_rayfed-0.2.0a0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-07 07:26 secretflow_rayfed-0.2.0a0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 23-Aug-07 07:26 secretflow_rayfed-0.2.0a0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3251 b- defN 23-Aug-07 07:26 secretflow_rayfed-0.2.0a0.dist-info/RECORD
+40 files, 166611 bytes uncompressed, 53486 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: fed/config.py
 Comment: 
 
 Filename: fed/fed_object.py
 Comment: 
 
+Filename: fed/tree_util.py
+Comment: 
+
 Filename: fed/utils.py
 Comment: 
 
 Filename: fed/_private/__init__.py
 Comment: 
 
 Filename: fed/_private/api.py
@@ -51,23 +54,68 @@
 
 Filename: fed/grpc/fed_pb2.py
 Comment: 
 
 Filename: fed/grpc/fed_pb2_grpc.py
 Comment: 
 
-Filename: secretflow_rayfed-0.1.1a4.dist-info/LICENSE
+Filename: fed/grpc/pb3/__init__.py
+Comment: 
+
+Filename: fed/grpc/pb3/fed_pb2.py
+Comment: 
+
+Filename: fed/grpc/pb3/fed_pb2_grpc.py
+Comment: 
+
+Filename: fed/grpc/pb4/__init__.py
+Comment: 
+
+Filename: fed/grpc/pb4/fed_pb2.py
+Comment: 
+
+Filename: fed/grpc/pb4/fed_pb2_grpc.py
+Comment: 
+
+Filename: fed/proxy/__init__.py
+Comment: 
+
+Filename: fed/proxy/barriers.py
+Comment: 
+
+Filename: fed/proxy/base_proxy.py
+Comment: 
+
+Filename: fed/proxy/brpc_link/__init__.py
+Comment: 
+
+Filename: fed/proxy/brpc_link/link.py
+Comment: 
+
+Filename: fed/proxy/brpc_link/link_config.py
+Comment: 
+
+Filename: fed/proxy/grpc/__init__.py
+Comment: 
+
+Filename: fed/proxy/grpc/grpc_options.py
+Comment: 
+
+Filename: fed/proxy/grpc/grpc_proxy.py
+Comment: 
+
+Filename: secretflow_rayfed-0.2.0a0.dist-info/LICENSE
 Comment: 
 
-Filename: secretflow_rayfed-0.1.1a4.dist-info/METADATA
+Filename: secretflow_rayfed-0.2.0a0.dist-info/METADATA
 Comment: 
 
-Filename: secretflow_rayfed-0.1.1a4.dist-info/WHEEL
+Filename: secretflow_rayfed-0.2.0a0.dist-info/WHEEL
 Comment: 
 
-Filename: secretflow_rayfed-0.1.1a4.dist-info/top_level.txt
+Filename: secretflow_rayfed-0.2.0a0.dist-info/top_level.txt
 Comment: 
 
-Filename: secretflow_rayfed-0.1.1a4.dist-info/RECORD
+Filename: secretflow_rayfed-0.2.0a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fed/__init__.py

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from fed.api import (get, init, kill, remote,
                      shutdown)
-from fed.barriers import recv, send
+from fed.proxy.barriers import recv, send
 from fed.fed_object import FedObject
 
 __all__ = [
     "get",
     "init",
     "kill",
     "remote",
```

## fed/api.py

```diff
@@ -19,84 +19,60 @@
 
 import cloudpickle
 import ray
 
 import fed._private.compatible_utils as compatible_utils
 import fed.config as fed_config
 import fed.utils as fed_utils
-from fed._private.constants import (
-    KEY_OF_CLUSTER_ADDRESSES,
-    KEY_OF_CLUSTER_CONFIG,
-    KEY_OF_CROSS_SILO_SERIALIZING_ALLOWED_LIST,
-    KEY_OF_CROSS_SILO_MESSAGES_MAX_SIZE_IN_BYTES,
-    KEY_OF_CURRENT_PARTY_NAME,
-    KEY_OF_JOB_CONFIG,
-    KEY_OF_TLS_CONFIG,
-    KEY_OF_CROSS_SILO_TIMEOUT_IN_SECONDS,
-    RAYFED_DATE_FMT,
-    RAYFED_LOG_FMT,
-)
+from fed._private import constants
 from fed._private.fed_actor import FedActorHandle
 from fed._private.fed_call_holder import FedCallHolder
-from fed._private.global_context import get_global_context
-from fed.barriers import ping_others, recv, send, start_recv_proxy, start_send_proxy
-from fed.cleanup import set_exit_on_failure_sending, wait_sending
+from fed._private.global_context import get_global_context, clear_global_context
+from fed.proxy.barriers import (
+    ping_others,
+    recv,
+    send,
+    _start_receiver_proxy,
+    _start_sender_proxy,
+    _start_sender_receiver_proxy,
+    set_receiver_proxy_actor_name,
+    set_sender_proxy_actor_name,
+)
+from fed.proxy.base_proxy import SenderProxy, ReceiverProxy, SenderReceiverProxy
+from fed.config import CrossSiloMessageConfig
 from fed.fed_object import FedObject
 from fed.utils import is_ray_object_refs, setup_logger
 
 logger = logging.getLogger(__name__)
 
 
 def init(
-    address: str = None,
-    cluster: Dict = None,
+    addresses: Dict = None,
     party: str = None,
+    config: Dict = {},
     tls_config: Dict = None,
     logging_level: str = 'info',
-    cross_silo_grpc_retry_policy: Dict = None,
-    cross_silo_send_max_retries: int = None,
-    cross_silo_serializing_allowed_list: Dict = None,
-    exit_on_failure_cross_silo_sending: bool = False,
-    cross_silo_messages_max_size_in_bytes: int = None,
-    cross_silo_timeout_in_seconds: int = 60,
-    enable_waiting_for_other_parties_ready: bool = False,
-    **kwargs,
+    sender_proxy_cls: SenderProxy = None,
+    receiver_proxy_cls: ReceiverProxy = None,
+    receiver_sender_proxy_cls: SenderReceiverProxy = None,
 ):
     """
-    Initialize a RayFed client. It connects an exist or starts a new local
-        cluster.
+    Initialize a RayFed client.
 
     Args:
-        address: optional; the address of Ray Cluster, same as `address` of
-            `ray.init`.
-        cluster: optional; a dict describes the cluster config. E.g.
+        addresses: optional; a dict describes the addresses configurations. E.g.
 
             .. code:: python
                 {
-                    'alice': {
-                        # The address for other parties.
-                        'address': '127.0.0.1:10001',
-                        # (Optional) the listen address, the `address` will be
-                        # used if not provided.
-                        'listen_addr': '0.0.0.0:10001'
-                    },
-                    'bob': {
-                        # The address for other parties.
-                        'address': '127.0.0.1:10002',
-                        # (Optional) the listen address, the `address` will be
-                        # used if not provided.
-                        'listen_addr': '0.0.0.0:10002'
-                    },
-                    'carol': {
-                        # The address for other parties.
-                        'address': '127.0.0.1:10003',
-                        # (Optional) the listen address, the `address` will be
-                        # used if not provided.
-                        'listen_addr': '0.0.0.0:10003'
-                    },
+                    # The address that can be connected to `alice` by other parties.
+                    'alice': '127.0.0.1:10001',
+                    # The address that can be connected to `bob` by other parties.
+                    'bob': '127.0.0.1:10002',
+                    # The address that can be connected to `carol` by other parties.
+                    'carol': '127.0.0.1:10003',
                 }
         party: optional; self party.
         tls_config: optional; a dict describes the tls config. E.g.
             For alice,
 
             .. code:: python
                 {
@@ -109,139 +85,143 @@
 
             .. code:: python
                 {
                     "ca_cert": "root ca cert of other parties.",
                     "cert": "bob's server cert",
                     "key": "bob's server cert key",
                 }
-
         logging_level: optional; the logging level, could be `debug`, `info`,
             `warning`, `error`, `critical`, not case sensititive.
-        cross_silo_grpc_retry_policy: a dict descibes the retry policy for
-            cross silo rpc call. If None, the following default retry policy
-            will be used. More details please refer to
-            `retry-policy <https://github.com/grpc/proposal/blob/master/A6-client-retries.md#retry-policy>`_. # noqa
-
-            .. code:: python
-                {
-                    "maxAttempts": 4,
-                    "initialBackoff": "0.1s",
-                    "maxBackoff": "1s",
-                    "backoffMultiplier": 2,
-                    "retryableStatusCodes": [
-                        "UNAVAILABLE"
-                    ]
-                }
-        cross_silo_send_max_retries: the max retries for sending data cross silo.
-        cross_silo_serializing_allowed_list: The package or class list allowed for
-            serializing(deserializating) cross silos. It's used for avoiding pickle
-            deserializing execution attack when crossing solis.
-        exit_on_failure_cross_silo_sending: whether exit when failure on
-            cross-silo sending. If True, a SIGTERM will be signaled to self
-            if failed to sending cross-silo data.
-        cross_silo_messages_max_size_in_bytes: The maximum length in bytes of
-            cross-silo messages.
-            If None, the default value of 500 MB is specified.
-        cross_silo_timeout_in_seconds: The timeout in seconds of a cross-silo RPC call.
-            It's 60 by default.
-        enable_waiting_for_other_parties_ready: ping other parties until they
-            are all ready if True.
-        kwargs: the args for ray.init().
 
     Examples:
         >>> import fed
-        >>> cluster = {
-        >>>    'alice': {'address': '127.0.0.1:10001'},
-        >>>    'bob': {'address': '127.0.0.1:10002'},
-        >>>    'carol': {'address': '127.0.0.1:10003'},
+        >>> import ray
+        >>> ray.init(address='local')
+        >>> addresses = {
+        >>>    'alice': '127.0.0.1:10001',
+        >>>    'bob': '127.0.0.1:10002',
+        >>>    'carol': '127.0.0.1:10003',
         >>> }
         >>> # Start as alice.
-        >>> fed.init(address='local', cluster=cluster, self_party='alice')
+        >>> fed.init(addresses=addresses, party='alice')
     """
-    assert cluster, "Cluster should be provided."
+    assert addresses, "Addresses should be provided."
     assert party, "Party should be provided."
-    assert party in cluster, f"Party {party} is not in cluster {cluster}."
+    assert party in addresses, f"Party {party} is not in the addresses {addresses}."
+
+    fed_utils.validate_addresses(addresses)
 
-    compatible_utils.init_ray(address=address, **kwargs)
     tls_config = {} if tls_config is None else tls_config
     if tls_config:
         assert (
             'cert' in tls_config and 'key' in tls_config
         ), 'Cert or key are not in tls_config.'
-    # A Ray private accessing, should be replaced in public API.
 
+    cross_silo_comm_dict = config.get("cross_silo_comm", {})
+    # A Ray private accessing, should be replaced in public API.
     compatible_utils._init_internal_kv()
-    compatible_utils.kv.initialize()
 
     cluster_config = {
-        KEY_OF_CLUSTER_ADDRESSES: cluster,
-        KEY_OF_CURRENT_PARTY_NAME: party,
-        KEY_OF_TLS_CONFIG: tls_config,
-        KEY_OF_CROSS_SILO_SERIALIZING_ALLOWED_LIST: cross_silo_serializing_allowed_list,
-        KEY_OF_CROSS_SILO_MESSAGES_MAX_SIZE_IN_BYTES:
-            cross_silo_messages_max_size_in_bytes,
-        KEY_OF_CROSS_SILO_TIMEOUT_IN_SECONDS: cross_silo_timeout_in_seconds,
+        constants.KEY_OF_CLUSTER_ADDRESSES: addresses,
+        constants.KEY_OF_CURRENT_PARTY_NAME: party,
+        constants.KEY_OF_TLS_CONFIG: tls_config,
     }
 
     job_config = {
-        "": "",
+        constants.KEY_OF_CROSS_SILO_COMM_CONFIG_DICT: cross_silo_comm_dict,
     }
-    compatible_utils.kv.put(KEY_OF_CLUSTER_CONFIG, cloudpickle.dumps(cluster_config))
-    compatible_utils.kv.put(KEY_OF_JOB_CONFIG, cloudpickle.dumps(job_config))
-
+    compatible_utils.kv.put(
+        constants.KEY_OF_CLUSTER_CONFIG, cloudpickle.dumps(cluster_config)
+    )
+    compatible_utils.kv.put(constants.KEY_OF_JOB_CONFIG, cloudpickle.dumps(job_config))
     # Set logger.
     # Note(NKcqx): This should be called after internal_kv has party value, i.e.
     # after `ray.init` and
     # `internal_kv._internal_kv_put(RAYFED_PARTY_KEY, cloudpickle.dumps(party))`
     setup_logger(
         logging_level=logging_level,
-        logging_format=RAYFED_LOG_FMT,
-        date_format=RAYFED_DATE_FMT,
+        logging_format=constants.RAYFED_LOG_FMT,
+        date_format=constants.RAYFED_DATE_FMT,
         party_val=_get_party(),
     )
 
     logger.info(f'Started rayfed with {cluster_config}')
-    set_exit_on_failure_sending(exit_on_failure_cross_silo_sending)
-    # Start recv proxy
-    start_recv_proxy(
-        cluster=cluster,
-        party=party,
-        logging_level=logging_level,
-        tls_config=tls_config,
-        retry_policy=cross_silo_grpc_retry_policy,
-    )
-    start_send_proxy(
-        cluster=cluster,
-        party=party,
-        logging_level=logging_level,
-        tls_config=tls_config,
-        retry_policy=cross_silo_grpc_retry_policy,
-        max_retries=cross_silo_send_max_retries,
+    cross_silo_comm_config = CrossSiloMessageConfig.from_dict(cross_silo_comm_dict)
+    get_global_context().get_cleanup_manager().start(
+        exit_on_sending_failure=cross_silo_comm_config.exit_on_sending_failure
     )
+    if receiver_sender_proxy_cls is not None:
+        proxy_actor_name = 'sender_recevier_actor'
+        set_sender_proxy_actor_name(proxy_actor_name)
+        set_receiver_proxy_actor_name(proxy_actor_name)
+        _start_sender_receiver_proxy(
+            addresses=addresses,
+            party=party,
+            logging_level=logging_level,
+            tls_config=tls_config,
+            proxy_cls=receiver_sender_proxy_cls,
+            proxy_config=cross_silo_comm_dict,
+            ready_timeout_second=cross_silo_comm_config.timeout_in_ms / 1000,
+        )
+    else:
+        if receiver_proxy_cls is None:
+            logger.debug(
+                (
+                    "There is no receiver proxy class specified, "
+                    "it uses `GrpcRecvProxy` by default."
+                )
+            )
+            from fed.proxy.grpc.grpc_proxy import GrpcReceiverProxy
+
+            receiver_proxy_cls = GrpcReceiverProxy
+        _start_receiver_proxy(
+            addresses=addresses,
+            party=party,
+            logging_level=logging_level,
+            tls_config=tls_config,
+            proxy_cls=receiver_proxy_cls,
+            proxy_config=cross_silo_comm_dict,
+            ready_timeout_second=cross_silo_comm_config.timeout_in_ms / 1000,
+        )
+
+        if sender_proxy_cls is None:
+            logger.debug(
+                "There is no sender proxy class specified, it uses `GrpcRecvProxy` by "
+                "default."
+            )
+            from fed.proxy.grpc.grpc_proxy import GrpcSenderProxy
+
+            sender_proxy_cls = GrpcSenderProxy
+        _start_sender_proxy(
+            addresses=addresses,
+            party=party,
+            logging_level=logging_level,
+            tls_config=tls_config,
+            proxy_cls=sender_proxy_cls,
+            proxy_config=cross_silo_comm_dict,
+            ready_timeout_second=cross_silo_comm_config.timeout_in_ms / 1000,
+        )
 
-    if enable_waiting_for_other_parties_ready:
+    if config.get("barrier_on_initializing", False):
         # TODO(zhouaihui): can be removed after we have a better retry strategy.
-        ping_others(cluster=cluster, self_party=party, tls_config=tls_config)
+        ping_others(addresses=addresses, self_party=party, max_retries=3600)
 
 
 def shutdown():
     """
     Shutdown a RayFed client.
     """
-    wait_sending()
-    compatible_utils.kv.delete(KEY_OF_CLUSTER_CONFIG)
-    compatible_utils.kv.delete(KEY_OF_JOB_CONFIG)
-    compatible_utils.kv.reset()
-    ray.shutdown()
-    logger.info('Shutdowned ray.')
+    compatible_utils._clear_internal_kv()
+    clear_global_context()
+    logger.info('Shutdowned rayfed.')
 
 
-def _get_cluster():
+def _get_addresses():
     """
-    Get the RayFed cluster configration.
+    Get the RayFed addresses configration.
     """
     return fed_config.get_cluster_config().cluster_addresses
 
 
 def _get_party():
     """
     A private util function to get the current party name.
@@ -276,17 +256,17 @@
     def options(self, **options):
         self._options = options
         if self._fed_call_holder:
             self._fed_call_holder.options(**options)
         return self
 
     def remote(self, *args, **kwargs):
-        assert (
-            self._node_party is not None
-        ), "A fed function should be specified within a party to execute."
+        if not self._node_party:
+            raise ValueError("You should specify a party name on the fed function.")
+
         return self._fed_call_holder.internal_remote(*args, **kwargs)
 
     def _execute_impl(self, args, kwargs):
         return (
             ray.remote(self._func_body).options(**self._options).remote(*args, **kwargs)
         )
 
@@ -305,15 +285,15 @@
         self._options = options
         return self
 
     def remote(self, *cls_args, **cls_kwargs):
         fed_class_task_id = get_global_context().next_seq_id()
         fed_actor_handle = FedActorHandle(
             fed_class_task_id,
-            _get_cluster(),
+            _get_addresses(),
             self._cls,
             _get_party(),
             self._party,
             self._options,
         )
         fed_call_holder = FedCallHolder(
             self._party, fed_actor_handle._execute_impl, self._options
@@ -356,15 +336,15 @@
     """
     if is_ray_object_refs(fed_objects):
         return ray.get(fed_objects)
 
     # A fake fed_task_id for a `fed.get()` operator. This is useful
     # to help contruct the whole DAG within `fed.get`.
     fake_fed_task_id = get_global_context().next_seq_id()
-    cluster = _get_cluster()
+    addresses = _get_addresses()
     current_party = _get_party()
     is_individual_id = isinstance(fed_objects, FedObject)
     if is_individual_id:
         fed_objects = [fed_objects]
 
     ray_refs = []
     for fed_object in fed_objects:
@@ -372,15 +352,15 @@
             # The code path of the fed_object is in current party, so
             # need to boardcast the data of the fed_object to other parties,
             # and then return the real data of that.
             ray_object_ref = fed_object.get_ray_object_ref()
             assert ray_object_ref is not None
             ray_refs.append(ray_object_ref)
 
-            for party_name in cluster:
+            for party_name in addresses:
                 if party_name == current_party:
                     continue
                 else:
                     if fed_object._was_sending_or_sent_to_party(party_name):
                         # This object was sending or sent to the target party,
                         # so no need to do it again.
                         continue
```

## fed/cleanup.py

```diff
@@ -19,94 +19,88 @@
 import time
 from collections import deque
 
 import ray
 
 logger = logging.getLogger(__name__)
 
-_sending_obj_refs_q = deque()
 
-_check_send_thread = None
+class CleanupManager:
+    """
+    This class is used to manage the related works when the fed driver exiting.
+    It monitors whether the main thread is broken and it needs wait until all sending
+    objects get repsonsed.
+
+    The main logic path is:
+        A. If `fed.shutdown()` is invoked in the main thread and every thing works well,
+        the `graceful_stop()` will be invoked as well and the checking thread will be
+        notifiled to exit gracefully.
+
+        B. If the main thread are broken before sending the notification flag to the
+        sending thread, the monitor thread will detect that and it joins until the main
+        thread exited, then notifys the checking thread.
+    """
+
+    def __init__(self) -> None:
+        # `deque()` is thread safe on `popleft` and `append` operations.
+        # See https://docs.python.org/3/library/collections.html#deque-objects
+        self._sending_obj_refs_q = deque()
+        self._check_send_thread = None
+        self._monitor_thread = None
 
-_EXIT_ON_FAILURE_SENDING = False
+    def start(self, exit_on_sending_failure=False):
+        self._exit_on_sending_failure = exit_on_sending_failure
 
+        def __check_func():
+            self._check_sending_objs()
 
-def set_exit_on_failure_sending(exit_when_failure_sending: bool):
-    global _EXIT_ON_FAILURE_SENDING
-    _EXIT_ON_FAILURE_SENDING = exit_when_failure_sending
-
-
-def get_exit_when_failure_sending():
-    global _EXIT_ON_FAILURE_SENDING
-    return _EXIT_ON_FAILURE_SENDING
-
-
-def _check_sending_objs():
-    def _signal_exit():
-        os.kill(os.getpid(), signal.SIGTERM)
-
-    global _sending_obj_refs_q
-    while True:
-        try:
-            obj_ref = _sending_obj_refs_q.popleft()
-        except IndexError:
-            time.sleep(0.5)
-            continue
-        if isinstance(obj_ref, bool):
-            break
-        try:
-            res = ray.get(obj_ref)
-        except Exception as e:
-            logger.warn(f'Failed to send {obj_ref} with error: {e}')
-            res = False
-        if not res and get_exit_when_failure_sending():
-            logger.warn('Signal self to exit.')
-            _signal_exit()
-            break
-
-    logger.info('Check sending thread was exited.')
-
-
-def _main_thread_monitor():
-    main_thread = threading.main_thread()
-    main_thread.join()
-    notify_to_exit()
-
-
-_monitor_thread = None
-
-
-def _start_check_sending():
-    global _check_send_thread
-    if not _check_send_thread:
-        _check_send_thread = threading.Thread(target=_check_sending_objs)
-        _check_send_thread.start()
+        self._check_send_thread = threading.Thread(target=__check_func)
+        self._check_send_thread.start()
         logger.info('Start check sending thread.')
 
-        global _monitor_thread
-        if not _monitor_thread:
-            _monitor_thread = threading.Thread(target=_main_thread_monitor)
-            _monitor_thread.start()
-            logger.info('Start check sending monitor thread.')
-
-
-def push_to_sending(obj_ref: ray.ObjectRef):
-    _start_check_sending()
-    global _sending_obj_refs_q
-    _sending_obj_refs_q.append(obj_ref)
-
-
-def notify_to_exit():
-    global _sending_obj_refs_q
-    _sending_obj_refs_q.append(True)
-    logger.info('Notify check sending thread to exit.')
-
-
-def wait_sending():
-    global _check_send_thread
-    if _check_send_thread:
-        notify_to_exit()
-        _check_send_thread.join()
-        _check_send_thread = None
-        logger.info('Clearing sending queue.')
-        global _sending_obj_refs_q
-        _sending_obj_refs_q.clear()
+        def _main_thread_monitor():
+            main_thread = threading.main_thread()
+            main_thread.join()
+            self._notify_to_exit()
+
+        self._monitor_thread = threading.Thread(target=_main_thread_monitor)
+        self._monitor_thread.start()
+        logger.info('Start check sending monitor thread.')
+
+    def graceful_stop(self):
+        assert self._check_send_thread is not None
+        self._notify_to_exit()
+        self._check_send_thread.join()
+
+    def _notify_to_exit(self):
+        # Sending the termination signal
+        self.push_to_sending(True)
+        logger.info('Notify check sending thread to exit.')
+
+    def push_to_sending(self, obj_ref: ray.ObjectRef):
+        self._sending_obj_refs_q.append(obj_ref)
+
+    def _check_sending_objs(self):
+        def _signal_exit():
+            os.kill(os.getpid(), signal.SIGTERM)
+
+        assert self._sending_obj_refs_q is not None
+
+        while True:
+            try:
+                obj_ref = self._sending_obj_refs_q.popleft()
+            except IndexError:
+                time.sleep(0.1)
+                continue
+            if isinstance(obj_ref, bool):
+                break
+            try:
+                res = ray.get(obj_ref)
+            except Exception as e:
+                logger.warn(f'Failed to send {obj_ref} with error: {e}')
+                res = False
+            if not res and self._exit_on_sending_failure:
+                logger.warn('Signal self to exit.')
+                _signal_exit()
+                break
+
+        logger.info('Check sending thread was exited.')
```

## fed/config.py

```diff
@@ -1,20 +1,23 @@
-
-
 """This module should be cached locally due to all configurations
    are mutable.
 """
 
 import fed._private.compatible_utils as compatible_utils
 import fed._private.constants as fed_constants
 import cloudpickle
+import json
+
+from typing import Dict, List, Optional
+from dataclasses import dataclass, fields
 
 
 class ClusterConfig:
     """A local cache of cluster configuration items."""
+
     def __init__(self, raw_bytes: bytes) -> None:
         self._data = cloudpickle.loads(raw_bytes)
 
     @property
     def cluster_addresses(self):
         return self._data[fed_constants.KEY_OF_CLUSTER_ADDRESSES]
 
@@ -22,42 +25,146 @@
     def current_party(self):
         return self._data[fed_constants.KEY_OF_CURRENT_PARTY_NAME]
 
     @property
     def tls_config(self):
         return self._data[fed_constants.KEY_OF_TLS_CONFIG]
 
-    @property
-    def serializing_allowed_list(self):
-        return self._data[fed_constants.KEY_OF_CROSS_SILO_SERIALIZING_ALLOWED_LIST]
 
-    @property
-    def cross_silo_timeout(self):
-        return self._data[fed_constants.KEY_OF_CROSS_SILO_TIMEOUT_IN_SECONDS]
+class JobConfig:
+    def __init__(self, raw_bytes: bytes) -> None:
+        if raw_bytes is None:
+            self._data = {}
+        else:
+            self._data = cloudpickle.loads(raw_bytes)
 
     @property
-    def cross_silo_messages_max_size(self):
-        return self._data[fed_constants.KEY_OF_CROSS_SILO_MESSAGES_MAX_SIZE_IN_BYTES]
-
-
-class JobConfig:
-    def __init__(self) -> None:
-        pass
+    def cross_silo_comm_config_dict(self) -> Dict:
+        return self._data.get(fed_constants.KEY_OF_CROSS_SILO_COMM_CONFIG_DICT, {})
 
 
 # A module level cache for the cluster configurations.
 _cluster_config = None
 
+_job_config = None
+
 
 def get_cluster_config():
     """This function is not thread safe to use."""
     global _cluster_config
     if _cluster_config is None:
         compatible_utils._init_internal_kv()
         compatible_utils.kv.initialize()
         raw_dict = compatible_utils.kv.get(fed_constants.KEY_OF_CLUSTER_CONFIG)
         _cluster_config = ClusterConfig(raw_dict)
     return _cluster_config
 
 
 def get_job_config():
-    raise NotImplementedError("This method is not implemented yet.")
+    """This config still acts like cluster config for now"""
+    global _job_config
+    if _job_config is None:
+        compatible_utils._init_internal_kv()
+        compatible_utils.kv.initialize()
+        raw_dict = compatible_utils.kv.get(fed_constants.KEY_OF_JOB_CONFIG)
+        _job_config = JobConfig(raw_dict)
+    return _job_config
+
+
+@dataclass
+class CrossSiloMessageConfig:
+    """A class to store parameters used for Proxy Actor
+
+    Attributes:
+        proxy_max_restarts: The max restart times for the send proxy.
+        serializing_allowed_list: The package or class list allowed for
+            serializing(deserializating) cross silos. It's used for avoiding pickle
+            deserializing execution attack when crossing solis.
+        send_resource_label: Customized resource label, the SenderProxyActor
+            will be scheduled based on the declared resource label. For example,
+            when setting to `{"my_label": 1}`, then the sender proxy actor will be
+            started only on Nodes with `{"resource": {"my_label": $NUM}}` where
+            $NUM >= 1.
+        recv_resource_label: Customized resource label, the ReceiverProxyActor
+            will be scheduled based on the declared resource label. For example,
+            when setting to `{"my_label": 1}`, then the receiver proxy actor will be
+            started only on Nodes with `{"resource": {"my_label": $NUM}}` where
+            $NUM >= 1.
+        exit_on_sending_failure: whether exit when failure on
+            cross-silo sending. If True, a SIGTERM will be signaled to self
+            if failed to sending cross-silo data.
+        messages_max_size_in_bytes: The maximum length in bytes of
+            cross-silo messages.
+            If None, the default value of 500 MB is specified.
+        timeout_in_ms: The timeout in mili-seconds of a cross-silo RPC call.
+            It's 60000 by default.
+        http_header: The HTTP header, e.g. metadata in grpc, sent with the RPC request.
+            This won't override basic tcp headers, such as `user-agent`, but concat
+            them together.
+        max_concurrency: the max_concurrency of the sender/receiver proxy actor.
+    """
+
+    proxy_max_restarts: int = None
+    timeout_in_ms: int = 60000
+    messages_max_size_in_bytes: int = None
+    exit_on_sending_failure: Optional[bool] = False
+    serializing_allowed_list: Optional[Dict[str, str]] = None
+    send_resource_label: Optional[Dict[str, str]] = None
+    recv_resource_label: Optional[Dict[str, str]] = None
+    http_header: Optional[Dict[str, str]] = None
+    max_concurrency: Optional[int] = None
+
+    def __json__(self):
+        return json.dumps(self.__dict__)
+
+    @classmethod
+    def from_json(cls, json_str):
+        data = json.loads(json_str)
+        return cls(**data)
+
+    @classmethod
+    def from_dict(cls, data: Dict) -> 'CrossSiloMessageConfig':
+        """Initialize CrossSiloMessageConfig from a dictionary.
+
+        Args:
+            data (Dict): Dictionary with keys as member variable names.
+
+        Returns:
+            CrossSiloMessageConfig: An instance of CrossSiloMessageConfig.
+        """
+        # Get the attributes of the class
+        data = data or {}
+        attrs = [field.name for field in fields(cls)]
+        # Filter the dictionary to only include keys that are attributes of the class
+        filtered_data = {key: value for key, value in data.items() if key in attrs}
+        return cls(**filtered_data)
+
+
+@dataclass
+class GrpcCrossSiloMessageConfig(CrossSiloMessageConfig):
+    """A class to store parameters used for GRPC communication
+
+    Attributes:
+        grpc_retry_policy: a dict descibes the retry policy for
+            cross silo rpc call. If None, the following default retry policy
+            will be used. More details please refer to
+            `retry-policy <https://github.com/grpc/proposal/blob/master/A6-client-retries.md#retry-policy>`_. # noqa
+
+            .. code:: python
+                {
+                    "maxAttempts": 4,
+                    "initialBackoff": "0.1s",
+                    "maxBackoff": "1s",
+                    "backoffMultiplier": 2,
+                    "retryableStatusCodes": [
+                        "UNAVAILABLE"
+                    ]
+                }
+        grpc_channel_options: A list of tuples to store GRPC channel options,
+            e.g. [
+                    ('grpc.enable_retries', 1),
+                    ('grpc.max_send_message_length', 50 * 1024 * 1024)
+                ]
+    """
+
+    grpc_channel_options: List = None
+    grpc_retry_policy: Dict[str, str] = None
```

## fed/utils.py

```diff
@@ -9,39 +9,61 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
+import re
+import sys
 
-import jax
 import ray
 
+import fed
+from fed._private.compatible_utils import _compare_version_strings
 from fed.fed_object import FedObject
 
 logger = logging.getLogger(__name__)
 
 
+def get_package_version(package_name: str) -> str:
+    """
+    This utility function can retrieve the version number
+     of a Python library in string format, such as '4.23.4'.
+    You don't need to worry about the Python version.
+    When using version 3.7 and below, it uses the built-in `pkg_resources`.
+    When using Python 3.8 and above, it uses `importlib.metadata`.
+    """
+    curr_python_version = sys.version.split(" ")[0]
+    if _compare_version_strings(curr_python_version, '3.7.99'):
+        import importlib.metadata
+
+        return importlib.metadata.version(package_name)
+    else:
+        import pkg_resources
+
+        return pkg_resources.get_distribution(package_name).version
+
+
 def resolve_dependencies(current_party, current_fed_task_id, *args, **kwargs):
-    from fed.barriers import recv
+    from fed.proxy.barriers import recv
 
-    flattened_args, tree = jax.tree_util.tree_flatten((args, kwargs))
+    flattened_args, tree = fed.tree_util.tree_flatten((args, kwargs))
     indexes = []
     resolved = []
     for idx, arg in enumerate(flattened_args):
         if isinstance(arg, FedObject):
             indexes.append(idx)
             if arg.get_party() == current_party:
                 logger.debug(f"Insert fed object, arg.party={arg.get_party()}")
                 resolved.append(arg.get_ray_object_ref())
             else:
                 logger.debug(
-                    f'Insert recv_op, arg task id {arg.get_fed_task_id()}, current'
-                    'task id {current_fed_task_id}'
+                    f'Insert recv_op, arg task id {arg.get_fed_task_id()}, current '
+                    f'task id {current_fed_task_id}'
                 )
                 if arg.get_ray_object_ref() is not None:
                     # This code path indicates the ray object is already received in
                     # this party, so there is no need to receive it any longer.
                     received_ray_obj = arg.get_ray_object_ref()
                 else:
                     received_ray_obj = recv(
@@ -52,15 +74,15 @@
                     )
                     arg._cache_ray_object_ref(received_ray_obj)
                 resolved.append(received_ray_obj)
     if resolved:
         for idx, actual_val in zip(indexes, resolved):
             flattened_args[idx] = actual_val
 
-    resolved_args, resolved_kwargs = jax.tree_util.tree_unflatten(tree, flattened_args)
+    resolved_args, resolved_kwargs = fed.tree_util.tree_unflatten(flattened_args, tree)
     return resolved_args, resolved_kwargs
 
 
 def is_ray_object_refs(objects) -> bool:
     if isinstance(objects, ray.ObjectRef):
         return True
 
@@ -137,7 +159,67 @@
     def check_cython(x):
         return type(x).__name__ == "cython_function_or_method"
 
     # Check if function or method, respectively
     return check_cython(obj) or (
         hasattr(obj, "__func__") and check_cython(obj.__func__)
     )
+
+
+def dict2tuple(dic):
+    """
+    Convert a dictionary to a two-dimensional tuple, for example:
+    {'key': 'value'} => (('key', 'value'), ).
+    """
+    if dic is None or isinstance(dic, tuple):
+        return dic
+    elif isinstance(dic, dict):
+        return tuple((k, v) for k, v in dic.items())
+    else:
+        logger.warn(
+            f"Unable to convert type {type(dic)} to tuple" f"skip converting {dic}."
+        )
+        return dic
+
+
+def validate_address(address: str) -> None:
+    if address is None:
+        raise ValueError("The address shouldn't be None.")
+
+    # The specific case for `local` or `localhost`.
+    if address == 'local' or address == 'localhost':
+        return
+
+    # Rule 1: "ip:port" format
+    ip_port_pattern = r'^\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}:\d+$'
+    if re.match(ip_port_pattern, address):
+        return
+
+    # Rule 2: "hostname:port" format
+    hostname_port_pattern = r'^[a-zA-Z0-9.-]+:\d+$'
+    if re.match(hostname_port_pattern, address):
+        return
+
+    # Rule 3: https or http link
+    link_pattern = r'^(https?://).*'
+    if re.match(link_pattern, address):
+        return
+
+    error_msg = (
+        "The address format is invalid. It should be in one of the following formats:\n"  # noqa
+        "- `local` for starting a new cluster, or `localhost` for connecting a local cluster.\n"  # noqa
+        "- 'ip:port' format, where the IP needs to follow the IP address specifications and the port is a number.\n"  # noqa
+        "- 'hostname:port' format, where the hostname is a string and the port is a number.\n"  # noqa
+        "- An HTTPS or HTTP link starting with 'https://' or 'http://'."
+    )  # noqa
+    raise ValueError(error_msg)
+
+
+def validate_addresses(addresses: dict):
+    """
+    Validate whether the addresses is in correct forms.
+    """
+    for address in addresses.values():
+        assert (
+            isinstance(address, str) and address
+        ), f'Address should be string but got {address}.'
+        validate_address(address)
```

## fed/_private/compatible_utils.py

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import abc
 import ray
 import fed._private.constants as fed_constants
 
 import ray.experimental.internal_kv as ray_internal_kv
-from ray._private.gcs_utils import GcsClient
+from fed._private import constants
 
 
 def _compare_version_strings(version1, version2):
     """
     This utility function compares two version strings and returns
     True if version1 is greater, and False if they're equal, and
     False if version2 is greater.
@@ -97,14 +97,21 @@
 class InternalKv(AbstractInternalKv):
     """The internal kv class for non Ray client mode.
     """
     def __init__(self) -> None:
         super().__init__()
 
     def initialize(self):
+        try:
+            from ray._private.gcs_utils import GcsClient
+        except ImportError:
+            # The GcsClient was moved to `ray._raylet` module in `ray-2.5.0`.
+            assert _compare_version_strings(ray.__version__, "2.4.0")
+            from ray._raylet import GcsClient
+
         gcs_client = GcsClient(
             address=_get_gcs_address_from_ray_worker(),
             nums_reconnect_retry=10)
         return ray_internal_kv._initialize_internal_kv(gcs_client)
 
     def put(self, k, v):
         return ray_internal_kv._internal_kv_put(k, v)
@@ -148,16 +155,33 @@
     def reset(self):
         o = self._internal_kv_actor.reset.remote()
         return ray.get(o)
 
 
 def _init_internal_kv():
     """An internal API that initialize the internal kv object."""
-    from ray._private.client_mode_hook import is_client_mode_enabled
-    if is_client_mode_enabled:
-        kv_actor = ray.remote(InternalKv).options(name="_INTERNAL_KV_ACTOR").remote()
-        response = kv_actor._ping.remote()
-        ray.get(response)
-    return ClientModeInternalKv() if is_client_mode_enabled else InternalKv()
+    global kv
+    if kv is None:
+        from ray._private.client_mode_hook import is_client_mode_enabled
+        if is_client_mode_enabled:
+            kv_actor = ray.remote(InternalKv).options(
+                name="_INTERNAL_KV_ACTOR").remote()
+            response = kv_actor._ping.remote()
+            ray.get(response)
+        kv = ClientModeInternalKv() if is_client_mode_enabled else InternalKv()
+        kv.initialize()
+
+
+def _clear_internal_kv():
+    global kv
+    if kv is not None:
+        kv.delete(constants.KEY_OF_CLUSTER_CONFIG)
+        kv.delete(constants.KEY_OF_JOB_CONFIG)
+        kv.reset()
+        from ray._private.client_mode_hook import is_client_mode_enabled
+        if is_client_mode_enabled:
+            _internal_kv_actor = ray.get_actor("_INTERNAL_KV_ACTOR")
+            ray.kill(_internal_kv_actor)
+        kv = None
 
 
-kv = _init_internal_kv()
+kv = None
```

## fed/_private/constants.py

```diff
@@ -13,24 +13,22 @@
 # limitations under the License.
 
 
 KEY_OF_CLUSTER_CONFIG = b"CLUSTER_CONFIG"
 
 KEY_OF_JOB_CONFIG = b"JOB_CONFIG"
 
+KEY_OF_GRPC_METADATA = b"GRPC_METADATA"
+
 KEY_OF_CLUSTER_ADDRESSES = "CLUSTER_ADDRESSES"
 
 KEY_OF_CURRENT_PARTY_NAME = "CURRENT_PARTY_NAME"
 
 KEY_OF_TLS_CONFIG = "TLS_CONFIG"
 
-KEY_OF_CROSS_SILO_SERIALIZING_ALLOWED_LIST = "CROSS_SILO_SERIALIZING_ALLOWED_LIST" # noqa
-
-KEY_OF_CROSS_SILO_MESSAGES_MAX_SIZE_IN_BYTES = "CROSS_SILO_MESSAGES_MAX_SIZE_IN_BYTES" # noqa
-
-KEY_OF_CROSS_SILO_TIMEOUT_IN_SECONDS = "CROSS_SILO_TIMEOUT_IN_SECONDS"
+KEY_OF_CROSS_SILO_COMM_CONFIG_DICT = "CROSS_SILO_COMM_CONFIG_DICT"
 
 RAYFED_LOG_FMT = "%(asctime)s %(levelname)s %(filename)s:%(lineno)s [%(party)s] --  %(message)s" # noqa
 
 RAYFED_DATE_FMT = "%Y-%m-%d %H:%M:%S"
 
 RAY_VERSION_2_0_0_STR = "2.0.0"
```

## fed/_private/fed_actor.py

```diff
@@ -21,36 +21,36 @@
 logger = logging.getLogger(__name__)
 
 
 class FedActorHandle:
     def __init__(
         self,
         fed_class_task_id,
-        cluster,
+        addresses,
         cls,
         party,
         node_party,
         options,
     ) -> None:
         self._fed_class_task_id = fed_class_task_id
-        self._cluster = cluster
+        self._addresses = addresses
         self._body = cls
         self._party = party
         self._node_party = node_party
         self._options = options
         self._actor_handle = None
 
     def __getattr__(self, method_name: str):
         # User trying to call .bind() without a bind class method
         if method_name == "remote" and "remote" not in dir(self._body):
             raise AttributeError(f".remote() cannot be used again on {type(self)} ")
         # Raise an error if the method is invalid.
         getattr(self._body, method_name)
         call_node = FedActorMethod(
-            self._cluster,
+            self._addresses,
             self._party,
             self._node_party,
             self,
             method_name,
         ).options(**self._options)
         return call_node
 
@@ -86,21 +86,21 @@
         )
         return ray_object_ref
 
 
 class FedActorMethod:
     def __init__(
         self,
-        cluster,
+        addresses,
         party,
         node_party,
         fed_actor_handle,
         method_name,
     ) -> None:
-        self._cluster = cluster
+        self._addresses = addresses
         self._party = party  # Current party
         self._node_party = node_party
         self._fed_actor_handle = fed_actor_handle
         self._method_name = method_name
         self._options = {}
         self._fed_call_holder = FedCallHolder(node_party, self._execute_impl)
```

## fed/_private/fed_call_holder.py

```diff
@@ -13,21 +13,19 @@
 # limitations under the License.
 
 import logging
 
 # Set config in the very beginning to avoid being overwritten by other packages.
 logging.basicConfig(level=logging.INFO)
 
-import jax
-
 from fed._private.global_context import get_global_context
-from fed.barriers import send
+from fed.proxy.barriers import send
 from fed.fed_object import FedObject
 from fed.utils import resolve_dependencies
-
+from fed.tree_util import tree_flatten
 import fed.config as fed_config
 
 logger = logging.getLogger(__name__)
 
 
 class FedCallHolder:
     """
@@ -54,14 +52,17 @@
         self._submit_ray_task_func = submit_ray_task_func
 
     def options(self, **options):
         self._options = options
         return self
 
     def internal_remote(self, *args, **kwargs):
+        if not self._node_party:
+            raise ValueError("You should specify a party name on the fed actor.")
+
         # Generate a new fed task id for this call.
         fed_task_id = get_global_context().next_seq_id()
         if self._party == self._node_party:
             resolved_args, resolved_kwargs = resolve_dependencies(
                 self._party, fed_task_id, *args, **kwargs
             )
             # TODO(qwang): Handle kwargs.
@@ -70,15 +71,15 @@
                 return [
                     FedObject(self._node_party, fed_task_id, ref, i)
                     for i, ref in enumerate(ray_obj_ref)
                 ]
             else:
                 return FedObject(self._node_party, fed_task_id, ray_obj_ref)
         else:
-            flattened_args, _ = jax.tree_util.tree_flatten((args, kwargs))
+            flattened_args, _ = tree_flatten((args, kwargs))
             for arg in flattened_args:
                 # TODO(qwang): We still need to cosider kwargs and a deeply object_ref
                 # in this party.
                 if isinstance(arg, FedObject) and arg.get_party() == self._party:
                     if arg._was_sending_or_sent_to_party(self._node_party):
                         # This object was sending or sent to the target party, so no
                         # need to do it again.
```

## fed/_private/global_context.py

```diff
@@ -8,25 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from fed.cleanup import CleanupManager
+
 
 class GlobalContext:
     def __init__(self) -> None:
         self._seq_count = 0
+        self._cleanup_manager = CleanupManager()
 
-    def next_seq_id(self):
+    def next_seq_id(self) -> int:
         self._seq_count += 1
         return self._seq_count
 
+    def get_cleanup_manager(self) -> CleanupManager:
+        return self._cleanup_manager
+
 
 _global_context = None
 
 
 def get_global_context():
     global _global_context
     if _global_context is None:
         _global_context = GlobalContext()
     return _global_context
+
+
+def clear_global_context():
+    global _global_context
+    _global_context.get_cleanup_manager().graceful_stop()
+    _global_context = None
```

## fed/_private/serialization_utils.py

```diff
@@ -26,27 +26,30 @@
     *,
     fix_imports=True,
     encoding="ASCII",
     errors="strict",
     buffers=None,
 ):
     from sys import version_info
+
     assert version_info.major == 3
 
     if version_info.minor >= 8:
         import pickle as pickle
     else:
         import pickle5 as pickle
 
     class RestrictedUnpickler(pickle.Unpickler):
         def find_class(self, module, name):
             if _pickle_whitelist is None or (
                 module in _pickle_whitelist
-                and (_pickle_whitelist[module] is None or name in _pickle_whitelist[
-                    module])
+                and (
+                    _pickle_whitelist[module] is None
+                    or name in _pickle_whitelist[module]
+                )
             ):
                 return super().find_class(module, name)
 
             if module == "fed._private":  # TODO(qwang): Not sure if it works.
                 return super().find_class(module, name)
 
             # Forbid everything else.
@@ -59,15 +62,18 @@
         file, fix_imports=fix_imports, buffers=buffers, encoding=encoding, errors=errors
     ).load()
 
 
 def _apply_loads_function_with_whitelist():
     global _pickle_whitelist
 
-    _pickle_whitelist = fed_config.get_cluster_config().serializing_allowed_list
+    cross_silo_comm_config = fed_config.CrossSiloMessageConfig.from_dict(
+        fed_config.get_job_config().cross_silo_comm_config_dict
+    )
+    _pickle_whitelist = cross_silo_comm_config.serializing_allowed_list
     if _pickle_whitelist is None:
         return
 
     if "*" in _pickle_whitelist:
         _pickle_whitelist = None
         return
```

## Comparing `secretflow_rayfed-0.1.1a4.dist-info/LICENSE` & `secretflow_rayfed-0.2.0a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `secretflow_rayfed-0.1.1a4.dist-info/METADATA` & `secretflow_rayfed-0.2.0a0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: secretflow-rayfed
-Version: 0.1.1a4
+Version: 0.2.0a0
 Summary: A multiple parties joint, distributed execution engine based on Ray,to help build your own federated learning frameworks in minutes.
 Home-page: https://github.com/ray-project/rayfed
 Author: RayFed Team
 Author-email: rayfed-dev@googlegroups.com
 License: Apache 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jax (>=0.3.0)
-Requires-Dist: jaxlib (>=0.3.0)
 Requires-Dist: cloudpickle
 Requires-Dist: protobuf
 Requires-Dist: secretflow-ray (>=2.1.0)
 Requires-Dist: pickle5 (==0.0.11) ; python_version < "3.8"
 Provides-Extra: dev
 Requires-Dist: pylint ; extra == 'dev'
 
 # RayFed
-![docs building](https://readthedocs.org/projects/rayfed/badge/?version=latest) ![test on ray 2.0.0](https://github.com/ray-project/rayfed/actions/workflows/test_on_ray2.0.0.yml/badge.svg) ![test on ray 1.13.0](https://github.com/ray-project/rayfed/actions/workflows/test_on_ray1.13.0.yml/badge.svg)
+![docs building](https://readthedocs.org/projects/rayfed/badge/?version=latest) ![test on many rays](https://github.com/ray-project/rayfed/actions/workflows/unit_tests_on_ray_matrix.yml/badge.svg) ![test on ray 1.13.0](https://github.com/ray-project/rayfed/actions/workflows/test_on_ray1.13.0.yml/badge.svg)
 
 A multiple parties joint, distributed execution engine based on Ray, to help build your own federated learning frameworks in minutes.
 
 ## Overview
 **Note: This project is now in actively developing.**
 
 RayFed is a distributed computing framework for cross-parties federated learning.
@@ -51,37 +48,43 @@
 
 - **Very Large Scale Federated Computing and Training**  
   
   Powered by the scalabilities and the distributed abilities from Ray, large scale federated computing and training jobs are naturally supported.
 
 
 ## Supported Ray Versions
-| RayFed Versions | ray-1.13.0 | ray-2.0.0 | ray-2.1.0 | ray-2.2.0 | ray-2.3.0 |
-|:---------------:|:--------:|:--------:|:--------:|:--------:|:--------:|
-| 0.1.0           |✅      | ✅      | ✅      | ✅      | ❌      |
-| 0.2.0           |not released|not released|not released|not released|not released|
+| RayFed Versions | ray-1.13.0 | ray-2.0.0 | ray-2.1.0 | ray-2.2.0 | ray-2.3.0 | ray-2.4.0 |
+|:---------------:|:--------:|:--------:|:--------:|:--------:|:--------:|:--------:|
+| 0.1.0           |✅      | ✅      | ✅      | ✅      | ✅      | ✅      |
+| 0.2.0           |not released|not released|not released|not released|not released|not released|
 
 
 ## Installation
 Install it from pypi.
 
 ```shell
 pip install -U rayfed
 ```
 
+Install the nightly released version from pypi.
+
+```shell
+pip install -U rayfed-nightly
+```
 ## Quick Start
 
 This example shows how to aggregate values across two participators.
 
 ### Step 1: Write an Actor that Generates Value
 The `MyActor` increment its value by `num`. 
 This actor will be executed within the explicitly declared party.
 
 ```python
 import sys
+import ray
 import fed
 
 @fed.remote
 class MyActor:
     def __init__(self, value):
         self.value = value
 
@@ -115,30 +118,33 @@
 1. Create two `MyActor`s separately in each party, i.e. 'alice' and 'bob';
 2. Increment by '1' in alice and '2' in 'bob';
 3. Execute the aggregation function in party 'bob'.
 
 ### Step 4: Declare Cross-party Cluster & Init 
 ```python
 def main(party):
-    cluster = {
-        'alice': {'address': '127.0.0.1:11010'},
-        'bob': {'address': '127.0.0.1:11011'},
+    ray.init(address='local')
+
+    addresses = {
+        'alice': '127.0.0.1:11012',
+        'bob': '127.0.0.1:11011',
     }
-    fed.init(address='local', cluster=cluster, party=party)
+    fed.init(addresses=addresses, party=party)
 ```
-This first declares a two-party cluster, whose addresses corresponding to '127.0.0.1:11010' in 'alice' and '127.0.0.1:11011' in 'bob'.
+This first declares a two-party cluster, whose addresses corresponding to '127.0.0.1:11012' in 'alice' and '127.0.0.1:11011' in 'bob'.
 And then, the `fed.init` create a cluster in the specified party.
 Note that `fed.init` should be called twice, passing in the different party each time.
 
 When executing codes in step 1~3, the 'alice' cluster will only execute functions whose "party" are also declared as 'alice'.
 
 ### Put it together !
 Save below codes as `demo.py`: 
 ```python
 import sys
+import ray
 import fed
 
 
 @fed.remote
 class MyActor:
     def __init__(self, value):
         self.value = value
@@ -150,31 +156,34 @@
 
 @fed.remote
 def aggregate(val1, val2):
     return val1 + val2
 
 
 def main(party):
-    cluster = {
-        'alice': {'address': '127.0.0.1:11010'},
-        'bob': {'address': '127.0.0.1:11011'},
+    ray.init(address='local')
+
+    addresses = {
+        'alice': '127.0.0.1:11012',
+        'bob': '127.0.0.1:11011',
     }
-    fed.init(address='local', cluster=cluster, party=party)
+    fed.init(addresses=addresses, party=party)
 
     actor_alice = MyActor.party("alice").remote(1)
     actor_bob = MyActor.party("bob").remote(1)
 
     val_alice = actor_alice.inc.remote(1)
     val_bob = actor_bob.inc.remote(2)
 
     sum_val_obj = aggregate.party("bob").remote(val_alice, val_bob)
     result = fed.get(sum_val_obj)
     print(f"The result in party {party} is {result}")
 
     fed.shutdown()
+    ray.shutdown()
 
 
 if __name__ == "__main__":
     assert len(sys.argv) == 2, 'Please run this script with party.'
     main(sys.argv[1])
 
 ```
@@ -202,9 +211,7 @@
 Then you will get `The result in party alice is 5` on the first terminal screen and `The result in party bob is 5` on the second terminal screen.
 
 Figure shows the execution under the hood:
 ![ppeH68x.png](https://s1.ax1x.com/2023/03/08/ppeH68x.png)
 
 ## Running untrusted codes
 As a general rule: Always execute untrusted codes inside a sandbox (e.g., [nsjail](https://github.com/google/nsjail)).
-
-
```

## Comparing `secretflow_rayfed-0.1.1a4.dist-info/RECORD` & `secretflow_rayfed-0.2.0a0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,40 @@
-fed/__init__.py,sha256=6Xds1gLndBN-E4GBTuxnc7gf3Zw_D8iNejjA3JTjWnc,853
-fed/api.py,sha256=EtcFX22S0gb9jmlN_0zcnpLJUE-K9PkcXyETbP7LHYg,15277
+fed/__init__.py,sha256=WN5lu4fAPUVxzlL4T6Z_ygmP3d9-DAVLWFRkd92SVmc,859
+fed/api.py,sha256=yk9NXWixcFmRDjd0o4X-MQkRojQSfego7UwIofxR5Vw,13964
 fed/barriers.py,sha256=_ZWzDqaiKNrx9HGt_Yw4b-483r_yR3pqKB_xlv7JarM,15513
-fed/cleanup.py,sha256=t0ftotRE2wYakf399mRtFRPiEzknQviaguNvsZJ4Q_U,3025
-fed/config.py,sha256=qB54s-COypgD6LtI3QypwkMK6RR7gM63HZt6YgiMHMA,1745
+fed/cleanup.py,sha256=he50D41g9pxbay3IvCMIZpqEOYyScbHYL6uxnPp5Hxo,3668
+fed/config.py,sha256=4KQHMKJVKZWE-pGX6IBhQ1ocEpq50DtOeWRCy0sLgDA,6254
 fed/fed_object.py,sha256=l2BRa9WZ3jqXSDjwFPURcAIK8XkH8A5UYA_OcY4TOD0,2877
-fed/utils.py,sha256=6Xguz67MpUdprvTaaQWIrnZk9o3MYTQy2K2sc9-LGyk,4806
+fed/tree_util.py,sha256=J29bCmCF_ChHUdXYBXDtItV6dmiHmhCskCXrmtSn1Ag,7912
+fed/utils.py,sha256=X_brj4FeyF4ePfZ-u4u7dJJftvqFFrgZ0vOH48w_yeg,7614
 fed/_private/__init__.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
 fed/_private/api.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
-fed/_private/compatible_utils.py,sha256=ZhaLX797pZ-PnwlNIMgRzkwrysW0wbruQLHm-WsNUUs,4487
-fed/_private/constants.py,sha256=Gx3BCM6ti1VJWsnaN3oYhklIEvfYm9TkCDXCbRmziVw,1227
-fed/_private/fed_actor.py,sha256=8nqXO_l9yOno5duMiEhWagp9q9-w696erKos-RgcnoU,3837
-fed/_private/fed_call_holder.py,sha256=RqxDPW1enEWA0wmYnqFcHC_xY45M-Lagite6QPIy4n4,3813
-fed/_private/global_context.py,sha256=QUEE9RttgdWOHvXZsycKnxeMTKo1E0nGp7Zyxnxb_Zw,933
+fed/_private/compatible_utils.py,sha256=4JdcL1qGlLwQx6DMBAs5lphPxOIJyz1YqYbS1Hq8Ruk,5269
+fed/_private/constants.py,sha256=32zdgXupZ13qbexm0TXwyL3WGVQeamRH3SC7CCd-uFw,1078
+fed/_private/fed_actor.py,sha256=juzgqrBsycl1kKaND-HwBeG0YOBcvk5rGcOQutA8RJ0,3851
+fed/_private/fed_call_holder.py,sha256=RDD3fet8CD2clUNfSX6ByXViaYlkcLQNDxaAADU-Ld4,3947
+fed/_private/global_context.py,sha256=JtRCuBHju_8OcIbtfNvhzPR9bDxeD_X8bRe-8SogNtY,1262
 fed/_private/grpc_options.py,sha256=_r43xjQfg0JmD0T447wHV42EYhP0YpBubsGKG22TuN4,2859
-fed/_private/serialization_utils.py,sha256=l63nacVabcyKpys9tVT2zUMmKecimeVflsJ6v45AYvc,2386
+fed/_private/serialization_utils.py,sha256=_yJdd97df1BCUU2PNe9R1L04UlbgjBGw4N8GmTTB0rs,2559
 fed/grpc/__init__.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
 fed/grpc/fed_pb2.py,sha256=CKRJyBIx8MG4XtqtARL9ETFEyIsX2ksO0IVU9JgBhWQ,5608
 fed/grpc/fed_pb2_grpc.py,sha256=PsTotUwY4gEHWV0gQnPwpoQWdNJCczNZti6bJBYFj5Q,2955
-secretflow_rayfed-0.1.1a4.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-secretflow_rayfed-0.1.1a4.dist-info/METADATA,sha256=1vUxpg7dOLobRPouYemvvDnD76SC-RH7Pss1hxZvYsk,7213
-secretflow_rayfed-0.1.1a4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-secretflow_rayfed-0.1.1a4.dist-info/top_level.txt,sha256=5gd1qhbpzLAi36ONV8p_s65_-iAiOSwFljYh-ONEwts,4
-secretflow_rayfed-0.1.1a4.dist-info/RECORD,,
+fed/grpc/pb3/__init__.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
+fed/grpc/pb3/fed_pb2.py,sha256=CKRJyBIx8MG4XtqtARL9ETFEyIsX2ksO0IVU9JgBhWQ,5608
+fed/grpc/pb3/fed_pb2_grpc.py,sha256=JabOU62bPbpb0uCeNYNV4W8uNq1nIiPaGGLU4tkUp8E,2959
+fed/grpc/pb4/__init__.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
+fed/grpc/pb4/fed_pb2.py,sha256=0JbbKEqCKx31MiIMVU3UOJ93ZgTbAr6g51z1EgIRNG8,2113
+fed/grpc/pb4/fed_pb2_grpc.py,sha256=S4kUT0IuU39iRacY9RDdRS1DK2JI_ivO1U6tPxxtdng,2980
+fed/proxy/__init__.py,sha256=zjmMrqPxcVeXa7sMvRccSdnmV8_A73tETlvUJtAd0lA,613
+fed/proxy/barriers.py,sha256=HoGtl1B8h7nEjeQp_8u0-8TaW1wjKAlFUHRUkooL6Iw,14523
+fed/proxy/base_proxy.py,sha256=gtukHs1GZEXhfa9oir_uqPigxL31FBPIUkV2raW4g_8,2661
+fed/proxy/brpc_link/__init__.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
+fed/proxy/brpc_link/link.py,sha256=1Sqya3oG0fb23K_acatJ-ob-TJWy9GMPb1ES0T51KkA,3983
+fed/proxy/brpc_link/link_config.py,sha256=_IqzexHX9bEGXTkEAICZsBtpbPsgW82byPVXVY5244k,2114
+fed/proxy/grpc/__init__.py,sha256=MDXwlZ-y7_o-tfqh8DVkjlO-6MlWqwLdbSIZUJfXtF0,581
+fed/proxy/grpc/grpc_options.py,sha256=8zdKKqcpvWQG3nTNzvgk0RLLbumocg7exX-ZfbQMv2c,2569
+fed/proxy/grpc/grpc_proxy.py,sha256=OHj8F7igHnPvAfPq8qPRGfu04TMLzCnTthFEAmd8tmM,12361
+secretflow_rayfed-0.2.0a0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+secretflow_rayfed-0.2.0a0.dist-info/METADATA,sha256=fxY07Ai_3Ii7hk43EICVi54KRuTD44XK82fIn8veEaA,7308
+secretflow_rayfed-0.2.0a0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+secretflow_rayfed-0.2.0a0.dist-info/top_level.txt,sha256=5gd1qhbpzLAi36ONV8p_s65_-iAiOSwFljYh-ONEwts,4
+secretflow_rayfed-0.2.0a0.dist-info/RECORD,,
```

