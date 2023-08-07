# Comparing `tmp/bolt11-1.0.3.tar.gz` & `tmp/bolt11-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt11-1.0.3.tar", max compression
+gzip compressed data, was "bolt11-1.0.4.tar", max compression
```

## Comparing `bolt11-1.0.3.tar` & `bolt11-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1112 2023-07-18 07:08:24.507071 bolt11-1.0.3/LICENSE
--rwxr-xr-x   0        0        0     3119 2023-07-18 07:08:24.507071 bolt11-1.0.3/README.md
--rw-r--r--   0        0        0      353 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/__init__.py
--rw-r--r--   0        0        0     1127 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/bit_utils.py
--rw-r--r--   0        0        0      599 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/cli.py
--rw-r--r--   0        0        0      243 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/compat.py
--rw-r--r--   0        0        0     3932 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/decode.py
--rw-r--r--   0        0        0     2926 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/encode.py
--rw-r--r--   0        0        0     2850 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/fallback.py
--rw-r--r--   0        0        0     3226 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/features.py
--rw-r--r--   0        0        0     1768 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/routehint.py
--rw-r--r--   0        0        0     2322 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/signature.py
--rw-r--r--   0        0        0       26 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/py.typed
--rw-r--r--   0        0        0     3962 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/types.py
--rw-r--r--   0        0        0     1947 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/utils.py
--rw-r--r--   0        0        0     1545 2023-07-18 07:08:24.507071 bolt11-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1112 2023-08-07 06:44:24.555202 bolt11-1.0.4/LICENSE
+-rwxr-xr-x   0        0        0     3119 2023-08-07 06:44:24.555202 bolt11-1.0.4/README.md
+-rw-r--r--   0        0        0      353 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/__init__.py
+-rw-r--r--   0        0        0     1127 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/bit_utils.py
+-rw-r--r--   0        0        0      599 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/cli.py
+-rw-r--r--   0        0        0      243 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/compat.py
+-rw-r--r--   0        0        0     3932 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/decode.py
+-rw-r--r--   0        0        0     2941 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/encode.py
+-rw-r--r--   0        0        0     2850 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/models/fallback.py
+-rw-r--r--   0        0        0     3226 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/models/features.py
+-rw-r--r--   0        0        0     1768 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/models/routehint.py
+-rw-r--r--   0        0        0     2322 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/models/signature.py
+-rw-r--r--   0        0        0       26 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/py.typed
+-rw-r--r--   0        0        0     3957 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/types.py
+-rw-r--r--   0        0        0     1947 2023-08-07 06:44:24.555202 bolt11-1.0.4/bolt11/utils.py
+-rw-r--r--   0        0        0     1545 2023-08-07 06:44:24.559202 bolt11-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.4/PKG-INFO
```

### Comparing `bolt11-1.0.3/LICENSE` & `bolt11-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/README.md` & `bolt11-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/bit_utils.py` & `bolt11-1.0.4/bolt11/bit_utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/cli.py` & `bolt11-1.0.4/bolt11/cli.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/decode.py` & `bolt11-1.0.4/bolt11/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
     tags: Dict[str, Any] = {}
 
     while data_part.pos != data_part.len:
         tag, tagdata, data_part = _pull_tagged(data_part)
         data_length = len(tagdata or []) / 5  # type: ignore
 
-        # MUST skip over unknown fields, OR an f field with unknown version, OR p, h, s or n
-        # fields that do NOT have data_lengths of 52, 52, 52 or 53, respectively.
+        # MUST skip over unknown fields, OR an f field with unknown version, OR p, h,
+        # s or n fields that do NOT have data_lengths of 52, 52, 52 or 53, respectively.
 
         if tag == "p" and data_length == 52 and not hasattr(tags, "p"):
             tags["p"] = trim_to_bytes(tagdata).hex()  # type: ignore
         elif tag == "h" and data_length == 52 and not hasattr(tags, "h") and not hasattr(tags, "d"):
             tags["h"] = trim_to_bytes(tagdata).hex()  # type: ignore
         elif tag == "s" and data_length == 52 and not hasattr(tags, "s"):
             tags["s"] = trim_to_bytes(tagdata).hex()  # type: ignore
@@ -81,23 +81,23 @@
         elif tag == "9":
             tags["9"] = Features.from_bitstring(tagdata)  # type: ignore
         elif tag == "r":
             tags["r"] = RouteHint.from_bitstring(tagdata)  # type: ignore
 
     signature = Signature(signature_data=signature_data, signing_data=hrp.encode() + data_part.tobytes())
 
-    # A reader MUST check that the `signature` is valid (see the `n` tagged field specified below).
-    # A reader MUST use the `n` field to validate the signature instead of
-    # performing signature recovery if a valid `n` field is provided.
+    # A reader MUST check that the `signature` is valid (see the `n` tagged field
+    # specified below). A reader MUST use the `n` field to validate the signature
+    # instead of performing signature recovery if a valid `n` field is provided.
     if hasattr(tags, "n"):
         # TODO: research why no test runs this?
         signature.verify(tags["n"])
     else:
         tags["n"] = signature.recover_public_key()
 
     return Bolt11(
         currency=currency,
-        amount=amount_msat,
-        timestamp=timestamp,
+        amount_msat=amount_msat,
+        date=timestamp,
         signature=signature,
         tags=tags,
     )
```

### Comparing `bolt11-1.0.3/bolt11/encode.py` & `bolt11-1.0.4/bolt11/encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,29 +33,29 @@
     """Get minimal length by trimming leading 5 bits at a time."""
     value = pack("intbe:64", tag)[4:64]
     while value.startswith("0b00000"):
         value = value[5:]
     return value
 
 
-def _create_hrp(currency: str, amount: Optional[MilliSatoshi]) -> str:
+def _create_hrp(currency: str, amount_msat: Optional[MilliSatoshi]) -> str:
     hrp = "ln" + currency
-    if amount:
-        hrp += msat_to_amount(amount)
+    if amount_msat:
+        hrp += msat_to_amount(amount_msat)
     return hrp
 
 
 def encode(invoice: Bolt11, private_key: Optional[str] = None) -> str:
     # A writer MUST include either a `d` or `h` field, and MUST NOT include
     if invoice.description and invoice.description_hash:
         raise ValueError("Cannot include both 'd' and 'h'")
     if not invoice.description and not invoice.description_hash:
         raise ValueError("Must include either 'd' or 'h'")
 
-    timestamp = BitArray(uint=invoice.timestamp, length=35)
+    timestamp = BitArray(uint=invoice.date, length=35)
     tags = BitArray()
 
     for k, tag in invoice.tags.items():
         if k == "s":
             tags += _tagged_bytes("s", bytes.fromhex(tag))
         elif k == "p":
             tags += _tagged_bytes("p", bytes.fromhex(tag))
@@ -75,15 +75,15 @@
         elif k == "c":
             tags += _tagged("c", _tagged_int(tag))
         elif k == "x":
             tags += _tagged("x", _tagged_int(tag))
         elif k == "r":
             tags += _tagged("r", tag.data)
 
-    hrp = _create_hrp(invoice.currency, invoice.amount)
+    hrp = _create_hrp(invoice.currency, invoice.amount_msat)
 
     if private_key:
         invoice.signature = Signature.from_private_key(private_key, hrp, timestamp + tags)
 
     if not invoice.signature:
         raise ValueError("Must include either 'signature' or 'private_key'")
```

### Comparing `bolt11-1.0.3/bolt11/models/fallback.py` & `bolt11-1.0.4/bolt11/models/fallback.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/models/features.py` & `bolt11-1.0.4/bolt11/models/features.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/models/routehint.py` & `bolt11-1.0.4/bolt11/models/routehint.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/models/signature.py` & `bolt11-1.0.4/bolt11/models/signature.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/bolt11/types.py` & `bolt11-1.0.4/bolt11/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 
 @dataclass
 class Bolt11:
     """Bolt11 Lightning invoice."""
 
     currency: str
-    timestamp: int
+    date: int
     tags: Dict[str, Any]
-    amount: Optional[MilliSatoshi] = None
+    amount_msat: Optional[MilliSatoshi] = None
     signature: Optional[Signature] = None
 
     @property
     def description(self) -> Optional[str]:
         return self.tags["d"] if "d" in self.tags else None
 
     @property
@@ -47,15 +47,15 @@
 
     @property
     def metadata(self) -> Optional[str]:
         return self.tags["m"] if "m" in self.tags else None
 
     @property
     def dt(self) -> datetime:
-        return datetime.fromtimestamp(self.timestamp)
+        return datetime.fromtimestamp(self.date)
 
     @property
     def expiry(self) -> Optional[int]:
         return self.tags["x"] if "x" in self.tags else None
 
     @property
     def features(self) -> Optional[Features]:
@@ -85,16 +85,16 @@
     def payee(self) -> Optional[str]:
         return self.tags["n"] if "n" in self.tags else None
 
     @property
     def json(self) -> str:
         json_data = {
             "currency": self.currency,
-            "amount": int(self.amount) if self.amount else 0,
-            "timestamp": self.timestamp,
+            "amount_msat": int(self.amount_msat) if self.amount_msat else 0,
+            "date": self.date,
             "signature": self.signature.hex if self.signature else "",
         }
         if self.description:
             json_data["description"] = self.description
         if self.description_hash:
             json_data["description_hash"] = self.description_hash
         if self.metadata:
@@ -116,15 +116,15 @@
         if self.payee:
             json_data["payee"] = self.payee
         return json.dumps(json_data)
 
     def has_expired(self) -> bool:
         if self.expiry is None:
             return False
-        return time.time() > self.timestamp + self.expiry
+        return time.time() > self.date + self.expiry
 
     def is_mainnet(self) -> bool:
         return self.currency == "bc"
 
     def is_testnet(self) -> bool:
         return self.currency == "tb"
```

### Comparing `bolt11-1.0.3/bolt11/utils.py` & `bolt11-1.0.4/bolt11/utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.3/pyproject.toml` & `bolt11-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bolt11"
-version = "1.0.3"
+version = "1.0.4"
 description = "A library for encoding and decoding BOLT11 payment requests."
 repository = "https://github.com/lnbits/bolt11"
 authors = [
     "eillarra <eneko@illarra.com>",
     "Alan Bits <alan@lnbits.com>"
 ]
 license = "MIT"
@@ -27,15 +27,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 isort = "^5.12.0"
-pyright = "^1.1.317"
+pyright = "^1.1.320"
 pylint = "^2.17.2"
 pre-commit = "^3.3.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bolt11-1.0.3/PKG-INFO` & `bolt11-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolt11
-Version: 1.0.3
+Version: 1.0.4
 Summary: A library for encoding and decoding BOLT11 payment requests.
 Home-page: https://github.com/lnbits/bolt11
 License: MIT
 Author: eillarra
 Author-email: eneko@illarra.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

