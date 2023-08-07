# Comparing `tmp/octo_api_client-1.1.4.tar.gz` & `tmp/octo_api_client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octo_api_client-1.1.4.tar", max compression
+gzip compressed data, was "octo_api_client-1.1.5.tar", max compression
```

## Comparing `octo_api_client-1.1.4.tar` & `octo_api_client-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      690 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/README.md
--rw-r--r--   0        0        0      111 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/__init__.py
--rw-r--r--   0        0        0    20193 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/client.py
--rw-r--r--   0        0        0     2391 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/const.py
--rw-r--r--   0        0        0      426 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/exceptions.py
--rw-r--r--   0        0        0    11968 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/octo_client/models.py
--rw-r--r--   0        0        0     1110 2023-05-08 08:57:27.524437 octo_api_client-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.4/setup.py
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      690 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/README.md
+-rw-r--r--   0        0        0      111 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/octo_client/__init__.py
+-rw-r--r--   0        0        0    21339 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/octo_client/client.py
+-rw-r--r--   0        0        0     2391 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/octo_client/const.py
+-rw-r--r--   0        0        0      426 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/octo_client/exceptions.py
+-rw-r--r--   0        0        0    11968 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/octo_client/models.py
+-rw-r--r--   0        0        0     1110 2023-08-07 09:17:36.303147 octo_api_client-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 octo_api_client-1.1.5/setup.py
+-rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 octo_api_client-1.1.5/PKG-INFO
```

### Comparing `octo_api_client-1.1.4/README.md` & `octo_api_client-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.4/octo_client/client.py` & `octo_api_client-1.1.5/octo_client/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -90,17 +90,17 @@
         )
 
     def _make_request(
         self,
         http_method: Callable,
         path: str,
         supplier_id=None,
-        json=None,
+        json: Optional[Dict] = None,
         params=None,
-        headers=None,
+        headers: Optional[Dict] = None,
     ):
         if headers is None:
             headers = {}
 
         if params is None:
             params = {}
 
@@ -166,87 +166,94 @@
 
     def _get_headers(self) -> Dict[str, str]:
         return {
             "Authorization": f"Bearer {self.token}",
             "Accept-Language": self.language,
         }
 
-    def _http_get(self, path: str, supplier_id: Optional[str] = None, params=None):
-        return self._make_request(requests.get, path, supplier_id=supplier_id, params=params)
+    def _http_get(self, path: str, supplier_id: Optional[str] = None, params=None, headers: Optional[Dict] = None):
+        return self._make_request(requests.get, path, supplier_id=supplier_id, params=params, headers=headers)
 
-    def _http_post(self, path: str, json: dict, supplier_id: str, params=None):
+    def _http_post(self, path: str, json: dict, supplier_id: str, params=None, headers: Optional[Dict] = None):
+        if headers is None:
+            headers = {}
         return self._make_request(
             requests.post,
             path,
             json=json,
             supplier_id=supplier_id,
             params=params,
-            headers={"Content-Type": "application/json"},
+            headers={"Content-Type": "application/json", **headers},
         )
 
-    def _http_patch(self, path: str, json: dict, supplier_id: str, params=None):
+    def _http_patch(self, path: str, json: dict, supplier_id: str, params=None, headers: Optional[Dict] = None):
+        if headers is None:
+            headers = {}
         return self._make_request(
             requests.patch,
             path,
             json=json,
             supplier_id=supplier_id,
             params=params,
-            headers={"Content-Type": "application/json"},
+            headers={"Content-Type": "application/json", **headers},
         )
 
-    def _http_delete(self, path: str, supplier_id: str, json: dict, params=None):
+    def _http_delete(self, path: str, supplier_id: str, json: dict, params=None, headers: Optional[Dict] = None):
+        if headers is None:
+            headers = {}
         return self._make_request(
             requests.delete,
             path,
             supplier_id=supplier_id,
             json=json,
             params=params,
-            headers={"Content-Type": "application/json"},
+            headers={"Content-Type": "application/json", **headers},
         )
 
-    def get_supplier(self, supplier_id: str) -> models.Supplier:
-        response = self._http_get(f"suppliers/{supplier_id}", supplier_id=supplier_id)
+    def get_supplier(self, supplier_id: str, headers: Optional[Dict] = None) -> models.Supplier:
+        response = self._http_get(f"suppliers/{supplier_id}", supplier_id=supplier_id, headers=headers)
         try:
             supplier = models.Supplier.from_dict(response, strict=self.strict)
         except AttributeError as e:
             raise exceptions.ApiError(response) from e
         return supplier
 
-    def get_suppliers(self) -> List[models.Supplier]:
-        response = self._http_get("suppliers")
+    def get_suppliers(self, headers: Optional[Dict] = None) -> List[models.Supplier]:
+        response = self._http_get("suppliers", headers=headers)
         try:
             suppliers = [
                 models.Supplier.from_dict(supplier, strict=self.strict) for supplier in response
             ]
         except AttributeError as e:
             raise exceptions.ApiError(response) from e
         self.logger.info("Found %s suppliers", len(suppliers), extra={"suppliers": response})
         self.supplier_url_map = {supplier.id: supplier.endpoint for supplier in suppliers}
         return suppliers
 
-    def get_products(self, supplier_id: str) -> List[models.Product]:
-        response = self._http_get("products", supplier_id=supplier_id)
+    def get_products(self, supplier_id: str, headers: Optional[Dict] = None) -> List[models.Product]:
+        response = self._http_get("products", supplier_id=supplier_id, headers=headers)
         products = [models.Product.from_dict(product, strict=self.strict) for product in response]
         self.logger.info("Found %s products", len(products), extra={"products": products})
         return products
 
-    def get_product(self, supplier_id: str, product_id: str) -> models.Product:
-        response = self._http_get(f"products/{product_id}", supplier_id=supplier_id)
+    def get_product(self, supplier_id: str, product_id: str, headers: Optional[Dict] = None) -> models.Product:
+        response = self._http_get(f"products/{product_id}", supplier_id=supplier_id, headers=headers)
         return models.Product.from_dict(response, strict=self.strict)
 
     def availability_check(
         self,
         supplier_id: str,
         product_id: str,
         option_id: str,
         units: Optional[List[models.UnitQuantity]] = None,
         local_date_start: Optional[date] = None,
         local_date_end: Optional[date] = None,
         local_date: Optional[date] = None,
         availability_ids: Optional[List[str]] = None,
+        headers: Optional[Dict] = None
     ) -> List[models.Availability]:
         payload: Dict[str, Any] = {
             "productId": product_id,
             "optionId": option_id,
         }
         if any([local_date_start, local_date_end]) and not all([local_date_start, local_date_end]):
             raise ValueError("local_date_start and local_date_end needs to be used together")
@@ -257,15 +264,15 @@
         if local_date:
             payload["localDate"] = local_date.isoformat()
         if availability_ids:
             payload["availabilityIds"] = availability_ids
         if units:
             payload["units"] = [unit.as_dict() for unit in units]
 
-        response = self._http_post("availability", supplier_id=supplier_id, json=payload)
+        response = self._http_post("availability", supplier_id=supplier_id, json=payload, headers=headers)
         detailed_availability = [
             models.Availability.from_dict(availability, strict=self.strict)
             for availability in response
         ]
         self.logger.info("Found %s items", len(detailed_availability))
         return detailed_availability
 
@@ -273,26 +280,28 @@
         self,
         supplier_id: str,
         product_id: str,
         option_id: str,
         local_date_start: date,
         local_date_end: date,
         units: Optional[List[models.UnitQuantity]] = None,
+        headers: Optional[Dict] = None,
     ) -> List[models.AvailabilityCalendarItem]:
         """This method retrieve the availability calendar for a range of dates.
 
         Args:
             supplier_id: retrieve calendar data for the supplier with this ID.
             product_id: retrieve calendar data for a product with this ID.
             option_id: retrieve calendar data for the option with this ID.
             local_date_start: retrieve calendar data from this date onwards.
             local_date_end: retrieve calendar data until this date.
             units: a list of units. Each unit requires:
                 - id
                 - quantity
+            headers: optional HTTP headers to send in the request.
 
         Returns: a list of availability objects; one object per each day in the range of dates.
         """
 
         payload: Dict[str, Any] = {
             "productId": product_id,
             "optionId": option_id,
@@ -300,15 +309,15 @@
         if local_date_start:
             payload["localDateStart"] = local_date_start.isoformat()
         if local_date_end:
             payload["localDateEnd"] = local_date_end.isoformat()
         if units:
             payload["units"] = [unit.as_dict() for unit in units]
 
-        response = self._http_post("availability/calendar", supplier_id=supplier_id, json=payload)
+        response = self._http_post("availability/calendar", supplier_id=supplier_id, json=payload, headers=headers)
         daily_availability = [
             models.AvailabilityCalendarItem.from_dict(availability, strict=self.strict)
             for availability in response
         ]
         self.logger.info("Found %s days", len(daily_availability))
         return daily_availability
 
@@ -318,14 +327,15 @@
         uuid: str,
         product_id: str,
         option_id: str,
         availability_id: str,
         unit_items: List[models.UnitItem],
         expiration_minutes: Optional[int] = None,
         notes: Optional[str] = None,
+        headers: Optional[Dict] = None,
     ) -> models.Booking:
         payload: Dict[str, Any] = {
             "uuid": uuid,
             "productId": product_id,
             "optionId": option_id,
             "availabilityId": availability_id,
             "unitItems": [unit.as_dict() for unit in unit_items],
@@ -334,26 +344,28 @@
             payload["expirationMinutes"] = expiration_minutes
         if notes:
             payload["notes"] = notes
         response = self._http_post(
             "bookings",
             supplier_id=supplier_id,
             json=payload,
+            headers=headers,
         )
         self.logger.info("Booking created", extra={"booking": response})
         return models.Booking.from_dict(response)
 
     def list_bookings(
         self,
         supplier_id: str,
         reseller_reference: Optional[str] = None,
         supplier_reference: Optional[str] = None,
         local_date: Optional[date] = None,
         local_date_start: Optional[date] = None,
         local_date_end: Optional[date] = None,
+        headers: Optional[Dict] = None,
     ) -> List[models.Booking]:
         if not any(
             [reseller_reference, supplier_reference, local_date, local_date_start or local_date_end]
         ):
             raise ValueError("One of the query parameters has to be provided.")
 
         if any([local_date_start, local_date_end]) and not all([local_date_start, local_date_end]):
@@ -366,19 +378,19 @@
             params["supplierReference"] = supplier_reference
         elif local_date:
             params["localDate"] = local_date.isoformat()
         elif local_date_start and local_date_end:
             params["localDateStart"] = local_date_start.isoformat()
             params["localDateEnd"] = local_date_end.isoformat()
 
-        response = self._http_get("bookings", supplier_id=supplier_id, params=params)
+        response = self._http_get("bookings", supplier_id=supplier_id, params=params, headers=headers)
         return [models.Booking.from_dict(booking) for booking in response]
 
-    def get_booking(self, supplier_id: str, uuid: str) -> models.Booking:
-        response = self._http_get(f"bookings/{uuid}", supplier_id=supplier_id)
+    def get_booking(self, supplier_id: str, uuid: str, headers: Optional[Dict] = None,) -> models.Booking:
+        response = self._http_get(f"bookings/{uuid}", supplier_id=supplier_id, headers=headers)
         return models.Booking.from_dict(response)
 
     def booking_confirmation(
         self,
         supplier_id: str,
         uuid: str,
         email_receipt: bool = False,
@@ -389,14 +401,15 @@
         contact_email_address: Optional[str] = None,
         contact_phone_number: Optional[str] = None,
         contact_locales: Optional[List[str]] = None,
         contact_postal_code: Optional[str] = None,
         contact_country: Optional[str] = None,
         contact_notes: Optional[str] = None,
         unit_items: Optional[List[models.ConfirmationUnitItem]] = None,
+        headers: Optional[Dict] = None,
     ) -> models.Booking:
         payload: Dict[str, Any] = {}
         if email_receipt:
             payload["emailReceipt"] = email_receipt
         if reseller_reference:
             payload["resellerReference"] = reseller_reference
         if any(
@@ -425,38 +438,39 @@
                     "notes": contact_notes,
                 }
             ).as_dict()
         if unit_items:
             payload["unitItems"] = [unit_item.as_dict() for unit_item in unit_items]
 
         response = self._http_post(
-            f"bookings/{uuid}/confirm", supplier_id=supplier_id, json=payload
+            f"bookings/{uuid}/confirm", supplier_id=supplier_id, json=payload, headers=headers
         )
         return models.Booking.from_dict(response)
 
     def extend_reservation(
-        self, supplier_id: str, uuid: str, expiration_minutes: int
+        self, supplier_id: str, uuid: str, expiration_minutes: int, headers: Optional[Dict] = None,
     ) -> models.Booking:
         payload = {"expirationMinutes": expiration_minutes}
-        response = self._http_post(f"bookings/{uuid}/extend", supplier_id=supplier_id, json=payload)
+        response = self._http_post(f"bookings/{uuid}/extend", supplier_id=supplier_id, json=payload, headers=headers)
         return models.Booking.from_dict(response)
 
     def booking_cancellation(
         self,
         supplier_id: str,
         uuid: str,
         reason: Optional[str] = None,
         force: Optional[bool] = False,
+        headers: Optional[Dict] = None,
     ) -> models.Booking:
         payload: Dict[str, Any] = {}
         if reason:
             payload["reason"] = reason
         if force:
             payload["force"] = force
-        response = self._http_delete(f"bookings/{uuid}", supplier_id=supplier_id, json=payload)
+        response = self._http_delete(f"bookings/{uuid}", supplier_id=supplier_id, json=payload, headers=headers)
         return models.Booking.from_dict(response)
 
     def booking_update(
         self,
         supplier_id: str,
         uuid: str,
         product_id: Optional[str] = None,
@@ -471,14 +485,15 @@
         contact_email_address: Optional[str] = None,
         contact_phone_number: Optional[str] = None,
         contact_locales: Optional[List[str]] = None,
         contact_postal_code: Optional[str] = None,
         contact_country: Optional[str] = None,
         contact_notes: Optional[str] = None,
         unit_items: Optional[List[models.ConfirmationUnitItem]] = None,
+        headers: Optional[Dict] = None,
     ):
         payload: Dict[str, Any] = {}
         if product_id:
             payload["productId"] = product_id
         if option_id:
             payload["optionId"] = option_id
         if availability_id:
@@ -522,9 +537,9 @@
                 payload["contact"]["country"] = contact_country
             if contact_notes:
                 payload["contact"]["notes"] = contact_notes
 
         if unit_items:
             payload["unitItems"] = [unit_item.as_dict() for unit_item in unit_items]
 
-        response = self._http_patch(f"bookings/{uuid}", supplier_id=supplier_id, json=payload)
+        response = self._http_patch(f"bookings/{uuid}", supplier_id=supplier_id, json=payload, headers=headers)
         return models.Booking.from_dict(response)
```

### Comparing `octo_api_client-1.1.4/octo_client/const.py` & `octo_api_client-1.1.5/octo_client/const.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.4/octo_client/models.py` & `octo_api_client-1.1.5/octo_client/models.py`

 * *Files identical despite different names*

### Comparing `octo_api_client-1.1.4/pyproject.toml` & `octo_api_client-1.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octo-api-client"
-version = "1.1.4"
+version = "1.1.5"
 description = "HTTP client for OCTo (Open Connection for Tourism) APIs."
 authors = ["Tiqets <connections@tiqets.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "octo_client"}]
 
 [tool.poetry.dependencies]
```

### Comparing `octo_api_client-1.1.4/setup.py` & `octo_api_client-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.20.0,<3', 'tonalite>=1.7.1,<2']
 
 setup_kwargs = {
     'name': 'octo-api-client',
-    'version': '1.1.4',
+    'version': '1.1.5',
     'description': 'HTTP client for OCTo (Open Connection for Tourism) APIs.',
     'long_description': "# OCTO API client\n\nPython HTTP client for OCTO (Open Connection for Tourism) APIs.\n\nMore info at [octospec.com](https://octospec.com/)\n\nAPI Specification: https://docs.octo.travel/docs/octo/r6gduoa5ah5ne-octo-api\n\n## Installation\n\n    pip install octo-api-client\n\n## Requirements\n\n* Python v3.7+\n\n## Development\n\n### Getting started\n\n    $ pip install poetry\n    $ poetry install\n\n### Running tests and linters\n\nTo run linters:\n\n    $ poetry run ruff octo_client\n    $ poetry run mypy octo_client\n\nTo run tests:\n\n    $ poetry run pytest\n\n\n## Usage\n\n```\nfrom octo_client import OctoClient\n\nclient = OctoClient('https://octo-api.mysupplier.com', 'MY-SECRET_TOKEN')\nclient.get_suppliers()\n```\n",
     'author': 'Tiqets',
     'author_email': 'connections@tiqets.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `octo_api_client-1.1.4/PKG-INFO` & `octo_api_client-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octo-api-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: HTTP client for OCTo (Open Connection for Tourism) APIs.
 License: MIT
 Author: Tiqets
 Author-email: connections@tiqets.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

