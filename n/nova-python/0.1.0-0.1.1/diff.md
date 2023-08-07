# Comparing `tmp/nova_python-0.1.0.tar.gz` & `tmp/nova_python-0.1.1.tar.gz`

## Comparing `nova_python-0.1.0.tar` & `nova_python-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 nova_python-0.1.0/Cargo.toml
--rwxrwxrwx   0     1000      998    35184 2023-08-07 00:42:06.000000 nova_python-0.1.0/LICENSE
--rwxrwxrwx   0     1000      998     1029 2023-08-07 08:22:06.000000 nova_python-0.1.0/README.md
--rwxrwxrwx   0     1000      998      472 2023-08-07 07:17:59.000000 nova_python-0.1.0/pyproject.toml
--rwxrwxrwx   0     1000      998     5384 2023-08-07 07:59:05.000000 nova_python-0.1.0/src/lib.rs
--rwxrwxrwx   0     1000      998    30430 2023-08-07 05:00:51.000000 nova_python-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 nova_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 nova_python-0.1.1/Cargo.toml
+-rwxrwxrwx   0     1000      998      945 2023-08-07 05:15:38.000000 nova_python-0.1.1/.gitignore
+-rwxrwxrwx   0     1000      998    35184 2023-08-07 00:42:06.000000 nova_python-0.1.1/LICENSE
+-rwxrwxrwx   0     1000      998     1663 2023-08-07 09:32:33.000000 nova_python-0.1.1/README.md
+-rwxrwxrwx   0     1000      998      544 2023-08-07 09:37:18.000000 nova_python-0.1.1/pyproject.toml
+-rwxrwxrwx   0     1000      998     6258 2023-08-07 09:16:40.000000 nova_python-0.1.1/src/lib.rs
+-rwxrwxrwx   0     1000      998    30430 2023-08-07 08:57:10.000000 nova_python-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 nova_python-0.1.1/PKG-INFO
```

### Comparing `nova_python-0.1.0/LICENSE` & `nova_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nova_python-0.1.0/README.md` & `nova_python-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,104 @@
 00000000: 2320 6e6f 7661 2d70 7974 686f 6e0d 0af0  # nova-python...
 00000010: 9f90 8d20 5079 7468 6f6e 206c 6962 7261  ... Python libra
 00000020: 7279 2066 6f72 2061 6363 6573 7369 6e67  ry for accessing
 00000030: 2074 6865 204e 6f76 6120 4150 490d 0a0d   the Nova API...
-00000040: 0a23 2320 5573 6167 6520 2323 0d0a 496d  .## Usage ##..Im
-00000050: 706f 7274 2074 6865 206d 6f64 756c 650d  port the module.
-00000060: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00000070: 206e 6f76 615f 7079 7468 6f6e 2069 6d70   nova_python imp
-00000080: 6f72 7420 456e 6470 6f69 6e74 732c 204d  ort Endpoints, M
-00000090: 6f64 656c 732c 204e 6f76 6143 6c69 656e  odels, NovaClien
-000000a0: 740d 0a60 6060 0d0a 0d0a 4372 6561 7465  t..```....Create
-000000b0: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
-000000c0: 4e6f 7661 436c 6965 6e74 2c20 7573 696e  NovaClient, usin
-000000d0: 6720 796f 7572 2041 5049 206b 6579 0d0a  g your API key..
-000000e0: 0d0a 6060 6070 7974 686f 6e0d 0a63 6c69  ..```python..cli
-000000f0: 656e 7420 3d20 4e6f 7661 436c 6965 6e74  ent = NovaClient
-00000100: 2822 594f 5552 5f41 5049 5f4b 4559 2229  ("YOUR_API_KEY")
-00000110: 0d0a 6060 600d 0a0d 0a6e 6f76 615f 7079  ..```....nova_py
-00000120: 7468 6f6e 2063 7572 7265 6e74 6c79 2069  thon currently i
-00000130: 6d70 6c65 6d65 6e74 7320 7477 6f20 656e  mplements two en
-00000140: 756d 733a 2045 6e64 706f 696e 7473 2061  ums: Endpoints a
-00000150: 6e64 204d 6f64 656c 732e 2054 686f 7365  nd Models. Those
-00000160: 2063 6f6e 7461 696e 3a0d 0a0d 0a23 2323   contain:....###
-00000170: 2045 6e64 706f 696e 7473 2023 2323 0d0a   Endpoints ###..
-00000180: 2a20 6045 6e64 706f 696e 7473 2e43 4841  * `Endpoints.CHA
-00000190: 545f 434f 4d50 4c45 5449 4f4e 600d 0a0d  T_COMPLETION`...
-000001a0: 0a2a 2a4d 6f64 656c 732a 2a0d 0a2a 2060  .**Models**..* `
-000001b0: 4d6f 6465 6c73 2e47 5054 3360 0d0a 2b20  Models.GPT3`..+ 
-000001c0: 604d 6f64 656c 732e 4750 5434 600d 0a0d  `Models.GPT4`...
-000001d0: 0a4e 6f77 2c20 746f 206d 616b 6520 6120  .Now, to make a 
-000001e0: 7265 7175 6573 742c 2075 7365 2074 6865  request, use the
-000001f0: 2060 6d61 6b65 5f72 6571 7565 7374 6020   `make_request` 
-00000200: 6675 6e63 7469 6f6e 2e0d 0a0d 0a60 6060  function.....```
-00000210: 7079 7468 6f6e 0d0a 6672 6f6d 206e 6f76  python..from nov
-00000220: 615f 7079 7468 6f6e 2069 6d70 6f72 7420  a_python import 
-00000230: 456e 6470 6f69 6e74 732c 204d 6f64 656c  Endpoints, Model
-00000240: 732c 204e 6f76 6143 6c69 656e 740d 0a63  s, NovaClient..c
-00000250: 6c69 656e 7420 3d20 4e6f 7661 436c 6965  lient = NovaClie
-00000260: 6e74 2822 594f 5552 5f41 5049 5f4b 4559  nt("YOUR_API_KEY
-00000270: 2229 0d0a 0d0a 636c 6965 6e74 2e6d 616b  ")....client.mak
-00000280: 655f 7265 7175 6573 7428 0d0a 2020 2020  e_request(..    
-00000290: 656e 6470 6f69 6e74 3d45 6e64 706f 696e  endpoint=Endpoin
-000002a0: 7473 2e43 4841 545f 434f 4d50 4c45 5449  ts.CHAT_COMPLETI
-000002b0: 4f4e 2c0d 0a20 2020 206d 6f64 656c 3d4d  ON,..    model=M
-000002c0: 6f64 656c 732e 4750 5433 2c0d 0a20 2020  odels.GPT3,..   
-000002d0: 2064 6174 613d 5b0d 0a20 2020 2020 2020   data=[..       
-000002e0: 207b 2272 6f6c 6522 3a20 2273 7973 7465   {"role": "syste
-000002f0: 6d22 2c20 2263 6f6e 7465 6e74 223a 2022  m", "content": "
-00000300: 596f 7520 6172 6520 6120 6865 6c70 6675  You are a helpfu
-00000310: 6c20 6173 7369 7374 616e 742e 227d 2c0d  l assistant."},.
-00000320: 0a20 2020 2020 2020 207b 2272 6f6c 6522  .        {"role"
-00000330: 3a20 2275 7365 7222 2c20 2263 6f6e 7465  : "user", "conte
-00000340: 6e74 223a 2022 4865 6c6c 6f21 227d 0d0a  nt": "Hello!"}..
-00000350: 2020 2020 5d0d 0a29 0d0a 6060 600d 0a0d      ]..)..```...
-00000360: 0a49 6620 6576 6572 7974 6869 6e67 2067  .If everything g
-00000370: 6f65 7320 746f 2070 6c61 6e2c 2079 6f75  oes to plan, you
-00000380: 276c 6c20 7265 6365 6976 6520 6120 7374  'll receive a st
-00000390: 7269 6e67 2063 6f6e 7461 696e 696e 6720  ring containing 
-000003a0: 4a53 4f4e 2d44 6174 612c 2077 6869 6368  JSON-Data, which
-000003b0: 2079 6f75 2063 616e 2074 6865 6e20 7573   you can then us
-000003c0: 6520 696e 2079 6f75 7220 7072 6f6a 6563  e in your projec
-000003d0: 742e 2020 0d0a 2a48 6170 7079 2070 726f  t.  ..*Happy pro
-000003e0: 6d70 7469 6e67 212a 0d0a 0d0a 4d61 6465  mpting!*....Made
-000003f0: 2077 6974 6820 f09f a9b8 2062 7920 4c65   with .... by Le
-00000400: 616e 6465 72                             ander
+00000040: 0a23 2320 5573 6167 6520 2323 0d0a 496e  .## Usage ##..In
+00000050: 7374 616c 6c20 7468 6520 6d6f 6475 6c65  stall the module
+00000060: 2028 5468 6973 2072 6571 7569 7265 7320   (This requires 
+00000070: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000080: 2f72 7573 7475 702e 7273 2f22 3e43 6172  /rustup.rs/">Car
+00000090: 676f 3c2f 613e 2920 200d 0a60 6060 7368  go</a>)  ..```sh
+000000a0: 0d0a 2420 7069 7020 696e 7374 616c 6c20  ..$ pip install 
+000000b0: 6e6f 7661 2d70 7974 686f 6e0d 0a60 6060  nova-python..```
+000000c0: 0d0a 0d0a 496d 706f 7274 2074 6865 206d  ....Import the m
+000000d0: 6f64 756c 650d 0a60 6060 7079 7468 6f6e  odule..```python
+000000e0: 0d0a 6672 6f6d 206e 6f76 615f 7079 7468  ..from nova_pyth
+000000f0: 6f6e 2069 6d70 6f72 7420 456e 6470 6f69  on import Endpoi
+00000100: 6e74 732c 204d 6f64 656c 732c 204e 6f76  nts, Models, Nov
+00000110: 6143 6c69 656e 740d 0a60 6060 0d0a 0d0a  aClient..```....
+00000120: 4372 6561 7465 2061 6e20 696e 7374 616e  Create an instan
+00000130: 6365 206f 6620 4e6f 7661 436c 6965 6e74  ce of NovaClient
+00000140: 2c20 7573 696e 6720 796f 7572 2041 5049  , using your API
+00000150: 206b 6579 0d0a 0d0a 6060 6070 7974 686f   key....```pytho
+00000160: 6e0d 0a63 6c69 656e 7420 3d20 4e6f 7661  n..client = Nova
+00000170: 436c 6965 6e74 2822 594f 5552 5f41 5049  Client("YOUR_API
+00000180: 5f4b 4559 2229 0d0a 6060 600d 0a0d 0a6e  _KEY")..```....n
+00000190: 6f76 615f 7079 7468 6f6e 2063 7572 7265  ova_python curre
+000001a0: 6e74 6c79 2069 6d70 6c65 6d65 6e74 7320  ntly implements 
+000001b0: 7477 6f20 656e 756d 733a 2045 6e64 706f  two enums: Endpo
+000001c0: 696e 7473 2061 6e64 204d 6f64 656c 732e  ints and Models.
+000001d0: 2054 686f 7365 2063 6f6e 7461 696e 3a0d   Those contain:.
+000001e0: 0a0d 0a2a 2a45 6e64 706f 696e 7473 2a2a  ...**Endpoints**
+000001f0: 0d0a 2a20 6045 6e64 706f 696e 7473 2e43  ..* `Endpoints.C
+00000200: 4841 545f 434f 4d50 4c45 5449 4f4e 600d  HAT_COMPLETION`.
+00000210: 0a2a 2060 456e 6470 6f69 6e74 732e 4d4f  .* `Endpoints.MO
+00000220: 4445 5241 5449 4f4e 600d 0a0d 0a2a 2a4d  DERATION`....**M
+00000230: 6f64 656c 732a 2a0d 0a2a 2060 4d6f 6465  odels**..* `Mode
+00000240: 6c73 2e47 5054 3360 0d0a 2a20 604d 6f64  ls.GPT3`..* `Mod
+00000250: 656c 732e 4750 5434 600d 0a2a 2060 4d6f  els.GPT4`..* `Mo
+00000260: 6465 6c73 2e4d 4f44 4552 4154 494f 4e5f  dels.MODERATION_
+00000270: 4c41 5445 5354 600d 0a2a 2060 4d6f 6465  LATEST`..* `Mode
+00000280: 6c73 2e4d 4f44 4552 4154 494f 4e5f 5354  ls.MODERATION_ST
+00000290: 4142 4c45 6020 200d 0a0d 0a4e 6f77 2c20  ABLE`  ....Now, 
+000002a0: 746f 206d 616b 6520 6120 7265 7175 6573  to make a reques
+000002b0: 742c 2075 7365 2074 6865 2060 6d61 6b65  t, use the `make
+000002c0: 5f72 6571 7565 7374 6020 6675 6e63 7469  _request` functi
+000002d0: 6f6e 2e20 466f 7220 6578 616d 706c 653a  on. For example:
+000002e0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+000002f0: 726f 6d20 6e6f 7661 5f70 7974 686f 6e20  rom nova_python 
+00000300: 696d 706f 7274 2045 6e64 706f 696e 7473  import Endpoints
+00000310: 2c20 4d6f 6465 6c73 2c20 4e6f 7661 436c  , Models, NovaCl
+00000320: 6965 6e74 0d0a 636c 6965 6e74 203d 204e  ient..client = N
+00000330: 6f76 6143 6c69 656e 7428 2259 4f55 525f  ovaClient("YOUR_
+00000340: 4150 495f 4b45 5922 290d 0a0d 0a63 6c69  API_KEY")....cli
+00000350: 656e 742e 6d61 6b65 5f72 6571 7565 7374  ent.make_request
+00000360: 280d 0a20 2020 2065 6e64 706f 696e 743d  (..    endpoint=
+00000370: 456e 6470 6f69 6e74 732e 4348 4154 5f43  Endpoints.CHAT_C
+00000380: 4f4d 504c 4554 494f 4e2c 0d0a 2020 2020  OMPLETION,..    
+00000390: 6d6f 6465 6c3d 4d6f 6465 6c73 2e47 5054  model=Models.GPT
+000003a0: 332c 0d0a 2020 2020 6461 7461 3d5b 0d0a  3,..    data=[..
+000003b0: 2020 2020 2020 2020 7b22 726f 6c65 223a          {"role":
+000003c0: 2022 7379 7374 656d 222c 2022 636f 6e74   "system", "cont
+000003d0: 656e 7422 3a20 2259 6f75 2061 7265 2061  ent": "You are a
+000003e0: 2068 656c 7066 756c 2061 7373 6973 7461   helpful assista
+000003f0: 6e74 2e22 7d2c 0d0a 2020 2020 2020 2020  nt."},..        
+00000400: 7b22 726f 6c65 223a 2022 7573 6572 222c  {"role": "user",
+00000410: 2022 636f 6e74 656e 7422 3a20 2248 656c   "content": "Hel
+00000420: 6c6f 2122 7d0d 0a20 2020 205d 0d0a 290d  lo!"}..    ]..).
+00000430: 0a60 6060 0d0a 0d0a 6f72 0d0a 0d0a 6060  .```....or....``
+00000440: 6070 7974 686f 6e0d 0a66 726f 6d20 6e6f  `python..from no
+00000450: 7661 5f70 7974 686f 6e20 696d 706f 7274  va_python import
+00000460: 2045 6e64 706f 696e 7473 2c20 4d6f 6465   Endpoints, Mode
+00000470: 6c73 2c20 4e6f 7661 436c 6965 6e74 0d0a  ls, NovaClient..
+00000480: 636c 6965 6e74 203d 204e 6f76 6143 6c69  client = NovaCli
+00000490: 656e 7428 2259 4f55 525f 4150 495f 4b45  ent("YOUR_API_KE
+000004a0: 5922 290d 0a0d 0a63 6c69 656e 742e 6d61  Y")....client.ma
+000004b0: 6b65 5f72 6571 7565 7374 280d 0a20 2020  ke_request(..   
+000004c0: 2065 6e64 706f 696e 743d 456e 6470 6f69   endpoint=Endpoi
+000004d0: 6e74 732e 4d4f 4445 5241 5449 4f4e 2c0d  nts.MODERATION,.
+000004e0: 0a20 2020 206d 6f64 656c 3d4d 6f64 656c  .    model=Model
+000004f0: 732e 4d4f 4445 5241 5449 4f4e 5f53 5441  s.MODERATION_STA
+00000500: 424c 452c 0d0a 2020 2020 6461 7461 3d5b  BLE,..    data=[
+00000510: 7b22 696e 7075 7422 3a20 2249 276d 2067  {"input": "I'm g
+00000520: 6f69 6e67 2074 6f20 6b69 6c6c 2074 6865  oing to kill the
+00000530: 6d2e 227d 5d0d 0a29 0d0a 6060 600d 0a0d  m."}]..)..```...
+00000540: 0a0d 0a49 6620 6576 6572 7974 6869 6e67  ...If everything
+00000550: 2067 6f65 7320 746f 2070 6c61 6e2c 2079   goes to plan, y
+00000560: 6f75 276c 6c20 7265 6365 6976 6520 6120  ou'll receive a 
+00000570: 7374 7269 6e67 2063 6f6e 7461 696e 696e  string containin
+00000580: 6720 4a53 4f4e 2d44 6174 612c 2077 6869  g JSON-Data, whi
+00000590: 6368 2079 6f75 2063 616e 2074 6865 6e20  ch you can then 
+000005a0: 7573 6520 696e 2079 6f75 7220 7072 6f6a  use in your proj
+000005b0: 6563 742e 2020 0d0a 2a48 6170 7079 2070  ect.  ..*Happy p
+000005c0: 726f 6d70 7469 6e67 212a 0d0a 0d0a 2323  rompting!*....##
+000005d0: 2046 4151 2023 230d 0a2a 2a51 3a2a 2a20   FAQ ##..**Q:** 
+000005e0: 4920 6765 7420 616e 2065 7272 6f72 2077  I get an error w
+000005f0: 6865 6e20 696e 7374 616c 6c69 6e67 2074  hen installing t
+00000600: 6865 2070 6163 6b61 6765 2020 0d0a 2a2a  he package  ..**
+00000610: 413a 2a2a 204d 616b 6520 796f 7520 7375  A:** Make you su
+00000620: 7265 2c20 7468 6174 2079 6f75 2068 6176  re, that you hav
+00000630: 6520 3c61 2068 7265 663d 2268 7474 7073  e <a href="https
+00000640: 3a2f 2f72 7573 7475 702e 7273 2f22 3e43  ://rustup.rs/">C
+00000650: 6172 676f 3c2f 613e 2069 6e73 7461 6c6c  argo</a> install
+00000660: 6564 0d0a 0d0a 4d61 6465 2077 6974 6820  ed....Made with 
+00000670: f09f a9b8 2062 7920 4c65 616e 6465 72    .... by Leander
```

### Comparing `nova_python-0.1.0/src/lib.rs` & `nova_python-0.1.1/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 #[pyclass(module = "nova_python", frozen)]
 #[derive(PartialEq)]
 #[derive(Clone)]
 enum Models {
     #[pyo3(name = "GPT3")]
     Gpt3,
     #[pyo3(name = "GPT4")]
-    Gpt4
+    Gpt4,
+    #[pyo3(name = "MODERATION_LATEST")]
+    ModerationLatest,
+    #[pyo3(name = "MODERATION_STABLE")]
+    ModerationStable,
 }
 
 #[pyclass(module = "nova_python", frozen)]
 #[derive(PartialEq)]
 #[derive(Clone)]
 enum Endpoints {
     #[pyo3(name = "CHAT_COMPLETION")]
     ChatCompletion,
+    #[pyo3(name = "MODERATION")]
+    Moderation,
 }
 
 #[pyclass(module = "nova_python", frozen)]
 struct NovaClient {
     #[pyo3(get)]
     api_key: String,
     url: String
@@ -80,14 +86,15 @@
 
 }
 
 impl NovaClient {
     fn get_request_url(&self, endpoint: &Endpoints) -> PyResult<String> {
         match endpoint {
             Endpoints::ChatCompletion => Ok(format!("{}chat/completions", self.url)),
+            Endpoints::Moderation => Ok(format!("{}moderations", self.url)),
             _ => Err(NovaClient::get_invalid_endpoint_error())
         }
     }
 
     fn get_request_body(&self, endpoint: &Endpoints, model: &Models, data: Vec<Py<PyDict>>) -> PyResult<String> {
         let request_data = Python::with_gil(|py| {
             let mut request_data = Vec::new();
@@ -101,14 +108,16 @@
         });
 
         let mut request_body = String::from("{");
 
         let model = match model {
             Models::Gpt3 => "gpt-3.5-turbo",
             Models::Gpt4 => "gpt-4",
+            Models::ModerationLatest => "text-moderation-latest",
+            Models::ModerationStable => "text-moderation-stable",
             _ => return Err(NovaClient::get_invalid_model_error())
         };
         request_body.push_str(&format!("\"model\":\"{}\"", model));
 
         if endpoint == &Endpoints::ChatCompletion {
             request_body.push_str(",\"messages\":[");
 
@@ -128,15 +137,24 @@
 
             if request_body.ends_with(",") {
                 request_body.pop();
             }
             
             request_body.push_str("]");
 
-        } else {
+        } 
+        
+        else if endpoint == &Endpoints::Moderation {
+            request_body.push_str(",\"input\":");
+
+            let input = format!("\"{}\"", request_data.get(0).unwrap().get("input").unwrap());
+            request_body.push_str(&input);
+        }
+
+        else {
             return Err(NovaClient::get_invalid_endpoint_error());
         }
 
         request_body.push_str("}");
         Ok(request_body)
     }
 
@@ -165,14 +183,22 @@
     if endpoint == &Endpoints::ChatCompletion {
         if [Models::Gpt3, Models::Gpt4].contains(model) {
             return true;
         } else {
             return false;
         }
     }
+    
+    else if endpoint == &Endpoints::Moderation {
+        if [Models::ModerationStable, Models::ModerationLatest].contains(model) {
+            return true;
+        } else {
+            return false;
+        }
+    }
 
     false
 }
 
 fn key_is_valid(api_key: &str) -> bool {
     if !api_key.starts_with("nv-") {
         return false;
```

### Comparing `nova_python-0.1.0/Cargo.lock` & `nova_python-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "nova-python"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "reqwest",
  "tokio",
 ]
 
 [[package]]
```

### Comparing `nova_python-0.1.0/PKG-INFO` & `nova_python-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 7661  : 2.1.Name: nova
 00000020: 2d70 7974 686f 6e0a 5665 7273 696f 6e3a  -python.Version:
-00000030: 2030 2e31 2e30 0a43 6c61 7373 6966 6965   0.1.0.Classifie
+00000030: 2030 2e31 2e31 0a43 6c61 7373 6966 6965   0.1.1.Classifie
 00000040: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
 00000050: 616e 6775 6167 6520 3a3a 2052 7573 740a  anguage :: Rust.
 00000060: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
 00000070: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000080: 203a 3a20 5079 7468 6f6e 203a 3a20 496d   :: Python :: Im
 00000090: 706c 656d 656e 7461 7469 6f6e 203a 3a20  plementation :: 
 000000a0: 4350 7974 686f 6e0a 436c 6173 7369 6669  CPython.Classifi
@@ -14,78 +14,119 @@
 000000d0: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
 000000e0: 7469 6f6e 203a 3a20 5079 5079 0a4c 6963  tion :: PyPy.Lic
 000000f0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
 00000100: 5345 0a53 756d 6d61 7279 3a20 f09f 908d  SE.Summary: ....
 00000110: 2050 7974 686f 6e20 6c69 6272 6172 7920   Python library 
 00000120: 666f 7220 6163 6365 7373 696e 6720 7468  for accessing th
 00000130: 6520 4e6f 7661 2041 5049 0a41 7574 686f  e Nova API.Autho
-00000140: 723a 204c 6561 6e64 6572 0a52 6571 7569  r: Leander.Requi
-00000150: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
-00000160: 370a 4465 7363 7269 7074 696f 6e2d 436f  7.Description-Co
-00000170: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000180: 2f6d 6172 6b64 6f77 6e3b 2063 6861 7273  /markdown; chars
-00000190: 6574 3d55 5446 2d38 3b20 7661 7269 616e  et=UTF-8; varian
-000001a0: 743d 4746 4d0a 0a23 206e 6f76 612d 7079  t=GFM..# nova-py
-000001b0: 7468 6f6e 0d0a f09f 908d 2050 7974 686f  thon...... Pytho
-000001c0: 6e20 6c69 6272 6172 7920 666f 7220 6163  n library for ac
-000001d0: 6365 7373 696e 6720 7468 6520 4e6f 7661  cessing the Nova
-000001e0: 2041 5049 0d0a 0d0a 2323 2055 7361 6765   API....## Usage
-000001f0: 2023 230d 0a49 6d70 6f72 7420 7468 6520   ##..Import the 
-00000200: 6d6f 6475 6c65 0d0a 6060 6070 7974 686f  module..```pytho
-00000210: 6e0d 0a66 726f 6d20 6e6f 7661 5f70 7974  n..from nova_pyt
-00000220: 686f 6e20 696d 706f 7274 2045 6e64 706f  hon import Endpo
-00000230: 696e 7473 2c20 4d6f 6465 6c73 2c20 4e6f  ints, Models, No
-00000240: 7661 436c 6965 6e74 0d0a 6060 600d 0a0d  vaClient..```...
-00000250: 0a43 7265 6174 6520 616e 2069 6e73 7461  .Create an insta
-00000260: 6e63 6520 6f66 204e 6f76 6143 6c69 656e  nce of NovaClien
-00000270: 742c 2075 7369 6e67 2079 6f75 7220 4150  t, using your AP
-00000280: 4920 6b65 790d 0a0d 0a60 6060 7079 7468  I key....```pyth
-00000290: 6f6e 0d0a 636c 6965 6e74 203d 204e 6f76  on..client = Nov
-000002a0: 6143 6c69 656e 7428 2259 4f55 525f 4150  aClient("YOUR_AP
-000002b0: 495f 4b45 5922 290d 0a60 6060 0d0a 0d0a  I_KEY")..```....
-000002c0: 6e6f 7661 5f70 7974 686f 6e20 6375 7272  nova_python curr
-000002d0: 656e 746c 7920 696d 706c 656d 656e 7473  ently implements
-000002e0: 2074 776f 2065 6e75 6d73 3a20 456e 6470   two enums: Endp
-000002f0: 6f69 6e74 7320 616e 6420 4d6f 6465 6c73  oints and Models
-00000300: 2e20 5468 6f73 6520 636f 6e74 6169 6e3a  . Those contain:
-00000310: 0d0a 0d0a 2323 2320 456e 6470 6f69 6e74  ....### Endpoint
-00000320: 7320 2323 230d 0a2a 2060 456e 6470 6f69  s ###..* `Endpoi
-00000330: 6e74 732e 4348 4154 5f43 4f4d 504c 4554  nts.CHAT_COMPLET
-00000340: 494f 4e60 0d0a 0d0a 2a2a 4d6f 6465 6c73  ION`....**Models
-00000350: 2a2a 0d0a 2a20 604d 6f64 656c 732e 4750  **..* `Models.GP
-00000360: 5433 600d 0a2b 2060 4d6f 6465 6c73 2e47  T3`..+ `Models.G
-00000370: 5054 3460 0d0a 0d0a 4e6f 772c 2074 6f20  PT4`....Now, to 
-00000380: 6d61 6b65 2061 2072 6571 7565 7374 2c20  make a request, 
-00000390: 7573 6520 7468 6520 606d 616b 655f 7265  use the `make_re
-000003a0: 7175 6573 7460 2066 756e 6374 696f 6e2e  quest` function.
-000003b0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
-000003c0: 726f 6d20 6e6f 7661 5f70 7974 686f 6e20  rom nova_python 
-000003d0: 696d 706f 7274 2045 6e64 706f 696e 7473  import Endpoints
-000003e0: 2c20 4d6f 6465 6c73 2c20 4e6f 7661 436c  , Models, NovaCl
-000003f0: 6965 6e74 0d0a 636c 6965 6e74 203d 204e  ient..client = N
-00000400: 6f76 6143 6c69 656e 7428 2259 4f55 525f  ovaClient("YOUR_
-00000410: 4150 495f 4b45 5922 290d 0a0d 0a63 6c69  API_KEY")....cli
-00000420: 656e 742e 6d61 6b65 5f72 6571 7565 7374  ent.make_request
-00000430: 280d 0a20 2020 2065 6e64 706f 696e 743d  (..    endpoint=
-00000440: 456e 6470 6f69 6e74 732e 4348 4154 5f43  Endpoints.CHAT_C
-00000450: 4f4d 504c 4554 494f 4e2c 0d0a 2020 2020  OMPLETION,..    
-00000460: 6d6f 6465 6c3d 4d6f 6465 6c73 2e47 5054  model=Models.GPT
-00000470: 332c 0d0a 2020 2020 6461 7461 3d5b 0d0a  3,..    data=[..
-00000480: 2020 2020 2020 2020 7b22 726f 6c65 223a          {"role":
-00000490: 2022 7379 7374 656d 222c 2022 636f 6e74   "system", "cont
-000004a0: 656e 7422 3a20 2259 6f75 2061 7265 2061  ent": "You are a
-000004b0: 2068 656c 7066 756c 2061 7373 6973 7461   helpful assista
-000004c0: 6e74 2e22 7d2c 0d0a 2020 2020 2020 2020  nt."},..        
-000004d0: 7b22 726f 6c65 223a 2022 7573 6572 222c  {"role": "user",
-000004e0: 2022 636f 6e74 656e 7422 3a20 2248 656c   "content": "Hel
-000004f0: 6c6f 2122 7d0d 0a20 2020 205d 0d0a 290d  lo!"}..    ]..).
-00000500: 0a60 6060 0d0a 0d0a 4966 2065 7665 7279  .```....If every
-00000510: 7468 696e 6720 676f 6573 2074 6f20 706c  thing goes to pl
-00000520: 616e 2c20 796f 7527 6c6c 2072 6563 6569  an, you'll recei
-00000530: 7665 2061 2073 7472 696e 6720 636f 6e74  ve a string cont
-00000540: 6169 6e69 6e67 204a 534f 4e2d 4461 7461  aining JSON-Data
-00000550: 2c20 7768 6963 6820 796f 7520 6361 6e20  , which you can 
-00000560: 7468 656e 2075 7365 2069 6e20 796f 7572  then use in your
-00000570: 2070 726f 6a65 6374 2e20 200d 0a2a 4861   project.  ..*Ha
-00000580: 7070 7920 7072 6f6d 7074 696e 6721 2a0d  ppy prompting!*.
-00000590: 0a0d 0a4d 6164 6520 7769 7468 20f0 9fa9  ...Made with ...
-000005a0: b820 6279 204c 6561 6e64 6572 0a         . by Leander.
+00000140: 723a 204c 6561 6e64 6572 203c 4068 656e  r: Leander <@hen
+00000150: 6365 6975 7365 6765 6e74 6f6f 3e0a 5265  ceiusegentoo>.Re
+00000160: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000170: 3d33 2e37 0a44 6573 6372 6970 7469 6f6e  =3.7.Description
+00000180: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000190: 6578 742f 6d61 726b 646f 776e 3b20 6368  ext/markdown; ch
+000001a0: 6172 7365 743d 5554 462d 383b 2076 6172  arset=UTF-8; var
+000001b0: 6961 6e74 3d47 464d 0a0a 2320 6e6f 7661  iant=GFM..# nova
+000001c0: 2d70 7974 686f 6e0d 0af0 9f90 8d20 5079  -python...... Py
+000001d0: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
+000001e0: 2061 6363 6573 7369 6e67 2074 6865 204e   accessing the N
+000001f0: 6f76 6120 4150 490d 0a0d 0a23 2320 5573  ova API....## Us
+00000200: 6167 6520 2323 0d0a 496e 7374 616c 6c20  age ##..Install 
+00000210: 7468 6520 6d6f 6475 6c65 2028 5468 6973  the module (This
+00000220: 2072 6571 7569 7265 7320 3c61 2068 7265   requires <a hre
+00000230: 663d 2268 7474 7073 3a2f 2f72 7573 7475  f="https://rustu
+00000240: 702e 7273 2f22 3e43 6172 676f 3c2f 613e  p.rs/">Cargo</a>
+00000250: 2920 200d 0a60 6060 7368 0d0a 2420 7069  )  ..```sh..$ pi
+00000260: 7020 696e 7374 616c 6c20 6e6f 7661 2d70  p install nova-p
+00000270: 7974 686f 6e0d 0a60 6060 0d0a 0d0a 496d  ython..```....Im
+00000280: 706f 7274 2074 6865 206d 6f64 756c 650d  port the module.
+00000290: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+000002a0: 206e 6f76 615f 7079 7468 6f6e 2069 6d70   nova_python imp
+000002b0: 6f72 7420 456e 6470 6f69 6e74 732c 204d  ort Endpoints, M
+000002c0: 6f64 656c 732c 204e 6f76 6143 6c69 656e  odels, NovaClien
+000002d0: 740d 0a60 6060 0d0a 0d0a 4372 6561 7465  t..```....Create
+000002e0: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
+000002f0: 4e6f 7661 436c 6965 6e74 2c20 7573 696e  NovaClient, usin
+00000300: 6720 796f 7572 2041 5049 206b 6579 0d0a  g your API key..
+00000310: 0d0a 6060 6070 7974 686f 6e0d 0a63 6c69  ..```python..cli
+00000320: 656e 7420 3d20 4e6f 7661 436c 6965 6e74  ent = NovaClient
+00000330: 2822 594f 5552 5f41 5049 5f4b 4559 2229  ("YOUR_API_KEY")
+00000340: 0d0a 6060 600d 0a0d 0a6e 6f76 615f 7079  ..```....nova_py
+00000350: 7468 6f6e 2063 7572 7265 6e74 6c79 2069  thon currently i
+00000360: 6d70 6c65 6d65 6e74 7320 7477 6f20 656e  mplements two en
+00000370: 756d 733a 2045 6e64 706f 696e 7473 2061  ums: Endpoints a
+00000380: 6e64 204d 6f64 656c 732e 2054 686f 7365  nd Models. Those
+00000390: 2063 6f6e 7461 696e 3a0d 0a0d 0a2a 2a45   contain:....**E
+000003a0: 6e64 706f 696e 7473 2a2a 0d0a 2a20 6045  ndpoints**..* `E
+000003b0: 6e64 706f 696e 7473 2e43 4841 545f 434f  ndpoints.CHAT_CO
+000003c0: 4d50 4c45 5449 4f4e 600d 0a2a 2060 456e  MPLETION`..* `En
+000003d0: 6470 6f69 6e74 732e 4d4f 4445 5241 5449  dpoints.MODERATI
+000003e0: 4f4e 600d 0a0d 0a2a 2a4d 6f64 656c 732a  ON`....**Models*
+000003f0: 2a0d 0a2a 2060 4d6f 6465 6c73 2e47 5054  *..* `Models.GPT
+00000400: 3360 0d0a 2a20 604d 6f64 656c 732e 4750  3`..* `Models.GP
+00000410: 5434 600d 0a2a 2060 4d6f 6465 6c73 2e4d  T4`..* `Models.M
+00000420: 4f44 4552 4154 494f 4e5f 4c41 5445 5354  ODERATION_LATEST
+00000430: 600d 0a2a 2060 4d6f 6465 6c73 2e4d 4f44  `..* `Models.MOD
+00000440: 4552 4154 494f 4e5f 5354 4142 4c45 6020  ERATION_STABLE` 
+00000450: 200d 0a0d 0a4e 6f77 2c20 746f 206d 616b   ....Now, to mak
+00000460: 6520 6120 7265 7175 6573 742c 2075 7365  e a request, use
+00000470: 2074 6865 2060 6d61 6b65 5f72 6571 7565   the `make_reque
+00000480: 7374 6020 6675 6e63 7469 6f6e 2e20 466f  st` function. Fo
+00000490: 7220 6578 616d 706c 653a 0d0a 0d0a 6060  r example:....``
+000004a0: 6070 7974 686f 6e0d 0a66 726f 6d20 6e6f  `python..from no
+000004b0: 7661 5f70 7974 686f 6e20 696d 706f 7274  va_python import
+000004c0: 2045 6e64 706f 696e 7473 2c20 4d6f 6465   Endpoints, Mode
+000004d0: 6c73 2c20 4e6f 7661 436c 6965 6e74 0d0a  ls, NovaClient..
+000004e0: 636c 6965 6e74 203d 204e 6f76 6143 6c69  client = NovaCli
+000004f0: 656e 7428 2259 4f55 525f 4150 495f 4b45  ent("YOUR_API_KE
+00000500: 5922 290d 0a0d 0a63 6c69 656e 742e 6d61  Y")....client.ma
+00000510: 6b65 5f72 6571 7565 7374 280d 0a20 2020  ke_request(..   
+00000520: 2065 6e64 706f 696e 743d 456e 6470 6f69   endpoint=Endpoi
+00000530: 6e74 732e 4348 4154 5f43 4f4d 504c 4554  nts.CHAT_COMPLET
+00000540: 494f 4e2c 0d0a 2020 2020 6d6f 6465 6c3d  ION,..    model=
+00000550: 4d6f 6465 6c73 2e47 5054 332c 0d0a 2020  Models.GPT3,..  
+00000560: 2020 6461 7461 3d5b 0d0a 2020 2020 2020    data=[..      
+00000570: 2020 7b22 726f 6c65 223a 2022 7379 7374    {"role": "syst
+00000580: 656d 222c 2022 636f 6e74 656e 7422 3a20  em", "content": 
+00000590: 2259 6f75 2061 7265 2061 2068 656c 7066  "You are a helpf
+000005a0: 756c 2061 7373 6973 7461 6e74 2e22 7d2c  ul assistant."},
+000005b0: 0d0a 2020 2020 2020 2020 7b22 726f 6c65  ..        {"role
+000005c0: 223a 2022 7573 6572 222c 2022 636f 6e74  ": "user", "cont
+000005d0: 656e 7422 3a20 2248 656c 6c6f 2122 7d0d  ent": "Hello!"}.
+000005e0: 0a20 2020 205d 0d0a 290d 0a60 6060 0d0a  .    ]..)..```..
+000005f0: 0d0a 6f72 0d0a 0d0a 6060 6070 7974 686f  ..or....```pytho
+00000600: 6e0d 0a66 726f 6d20 6e6f 7661 5f70 7974  n..from nova_pyt
+00000610: 686f 6e20 696d 706f 7274 2045 6e64 706f  hon import Endpo
+00000620: 696e 7473 2c20 4d6f 6465 6c73 2c20 4e6f  ints, Models, No
+00000630: 7661 436c 6965 6e74 0d0a 636c 6965 6e74  vaClient..client
+00000640: 203d 204e 6f76 6143 6c69 656e 7428 2259   = NovaClient("Y
+00000650: 4f55 525f 4150 495f 4b45 5922 290d 0a0d  OUR_API_KEY")...
+00000660: 0a63 6c69 656e 742e 6d61 6b65 5f72 6571  .client.make_req
+00000670: 7565 7374 280d 0a20 2020 2065 6e64 706f  uest(..    endpo
+00000680: 696e 743d 456e 6470 6f69 6e74 732e 4d4f  int=Endpoints.MO
+00000690: 4445 5241 5449 4f4e 2c0d 0a20 2020 206d  DERATION,..    m
+000006a0: 6f64 656c 3d4d 6f64 656c 732e 4d4f 4445  odel=Models.MODE
+000006b0: 5241 5449 4f4e 5f53 5441 424c 452c 0d0a  RATION_STABLE,..
+000006c0: 2020 2020 6461 7461 3d5b 7b22 696e 7075      data=[{"inpu
+000006d0: 7422 3a20 2249 276d 2067 6f69 6e67 2074  t": "I'm going t
+000006e0: 6f20 6b69 6c6c 2074 6865 6d2e 227d 5d0d  o kill them."}].
+000006f0: 0a29 0d0a 6060 600d 0a0d 0a0d 0a49 6620  .)..```......If 
+00000700: 6576 6572 7974 6869 6e67 2067 6f65 7320  everything goes 
+00000710: 746f 2070 6c61 6e2c 2079 6f75 276c 6c20  to plan, you'll 
+00000720: 7265 6365 6976 6520 6120 7374 7269 6e67  receive a string
+00000730: 2063 6f6e 7461 696e 696e 6720 4a53 4f4e   containing JSON
+00000740: 2d44 6174 612c 2077 6869 6368 2079 6f75  -Data, which you
+00000750: 2063 616e 2074 6865 6e20 7573 6520 696e   can then use in
+00000760: 2079 6f75 7220 7072 6f6a 6563 742e 2020   your project.  
+00000770: 0d0a 2a48 6170 7079 2070 726f 6d70 7469  ..*Happy prompti
+00000780: 6e67 212a 0d0a 0d0a 2323 2046 4151 2023  ng!*....## FAQ #
+00000790: 230d 0a2a 2a51 3a2a 2a20 4920 6765 7420  #..**Q:** I get 
+000007a0: 616e 2065 7272 6f72 2077 6865 6e20 696e  an error when in
+000007b0: 7374 616c 6c69 6e67 2074 6865 2070 6163  stalling the pac
+000007c0: 6b61 6765 2020 0d0a 2a2a 413a 2a2a 204d  kage  ..**A:** M
+000007d0: 616b 6520 796f 7520 7375 7265 2c20 7468  ake you sure, th
+000007e0: 6174 2079 6f75 2068 6176 6520 3c61 2068  at you have <a h
+000007f0: 7265 663d 2268 7474 7073 3a2f 2f72 7573  ref="https://rus
+00000800: 7475 702e 7273 2f22 3e43 6172 676f 3c2f  tup.rs/">Cargo</
+00000810: 613e 2069 6e73 7461 6c6c 6564 0d0a 0d0a  a> installed....
+00000820: 4d61 6465 2077 6974 6820 f09f a9b8 2062  Made with .... b
+00000830: 7920 4c65 616e 6465 720a                 y Leander.
```

