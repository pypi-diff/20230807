# Comparing `tmp/authress-3.0.30.tar.gz` & `tmp/authress-3.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authress-3.0.30.tar", last modified: Mon Aug  7 18:32:50 2023, max compression
+gzip compressed data, was "authress-3.0.33.tar", last modified: Mon Aug  7 18:40:52 2023, max compression
```

## Comparing `authress-3.0.30.tar` & `authress-3.0.33.tar`

### file list

```diff
@@ -1,190 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.844872 authress-3.0.30/
--rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-08-07 18:32:50.844872 authress-3.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-08-07 18:32:12.000000 authress-3.0.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.800871 authress-3.0.30/authress/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-08-07 18:32:12.000000 authress-3.0.30/authress/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     6670 2023-08-07 18:32:12.000000 authress-3.0.30/authress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.808872 authress-3.0.30/authress/api/
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    78070 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/access_records_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    26872 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     9116 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/applications_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    40628 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/connections_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    54954 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/extensions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    35075 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/groups_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    27251 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/invites_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    30337 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/resource_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    32205 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/roles_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/service_client_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    47502 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/service_clients_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    32499 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/tenants_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    37628 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/user_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api/users_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-07 18:32:12.000000 authress-3.0.30/authress/api_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4416 2023-08-07 18:32:12.000000 authress-3.0.30/authress/authress_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-08-07 18:32:12.000000 authress-3.0.30/authress/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    29331 2023-08-07 18:32:12.000000 authress-3.0.30/authress/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.824872 authress-3.0.30/authress/models/
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9092 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_record_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_record_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_record_statement.py
--rw-r--r--   0 runner    (1001) docker     (122)     5053 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_request_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/access_template.py
--rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/account_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/account_links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/application_delegation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/claim_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/client_access_key.py
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/client_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4000 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/client_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/collection_links.py
--rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3523 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3831 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/connection_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/connection_default_connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/extension_application.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/extension_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/extension_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5479 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/group.py
--rw-r--r--   0 runner    (1001) docker     (122)     3824 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/group_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3241 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/identity_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4223 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/invite.py
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/link.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/linked_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/links.py
--rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/metadata_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     2668 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/metadata_object_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/o_auth_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/o_auth_token_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/o_auth_token_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     3174 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/pagination_next.py
--rw-r--r--   0 runner    (1001) docker     (122)     3940 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/permission_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/permission_collection_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/permission_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/permissioned_resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/permissioned_resource_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/resource_permission.py
--rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/resource_users_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4302 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/role.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/role_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4610 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/statement.py
--rw-r--r--   0 runner    (1001) docker     (122)     4984 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/tenant.py
--rw-r--r--   0 runner    (1001) docker     (122)     3439 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/tenant_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/tenant_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/tenant_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/token_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_connection_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)     3164 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_identity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_resources_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-08-07 18:32:12.000000 authress-3.0.30/authress/models/user_token.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:12.000000 authress-3.0.30/authress/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    12101 2023-08-07 18:32:12.000000 authress-3.0.30/authress/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.800871 authress-3.0.30/authress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-08-07 18:32:50.000000 authress-3.0.30/authress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-08-07 18:32:50.000000 authress-3.0.30/authress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 18:32:50.000000 authress-3.0.30/authress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-08-07 18:32:50.000000 authress-3.0.30/authress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-07 18:32:50.000000 authress-3.0.30/authress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-08-07 18:32:12.000000 authress-3.0.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-08-07 18:32:50.848872 authress-3.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-08-07 18:32:12.000000 authress-3.0.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.844872 authress-3.0.30/test/
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_record_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     6953 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_record_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_records_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4610 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_request_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4019 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_access_template.py
--rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_account_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_account_links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_application_delegation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_applications_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_claim_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_client_access_key.py
--rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_client_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_client_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_collection_links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2851 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_connection_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_connection_default_connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_connections_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_extension_application.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_extension_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_extension_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_extensions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_group_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_identity_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_invite.py
--rw-r--r--   0 runner    (1001) docker     (122)     1922 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_invites_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_link.py
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_linked_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_metadata_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_metadata_object_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_o_auth_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_o_auth_token_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_o_auth_token_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_pagination_next.py
--rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_permission_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_permission_collection_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_permission_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     2618 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_permissioned_resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     3943 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_permissioned_resource_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_resource_permission.py
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_resource_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3777 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_resource_users_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     4121 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_roles_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_service_client_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_service_clients_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_statement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_tenant.py
--rw-r--r--   0 runner    (1001) docker     (122)     3494 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_tenant_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_tenant_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_tenant_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_tenants_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     2322 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_connection_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_identity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_permissions_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_resources_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     2527 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_user_token.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-08-07 18:32:12.000000 authress-3.0.30/test/test_users_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:50.844872 authress-3.0.30/tests_integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 18:32:12.000000 authress-3.0.30/tests_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-08-07 18:32:12.000000 authress-3.0.30/tests_integration/test_service_client_token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.601869 authress-3.0.33/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-08-07 18:40:25.000000 authress-3.0.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-08-07 18:40:52.601869 authress-3.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-08-07 18:40:25.000000 authress-3.0.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.577869 authress-3.0.33/authress/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-08-07 18:40:26.000000 authress-3.0.33/authress/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     6670 2023-08-07 18:40:25.000000 authress-3.0.33/authress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.581869 authress-3.0.33/authress/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78070 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/access_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26872 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9116 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/applications_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40628 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54954 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/extensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35075 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27251 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/invites_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30337 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/resource_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32205 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/service_client_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47502 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/service_clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32499 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/tenants_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37628 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/user_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-08-07 18:40:25.000000 authress-3.0.33/authress/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4416 2023-08-07 18:40:25.000000 authress-3.0.33/authress/authress_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-08-07 18:40:25.000000 authress-3.0.33/authress/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29331 2023-08-07 18:40:25.000000 authress-3.0.33/authress/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.589869 authress-3.0.33/authress/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     4996 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9092 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_record_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_record_statement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5053 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_request_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/access_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/account_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/account_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/application_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/claim_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4840 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/client_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/client_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4000 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/client_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/collection_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3523 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3831 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/connection_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/connection_default_connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4548 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/extension_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/extension_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/extension_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5479 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3824 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/group_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3069 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3241 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/identity_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4223 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/invite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/linked_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/metadata_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2668 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/metadata_object_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/o_auth_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/o_auth_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/o_auth_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3174 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/pagination_next.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3940 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/permission_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/permission_collection_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/permissioned_resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/permissioned_resource_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3218 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2925 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/resource_permission.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3963 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/resource_users_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4302 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4610 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/statement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4984 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3439 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/tenant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/tenant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/tenant_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_connection_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3164 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_identity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_resources_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3372 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-08-07 18:40:25.000000 authress-3.0.33/authress/models/user_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:25.000000 authress-3.0.33/authress/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    12101 2023-08-07 18:40:25.000000 authress-3.0.33/authress/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.577869 authress-3.0.33/authress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-08-07 18:40:52.000000 authress-3.0.33/authress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5794 2023-08-07 18:40:52.000000 authress-3.0.33/authress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-07 18:40:52.000000 authress-3.0.33/authress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-08-07 18:40:52.000000 authress-3.0.33/authress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-07 18:40:52.000000 authress-3.0.33/authress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-08-07 18:40:25.000000 authress-3.0.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-08-07 18:40:52.601869 authress-3.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-08-07 18:40:25.000000 authress-3.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.597869 authress-3.0.33/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_record_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6953 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4610 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_request_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4019 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_access_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_account_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_account_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2284 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_application_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_applications_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_claim_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_client_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_client_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_client_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2484 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_collection_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2851 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_connection_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_connection_default_connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3516 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_extension_application.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_extension_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_extension_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_extensions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4923 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_group_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2022 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_identity_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_invite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1922 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_invites_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_linked_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_metadata_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_metadata_object_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_o_auth_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_o_auth_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_o_auth_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_pagination_next.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2998 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_permission_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_permission_collection_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2618 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_permissioned_resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3943 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_permissioned_resource_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_resource_permission.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_resource_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3777 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_resource_users_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4121 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1999 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_roles_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3905 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_service_client_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_service_clients_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_statement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2476 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3494 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_tenant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_tenant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_tenant_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_tenants_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2322 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_connection_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_identity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_permissions_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_resources_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2527 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2585 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-08-07 18:40:25.000000 authress-3.0.33/test/test_users_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:52.601869 authress-3.0.33/tests_integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-07 18:40:25.000000 authress-3.0.33/tests_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-08-07 18:40:25.000000 authress-3.0.33/tests_integration/test_service_client_token_provider.py
```

### Comparing `authress-3.0.30/PKG-INFO` & `authress-3.0.33/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: authress
-Version: 3.0.30
+Version: 3.0.33
 Summary: Authress SDK for authorization as a service and interact with the Authress API.
 Home-page: https://github.com/Authress/authress-sdk.py.git
 Author: Authress Developers
 Author-email: developers@authress.io
 License: Apache-2.0
 Keywords: Authorization as a service,Security,authorization,authorization as a service,authentication,user authentication,Authress,Authress client,access management,access management as a service,user security,oso,polar,open source policy engine,embedded authorization,batteries included authorization
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 <p align="center">
     <img src="https://github.com/Authress/authress-local/assets/5056218/156e3881-b359-4810-bc96-7abeaf9ddbdb" height="300px" alt="Authress Media Banner">
 </p>
 
 # Authress SDK for Python
@@ -23,15 +24,15 @@
 <p align="center">
     <a href="https://badge.fury.io/py/authress" alt="Authress pypi package">
         <img src="https://badge.fury.io/py/authress.svg">
     </a>
     <a href="https://github.com/Authress/authress-sdk.py/actions/workflows/build.yml" alt="Build status">
       <img src="https://github.com/Authress/authress-sdk.py/actions/workflows/build.yml/badge.svg">
     </a>
-    <a href="./LICENSE" alt="Apache-2.0">
+    <a href="https://github.com/Authress/authress-sdk.py/blob/release/3.0/LICENSE" alt="Apache-2.0">
       <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
     </a>
     <a href="https://authress.io/community" alt="authress community">
       <img src="https://img.shields.io/badge/Community-Authress-fbaf0b.svg">
     </a>
 </p>
 
@@ -50,21 +51,21 @@
 ## Getting Started
 
 
 ### Reference Guide
 
 See the SDK reference guide for a examples of commonly executed blocks with descriptions.
 
-[SDK Documentation](./docs/README.md)
+[SDK Documentation](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/README.md)
 
 
 ## Quick Examples:
 
-* [Authorize using a user token](./docs/EXAMPLES.md)
-* [Authorize with a service client](./docs/EXAMPLES.md)
-* [Using the Authress service client as an API key](./docs/EXAMPLES.md)
-* [Embedding service clients into your api](./docs/EXAMPLES.md)
-* [Token verification](./docs/EXAMPLES.md)
+* [Authorize using a user token](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#authorize-using-a-user-token)
+* [Authorize with a service client](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#authorize-with-a-service-client)
+* [Using the Authress service client as an API key](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#using-the-authress-service-client-as-an-api-key)
+* [Embedding service clients into your api](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#generation-of-service-client)
+* [Token verification](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#token-verifier)
 
 ## Contribution Guide
 
-[Developing for the Python SDK](./contributing.md)
+[Developing for the Python SDK](https://github.com/Authress/authress-sdk.py/blob/release/3.0/contributing.md)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: authress Version: 3.0.30 Summary: Authress SDK for
+Metadata-Version: 2.1 Name: authress Version: 3.0.33 Summary: Authress SDK for
 authorization as a service and interact with the Authress API. Home-page:
 https://github.com/Authress/authress-sdk.py.git Author: Authress Developers
 Author-email: developers@authress.io License: Apache-2.0 Keywords:
 Authorization as a service,Security,authorization,authorization as a
 service,authentication,user authentication,Authress,Authress client,access
 management,access management as a service,user security,oso,polar,open source
 policy engine,embedded authorization,batteries included authorization
-Description-Content-Type: text/markdown
+Description-Content-Type: text/markdown License-File: LICENSE
                             [Authress Media Banner]
 # Authress SDK for Python This is the Authress SDK for Python. Authress
 provides an authorization API for user identity, access control, and api key
 management as a drop in SaaS. The Nuget package connects to the [Authress API]
 (https://authress.io/app/#/api). You can use Authress to build authentication
 and authorization directly into your applications and services. Additionally,
 Authress can be used locally to develop faster without needing an [Authress
@@ -19,13 +19,21 @@
  sdk.py/actions/workflows/build.yml/badge.svg] [https://img.shields.io/badge/
     License-Apache%202.0-blue.svg] [https://img.shields.io/badge/Community-
                              Authress-fbaf0b.svg]
 ## Usage ```sh pip install authress ``` (you may need to run `pip` with root
 permission: `sudo pip install authress`) Then import the package: ```python
 import authress ``` ## Getting Started ### Reference Guide See the SDK
 reference guide for a examples of commonly executed blocks with descriptions.
-[SDK Documentation](./docs/README.md) ## Quick Examples: * [Authorize using a
-user token](./docs/EXAMPLES.md) * [Authorize with a service client](./docs/
-EXAMPLES.md) * [Using the Authress service client as an API key](./docs/
-EXAMPLES.md) * [Embedding service clients into your api](./docs/EXAMPLES.md) *
-[Token verification](./docs/EXAMPLES.md) ## Contribution Guide [Developing for
-the Python SDK](./contributing.md)
+[SDK Documentation](https://github.com/Authress/authress-sdk.py/blob/release/
+3.0/docs/README.md) ## Quick Examples: * [Authorize using a user token](https:/
+/github.com/Authress/authress-sdk.py/blob/release/3.0/docs/
+EXAMPLES.md#authorize-using-a-user-token) * [Authorize with a service client]
+(https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/
+EXAMPLES.md#authorize-with-a-service-client) * [Using the Authress service
+client as an API key](https://github.com/Authress/authress-sdk.py/blob/release/
+3.0/docs/EXAMPLES.md#using-the-authress-service-client-as-an-api-key) *
+[Embedding service clients into your api](https://github.com/Authress/authress-
+sdk.py/blob/release/3.0/docs/EXAMPLES.md#generation-of-service-client) * [Token
+verification](https://github.com/Authress/authress-sdk.py/blob/release/3.0/
+docs/EXAMPLES.md#token-verifier) ## Contribution Guide [Developing for the
+Python SDK](https://github.com/Authress/authress-sdk.py/blob/release/3.0/
+contributing.md)
```

### Comparing `authress-3.0.30/README.md` & `authress-3.0.33/authress.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: authress
+Version: 3.0.33
+Summary: Authress SDK for authorization as a service and interact with the Authress API.
+Home-page: https://github.com/Authress/authress-sdk.py.git
+Author: Authress Developers
+Author-email: developers@authress.io
+License: Apache-2.0
+Keywords: Authorization as a service,Security,authorization,authorization as a service,authentication,user authentication,Authress,Authress client,access management,access management as a service,user security,oso,polar,open source policy engine,embedded authorization,batteries included authorization
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 <p align="center">
     <img src="https://github.com/Authress/authress-local/assets/5056218/156e3881-b359-4810-bc96-7abeaf9ddbdb" height="300px" alt="Authress Media Banner">
 </p>
 
 # Authress SDK for Python
 
@@ -12,15 +24,15 @@
 <p align="center">
     <a href="https://badge.fury.io/py/authress" alt="Authress pypi package">
         <img src="https://badge.fury.io/py/authress.svg">
     </a>
     <a href="https://github.com/Authress/authress-sdk.py/actions/workflows/build.yml" alt="Build status">
       <img src="https://github.com/Authress/authress-sdk.py/actions/workflows/build.yml/badge.svg">
     </a>
-    <a href="./LICENSE" alt="Apache-2.0">
+    <a href="https://github.com/Authress/authress-sdk.py/blob/release/3.0/LICENSE" alt="Apache-2.0">
       <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg">
     </a>
     <a href="https://authress.io/community" alt="authress community">
       <img src="https://img.shields.io/badge/Community-Authress-fbaf0b.svg">
     </a>
 </p>
 
@@ -39,21 +51,21 @@
 ## Getting Started
 
 
 ### Reference Guide
 
 See the SDK reference guide for a examples of commonly executed blocks with descriptions.
 
-[SDK Documentation](./docs/README.md)
+[SDK Documentation](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/README.md)
 
 
 ## Quick Examples:
 
-* [Authorize using a user token](./docs/EXAMPLES.md)
-* [Authorize with a service client](./docs/EXAMPLES.md)
-* [Using the Authress service client as an API key](./docs/EXAMPLES.md)
-* [Embedding service clients into your api](./docs/EXAMPLES.md)
-* [Token verification](./docs/EXAMPLES.md)
+* [Authorize using a user token](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#authorize-using-a-user-token)
+* [Authorize with a service client](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#authorize-with-a-service-client)
+* [Using the Authress service client as an API key](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#using-the-authress-service-client-as-an-api-key)
+* [Embedding service clients into your api](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#generation-of-service-client)
+* [Token verification](https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/EXAMPLES.md#token-verifier)
 
 ## Contribution Guide
 
-[Developing for the Python SDK](./contributing.md)
+[Developing for the Python SDK](https://github.com/Authress/authress-sdk.py/blob/release/3.0/contributing.md)
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: authress Version: 3.0.33 Summary: Authress SDK for
+authorization as a service and interact with the Authress API. Home-page:
+https://github.com/Authress/authress-sdk.py.git Author: Authress Developers
+Author-email: developers@authress.io License: Apache-2.0 Keywords:
+Authorization as a service,Security,authorization,authorization as a
+service,authentication,user authentication,Authress,Authress client,access
+management,access management as a service,user security,oso,polar,open source
+policy engine,embedded authorization,batteries included authorization
+Description-Content-Type: text/markdown License-File: LICENSE
                             [Authress Media Banner]
 # Authress SDK for Python This is the Authress SDK for Python. Authress
 provides an authorization API for user identity, access control, and api key
 management as a drop in SaaS. The Nuget package connects to the [Authress API]
 (https://authress.io/app/#/api). You can use Authress to build authentication
 and authorization directly into your applications and services. Additionally,
 Authress can be used locally to develop faster without needing an [Authress
@@ -10,13 +19,21 @@
  sdk.py/actions/workflows/build.yml/badge.svg] [https://img.shields.io/badge/
     License-Apache%202.0-blue.svg] [https://img.shields.io/badge/Community-
                              Authress-fbaf0b.svg]
 ## Usage ```sh pip install authress ``` (you may need to run `pip` with root
 permission: `sudo pip install authress`) Then import the package: ```python
 import authress ``` ## Getting Started ### Reference Guide See the SDK
 reference guide for a examples of commonly executed blocks with descriptions.
-[SDK Documentation](./docs/README.md) ## Quick Examples: * [Authorize using a
-user token](./docs/EXAMPLES.md) * [Authorize with a service client](./docs/
-EXAMPLES.md) * [Using the Authress service client as an API key](./docs/
-EXAMPLES.md) * [Embedding service clients into your api](./docs/EXAMPLES.md) *
-[Token verification](./docs/EXAMPLES.md) ## Contribution Guide [Developing for
-the Python SDK](./contributing.md)
+[SDK Documentation](https://github.com/Authress/authress-sdk.py/blob/release/
+3.0/docs/README.md) ## Quick Examples: * [Authorize using a user token](https:/
+/github.com/Authress/authress-sdk.py/blob/release/3.0/docs/
+EXAMPLES.md#authorize-using-a-user-token) * [Authorize with a service client]
+(https://github.com/Authress/authress-sdk.py/blob/release/3.0/docs/
+EXAMPLES.md#authorize-with-a-service-client) * [Using the Authress service
+client as an API key](https://github.com/Authress/authress-sdk.py/blob/release/
+3.0/docs/EXAMPLES.md#using-the-authress-service-client-as-an-api-key) *
+[Embedding service clients into your api](https://github.com/Authress/authress-
+sdk.py/blob/release/3.0/docs/EXAMPLES.md#generation-of-service-client) * [Token
+verification](https://github.com/Authress/authress-sdk.py/blob/release/3.0/
+docs/EXAMPLES.md#token-verifier) ## Contribution Guide [Developing for the
+Python SDK](https://github.com/Authress/authress-sdk.py/blob/release/3.0/
+contributing.md)
```

### Comparing `authress-3.0.30/authress/__init__.py` & `authress-3.0.33/authress/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/__init__.py` & `authress-3.0.33/authress/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/access_records_api.py` & `authress-3.0.33/authress/api/access_records_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/accounts_api.py` & `authress-3.0.33/authress/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/applications_api.py` & `authress-3.0.33/authress/api/applications_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/connections_api.py` & `authress-3.0.33/authress/api/connections_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/extensions_api.py` & `authress-3.0.33/authress/api/extensions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/groups_api.py` & `authress-3.0.33/authress/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/invites_api.py` & `authress-3.0.33/authress/api/invites_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/resource_permissions_api.py` & `authress-3.0.33/authress/api/resource_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/roles_api.py` & `authress-3.0.33/authress/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/service_client_token_provider.py` & `authress-3.0.33/authress/api/service_client_token_provider.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/service_clients_api.py` & `authress-3.0.33/authress/api/service_clients_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/tenants_api.py` & `authress-3.0.33/authress/api/tenants_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/token_verifier.py` & `authress-3.0.33/authress/api/token_verifier.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/user_permissions_api.py` & `authress-3.0.33/authress/api/user_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api/users_api.py` & `authress-3.0.33/authress/api/users_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/api_response.py` & `authress-3.0.33/authress/api_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/authress_client.py` & `authress-3.0.33/authress/authress_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/exceptions.py` & `authress-3.0.33/authress/exceptions.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/http_client.py` & `authress-3.0.33/authress/http_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/__init__.py` & `authress-3.0.33/authress/models/__init__.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_record.py` & `authress-3.0.33/authress/models/access_record.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_record_account.py` & `authress-3.0.33/authress/models/access_record_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_record_collection.py` & `authress-3.0.33/authress/models/access_record_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_record_statement.py` & `authress-3.0.33/authress/models/access_record_statement.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_request.py` & `authress-3.0.33/authress/models/access_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_request_collection.py` & `authress-3.0.33/authress/models/access_request_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_request_response.py` & `authress-3.0.33/authress/models/access_request_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/access_template.py` & `authress-3.0.33/authress/models/access_template.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/account.py` & `authress-3.0.33/authress/models/account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/account_collection.py` & `authress-3.0.33/authress/models/account_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/account_links.py` & `authress-3.0.33/authress/models/account_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/application_delegation.py` & `authress-3.0.33/authress/models/application_delegation.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/claim_request.py` & `authress-3.0.33/authress/models/claim_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/client.py` & `authress-3.0.33/authress/models/client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/client_access_key.py` & `authress-3.0.33/authress/models/client_access_key.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/client_collection.py` & `authress-3.0.33/authress/models/client_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/client_options.py` & `authress-3.0.33/authress/models/client_options.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/collection_links.py` & `authress-3.0.33/authress/models/collection_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/connection.py` & `authress-3.0.33/authress/models/connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/connection_collection.py` & `authress-3.0.33/authress/models/connection_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/connection_data.py` & `authress-3.0.33/authress/models/connection_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/connection_default_connection_properties.py` & `authress-3.0.33/authress/models/connection_default_connection_properties.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/extension.py` & `authress-3.0.33/authress/models/extension.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/extension_application.py` & `authress-3.0.33/authress/models/extension_application.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/extension_client.py` & `authress-3.0.33/authress/models/extension_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/extension_collection.py` & `authress-3.0.33/authress/models/extension_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/group.py` & `authress-3.0.33/authress/models/group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/group_collection.py` & `authress-3.0.33/authress/models/group_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/identity.py` & `authress-3.0.33/authress/models/identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/identity_collection.py` & `authress-3.0.33/authress/models/identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/identity_request.py` & `authress-3.0.33/authress/models/identity_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/invite.py` & `authress-3.0.33/authress/models/invite.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/link.py` & `authress-3.0.33/authress/models/link.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/linked_group.py` & `authress-3.0.33/authress/models/linked_group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/links.py` & `authress-3.0.33/authress/models/links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/metadata_object.py` & `authress-3.0.33/authress/models/metadata_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/metadata_object_account.py` & `authress-3.0.33/authress/models/metadata_object_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/o_auth_authorize_response.py` & `authress-3.0.33/authress/models/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/o_auth_token_request.py` & `authress-3.0.33/authress/models/o_auth_token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/o_auth_token_response.py` & `authress-3.0.33/authress/models/o_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/pagination.py` & `authress-3.0.33/authress/models/pagination.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/pagination_next.py` & `authress-3.0.33/authress/models/pagination_next.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/permission_collection.py` & `authress-3.0.33/authress/models/permission_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/permission_collection_account.py` & `authress-3.0.33/authress/models/permission_collection_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/permission_object.py` & `authress-3.0.33/authress/models/permission_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/permissioned_resource.py` & `authress-3.0.33/authress/models/permissioned_resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/permissioned_resource_collection.py` & `authress-3.0.33/authress/models/permissioned_resource_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/resource.py` & `authress-3.0.33/authress/models/resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/resource_permission.py` & `authress-3.0.33/authress/models/resource_permission.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/resource_users_collection.py` & `authress-3.0.33/authress/models/resource_users_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/role.py` & `authress-3.0.33/authress/models/role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/role_collection.py` & `authress-3.0.33/authress/models/role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/statement.py` & `authress-3.0.33/authress/models/statement.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/tenant.py` & `authress-3.0.33/authress/models/tenant.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/tenant_collection.py` & `authress-3.0.33/authress/models/tenant_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/tenant_connection.py` & `authress-3.0.33/authress/models/tenant_connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/tenant_data.py` & `authress-3.0.33/authress/models/tenant_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/token_request.py` & `authress-3.0.33/authress/models/token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user.py` & `authress-3.0.33/authress/models/user.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_connection_credentials.py` & `authress-3.0.33/authress/models/user_connection_credentials.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_identity.py` & `authress-3.0.33/authress/models/user_identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_identity_collection.py` & `authress-3.0.33/authress/models/user_identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_resources_collection.py` & `authress-3.0.33/authress/models/user_resources_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_role.py` & `authress-3.0.33/authress/models/user_role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_role_collection.py` & `authress-3.0.33/authress/models/user_role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/models/user_token.py` & `authress-3.0.33/authress/models/user_token.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress/rest.py` & `authress-3.0.33/authress/rest.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/authress.egg-info/SOURCES.txt` & `authress-3.0.33/authress.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 authress/VERSION
 authress/__init__.py
 authress/api_response.py
```

### Comparing `authress-3.0.30/pyproject.toml` & `authress-3.0.33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/setup.py` & `authress-3.0.33/setup.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_record.py` & `authress-3.0.33/test/test_access_record.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_record_account.py` & `authress-3.0.33/test/test_access_record_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_record_collection.py` & `authress-3.0.33/test/test_access_record_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_records_api.py` & `authress-3.0.33/test/test_access_records_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_request.py` & `authress-3.0.33/test/test_access_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_request_collection.py` & `authress-3.0.33/test/test_access_request_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_request_response.py` & `authress-3.0.33/test/test_access_request_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_access_template.py` & `authress-3.0.33/test/test_access_template.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_account.py` & `authress-3.0.33/test/test_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_account_collection.py` & `authress-3.0.33/test/test_account_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_account_links.py` & `authress-3.0.33/test/test_account_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_accounts_api.py` & `authress-3.0.33/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_application_delegation.py` & `authress-3.0.33/test/test_application_delegation.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_applications_api.py` & `authress-3.0.33/test/test_applications_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_claim_request.py` & `authress-3.0.33/test/test_claim_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_client.py` & `authress-3.0.33/test/test_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_client_access_key.py` & `authress-3.0.33/test/test_client_access_key.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_client_collection.py` & `authress-3.0.33/test/test_client_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_client_options.py` & `authress-3.0.33/test/test_client_options.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_collection_links.py` & `authress-3.0.33/test/test_collection_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_connection.py` & `authress-3.0.33/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_connection_collection.py` & `authress-3.0.33/test/test_connection_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_connection_data.py` & `authress-3.0.33/test/test_connection_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_connection_default_connection_properties.py` & `authress-3.0.33/test/test_connection_default_connection_properties.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_connections_api.py` & `authress-3.0.33/test/test_connections_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_extension.py` & `authress-3.0.33/test/test_extension.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_extension_application.py` & `authress-3.0.33/test/test_extension_application.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_extension_client.py` & `authress-3.0.33/test/test_extension_client.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_extension_collection.py` & `authress-3.0.33/test/test_extension_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_extensions_api.py` & `authress-3.0.33/test/test_extensions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_group.py` & `authress-3.0.33/test/test_group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_group_collection.py` & `authress-3.0.33/test/test_group_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_groups_api.py` & `authress-3.0.33/test/test_groups_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_identity.py` & `authress-3.0.33/test/test_identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_identity_collection.py` & `authress-3.0.33/test/test_identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_identity_request.py` & `authress-3.0.33/test/test_identity_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_invite.py` & `authress-3.0.33/test/test_invite.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_invites_api.py` & `authress-3.0.33/test/test_invites_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_link.py` & `authress-3.0.33/test/test_link.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_linked_group.py` & `authress-3.0.33/test/test_linked_group.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_links.py` & `authress-3.0.33/test/test_links.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_metadata_object.py` & `authress-3.0.33/test/test_metadata_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_metadata_object_account.py` & `authress-3.0.33/test/test_metadata_object_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_o_auth_authorize_response.py` & `authress-3.0.33/test/test_o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_o_auth_token_request.py` & `authress-3.0.33/test/test_o_auth_token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_o_auth_token_response.py` & `authress-3.0.33/test/test_o_auth_token_response.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_pagination.py` & `authress-3.0.33/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_pagination_next.py` & `authress-3.0.33/test/test_pagination_next.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_permission_collection.py` & `authress-3.0.33/test/test_permission_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_permission_collection_account.py` & `authress-3.0.33/test/test_permission_collection_account.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_permission_object.py` & `authress-3.0.33/test/test_permission_object.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_permissioned_resource.py` & `authress-3.0.33/test/test_permissioned_resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_permissioned_resource_collection.py` & `authress-3.0.33/test/test_permissioned_resource_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_resource.py` & `authress-3.0.33/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_resource_permission.py` & `authress-3.0.33/test/test_resource_permission.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_resource_permissions_api.py` & `authress-3.0.33/test/test_resource_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_resource_users_collection.py` & `authress-3.0.33/test/test_resource_users_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_role.py` & `authress-3.0.33/test/test_role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_role_collection.py` & `authress-3.0.33/test/test_role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_roles_api.py` & `authress-3.0.33/test/test_roles_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_service_client_token_provider.py` & `authress-3.0.33/test/test_service_client_token_provider.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_service_clients_api.py` & `authress-3.0.33/test/test_service_clients_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_statement.py` & `authress-3.0.33/test/test_statement.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_tenant.py` & `authress-3.0.33/test/test_tenant.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_tenant_collection.py` & `authress-3.0.33/test/test_tenant_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_tenant_connection.py` & `authress-3.0.33/test/test_tenant_connection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_tenant_data.py` & `authress-3.0.33/test/test_tenant_data.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_tenants_api.py` & `authress-3.0.33/test/test_tenants_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_token_request.py` & `authress-3.0.33/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_token_verifier.py` & `authress-3.0.33/test/test_token_verifier.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user.py` & `authress-3.0.33/test/test_user.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_connection_credentials.py` & `authress-3.0.33/test/test_user_connection_credentials.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_identity.py` & `authress-3.0.33/test/test_user_identity.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_identity_collection.py` & `authress-3.0.33/test/test_user_identity_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_permissions_api.py` & `authress-3.0.33/test/test_user_permissions_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_resources_collection.py` & `authress-3.0.33/test/test_user_resources_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_role.py` & `authress-3.0.33/test/test_user_role.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_role_collection.py` & `authress-3.0.33/test/test_user_role_collection.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_user_token.py` & `authress-3.0.33/test/test_user_token.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/test/test_users_api.py` & `authress-3.0.33/test/test_users_api.py`

 * *Files identical despite different names*

### Comparing `authress-3.0.30/tests_integration/test_service_client_token_provider.py` & `authress-3.0.33/tests_integration/test_service_client_token_provider.py`

 * *Files identical despite different names*

