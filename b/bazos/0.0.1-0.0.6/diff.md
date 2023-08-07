# Comparing `tmp/bazos-0.0.1.tar.gz` & `tmp/bazos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bazos-0.0.1.tar", last modified: Sun Aug  6 17:38:15 2023, max compression
+gzip compressed data, was "bazos-0.0.6.tar", last modified: Mon Aug  7 00:08:37 2023, max compression
```

## Comparing `bazos-0.0.1.tar` & `bazos-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.435632 bazos-0.0.1/
--rw-r--r--   0 zlapik     (501) staff       (20)     1511 2023-08-06 17:38:15.435363 bazos-0.0.1/PKG-INFO
--rw-r--r--   0 zlapik     (501) staff       (20)      997 2023-08-06 17:16:45.000000 bazos-0.0.1/README.md
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.430138 bazos-0.0.1/bazos/
--rw-r--r--   0 zlapik     (501) staff       (20)      857 2023-08-06 17:24:28.000000 bazos-0.0.1/bazos/__init__.py
--rw-r--r--   0 zlapik     (501) staff       (20)    10406 2023-08-06 17:23:03.000000 bazos-0.0.1/bazos/bazos.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.432243 bazos-0.0.1/bazos/core/
--rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/core/__init__.py
--rw-r--r--   0 zlapik     (501) staff       (20)      377 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/core/settings.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.433791 bazos-0.0.1/bazos/info/
--rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/info/__init__.py
--rw-r--r--   0 zlapik     (501) staff       (20)     3765 2023-08-06 17:25:04.000000 bazos-0.0.1/bazos/info/product.py
--rw-r--r--   0 zlapik     (501) staff       (20)    17983 2023-08-06 17:25:09.000000 bazos-0.0.1/bazos/info/rubric_category.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.434084 bazos-0.0.1/bazos/info/tests/
--rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/info/tests/__init__.py
--rw-r--r--   0 zlapik     (501) staff       (20)      648 2023-08-06 17:25:12.000000 bazos-0.0.1/bazos/info/user.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.434538 bazos-0.0.1/bazos/shared/
--rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/shared/__init__.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.434840 bazos-0.0.1/bazos/shared/tests/
--rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/shared/tests/__init__.py
--rw-r--r--   0 zlapik     (501) staff       (20)     1895 2023-08-06 17:24:56.000000 bazos-0.0.1/bazos/shared/utils.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.435078 bazos-0.0.1/bazos/tests/
--rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-07-13 17:35:55.000000 bazos-0.0.1/bazos/tests/__init__.py
-drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-06 17:38:15.431738 bazos-0.0.1/bazos.egg-info/
--rw-r--r--   0 zlapik     (501) staff       (20)     1511 2023-08-06 17:38:15.000000 bazos-0.0.1/bazos.egg-info/PKG-INFO
--rw-r--r--   0 zlapik     (501) staff       (20)      470 2023-08-06 17:38:15.000000 bazos-0.0.1/bazos.egg-info/SOURCES.txt
--rw-r--r--   0 zlapik     (501) staff       (20)        1 2023-08-06 17:38:15.000000 bazos-0.0.1/bazos.egg-info/dependency_links.txt
--rw-r--r--   0 zlapik     (501) staff       (20)       37 2023-08-06 17:38:15.000000 bazos-0.0.1/bazos.egg-info/entry_points.txt
--rw-r--r--   0 zlapik     (501) staff       (20)        6 2023-08-06 17:38:15.000000 bazos-0.0.1/bazos.egg-info/top_level.txt
--rw-r--r--   0 zlapik     (501) staff       (20)       38 2023-08-06 17:38:15.435705 bazos-0.0.1/setup.cfg
--rw-r--r--   0 zlapik     (501) staff       (20)      993 2023-08-06 17:26:18.000000 bazos-0.0.1/setup.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.280281 bazos-0.0.6/
+-rw-r--r--   0 zlapik     (501) staff       (20)     2406 2023-08-07 00:08:37.280067 bazos-0.0.6/PKG-INFO
+-rw-r--r--   0 zlapik     (501) staff       (20)     1892 2023-08-06 23:40:44.000000 bazos-0.0.6/README.md
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.275025 bazos-0.0.6/bazos/
+-rw-r--r--   0 zlapik     (501) staff       (20)      929 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/__init__.py
+-rw-r--r--   0 zlapik     (501) staff       (20)    10771 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/bazos.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.277220 bazos-0.0.6/bazos/core/
+-rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/core/__init__.py
+-rw-r--r--   0 zlapik     (501) staff       (20)      377 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/core/settings.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.278703 bazos-0.0.6/bazos/info/
+-rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/info/__init__.py
+-rw-r--r--   0 zlapik     (501) staff       (20)     3867 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/info/product.py
+-rw-r--r--   0 zlapik     (501) staff       (20)    17743 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/info/rubric_category.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.278926 bazos-0.0.6/bazos/info/tests/
+-rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/info/tests/__init__.py
+-rw-r--r--   0 zlapik     (501) staff       (20)      661 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/info/user.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.279375 bazos-0.0.6/bazos/shared/
+-rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/shared/__init__.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.279629 bazos-0.0.6/bazos/shared/tests/
+-rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/shared/tests/__init__.py
+-rw-r--r--   0 zlapik     (501) staff       (20)     1764 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/shared/utils.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.279822 bazos-0.0.6/bazos/tests/
+-rw-r--r--   0 zlapik     (501) staff       (20)        0 2023-08-06 23:00:37.000000 bazos-0.0.6/bazos/tests/__init__.py
+drwxr-xr-x   0 zlapik     (501) staff       (20)        0 2023-08-07 00:08:37.276373 bazos-0.0.6/bazos.egg-info/
+-rw-r--r--   0 zlapik     (501) staff       (20)     2406 2023-08-07 00:08:37.000000 bazos-0.0.6/bazos.egg-info/PKG-INFO
+-rw-r--r--   0 zlapik     (501) staff       (20)      485 2023-08-07 00:08:37.000000 bazos-0.0.6/bazos.egg-info/SOURCES.txt
+-rw-r--r--   0 zlapik     (501) staff       (20)        1 2023-08-07 00:08:37.000000 bazos-0.0.6/bazos.egg-info/dependency_links.txt
+-rw-r--r--   0 zlapik     (501) staff       (20)       37 2023-08-07 00:08:37.000000 bazos-0.0.6/bazos.egg-info/entry_points.txt
+-rw-r--r--   0 zlapik     (501) staff       (20)        6 2023-08-07 00:08:37.000000 bazos-0.0.6/bazos.egg-info/top_level.txt
+-rw-r--r--   0 zlapik     (501) staff       (20)     1015 2023-08-06 23:00:37.000000 bazos-0.0.6/pyproject.toml
+-rw-r--r--   0 zlapik     (501) staff       (20)       38 2023-08-07 00:08:37.280345 bazos-0.0.6/setup.cfg
+-rw-r--r--   0 zlapik     (501) staff       (20)     1184 2023-08-07 00:06:57.000000 bazos-0.0.6/setup.py
```

### Comparing `bazos-0.0.1/PKG-INFO` & `bazos-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,81 @@
 Metadata-Version: 2.1
 Name: bazos
-Version: 0.0.1
+Version: 0.0.6
 Summary: Bazos API, that allows you to scrape bazos and upload products to bazos website.
 Author: Zdenek Lapes
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # BAZOS-API
 
-Current functionality supports removing and adding items to bazos.cz and .sk
+Current functionality supports removing and adding items to bazos.cz, bazos.sk, bazos.at and bazos.pl.
 
-## Installation:
+## Goal
+Create full-featured API for bazos.cz, bazos.sk, bazos.at and bazos.pl.
+
+## Installation
 
 ```shell
-python3 -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
+pip3 install bazos
 ```
 
+## Run
+
 ```shell
-python3 bazos --help
-python3 bazos -b --country cz sk --path $HOME/Documents/photos-archive # Remove all items from bazos.cz and bazos.sk and add new items from $HOME/Documents/photos-archive
-python3 bazos -b --country cz sk --add-only --path $HOME/Documents/photos-archive # Add new items from $HOME/Documents/photos-archive
+bazos --help
+bazos -b --country cz sk --path $HOME/Documents/photos-archive # Remove all items from bazos.cz and bazos.sk and add new items from $HOME/Documents/photos-archive
+bazos -b --country cz sk --add-only --path $HOME/Documents/photos-archive # Add new items from $HOME/Documents/photos-archive
 ```
 
+### `--country` argument
+Supported countries: `cz`, `sk`, `at`, `pl`
+
+
+### `-b|--bazos` argument
+This turn on run.
+
 ### `--path` argument
+The folder where all photos and `user_{country}.yml` file.
 
-The folder structure of directory passed to `--path` argument should look like this:
+How to structure folder defined in `--path` argument:
 
-```shell
-$HOME/Documents/photos-archive
-$HOME/Documents/photos-archive/folder1/photos/photo1.jpg
-$HOME/Documents/photos-archive/folder1/info.txt
+```yml
+# user_${bazos_country}.yml e.g.: user_cz.yml
+name: Jmeno
+phone_number: '+420123456789'
+email: user@example.com
+psc: 60200
+password: 123456
 ```
 
-### `info.txt` file structure
 
-Must follow this format:
+### Example of folder structure
+
+```shell
+bazos-ads/
+bazos-ads/user_cz.yml
+bazos-ads/user_sk.yml
+bazos-ads/item1/photos/photo1.jpg
+bazos-ads/item1/photos/photo2.jpg
+bazos-ads/item1/info.txt
+bazos-ads/item2/photos/photo1.jpg
+bazos-ads/item2/photos/photo2.jpg
+bazos-ads/item2/info.txt
+...
+```
+
+### `info.txt` syntax
 
 ```shell
 >>RUBRIC
 PC
 
 >>CATEGORY
 Notebooky
@@ -58,7 +86,32 @@
 >>PRICE
 25000
 
 >>DESCRIPTION
 Your sentences1.
 Your sentences2.
 ```
+
+
+
+## Contribution and Development
+
+Every contribution is welcome!
+
+Please follow rules inside `.pre-commit-config.yml` file.
+
+Before creating pull request, please run `pre-commit run --all-files` to check if there are no errors.
+
+### Install pre-commit hooks
+
+```shell
+pre-commit install
+```
+
+### Create virtual environment and install dependencies
+
+```shell
+python3 -m venv venv
+source venv/bin/activate
+pip install -r requirements.txt
+pip install -e .
+```
```

### Comparing `bazos-0.0.1/bazos/__init__.py` & `bazos-0.0.6/bazos/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 from bazos.bazos import bazos as bz
 
 
 def parse_cli_argument() -> Dict[str, Any]:
     parser = argparse.ArgumentParser()
     parser.add_argument('-b', '--bazos', action='store_true', help='Use bazos')
-    parser.add_argument('--add-only', action='store_true', help='Add only new products, not remove old ones')
-    parser.add_argument('--print-rubrics', action='store_true', help='Print rubrics')
-    parser.add_argument('--country', nargs="+", help="What bazos country to use", default=['cz', 'sk'])
+    parser.add_argument('--add-only', action='store_true',
+                        help='Add only new products, not remove old ones')
+    parser.add_argument('--print-rubrics',
+                        action='store_true', help='Print rubrics')
+    parser.add_argument('--country', nargs="+",
+                        help="What bazos country to use", default=['cz', 'sk'])
     parser.add_argument('-p', '--path', help='Path to products directory')
     cli_args = vars(parser.parse_args())
     return cli_args
 
 
 def main():
     cli_args = parse_cli_argument()
```

### Comparing `bazos-0.0.1/bazos/bazos.py` & `bazos-0.0.6/bazos/bazos.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,84 +62,98 @@
         self.url_bazos = f"https://bazos.{country}"
         self.url_moje_inzeraty = path.join(self.url_bazos, 'moje-inzeraty.php')
 
     def __del__(self):
         self.driver.quit()
 
     def print_all_rubrics_and_categories(self):
-        self.driver.find_element(By.CLASS_NAME, 'pridati').click()  # go to add page
+        self.driver.find_element(
+            By.CLASS_NAME, 'pridati').click()  # go to add page
         sections = self.driver.find_elements(By.CLASS_NAME, 'iconstblcell')
         sections[0].find_element(By.TAG_NAME, 'a').click()
-        select_rubrik = Select(self.driver.find_element(By.XPATH, XPathsBazos.select_rubrik))
+        select_rubrik = Select(self.driver.find_element(
+            By.XPATH, XPathsBazos.select_rubrik))
 
         _dict = {}
         rubric_options = [opt.text for opt in select_rubrik.options]
         for option in rubric_options:
 
             # Rubric
-            Select(self.driver.find_element(By.XPATH, XPathsBazos.select_rubrik)).select_by_visible_text(option)
+            Select(self.driver.find_element(
+                By.XPATH, XPathsBazos.select_rubrik)).select_by_visible_text(option)
 
             # Category
-            select_category = Select(self.driver.find_element(By.XPATH, XPathsBazos.select_category))
+            select_category = Select(self.driver.find_element(
+                By.XPATH, XPathsBazos.select_category))
             _dict[option] = []
             for idx, category in enumerate(select_category.options):
                 if idx == 0:
                     continue
                 _dict[option].append(category.text)
 
         print(_dict)
 
     def check_user_files_available(self) -> None:
         if (not os.path.isfile(f"{settings.COOKIES_FILE}_{self.bazos_country}.pkl")
-            or not os.path.isfile(f"{settings.LOCAL_STORAGE_FILE}_{self.bazos_country}.pkl")):
+                or not os.path.isfile(f"{settings.LOCAL_STORAGE_FILE}_{self.bazos_country}.pkl")):
             self.save_authentication(user=self.user)
 
     def check_authentication(self) -> None:
-        user_input = self.driver.find_elements(By.XPATH, XPathsBazos.user_inputs)
+        user_input = self.driver.find_elements(
+            By.XPATH, XPathsBazos.user_inputs)
         # tel_input = self.driver.find_element(By.XPATH, XPathsBazos.auth_phone_input)
         if len(user_input) != 3:  # Mean is Authenticated, because there is not "Overit" button
             self.save_authentication(user=self.user)
 
     def load_page_with_cookies(self) -> None:
         self.driver.get(self.url_moje_inzeraty)
         for cookie_dict in pickle.load(open(f"{settings.COOKIES_FILE}_{self.bazos_country}.pkl", 'rb')):
             self.driver.add_cookie(cookie_dict)
         self.driver.get(self.url_moje_inzeraty)
 
     def save_authentication(self, user: User) -> None:
         self.driver.get(self.url_moje_inzeraty)
 
         # Prepare authentication
-        telefon_input = self.driver.find_element(By.XPATH, XPathsBazos.auth_phone_input)
+        telefon_input = self.driver.find_element(
+            By.XPATH, XPathsBazos.auth_phone_input)
         telefon_input.clear()
         telefon_input.send_keys(user.phone_number)
-        self.driver.find_element(By.XPATH, XPathsBazos.auth_phone_check_submit).click()  # Submit
+        self.driver.find_element(
+            By.XPATH, XPathsBazos.auth_phone_check_submit).click()  # Submit
 
         # Authenticate
-        code_input = self.driver.find_element(By.XPATH, XPathsBazos.auth_code_input)
+        code_input = self.driver.find_element(
+            By.XPATH, XPathsBazos.auth_code_input)
         code_input.clear()
-        code_input.send_keys(input('Please provide authentification code sended to your phone: '))
-        self.driver.find_element(By.XPATH, XPathsBazos.auth_code_submit).click()  # Submit
+        code_input.send_keys(
+            input('Please provide authentification code sended to your phone: '))
+        self.driver.find_element(
+            By.XPATH, XPathsBazos.auth_code_submit).click()  # Submit
 
         # Save cookies
         pickle.dump(self.driver.get_cookies(),
                     file=open(f"{settings.COOKIES_FILE}_{self.bazos_country}.pkl", "wb"))
         # Save Local Storage
         pickle.dump(self.driver.execute_script("return window.localStorage;"),
                     file=open(f"{settings.LOCAL_STORAGE_FILE}_{self.bazos_country}.pkl", "wb"))
 
     def remove_advertisment(self, user: User):
-        self.driver.find_element(By.CLASS_NAME, 'inzeratydetdel').find_element(By.TAG_NAME, 'a').click()
-        pwd_input = self.driver.find_element(By.XPATH, XPathsBazos.delete_pwd_input)
+        self.driver.find_element(By.CLASS_NAME, 'inzeratydetdel').find_element(
+            By.TAG_NAME, 'a').click()
+        pwd_input = self.driver.find_element(
+            By.XPATH, XPathsBazos.delete_pwd_input)
         pwd_input.clear()
         pwd_input.send_keys(user.password)
-        self.driver.find_element(By.XPATH, XPathsBazos.delete_submit).click()  # Submit-Delete
+        self.driver.find_element(
+            By.XPATH, XPathsBazos.delete_submit).click()  # Submit-Delete
 
     def remove_advertisements(self, user: User):
-        self.advertisements = len(self.driver.find_elements(By.CLASS_NAME, 'nadpis'))
+        self.advertisements = len(
+            self.driver.find_elements(By.CLASS_NAME, 'nadpis'))
 
         print("==> Removing old advertisements")
         for i in range(self.advertisements):
             element = self.driver.find_element(By.CLASS_NAME, 'nadpis')
             print(f"Removing[{i}/{self.advertisements}]: {element.text}")
 
             #
@@ -147,60 +161,71 @@
             element.find_element(By.TAG_NAME, 'a').click()
             wait_random_time()
             self.remove_advertisment(user=user)
             wait_random_time()
 
     def add_advertisement(self, product: Product, user: User):
         # Rubrik
-        select_rubrik = Select(self.driver.find_element(By.XPATH, XPathsBazos.product_rubric))
-        select_rubrik.select_by_visible_text(get_rubric(self.bazos_country, product.rubric))
+        select_rubrik = Select(self.driver.find_element(
+            By.XPATH, XPathsBazos.product_rubric))
+        select_rubrik.select_by_visible_text(
+            get_rubric(self.bazos_country, product.rubric))
 
         # Product
-        select_category = Select(self.driver.find_element(By.XPATH, XPathsBazos.product_category))
-        select_category.select_by_visible_text(get_category(self.bazos_country, product.rubric, product.category))
+        select_category = Select(self.driver.find_element(
+            By.XPATH, XPathsBazos.product_category))
+        select_category.select_by_visible_text(get_category(
+            self.bazos_country, product.rubric, product.category))
         wait_random_time()
         self.driver.find_element(By.ID, 'nadpis').send_keys(product.title)
         self.driver.find_element(By.ID, 'popis').send_keys(product.description)
-        self.driver.find_element(By.ID, 'cena').send_keys(product.get_location_price(self.bazos_country))
+        self.driver.find_element(By.ID, 'cena').send_keys(
+            product.get_location_price(self.bazos_country))
 
         wait_random_time()
         self.driver.find_element(By.ID, 'lokalita').clear()
         self.driver.find_element(By.ID, 'lokalita').send_keys(user.psc)
         self.driver.find_element(By.ID, 'jmeno').clear()
         self.driver.find_element(By.ID, 'jmeno').send_keys(user.name)
         self.driver.find_element(By.ID, 'telefoni').clear()
-        self.driver.find_element(By.ID, 'telefoni').send_keys(user.phone_number)
+        self.driver.find_element(
+            By.ID, 'telefoni').send_keys(user.phone_number)
         self.driver.find_element(By.ID, 'maili').clear()
         self.driver.find_element(By.ID, 'maili').send_keys(user.email)
         self.driver.find_element(By.ID, 'heslobazar').clear()
         self.driver.find_element(By.ID, 'heslobazar').send_keys(user.password)
 
         wait_random_time()
         self.driver.find_element(By.CLASS_NAME, 'ovse').click()
-        self.driver.find_element(By.XPATH, XPathsBazos.product_img_input).send_keys('\n'.join(product.images))
+        self.driver.find_element(By.XPATH, XPathsBazos.product_img_input).send_keys(
+            '\n'.join(product.images))
 
         wait_random_time()
         self.driver.find_element(By.XPATH, XPathsBazos.product_submit).click()
 
     def add_advertisements(self, user: User) -> None:
-        products = get_all_products(products_path=user.products_path, country=self.bazos_country)
+        products = get_all_products(
+            products_path=user.products_path, country=self.bazos_country)
         self.advertisements = len(products)
 
         print("==> Adding advertisements")
         for idx, product in enumerate(products):
 
             if self.product_already_advertised(product):
-                print(f"Skipping[{idx}/{self.advertisements}]: {product.product_path}")
+                print(
+                    f"Skipping[{idx}/{self.advertisements}]: {product.product_path}")
                 continue
 
-            print(f"Adding[{idx}/{self.advertisements}]: {product.product_path}")
+            print(
+                f"Adding[{idx}/{self.advertisements}]: {product.product_path}")
 
             # product not advertised ADD them
             wait_random_time()
-            self.driver.find_element(By.CLASS_NAME, 'pridati').click()  # go to add page
+            self.driver.find_element(
+                By.CLASS_NAME, 'pridati').click()  # go to add page
 
             wait_random_time()
             self.driver.find_elements(By.CLASS_NAME, 'iconstblcell')[0].click()
             self.add_advertisement(product=product, user=user)
 
     def product_already_advertised(self, product: Product) -> bool:
         self.load_page_with_cookies()
@@ -226,13 +251,14 @@
 
         bazos_scrapper = BazosScrapper(country=country, cli_args=cli_args)
         bazos_scrapper.check_user_files_available()
         bazos_scrapper.load_page_with_cookies()
         bazos_scrapper.check_authentication()
 
         # Restore advertisements
-        if '--add-only' not in sys.argv: bazos_scrapper.remove_advertisements(user=bazos_scrapper.user)
+        if '--add-only' not in sys.argv:
+            bazos_scrapper.remove_advertisements(user=bazos_scrapper.user)
         bazos_scrapper.add_advertisements(user=bazos_scrapper.user)
 
 
 if __name__ == '__main__':
     bazos({})
```

### Comparing `bazos-0.0.1/bazos/info/product.py` & `bazos-0.0.6/bazos/info/product.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             'EURUSD': 1.2,
             'EURGBP': 0.9,
 
         }
 
     def get_rate(self, rate: str = "EURCZK") -> float:
         cc = CurrencyConverter()
-        if len(rate) != 6: raise ValueError(f"Rate {rate} is not correct. Should be 6 characters long.")
+        if len(rate) != 6:
+            raise ValueError(
+                f"Rate {rate} is not correct. Should be 6 characters long.")
         try:
             return cc.convert(1, rate[:3], rate[3:])
         except Exception:
             return self.rates_default[rate]
 
 
 class Product:
@@ -58,33 +60,36 @@
             return self.price
 
     def get_current_section(self, line) -> str:
         for key, value in product_info.items():
             if value in line:
                 return key
 
-        raise Exception(f"Key not found: key={key}, value={value}, line={line}")
+        raise Exception(
+            f"Key not found: key={key}, value={value}, line={line}")
 
     def load_product_info(self, *, product_dir):
         # NOTE: Rewrite this shit code
         with open(file=path.join(product_dir, 'info.txt'), mode='r') as file:
             for line in file.readlines():
                 if '>>' in line:
-                    current_product_info_key = self.get_current_section(line=line)
+                    current_product_info_key = self.get_current_section(
+                        line=line)
                     continue
 
                 if line.replace(' ', '').replace('\t', '').replace('\n', '') == '':
                     continue
 
                 if product_info[current_product_info_key] == product_info['rubric']:
                     self.rubric = line.strip()
                 elif product_info[current_product_info_key] == product_info['category']:
                     self.category = line.strip()
                 elif product_info[current_product_info_key] == product_info['title']:
-                    self.title = line[:60].strip()  # Bazos doesn't support longer title than 60 chars
+                    # Bazos doesn't support longer title than 60 chars
+                    self.title = line[:60].strip()
                 elif product_info[current_product_info_key] == product_info['price']:
                     self.price = line.strip()
                 # NOTE: Only here we append line, must be at the end of info.txt
                 elif product_info[current_product_info_key] == product_info['description']:
                     self.description += line
 
 
@@ -92,15 +97,16 @@
     print("==> Loading products")
 
     # Filter out all files and hidden directories
     dirs = [d for d in os.listdir(path=products_path)
             if path.isdir(path.join(products_path, d)) and d.startswith('.') is False]
 
     # Get ready all products
-    products = [Product(product_path=path.join(products_path, d)) for d in dirs]
+    products = [Product(product_path=path.join(products_path, d))
+                for d in dirs]
 
     print(f"Product loaded: {len(products)}")
     return products
 
 
 def validate_products():
     # TODO
```

### Comparing `bazos-0.0.1/bazos/info/rubric_category.py` & `bazos-0.0.6/bazos/info/rubric_category.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,181 +1,267 @@
 def get_rubric(country: str, rubric: str):
     if country.lower() == "cz":
         return rubric
     elif country.lower() == "sk":
         cz_idx = list(RUBRICS_CZ.keys()).index(rubric)
-        sk_rubric = list(RUBRICS_SK.keys())[cz_idx]
+        sk_rubric = list(RUBRICS_SK.keys())[
+            cz_idx
+        ]
         return sk_rubric
 
 
 def get_category(country: str, rubric: str, category: str):
     if country.lower() == "cz":
         return category
     elif country.lower() == "sk":
         cz_idx = RUBRICS_CZ[rubric].index(category)
         sk_category = RUBRICS_SK[get_rubric(country, rubric)][cz_idx]
         return sk_category
 
 
 RUBRICS_CZ = {
-    'Auto': ['Alfa Romeo', 'Audi', 'BMW', 'Chevrolet', 'Citroën', 'Dacia', 'Fiat', 'Ford', 'Honda', 'Hyundai', 'Kia',
-             'Mazda', 'Mercedes-Benz', 'Mitsubishi', 'Nissan', 'Opel', 'Peugeot', 'Renault', 'Seat', 'Suzuki', 'Škoda',
-             'Toyota', 'Volkswagen', 'Volvo', 'Havarovaná', 'Ostatní značky', 'Náhradní díly', 'Pneumatiky, kola',
-             'Příslušenství', 'Tuning', 'Veteráni', 'Autobusy', 'Dodávky', 'Karavany, vozíky', 'Mikrobusy',
-             'Nákladní auta', 'Pick-up', 'Ostatní užitková', 'Havarovaná užitková', 'Náhradní díly užitková'],
-    'Děti': ['Autosedačky', 'Baby monitory, chůvičky', 'Hračky', 'Chodítka a hopsadla', 'Kočárky', 'Kojenecké potřeby',
-             'Kola', 'Nábytek pro děti', 'Nosítka', 'Odrážedla', 'Sedačky na kolo', 'Sportovní potřeby',
-             'Školní potřeby', 'Ostatní', 'Body, dupačky a overaly', 'Bundy a kabátky', 'Čepice a kloboučky',
-             'Kalhoty, kraťasy a tepláky', 'Kombinézy', 'Komplety', 'Mikiny a svetry', 'Obuv', 'Plavky',
-             'Ponožky a punčocháče', 'Pyžámka a župánky', 'Rukavice a šály', 'Spodní prádlo', 'Sukýnky a šatičky',
-             'Trička a košile', 'Ostatní oblečení'],
-    'Dům a zahrada': ['Bazény', 'Čerpadla', 'Dveře, vrata', 'Klimatizace', 'Kotle, Kamna, Bojlery',
-                      'Malotraktory, Kultivátory', 'Míchačky', 'Nářadí', 'Okna', 'Pily', 'Radiátory', 'Rostliny',
-                      'Sekačky', 'Sněžná technika', 'Stavební materiál', 'Vybavení dílen', 'Vysavače/Foukače',
-                      'Zahradní grily', 'Zahradní technika', 'Ostatní'],
-    'Elektro': ['Autorádia', 'Digestoře', 'Domácí kina', 'Epilátory, Depilátory', 'Fény, Kulmy', 'Hifi systémy, Rádia',
-                'Holící strojky', 'Kávovary', 'Ledničky', 'Mikrovlnné trouby', 'Mrazáky', 'Myčky', 'Nabíječky baterií',
-                'Pračky', 'Projektory', 'Repro soustavy', 'Ruční šlehače, Mixéry', 'Šicí stroje', 'Sluchátka',
-                'Sporáky', 'Sušičky', 'Svítidla, Lampy', 'Televize', 'Video, DVD přehrávače', 'Vysavače', 'Vysílačky',
-                'Zesilovače', 'Zvlhčovače vzduchu', 'Žehličky', 'Ostatní - bílá', 'Ostatní audio video',
-                'Ostatní drobné'],
-    'Foto': ['Analogové fotoaparáty', 'Digitální fotoaparáty', 'Drony', 'Videokamery', 'Zrcadlovky', 'Baterie',
-             'Blesky a osvětlení', 'Brašny a pouzdra', 'Datové kabely', 'Filtry', 'Nabíječky baterií', 'Objektivy',
-             'Paměťové karty', 'Stativy', 'Ostatní'],
-    'Hudba': ['Bicí nástroje', 'Dechové nástroje', 'Klávesové nástroje', 'Smyčcové nástroje', 'Strunné nástroje',
-              'Ostatní nástroje', 'DVD, CD, MC, LP', 'Hudebníci a skupiny', 'Koncerty', 'Noty, texty',
-              'Světelná technika', 'Zkušebny', 'Zvuková technika', 'Ostatní'],
-    'Knihy': ['Beletrie', 'Časopisy', 'Cizojazyčná literatura', 'Detektivky', 'Dětská literatura', 'Drama',
-              'Encyklopedie', 'Esoterika', 'Historické romány', 'Hobby, odborné knihy', 'Kuchařky',
-              'Mapy, cestovní průvodci', 'Počítačová literatura', 'Pro mládež', 'Romány pro ženy', 'Sci-fi, Fantasy',
-              'Učebnice, skripta - Jazykové', 'Učebnice, skripta - SŠ', 'Učebnice, skripta - VŠ',
-              'Učebnice, skripta - ZŠ', 'Zábavná', 'Zdravý životní styl', 'Ostatní'],
-    'Mobily': ['Apple', 'HTC', 'Huawei, Honor', 'LG', 'Motorola, Lenovo', 'Nokia, Microsoft', 'Samsung', 'Sony',
-               'Xiaomi', 'Ostatní značky', 'Baterie', 'Bezdrátové telefony', 'Datové kabely', 'Faxy', 'Headsety',
-               'HF Sady do auta', 'Chytré hodinky', 'Kryty', 'Nabíječky', 'Paměťové karty', 'Stolní telefony',
-               'Ostatní'],
-    'Motorky': ['Cestovní motocykly', 'Chopper', 'Čtyřkolky', 'Enduro', 'Minibike', 'Mopedy', 'Silniční motocykly',
-                'Skútry', 'Skútry sněžné', 'Skútry vodní', 'Tříkolky', 'Veteráni', 'Náhradní díly',
-                'Oblečení, obuv, helmy', 'Ostatní'],
-    'Nábytek': ['Jídelní kouty', 'Knihovny', 'Koberce a podlah. krytina', 'Koupelny', 'Křesla a gauče', 'Kuchyně',
-                'Lampy, osvětlení', 'Ložnice', 'Matrace', 'Obývací stěny', 'Postele', 'Sedací soupravy', 'Skříně',
-                'Stoly', 'Zahradní nábytek', 'Židle', 'Doplňky', 'Ostatní nábytek'],
-    'Oblečení': ['Batohy, Kufry', 'Boty', 'Bundy a Kabáty', 'Čepice a Šátky', 'Doplňky', 'Džíny', 'Halenky', 'Hodinky',
-                 'Kabelky', 'Kalhoty', 'Košile', 'Kožené oděvy', 'Mikiny', 'Obleky a Saka', 'Plavky', 'Roušky',
-                 'Rukavice a Šály', 'Šaty, Kostýmky', 'Šortky', 'Šperky', 'Spodní prádlo', 'Sportovní oblečení',
-                 'Sukně', 'Svatební šaty', 'Těhotenské oblečení', 'Svetry', 'Termo prádlo', 'Trička, tílka', 'Ostatní'],
-    'PC': ['Chladiče', 'DVD, Blu-ray mechaniky', 'GPS navigace', 'Grafické karty', 'Hard disky, SSD', 'Herní konzole',
-           'Herní zařízení', 'Hry', 'Klávesnice, myši', 'Kopírovací stroje', 'LCD monitory', 'Modemy', 'Myši',
-           'Notebooky', 'Paměti', 'PC, Počítače', 'Procesory', 'Scanery', 'Síťové prvky', 'Skříně, zdroje', 'Software',
-           'Spotřební materiál', 'Tablety, E-čtečky', 'Tiskárny', 'Wireless, WiFi', 'Základní desky', 'Záložní zdroje',
-           'Zvukové karty', 'Ostatní'],
-    'Práce': ['Administrativa', 'Brigády', 'Chemie a potravinářství', 'Doprava a logistika', 'Finance a ekonomika',
-              'IT a telekomunikace', 'Management', 'Marketing a reklama', 'Obchod a prodej', 'Obrana a bezpečnost',
-              'Pohostinství a ubytování', 'Práce v domácnosti', 'Právo, legislativa', 'Průmysl a výroba',
-              'Řemeslné práce', 'Servis a služby', 'Stavebnictví', 'Technika a energetika', 'Tisk a polygrafie',
-              'Výzkum a vývoj', 'Vzdělávání a personalistika', 'Zdravotnictví', 'Zemědělství', 'Ostatní'],
-    'Reality': ['Prodej', 'Pronájem'],
-    'Služby': ['Auto Moto', 'Cestování', 'Domácí práce', 'Esoterika', 'Hlídání dětí', 'IT, webdesign', 'Koně - služby',
-               'Kurzy a školení', 'Opravy, servis', 'Pořádání akcí', 'Právo a bezpečnost', 'Překladatelství',
-               'Přeprava a Stěhování', 'Půjčovny', 'Realitní služby', 'Reklama na auto', 'Reklamní plochy - ostatní',
-               'Řemeslné a stavební práce', 'Služby pro zvířata', 'Tvůrčí služby', 'Ubytování',
-               'Účetnictví, poradenství', 'Úklid', 'Výroba', 'Výuka hudby', 'Výuka, doučování', 'Zdraví a krása',
-               'Zprostředkovatelské služby', 'Ostatní'],
-    'Sport': ['Fitness, jogging', 'Fotbal', 'Golf', 'In-line, Skateboarding', 'Kempink', 'Letectví', 'Míčové hry',
-              'Myslivost, lov', 'Paintball, airsoft', 'Rybaření', 'Společenské hry', 'Tenis, squash, badminton',
-              'Turistika, horolezectví', 'Vodní sporty, potápění', 'Vše ostatní', 'Koloběžky', 'Horská kola',
-              'Silniční kola', 'Součástky a díly', 'Ostatní cyklistika', 'Běžkování', 'Lyžování', 'Skialpy',
-              'Snowboarding', 'Hokej, bruslení', 'Ostatní zimní'],
-    'Stroje': ['Čerpadla', 'Čistící stroje', 'Dřevoobráběcí stroje', 'Generátory', 'Historické stroje',
-               'Kovoobráběcí stroje', 'Motory', 'Potravinářské stroje', 'Skladová technika', 'Stavební stroje',
-               'Textilní stroje', 'Tiskařské stroje', 'Vybavení provozoven', 'Výrobní linky', 'Zemědělská technika',
-               'Náhradní díly', 'Ostatní'],
-    'Vstupenky': ['Dálniční známky', 'Dárkové poukazky', 'Jízdenky', 'Letenky', 'Permanentky', 'Divadlo', 'Festivaly',
-                  'Hudba, Koncerty', 'Pro děti', 'Společenské akce', 'Sport', 'Výstavy', 'Ostatní'],
-    'Zvířata': ['Akvarijní rybičky', 'Drobní savci', 'Kočky', 'Koně', 'Koně - potřeby', 'Psi', 'Ptactvo',
-                'Terarijní zvířata', 'Ostatní domácí zvířata', 'Krytí', 'Ztraceni a nalezeni', 'Chovatelské potřeby',
-                'Drůbež', 'Králíci', 'Ovce a kozy', 'Prasata', 'Skot', 'Ostatní hospodářská zvířata'],
-    'Ostatní': ['Mince, bankovky', 'Modelářství', 'Potraviny', 'Sběratelství', 'Sklo, keramika', 'Starožitnosti',
-                'Umělecké předměty', 'Zdraví a krása', 'Známky, pohledy', 'Ostatní']}
+    'Auto': [
+        'Alfa Romeo', 'Audi', 'BMW', 'Chevrolet', 'Citroën', 'Dacia', 'Fiat', 'Ford', 'Honda', 'Hyundai', 'Kia',
+        'Mazda', 'Mercedes-Benz', 'Mitsubishi', 'Nissan', 'Opel', 'Peugeot', 'Renault', 'Seat', 'Suzuki', 'Škoda',
+        'Toyota', 'Volkswagen', 'Volvo', 'Havarovaná', 'Ostatní značky', 'Náhradní díly', 'Pneumatiky, kola',
+        'Příslušenství', 'Tuning', 'Veteráni', 'Autobusy', 'Dodávky', 'Karavany, vozíky', 'Mikrobusy',
+        'Nákladní auta', 'Pick-up', 'Ostatní užitková', 'Havarovaná užitková', 'Náhradní díly užitková'
+    ],
+    'Děti': [
+        'Autosedačky', 'Baby monitory, chůvičky', 'Hračky', 'Chodítka a hopsadla', 'Kočárky', 'Kojenecké potřeby',
+        'Kola', 'Nábytek pro děti', 'Nosítka', 'Odrážedla', 'Sedačky na kolo', 'Sportovní potřeby',
+        'Školní potřeby', 'Ostatní', 'Body, dupačky a overaly', 'Bundy a kabátky', 'Čepice a kloboučky',
+        'Kalhoty, kraťasy a tepláky', 'Kombinézy', 'Komplety', 'Mikiny a svetry', 'Obuv', 'Plavky',
+        'Ponožky a punčocháče', 'Pyžámka a župánky', 'Rukavice a šály', 'Spodní prádlo', 'Sukýnky a šatičky',
+        'Trička a košile', 'Ostatní oblečení'
+    ],
+    'Dům a zahrada': [
+        'Bazény', 'Čerpadla', 'Dveře, vrata', 'Klimatizace', 'Kotle, Kamna, Bojlery',
+        'Malotraktory, Kultivátory', 'Míchačky', 'Nářadí', 'Okna', 'Pily', 'Radiátory', 'Rostliny',
+        'Sekačky', 'Sněžná technika', 'Stavební materiál', 'Vybavení dílen', 'Vysavače/Foukače',
+        'Zahradní grily', 'Zahradní technika', 'Ostatní'
+    ],
+    'Elektro': [
+        'Autorádia', 'Digestoře', 'Domácí kina', 'Epilátory, Depilátory', 'Fény, Kulmy', 'Hifi systémy, Rádia',
+        'Holící strojky', 'Kávovary', 'Ledničky', 'Mikrovlnné trouby', 'Mrazáky', 'Myčky', 'Nabíječky baterií',
+        'Pračky', 'Projektory', 'Repro soustavy', 'Ruční šlehače, Mixéry', 'Šicí stroje', 'Sluchátka',
+        'Sporáky', 'Sušičky', 'Svítidla, Lampy', 'Televize', 'Video, DVD přehrávače', 'Vysavače', 'Vysílačky',
+        'Zesilovače', 'Zvlhčovače vzduchu', 'Žehličky', 'Ostatní - bílá', 'Ostatní audio video',
+        'Ostatní drobné'
+    ],
+    'Foto': [
+        'Analogové fotoaparáty', 'Digitální fotoaparáty', 'Drony', 'Videokamery', 'Zrcadlovky', 'Baterie',
+        'Blesky a osvětlení', 'Brašny a pouzdra', 'Datové kabely', 'Filtry', 'Nabíječky baterií', 'Objektivy',
+        'Paměťové karty', 'Stativy', 'Ostatní'
+    ],
+    'Hudba': [
+        'Bicí nástroje', 'Dechové nástroje', 'Klávesové nástroje', 'Smyčcové nástroje', 'Strunné nástroje',
+        'Ostatní nástroje', 'DVD, CD, MC, LP', 'Hudebníci a skupiny', 'Koncerty', 'Noty, texty',
+        'Světelná technika', 'Zkušebny', 'Zvuková technika', 'Ostatní'
+    ],
+    'Knihy': [
+        'Beletrie', 'Časopisy', 'Cizojazyčná literatura', 'Detektivky', 'Dětská literatura', 'Drama',
+        'Encyklopedie', 'Esoterika', 'Historické romány', 'Hobby, odborné knihy', 'Kuchařky',
+        'Mapy, cestovní průvodci', 'Počítačová literatura', 'Pro mládež', 'Romány pro ženy', 'Sci-fi, Fantasy',
+        'Učebnice, skripta - Jazykové', 'Učebnice, skripta - SŠ', 'Učebnice, skripta - VŠ',
+        'Učebnice, skripta - ZŠ', 'Zábavná', 'Zdravý životní styl', 'Ostatní'
+    ],
+    'Mobily': [
+        'Apple', 'HTC', 'Huawei, Honor', 'LG', 'Motorola, Lenovo', 'Nokia, Microsoft', 'Samsung', 'Sony',
+        'Xiaomi', 'Ostatní značky', 'Baterie', 'Bezdrátové telefony', 'Datové kabely', 'Faxy', 'Headsety',
+        'HF Sady do auta', 'Chytré hodinky', 'Kryty', 'Nabíječky', 'Paměťové karty', 'Stolní telefony',
+        'Ostatní'
+        ''],
+    'Motorky': [
+        'Cestovní motocykly', 'Chopper', 'Čtyřkolky', 'Enduro', 'Minibike', 'Mopedy', 'Silniční motocykly',
+        'Skútry', 'Skútry sněžné', 'Skútry vodní', 'Tříkolky', 'Veteráni', 'Náhradní díly',
+        'Oblečení, obuv, helmy', 'Ostatní'
+    ],
+    'Nábytek': [
+        'Jídelní kouty', 'Knihovny', 'Koberce a podlah. krytina', 'Koupelny', 'Křesla a gauče', 'Kuchyně',
+        'Lampy, osvětlení', 'Ložnice', 'Matrace', 'Obývací stěny', 'Postele', 'Sedací soupravy', 'Skříně',
+        'Stoly', 'Zahradní nábytek', 'Židle', 'Doplňky', 'Ostatní nábytek'
+    ],
+    'Oblečení': [
+        'Batohy, Kufry', 'Boty', 'Bundy a Kabáty', 'Čepice a Šátky', 'Doplňky', 'Džíny', 'Halenky', 'Hodinky',
+        'Kabelky', 'Kalhoty', 'Košile', 'Kožené oděvy', 'Mikiny', 'Obleky a Saka', 'Plavky', 'Roušky',
+        'Rukavice a Šály', 'Šaty, Kostýmky', 'Šortky', 'Šperky', 'Spodní prádlo', 'Sportovní oblečení',
+        'Sukně', 'Svatební šaty', 'Těhotenské oblečení', 'Svetry', 'Termo prádlo', 'Trička, tílka', 'Ostatní'
+    ],
+    'PC': [
+        'Chladiče', 'DVD, Blu-ray mechaniky', 'GPS navigace', 'Grafické karty', 'Hard disky, SSD', 'Herní konzole',
+        'Herní zařízení', 'Hry', 'Klávesnice, myši', 'Kopírovací stroje', 'LCD monitory', 'Modemy', 'Myši',
+        'Notebooky', 'Paměti', 'PC, Počítače', 'Procesory', 'Scanery', 'Síťové prvky', 'Skříně, zdroje', 'Software',
+        'Spotřební materiál', 'Tablety, E-čtečky', 'Tiskárny', 'Wireless, WiFi', 'Základní desky', 'Záložní zdroje',
+        'Zvukové karty', 'Ostatní'
+    ],
+    'Práce': [
+        'Administrativa', 'Brigády', 'Chemie a potravinářství', 'Doprava a logistika', 'Finance a ekonomika',
+        'IT a telekomunikace', 'Management', 'Marketing a reklama', 'Obchod a prodej', 'Obrana a bezpečnost',
+        'Pohostinství a ubytování', 'Práce v domácnosti', 'Právo, legislativa', 'Průmysl a výroba',
+        'Řemeslné práce', 'Servis a služby', 'Stavebnictví', 'Technika a energetika', 'Tisk a polygrafie',
+        'Výzkum a vývoj', 'Vzdělávání a personalistika', 'Zdravotnictví', 'Zemědělství', 'Ostatní'
+    ],
+    'Reality': [
+        'Prodej', 'Pronájem'
+    ],
+    'Služby': [
+        'Auto Moto', 'Cestování', 'Domácí práce', 'Esoterika', 'Hlídání dětí', 'IT, webdesign', 'Koně - služby',
+        'Kurzy a školení', 'Opravy, servis', 'Pořádání akcí', 'Právo a bezpečnost', 'Překladatelství',
+        'Přeprava a Stěhování', 'Půjčovny', 'Realitní služby', 'Reklama na auto', 'Reklamní plochy - ostatní',
+        'Řemeslné a stavební práce', 'Služby pro zvířata', 'Tvůrčí služby', 'Ubytování',
+        'Účetnictví, poradenství', 'Úklid', 'Výroba', 'Výuka hudby', 'Výuka, doučování', 'Zdraví a krása',
+        'Zprostředkovatelské služby', 'Ostatní'
+    ],
+    'Sport': [
+        'Fitness, jogging', 'Fotbal', 'Golf', 'In-line, Skateboarding', 'Kempink', 'Letectví', 'Míčové hry',
+        'Myslivost, lov', 'Paintball, airsoft', 'Rybaření', 'Společenské hry', 'Tenis, squash, badminton',
+        'Turistika, horolezectví', 'Vodní sporty, potápění', 'Vše ostatní', 'Koloběžky', 'Horská kola',
+        'Silniční kola', 'Součástky a díly', 'Ostatní cyklistika', 'Běžkování', 'Lyžování', 'Skialpy',
+        'Snowboarding', 'Hokej, bruslení', 'Ostatní zimní'
+    ],
+    'Stroje': [
+        'Čerpadla', 'Čistící stroje', 'Dřevoobráběcí stroje', 'Generátory', 'Historické stroje',
+        'Kovoobráběcí stroje', 'Motory', 'Potravinářské stroje', 'Skladová technika', 'Stavební stroje',
+        'Textilní stroje', 'Tiskařské stroje', 'Vybavení provozoven', 'Výrobní linky', 'Zemědělská technika',
+        'Náhradní díly', 'Ostatní'
+    ],
+    'Vstupenky': [
+        'Dálniční známky', 'Dárkové poukazky', 'Jízdenky', 'Letenky', 'Permanentky', 'Divadlo', 'Festivaly',
+        'Hudba, Koncerty', 'Pro děti', 'Společenské akce', 'Sport', 'Výstavy', 'Ostatní'
+    ],
+    'Zvířata': [
+
+        'Akvarijní rybičky', 'Drobní savci', 'Kočky', 'Koně', 'Koně - potřeby', 'Psi', 'Ptactvo',
+        'Terarijní zvířata', 'Ostatní domácí zvířata', 'Krytí', 'Ztraceni a nalezeni', 'Chovatelské potřeby',
+        'Drůbež', 'Králíci', 'Ovce a kozy', 'Prasata', 'Skot', 'Ostatní hospodářská zvířata'
+
+    ],
+    'Ostatní': [
+        'Mince, bankovky', 'Modelářství', 'Potraviny', 'Sběratelství', 'Sklo, keramika', 'Starožitnosti',
+        'Umělecké předměty', 'Zdraví a krása', 'Známky, pohledy', 'Ostatní'
+    ]
+}
 
 RUBRICS_SK = {
-    'Auto': ['Alfa Romeo', 'Audi', 'BMW', 'Chevrolet', 'Citroën', 'Dacia', 'Fiat', 'Ford', 'Honda', 'Hyundai', 'Kia',
-             'Mazda', 'Mercedes-Benz', 'Mitsubishi', 'Nissan', 'Opel', 'Peugeot', 'Renault', 'Seat', 'Suzuki', 'Škoda',
-             'Toyota', 'Volkswagen', 'Volvo', 'Havarované', 'Ostatné značky', 'Náhradné diely', 'Pneumatiky, kolesá',
-             'Príslušenstvo', 'Tuning', 'Veterány', 'Autobusy', 'Dodávky', 'Karavany, vozíky', 'Mikrobusy',
-             'Nákladné autá', 'Pick-up', 'Ostatná užitková', 'Havarované užitková', 'Náhradné diely užitková'],
-    'Deti': ['Autosedačky', 'Baby monitory', 'Bicykle', 'Hračky', 'Chodítka a hopsadlá', 'Kočíky', 'Kojenecké potreby',
-             'Nábytok pre deti', 'Nosiče', 'Odrážadlá', 'Sedačky na bicykel', 'Školské potreby', 'Športové potreby',
-             'Ostatné', 'Body, dupačky a overaly', 'Bundy a kabátiky', 'Čiapky a klobúčiky', 'Kombinézy', 'Komplety',
-             'Mikiny a svetre', 'Nohavice, kraťasy a tepláky', 'Obuv', 'Plavky', 'Ponožky a pančušky',
-             'Pyžamká a župančeky', 'Rukavice a šály', 'Spodná bielizeň', 'Sukničky a šatočky', 'Tričká a košieľky',
-             'Ostatné oblečenie'],
-    'Dom a záhrada': ['Bazény', 'Čerpadlá', 'Dvere, brány', 'Klimatizácie', 'Kosačky', 'Kotle, Kachle, Bojlery',
-                      'Malotraktory, Kultivátory', 'Miešačky', 'Náradie', 'Okná', 'Píly', 'Radiátory', 'Rastliny',
-                      'Snežná technika', 'Stavebný materiál', 'Vybavenie dielne', 'Vysávače/Fúkače',
-                      'Záhradná technika', 'Záhradné grily', 'Ostatné'],
-    'Elektro': ['Autorádiá', 'Chladničky', 'Digestory', 'Domáce kiná', 'Epilátory, Depilátory', 'Fény, Kulmy',
-                'Hifi systémy, Rádiá', 'Holiace strojčeky', 'Kávovary', 'Mikrovlnné rúry', 'Mrazničky',
-                'Nabíjačky batérií', 'Práčky', 'Projektory', 'Repro sústavy', 'Ručné šľahače, Mixéry', 'Šijacie stroje',
-                'Slúchadlá', 'Sporáky', 'Sušičky', 'Svietidlá, Lampy', 'Televízory', 'Umývačky riadu',
-                'Video, DVD prehrávače', 'Vysávače', 'Vysielačky', 'Zosilňovače', 'Zvlhčovače vzduchu', 'Žehličky',
-                'Ostatné - biela', 'Ostatné audio video', 'Ostatné drobné'],
-    'Foto': ['Kinofilm', 'Digitálne fotoaparáty', 'Drony', 'Videokamery', 'Zrkadlovky', 'Batérie',
-             'Blesky a osvetlenie', 'Brašne a púzdra', 'Dátové káble', 'Filtre', 'Nabíjačky', 'Objektívy',
-             'Pamäťové karty', 'Statívy', 'Ostatné'],
-    'Hudba': ['Bicie nástroje', 'Dychové nástroje', 'Klávesové nástroje', 'Sláčikové nástroje', 'Strunové nástroje',
-              'Ostatné nástroje', 'DVD, CD, MC, LP', 'Hudobníci a skupiny', 'Koncerty', 'Noty, texty', 'Skúšobne',
-              'Svetelná technika', 'Zvuková technika', 'Ostatné'],
-    'Knihy': ['Beletria', 'Časopisy', 'Cudzojazyčná literatúra', 'Detektívky', 'Detská literatúra', 'Dráma',
-              'Encyklopédie', 'Ezoterika', 'Historické romány', 'Hobby, odborné knihy', 'Kuchárky', 'Mapy, cestovanie',
-              'Počítačová literatúra', 'Pre mládež', 'Romány pre ženy', 'Sci-fi, Fantasy',
-              'Učebnice, skriptá - Jazykové', 'Učebnice, skriptá - SŠ', 'Učebnice, skriptá - VŠ',
-              'Učebnice, skriptá - ZŠ', 'Zábavná literatúra', 'Zdravý životný štýl', 'Ostatné'],
-    'Mobily': ['Apple', 'HTC', 'Huawei, Honor', 'LG', 'Motorola, Lenovo', 'Nokia, Microsoft', 'Samsung', 'Sony',
-               'Xiaomi', 'Ostatné značky', 'Batérie', 'Bezdrôtové telefóny', 'Dátové kabely', 'Faxy', 'Headsety',
-               'HF Sady do auta', 'Inteligentné hodinky', 'Klasické telefóny', 'Kryty', 'Nabíjačky', 'Pamäťové karty',
-               'Ostatné'],
-    'Motocykle': ['Cestné motocykle', 'Cestovné motocykle', 'Chopper', 'Enduro', 'Minibike', 'Mopedy', 'Skútre',
-                  'Skútre snežné', 'Skútre vodné', 'Štvorkolky', 'Trojkolky', 'Veterány', 'Náhradné diely',
-                  'Oblečenie, obuv, helmy', 'Ostatné'],
-    'Nábytok': ['Jedálenské kúty', 'Knižnice', 'Koberce a podlahová krytina', 'Kreslá a gauče', 'Kuchyne', 'Kúpeľne',
-                'Lampy, osvetlenie', 'Matrace', 'Obývacie steny', 'Postele', 'Sedacie súpravy', 'Skrine', 'Spálne',
-                'Stoličky', 'Stoly', 'Záhradný nábytok', 'Doplnky', 'Ostatný nábytok'],
-    'Oblečenie': ['Blúzky', 'Bundy a Kabáty', 'Čiapky, Šatky', 'Doplnky', 'Džínsy', 'Funkčné prádlo', 'Hodinky',
-                  'Kabelky', 'Košele', 'Kožené oblečenie', 'Mikiny', 'Nohavice', 'Obleky, Saká', 'Plavky',
-                  'Plecniaky a kufre', 'Rukavice a Šály', 'Rúška', 'Šaty, Kostýmy', 'Šortky', 'Šperky',
-                  'Spodná bielizeň', 'Športové oblečenie', 'Sukne', 'Svadobné šaty', 'Svetre', 'Tehotenské oblečenie',
-                  'Topánky, obuv', 'Tričká, roláky, tielka', 'Ostatné'],
-    'PC': ['Chladiče', 'DVD, Blu-ray mechaniky', 'FDD, ZIPy', 'GPS navigácia', 'Grafické karty', 'Hard disky, SSD',
-           'Herné konzoly', 'Herné zariadenia', 'Hry', 'Klávesnice', 'Kopírovacie stroje', 'LCD monitory', 'Modemy',
-           'Myši', 'Notebooky', 'Pamäte', 'PC, Počítače', 'Procesory', 'Scanery', 'Sieťové komponenty',
-           'Skrine, zdroje', 'Software', 'Spotrebný materiál', 'Tablety, E-čítačky', 'Tlačiarne', 'Wireless, WiFi',
-           'Základné dosky', 'Záložné zdroje', 'Zvukové karty', 'Ostatné'],
-    'Práca': ['Administratíva', 'Brigády', 'Chémia a potravinárstvo', 'Doprava a logistika', 'Financie a ekonomika',
-              'IT a telekomunikácie', 'Management', 'Marketing a reklama', 'Obchod a predaj', 'Obrana a bezpečnosť',
-              'Pohostinstvá a ubytovanie', 'Poľnohospodárstvo', 'Práca v domácnosti', 'Právo, legislatíva',
-              'Priemysel a výroba', 'Remeselné práce', 'Servis a služby', 'Stavebníctvo', 'Technika a energetika',
-              'Tlač a polygrafia', 'Výskum a vývoj', 'Vzdelávánie a personalistika', 'Zdravotníctvo', 'Ostatné'],
-    'Reality': ['Predaj', 'Prenájom'],
-    'Služby': ['Auto Moto', 'Cestovanie', 'Domáce práce', 'Ezoterika', 'IT, webdesign', 'Kone - služby',
-               'Kurzy a školenia', 'Opravy a servis', 'Organizovanie akcií', 'Požičovne', 'Právo a bezpečnosť',
-               'Prekladateľstvo', 'Preprava a sťahovanie', 'Realitné služby', 'Reklama na auto',
-               'Reklamné plochy - ostatné', 'Remeselné a stavebné práce', 'Služby pre zvieratá',
-               'Sprostredkovateľské služby', 'Stráženie detí', 'Tvorivá práca', 'Ubytovanie',
-               'Účtovníctvo, poradenstvo', 'Upratovanie', 'Výroba', 'Výuka hudby', 'Výuka, doučovanie',
-               'Zdravie a krása', 'Ostatné'],
-    'Šport': ['Fitness, jogging', 'Futbal', 'Golf', 'In-lines, Skateboarding', 'Kemping', 'Letectvo', 'Loptové hry',
-              'Paintball, airsoft', 'Poľovníctvo', 'Rybolov', 'Spoločenské hry', 'Tenis, squash, badminton',
-              'Turistika, horolezectvo', 'Vodné športy, potápanie', 'Všetko ostatné', 'Kolobežky', 'Cestné bicykle',
-              'Horské bicykle', 'Súčiastky a diely', 'Ostatná cyklistika', 'Bežkovanie', 'Lyžovanie', 'Skialpy',
-              'Snowboarding', 'Hokej, korčuľovanie', 'Ostatné zimné'],
-    'Stroje': ['Čerpadlá', 'Čistiace stroje', 'Drevoobrábacie stroje', 'Generátory', 'Historické stroje',
-               'Kovoobrábacie stroje', 'Motory', 'Poľnohospodárska technika', 'Potravinárske stroje',
-               'Skladová technika', 'Stavebné stroje', 'Textilné stroje', 'Tlačiarenské stroje',
-               'Vybavenie prevádzkarne', 'Výrobná linka', 'Náhradné diely', 'Ostatné'],
-    'Vstupenky': ['Darčekové poukážky', 'Diaľničné známky', 'Cestovné lístky', 'Letenky', 'Permanentky', 'Divadlo',
-                  'Festivaly', 'Hudba, Koncerty', 'Pre deti', 'Spoločenské akcie', 'Šport', 'Výstavy', 'Ostatné'],
-    'Zvieratá': ['Akvarijné rybičky', 'Drobné cicavce', 'Kone', 'Kone - potreby', 'Mačky', 'Psy', 'Terárijné zvieratá',
-                 'Vtáctvo', 'Ostatné domáce zvieratá', 'Krytie', 'Stratení a nájdení', 'Chovateľské potreby', 'Dobytok',
-                 'Hydina', 'Králiky', 'Ovce a kozy', 'Prasatá', 'Ostatné hospodárske zvieratá'],
-    'Ostatné': ['Mince, bankovky', 'Modelárstvo', 'Potraviny', 'Sklo, keramika', 'Starožitnosti', 'Umelecké predmety',
-                'Zberateľstvo', 'Zdravie a krása', 'Známky, pohľadnice', 'Ostatné']}
+    'Auto': [
+        'Alfa Romeo', 'Audi', 'BMW', 'Chevrolet', 'Citroën', 'Dacia', 'Fiat', 'Ford', 'Honda', 'Hyundai', 'Kia',
+        'Mazda', 'Mercedes-Benz', 'Mitsubishi', 'Nissan', 'Opel', 'Peugeot', 'Renault', 'Seat', 'Suzuki', 'Škoda',
+        'Toyota', 'Volkswagen', 'Volvo', 'Havarované', 'Ostatné značky', 'Náhradné diely', 'Pneumatiky, kolesá',
+        'Príslušenstvo', 'Tuning', 'Veterány', 'Autobusy', 'Dodávky', 'Karavany, vozíky', 'Mikrobusy',
+        'Nákladné autá', 'Pick-up', 'Ostatná užitková', 'Havarované užitková', 'Náhradné diely užitková'
+    ],
+    'Deti': [
+        'Autosedačky', 'Baby monitory', 'Bicykle', 'Hračky', 'Chodítka a hopsadlá', 'Kočíky', 'Kojenecké potreby',
+        'Nábytok pre deti', 'Nosiče', 'Odrážadlá', 'Sedačky na bicykel', 'Školské potreby', 'Športové potreby',
+        'Ostatné', 'Body, dupačky a overaly', 'Bundy a kabátiky', 'Čiapky a klobúčiky', 'Kombinézy', 'Komplety',
+        'Mikiny a svetre', 'Nohavice, kraťasy a tepláky', 'Obuv', 'Plavky', 'Ponožky a pančušky',
+        'Pyžamká a župančeky', 'Rukavice a šály', 'Spodná bielizeň', 'Sukničky a šatočky', 'Tričká a košieľky',
+        'Ostatné oblečenie'
+    ],
+    'Dom a záhrada': [
+        'Bazény', 'Čerpadlá', 'Dvere, brány', 'Klimatizácie', 'Kosačky', 'Kotle, Kachle, Bojlery',
+        'Malotraktory, Kultivátory', 'Miešačky', 'Náradie', 'Okná', 'Píly', 'Radiátory', 'Rastliny',
+        'Snežná technika', 'Stavebný materiál', 'Vybavenie dielne', 'Vysávače/Fúkače',
+        'Záhradná technika', 'Záhradné grily', 'Ostatné'
+    ],
+    'Elektro': [
+        'Autorádiá', 'Chladničky', 'Digestory', 'Domáce kiná', 'Epilátory, Depilátory', 'Fény, Kulmy',
+        'Hifi systémy, Rádiá', 'Holiace strojčeky', 'Kávovary', 'Mikrovlnné rúry', 'Mrazničky',
+        'Nabíjačky batérií', 'Práčky', 'Projektory', 'Repro sústavy', 'Ručné šľahače, Mixéry', 'Šijacie stroje',
+        'Slúchadlá', 'Sporáky', 'Sušičky', 'Svietidlá, Lampy', 'Televízory', 'Umývačky riadu',
+        'Video, DVD prehrávače', 'Vysávače', 'Vysielačky', 'Zosilňovače', 'Zvlhčovače vzduchu', 'Žehličky',
+        'Ostatné - biela', 'Ostatné audio video', 'Ostatné drobné'
+    ],
+    'Foto': [
+        'Kinofilm', 'Digitálne fotoaparáty', 'Drony', 'Videokamery', 'Zrkadlovky', 'Batérie',
+        'Blesky a osvetlenie', 'Brašne a púzdra', 'Dátové káble', 'Filtre', 'Nabíjačky', 'Objektívy',
+        'Pamäťové karty', 'Statívy', 'Ostatné'
+    ],
+    'Hudba': [
+        'Bicie nástroje', 'Dychové nástroje', 'Klávesové nástroje', 'Sláčikové nástroje', 'Strunové nástroje',
+        'Ostatné nástroje', 'DVD, CD, MC, LP', 'Hudobníci a skupiny', 'Koncerty', 'Noty, texty', 'Skúšobne',
+        'Svetelná technika', 'Zvuková technika', 'Ostatné'
+    ],
+    'Knihy': [
+        'Beletria', 'Časopisy', 'Cudzojazyčná literatúra', 'Detektívky', 'Detská literatúra', 'Dráma',
+        'Encyklopédie', 'Ezoterika', 'Historické romány', 'Hobby, odborné knihy', 'Kuchárky', 'Mapy, cestovanie',
+        'Počítačová literatúra', 'Pre mládež', 'Romány pre ženy', 'Sci-fi, Fantasy',
+        'Učebnice, skriptá - Jazykové', 'Učebnice, skriptá - SŠ', 'Učebnice, skriptá - VŠ',
+        'Učebnice, skriptá - ZŠ', 'Zábavná literatúra', 'Zdravý životný štýl', 'Ostatné'
+    ],
+    'Mobily': [
+        'Apple', 'HTC', 'Huawei, Honor', 'LG', 'Motorola, Lenovo', 'Nokia, Microsoft', 'Samsung', 'Sony',
+        'Xiaomi', 'Ostatné značky', 'Batérie', 'Bezdrôtové telefóny', 'Dátové kabely', 'Faxy', 'Headsety',
+        'HF Sady do auta', 'Inteligentné hodinky', 'Klasické telefóny', 'Kryty', 'Nabíjačky', 'Pamäťové karty',
+        'Ostatné'
+    ],
+    'Motocykle': [
+        'Cestné motocykle', 'Cestovné motocykle', 'Chopper', 'Enduro', 'Minibike', 'Mopedy', 'Skútre',
+        'Skútre snežné', 'Skútre vodné', 'Štvorkolky', 'Trojkolky', 'Veterány', 'Náhradné diely',
+        'Oblečenie, obuv, helmy', 'Ostatné'
+    ],
+    'Nábytok': [
+        'Jedálenské kúty', 'Knižnice', 'Koberce a podlahová krytina', 'Kreslá a gauče', 'Kuchyne', 'Kúpeľne',
+        'Lampy, osvetlenie', 'Matrace', 'Obývacie steny', 'Postele', 'Sedacie súpravy', 'Skrine', 'Spálne',
+        'Stoličky', 'Stoly', 'Záhradný nábytok', 'Doplnky', 'Ostatný nábytok'
+    ],
+    'Oblečenie': [
+        'Blúzky', 'Bundy a Kabáty', 'Čiapky, Šatky', 'Doplnky', 'Džínsy', 'Funkčné prádlo', 'Hodinky',
+        'Kabelky', 'Košele', 'Kožené oblečenie', 'Mikiny', 'Nohavice', 'Obleky, Saká', 'Plavky',
+        'Plecniaky a kufre', 'Rukavice a Šály', 'Rúška', 'Šaty, Kostýmy', 'Šortky', 'Šperky',
+        'Spodná bielizeň', 'Športové oblečenie', 'Sukne', 'Svadobné šaty', 'Svetre', 'Tehotenské oblečenie',
+        'Topánky, obuv', 'Tričká, roláky, tielka', 'Ostatné'
+    ],
+    'PC': [
+        'Chladiče', 'DVD, Blu-ray mechaniky', 'FDD, ZIPy', 'GPS navigácia', 'Grafické karty', 'Hard disky, SSD',
+        'Herné konzoly', 'Herné zariadenia', 'Hry', 'Klávesnice', 'Kopírovacie stroje', 'LCD monitory', 'Modemy',
+        'Myši', 'Notebooky', 'Pamäte', 'PC, Počítače', 'Procesory', 'Scanery', 'Sieťové komponenty',
+        'Skrine, zdroje', 'Software', 'Spotrebný materiál', 'Tablety, E-čítačky', 'Tlačiarne', 'Wireless, WiFi',
+        'Základné dosky', 'Záložné zdroje', 'Zvukové karty', 'Ostatné'
+    ],
+    'Práca': [
+        'Administratíva', 'Brigády', 'Chémia a potravinárstvo', 'Doprava a logistika', 'Financie a ekonomika',
+        'IT a telekomunikácie', 'Management', 'Marketing a reklama', 'Obchod a predaj', 'Obrana a bezpečnosť',
+        'Pohostinstvá a ubytovanie', 'Poľnohospodárstvo', 'Práca v domácnosti', 'Právo, legislatíva',
+        'Priemysel a výroba', 'Remeselné práce', 'Servis a služby', 'Stavebníctvo', 'Technika a energetika',
+        'Tlač a polygrafia', 'Výskum a vývoj', 'Vzdelávánie a personalistika', 'Zdravotníctvo', 'Ostatné'
+    ],
+    'Reality': [
+        'Predaj', 'Prenájom'
+    ],
+    'Služby': [
+        'Auto Moto', 'Cestovanie', 'Domáce práce', 'Ezoterika', 'IT, webdesign', 'Kone - služby',
+        'Kurzy a školenia', 'Opravy a servis', 'Organizovanie akcií', 'Požičovne', 'Právo a bezpečnosť',
+        'Prekladateľstvo', 'Preprava a sťahovanie', 'Realitné služby', 'Reklama na auto',
+        'Reklamné plochy - ostatné', 'Remeselné a stavebné práce', 'Služby pre zvieratá',
+        'Sprostredkovateľské služby', 'Stráženie detí', 'Tvorivá práca', 'Ubytovanie',
+        'Účtovníctvo, poradenstvo', 'Upratovanie', 'Výroba', 'Výuka hudby', 'Výuka, doučovanie',
+        'Zdravie a krása', 'Ostatné'
+    ],
+    'Šport': [
+        'Fitness, jogging', 'Futbal', 'Golf', 'In-lines, Skateboarding', 'Kemping', 'Letectvo', 'Loptové hry',
+        'Paintball, airsoft', 'Poľovníctvo', 'Rybolov', 'Spoločenské hry', 'Tenis, squash, badminton',
+        'Turistika, horolezectvo', 'Vodné športy, potápanie', 'Všetko ostatné', 'Kolobežky', 'Cestné bicykle',
+        'Horské bicykle', 'Súčiastky a diely', 'Ostatná cyklistika', 'Bežkovanie', 'Lyžovanie', 'Skialpy',
+        'Snowboarding', 'Hokej, korčuľovanie', 'Ostatné zimné'
+    ],
+    'Stroje': [
+        'Čerpadlá', 'Čistiace stroje', 'Drevoobrábacie stroje', 'Generátory', 'Historické stroje',
+        'Kovoobrábacie stroje', 'Motory', 'Poľnohospodárska technika', 'Potravinárske stroje',
+        'Skladová technika', 'Stavebné stroje', 'Textilné stroje', 'Tlačiarenské stroje',
+        'Vybavenie prevádzkarne', 'Výrobná linka', 'Náhradné diely', 'Ostatné'
+    ],
+    'Vstupenky': [
+        'Darčekové poukážky', 'Diaľničné známky', 'Cestovné lístky', 'Letenky', 'Permanentky', 'Divadlo',
+        'Festivaly', 'Hudba, Koncerty', 'Pre deti', 'Spoločenské akcie', 'Šport', 'Výstavy', 'Ostatné'
+    ],
+    'Zvieratá': [
+        'Akvarijné rybičky', 'Drobné cicavce', 'Kone', 'Kone - potreby', 'Mačky', 'Psy', 'Terárijné zvieratá',
+        'Vtáctvo', 'Ostatné domáce zvieratá', 'Krytie', 'Stratení a nájdení', 'Chovateľské potreby', 'Dobytok',
+        'Hydina', 'Králiky', 'Ovce a kozy', 'Prasatá', 'Ostatné hospodárske zvieratá'
+    ],
+    'Ostatné': [
+        'Mince, bankovky', 'Modelárstvo', 'Potraviny', 'Sklo, keramika', 'Starožitnosti', 'Umelecké predmety',
+        'Zberateľstvo', 'Zdravie a krása', 'Známky, pohľadnice', 'Ostatné'
+    ]
+}
```

### Comparing `bazos-0.0.1/bazos/info/user.py` & `bazos-0.0.6/bazos/info/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # TODO: @dataclass maybe
 class User:
     def __init__(self, country: str, products_path: str):
         self.country = country
         if len(sys.argv) > 2 and path.isdir(sys.argv[1]):
             products_path = sys.argv[1]
 
-        user_info = parse_yaml(filename=path.join(products_path, f"user_{country}.yml"))
+        user_info = parse_yaml(filename=path.join(
+            products_path, f"user_{country}.yml"))
 
         self.name = user_info['name']
         self.phone_number = user_info['phone_number']
         self.email = user_info['email']
         self.password = user_info['password']
         self.psc = user_info['psc']
         self.products_path = products_path
```

### Comparing `bazos-0.0.1/bazos/shared/utils.py` & `bazos-0.0.6/bazos/shared/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,24 +49,20 @@
 
     def stop(self):
         self._timer.cancel()
         self.is_running = False
 
 
 def refactor_info_txt(_path: str):
-  for dir in next(os.walk(_path))[1]:  # loop through all directories
-    file = path.join(_path, dir, 'info.txt')
+    for dir in next(os.walk(_path))[1]:  # loop through all directories
+        file = path.join(_path, dir, 'info.txt')
 
-    assert path.isfile(file), 'File not exist: info.txt'
+        assert path.isfile(file), 'File not exist: info.txt'
 
-    with open(file=file, mode='r') as f:
-      lines = f.readlines()
+        with open(file=file, mode='r') as f:
+            lines = f.readlines()
 
-    try:
-      idx_rubric = lines.index('>>RUBRIKA\n')
-      idx_category = lines.index('>>KATEGORIE\n')
-      # lines[idx_rubric] = '>>RUBRIC\n'
-      # lines[idx_category] = '>>CATEGORY\n'
-      # with open(file=file, mode='w') as f:
-      #     f.writelines(lines)
-    except:
-      pass
+        try:
+            lines.index('>>RUBRIKA\n')
+            lines.index('>>KATEGORIE\n')
+        except BaseException:
+            pass
```

### Comparing `bazos-0.0.1/bazos.egg-info/PKG-INFO` & `bazos-0.0.6/bazos.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,81 @@
 Metadata-Version: 2.1
 Name: bazos
-Version: 0.0.1
+Version: 0.0.6
 Summary: Bazos API, that allows you to scrape bazos and upload products to bazos website.
 Author: Zdenek Lapes
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # BAZOS-API
 
-Current functionality supports removing and adding items to bazos.cz and .sk
+Current functionality supports removing and adding items to bazos.cz, bazos.sk, bazos.at and bazos.pl.
 
-## Installation:
+## Goal
+Create full-featured API for bazos.cz, bazos.sk, bazos.at and bazos.pl.
+
+## Installation
 
 ```shell
-python3 -m venv venv
-source venv/bin/activate
-pip install -r requirements.txt
+pip3 install bazos
 ```
 
+## Run
+
 ```shell
-python3 bazos --help
-python3 bazos -b --country cz sk --path $HOME/Documents/photos-archive # Remove all items from bazos.cz and bazos.sk and add new items from $HOME/Documents/photos-archive
-python3 bazos -b --country cz sk --add-only --path $HOME/Documents/photos-archive # Add new items from $HOME/Documents/photos-archive
+bazos --help
+bazos -b --country cz sk --path $HOME/Documents/photos-archive # Remove all items from bazos.cz and bazos.sk and add new items from $HOME/Documents/photos-archive
+bazos -b --country cz sk --add-only --path $HOME/Documents/photos-archive # Add new items from $HOME/Documents/photos-archive
 ```
 
+### `--country` argument
+Supported countries: `cz`, `sk`, `at`, `pl`
+
+
+### `-b|--bazos` argument
+This turn on run.
+
 ### `--path` argument
+The folder where all photos and `user_{country}.yml` file.
 
-The folder structure of directory passed to `--path` argument should look like this:
+How to structure folder defined in `--path` argument:
 
-```shell
-$HOME/Documents/photos-archive
-$HOME/Documents/photos-archive/folder1/photos/photo1.jpg
-$HOME/Documents/photos-archive/folder1/info.txt
+```yml
+# user_${bazos_country}.yml e.g.: user_cz.yml
+name: Jmeno
+phone_number: '+420123456789'
+email: user@example.com
+psc: 60200
+password: 123456
 ```
 
-### `info.txt` file structure
 
-Must follow this format:
+### Example of folder structure
+
+```shell
+bazos-ads/
+bazos-ads/user_cz.yml
+bazos-ads/user_sk.yml
+bazos-ads/item1/photos/photo1.jpg
+bazos-ads/item1/photos/photo2.jpg
+bazos-ads/item1/info.txt
+bazos-ads/item2/photos/photo1.jpg
+bazos-ads/item2/photos/photo2.jpg
+bazos-ads/item2/info.txt
+...
+```
+
+### `info.txt` syntax
 
 ```shell
 >>RUBRIC
 PC
 
 >>CATEGORY
 Notebooky
@@ -58,7 +86,32 @@
 >>PRICE
 25000
 
 >>DESCRIPTION
 Your sentences1.
 Your sentences2.
 ```
+
+
+
+## Contribution and Development
+
+Every contribution is welcome!
+
+Please follow rules inside `.pre-commit-config.yml` file.
+
+Before creating pull request, please run `pre-commit run --all-files` to check if there are no errors.
+
+### Install pre-commit hooks
+
+```shell
+pre-commit install
+```
+
+### Create virtual environment and install dependencies
+
+```shell
+python3 -m venv venv
+source venv/bin/activate
+pip install -r requirements.txt
+pip install -e .
+```
```

### Comparing `bazos-0.0.1/setup.py` & `bazos-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import os
 from setuptools import setup, find_packages
+from subprocess import Popen, PIPE
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
+version = Popen(
+    "git describe --tags | cut -d'-' -f1", stdout=PIPE, stderr=PIPE, shell=True
+).stdout.read().decode().strip()
 
 setup(
     name='bazos',
-    version='0.0.1',
+    version=version,
+    use_scm_version=True,
     description='Bazos API, that allows you to scrape bazos and upload products to bazos website.',
     author='Zdenek Lapes',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={'console_scripts': ['bazos=bazos:main']},
```

