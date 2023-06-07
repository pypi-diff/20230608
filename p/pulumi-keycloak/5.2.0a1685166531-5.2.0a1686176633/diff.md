# Comparing `tmp/pulumi_keycloak-5.2.0a1685166531.tar.gz` & `tmp/pulumi_keycloak-5.2.0a1686176633.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_keycloak-5.2.0a1685166531.tar", last modified: Sat May 27 06:01:03 2023, max compression
+gzip compressed data, was "pulumi_keycloak-5.2.0a1686176633.tar", last modified: Wed Jun  7 22:36:49 2023, max compression
```

## Comparing `pulumi_keycloak-5.2.0a1685166531.tar` & `pulumi_keycloak-5.2.0a1686176633.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.647539 pulumi_keycloak-5.2.0a1685166531/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-27 06:01:03.647539 pulumi_keycloak-5.2.0a1685166531/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.631539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/
--rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102617 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/attribute_to_role_identity_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.639539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/execution_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/subflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.639539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/custom_identity_provider_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/custom_user_federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/default_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_client_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_client_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_authentication_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_authentication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_client_description_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    37193 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_realm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_realm_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_user_realm_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/hardcoded_role_identity_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.639539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/full_name_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    57296 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/hardcoded_group_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/hardcoded_role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46485 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/role_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/user_attribute_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    85992 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/user_federation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.639539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69494 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/oidc/google_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    82330 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/oidc/identity_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.647539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/audience_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
--rw-r--r--   0 runner    (1001) docker     (123)   146214 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_aggregate_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18086 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_authorization_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_authorization_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_authorization_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_default_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_group_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_js_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_optional_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20270 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_service_account_realm_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_service_account_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_time_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_user_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/full_name_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client_authorization_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client_service_account_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    29689 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/group_membership_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    32107 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34832 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    37290 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30199 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    94592 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   154864 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_aes_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_ecdsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_hmac_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_java_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    19806 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_rsa_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/required_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.647539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    99872 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/client_default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/client_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/get_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/get_client_installation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)   101571 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28175 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/script_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    25945 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/user_property_protocol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/users_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 06:01:03.635539 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 06:01:03.647539 pulumi_keycloak-5.2.0a1685166531/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-27 06:01:03.000000 pulumi_keycloak-5.2.0a1685166531/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.984303 pulumi_keycloak-5.2.0a1686176633/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-07 22:36:49.984303 pulumi_keycloak-5.2.0a1686176633/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.968303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/
+-rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102617 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/attribute_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/attribute_to_role_identity_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.972303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15432 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/execution_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23130 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/subflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.972303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/custom_identity_provider_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29602 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/custom_user_federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/default_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_client_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_client_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_authentication_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_authentication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_client_description_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37193 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_realm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_realm_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_user_realm_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18844 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/hardcoded_role_identity_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.976303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/full_name_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57296 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/hardcoded_group_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19079 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/hardcoded_role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/msad_user_account_control_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46485 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/role_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31107 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/user_attribute_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85992 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/user_federation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.976303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69494 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/oidc/google_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82330 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/oidc/identity_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.980303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/audience_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146214 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_aggregate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18086 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_authorization_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_authorization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_authorization_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_default_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_group_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14315 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_js_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_optional_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23020 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20270 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_service_account_realm_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_service_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_time_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/full_name_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client_authorization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client_service_account_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29689 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/group_membership_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32107 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21973 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34832 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37290 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38593 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_client_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30199 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_session_note_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94592 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   157967 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_aes_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_ecdsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_hmac_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25062 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_java_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19806 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_rsa_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18132 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/required_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.984303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99872 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/client_default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/client_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/get_client_installation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103281 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28175 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/script_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25945 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/user_attribute_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/user_property_protocol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27809 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16660 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user_template_importer_identity_provider_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/users_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:36:49.972303 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:36:49.984303 pulumi_keycloak-5.2.0a1686176633/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-07 22:36:49.000000 pulumi_keycloak-5.2.0a1686176633/setup.py
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/PKG-INFO` & `pulumi_keycloak-5.2.0a1686176633/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_keycloak
-Version: 5.2.0a1685166531
+Version: 5.2.0a1686176633
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi keycloak
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-keycloak/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-keycloak/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fkeycloak.svg)](https://www.npmjs.com/package/@pulumi/keycloak)
 [![Python version](https://badge.fury.io/py/pulumi-keycloak.svg)](https://pypi.org/project/pulumi-keycloak)
 [![NuGet version](https://badge.fury.io/nu/pulumi.keycloak.svg)](https://badge.fury.io/nu/pulumi.keycloak)
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/README.md` & `pulumi_keycloak-5.2.0a1686176633/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/__init__.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/_inputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/_utilities.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/attribute_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/attribute_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/attribute_to_role_identity_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/attribute_to_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/bindings.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/bindings.py`

 * *Files 6% similar despite different names*

```diff
@@ -260,14 +260,28 @@
                  direct_grant_flow: Optional[pulumi.Input[str]] = None,
                  docker_authentication_flow: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  registration_flow: Optional[pulumi.Input[str]] = None,
                  reset_credentials_flow: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Allows for creating and managing realm authentication flow bindings within Keycloak.
+
+        [Authentication flows](https://www.keycloak.org/docs/latest/server_admin/index.html#_authentication-flows) describe a sequence
+        of actions that a user or service must perform in order to be authenticated to Keycloak. The authentication flow itself
+        is a container for these actions, which are otherwise known as executions.
+
+        Realms assign authentication flows to supported user flows such as `registration` and `browser`. This resource allows the
+        updating of realm authentication flow bindings to custom authentication flows created by `authentication.Flow`.
+
+        Note that you can also use the `Realm` resource to assign authentication flow bindings at the realm level. This
+        resource is useful if you would like to create a realm and an authentication flow, and assign this flow to the realm within
+        a single run of `pulumi up`. In any case, do not attempt to use both the arguments within the `Realm` resource
+        and this resource to manage authentication flow bindings, you should choose one or the other.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
@@ -307,14 +321,28 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: BindingsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Allows for creating and managing realm authentication flow bindings within Keycloak.
+
+        [Authentication flows](https://www.keycloak.org/docs/latest/server_admin/index.html#_authentication-flows) describe a sequence
+        of actions that a user or service must perform in order to be authenticated to Keycloak. The authentication flow itself
+        is a container for these actions, which are otherwise known as executions.
+
+        Realms assign authentication flows to supported user flows such as `registration` and `browser`. This resource allows the
+        updating of realm authentication flow bindings to custom authentication flows created by `authentication.Flow`.
+
+        Note that you can also use the `Realm` resource to assign authentication flow bindings at the realm level. This
+        resource is useful if you would like to create a realm and an authentication flow, and assign this flow to the realm within
+        a single run of `pulumi up`. In any case, do not attempt to use both the arguments within the `Realm` resource
+        and this resource to manage authentication flow bindings, you should choose one or the other.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/execution.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/execution_config.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/execution_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/flow.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/authentication/subflow.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/authentication/subflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/config/vars.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/custom_identity_provider_mapping.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/custom_identity_provider_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/custom_user_federation.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/custom_user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/default_groups.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/default_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/default_roles.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_client_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_client_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_client_role_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_client_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/generic_role_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/generic_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_authentication_execution.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_authentication_execution.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_authentication_flow.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_authentication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_client_description_converter.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_client_description_converter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_group.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_realm.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_realm.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_realm_keys.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_realm_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_role.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_user.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/get_user_realm_roles.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/get_user_realm_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group_memberships.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group_memberships.py`

 * *Files 23% similar despite different names*

```diff
@@ -127,14 +127,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Allows for managing a Keycloak group's members.
+
+        Note that this resource attempts to be an **authoritative** source over group members. When this resource takes control
+        over a group's members, users that are manually added to the group will be removed, and users that are manually removed
+        from the group will be added upon the next run of `pulumi up`.
+
+        Also note that you should not use `GroupMemberships` with a group has been assigned as a default group via
+        `DefaultGroups`.
+
+        This resource **should not** be used to control membership of a group that has its members federated from an external
+        source via group mapping.
+
+        To non-exclusively manage the group's of a user, see the [`UserGroups` resource][1]
+
+        This resource paginates its data loading on refresh by 50 items.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
@@ -163,14 +179,30 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GroupMembershipsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Allows for managing a Keycloak group's members.
+
+        Note that this resource attempts to be an **authoritative** source over group members. When this resource takes control
+        over a group's members, users that are manually added to the group will be removed, and users that are manually removed
+        from the group will be added upon the next run of `pulumi up`.
+
+        Also note that you should not use `GroupMemberships` with a group has been assigned as a default group via
+        `DefaultGroups`.
+
+        This resource **should not** be used to control membership of a group that has its members federated from an external
+        source via group mapping.
+
+        To non-exclusively manage the group's of a user, see the [`UserGroups` resource][1]
+
+        This resource paginates its data loading on refresh by 50 items.
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group_permissions.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/group_roles.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/group_roles.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,23 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  exhaustive: Optional[pulumi.Input[bool]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  role_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
+        Allows you to manage roles assigned to a Keycloak group.
+
+        If `exhaustive` is true, this resource attempts to be an **authoritative** source over group roles: roles that are manually added to the group will be removed, and roles that are manually removed from the
+        group will be added upon the next run of `pulumi up`.
+        If `exhaustive` is false, this resource is a partial assignation of roles to a group. As a result, you can get multiple `GroupRoles` for the same `group_id`.
+
+        Note that when assigning composite roles to a group, you may see a non-empty plan following a `pulumi up` if you
+        assign a role and a composite that includes that role to the same group.
+
         ## Example Usage
         ### Exhaustive Roles)
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
@@ -246,14 +255,23 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GroupRolesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Allows you to manage roles assigned to a Keycloak group.
+
+        If `exhaustive` is true, this resource attempts to be an **authoritative** source over group roles: roles that are manually added to the group will be removed, and roles that are manually removed from the
+        group will be added upon the next run of `pulumi up`.
+        If `exhaustive` is false, this resource is a partial assignation of roles to a group. As a result, you can get multiple `GroupRoles` for the same `group_id`.
+
+        Note that when assigning composite roles to a group, you may see a non-empty plan following a `pulumi up` if you
+        assign a role and a composite that includes that role to the same group.
+
         ## Example Usage
         ### Exhaustive Roles)
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/hardcoded_attribute_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/hardcoded_role_identity_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/hardcoded_role_identity_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/identity_provider_token_exchange_scope_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/__init__.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/_inputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/full_name_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/full_name_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/group_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/hardcoded_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/hardcoded_group_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/hardcoded_group_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/hardcoded_role_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/hardcoded_role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/msad_lds_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/msad_user_account_control_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/msad_user_account_control_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/outputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/role_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/role_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/user_attribute_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/user_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/ldap/user_federation.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/ldap/user_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/oidc/google_identity_provider.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/oidc/google_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/oidc/identity_provider.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/oidc/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/__init__.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/_inputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/audience_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/audience_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/audience_resolve_protocol_mappter.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_aggregate_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_aggregate_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_authorization_permission.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_authorization_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_authorization_resource.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_authorization_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_authorization_scope.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_authorization_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_default_scopes.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_default_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_group_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_group_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_js_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_js_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_optional_scopes.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_optional_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_permissions.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_role_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_scope.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_service_account_realm_role.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_service_account_realm_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_service_account_role.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_service_account_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_time_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_time_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/client_user_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/client_user_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/full_name_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/full_name_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client_authorization_policy.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client_authorization_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClientAuthorizationPolicyResult:
     """
     This data source can be used to fetch policy and permission information for an OpenID client that has authorization enabled.
 
     ## Example Usage
 
     In this example, we'll create a new OpenID client with authorization enabled. This will cause Keycloak to create a default
-    permission for this client called "Default Permission". We'll use the _openid_get_client_authorization_policy_ data
+    permission for this client called "Default Permission". We'll use the `openid_get_client_authorization_policy` data
     source to fetch information about this permission, so we can use it to create a new resource-based authorization permission.
 
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
@@ -233,15 +233,15 @@
                                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClientAuthorizationPolicyResult]:
     """
     This data source can be used to fetch policy and permission information for an OpenID client that has authorization enabled.
 
     ## Example Usage
 
     In this example, we'll create a new OpenID client with authorization enabled. This will cause Keycloak to create a default
-    permission for this client called "Default Permission". We'll use the _openid_get_client_authorization_policy_ data
+    permission for this client called "Default Permission". We'll use the `openid_get_client_authorization_policy` data
     source to fetch information about this permission, so we can use it to create a new resource-based authorization permission.
 
     ```python
     import pulumi
     import pulumi_keycloak as keycloak
 
     realm = keycloak.Realm("realm",
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client_scope.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/get_client_service_account_user.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/get_client_service_account_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/group_membership_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/group_membership_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/hardcoded_claim_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/hardcoded_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/outputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/script_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_client_role_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_client_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_property_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_realm_role_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/openid/user_session_note_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/openid/user_session_note_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/outputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/provider.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,26 @@
         :param pulumi.Input[bool] edit_username_allowed: When true, the username field is editable.
         :param pulumi.Input[str] email_theme: Used for emails that are sent by Keycloak.
         :param pulumi.Input[bool] enabled: When `false`, users and clients will not be able to access this realm. Defaults to `true`.
         :param pulumi.Input[str] internal_id: When specified, this will be used as the realm's internal ID within Keycloak. When not specified, the realm's internal ID will be set to the realm's name.
         :param pulumi.Input[str] login_theme: Used for the login, forgot password, and registration pages.
         :param pulumi.Input[bool] login_with_email_allowed: When true, users may log in with their email address.
         :param pulumi.Input[str] oauth2_device_code_lifespan: The maximum amount of time a client has to finish the device code flow before it expires.
+               
+               The attributes below should be specified in seconds.
         :param pulumi.Input[int] oauth2_device_polling_interval: The minimum amount of time in seconds that the client should wait between polling requests to the token endpoint.
         :param pulumi.Input[str] offline_session_idle_timeout: The amount of time an offline session can be idle before it expires.
         :param pulumi.Input[str] offline_session_max_lifespan: The maximum amount of time before an offline session expires regardless of activity.
         :param pulumi.Input[bool] offline_session_max_lifespan_enabled: Enable `offline_session_max_lifespan`.
         :param pulumi.Input[str] password_policy: The password policy for users within the realm.
+               
+               The arguments below can be used to configure authentication flow bindings:
         :param pulumi.Input[int] refresh_token_max_reuse: Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+               
+               The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         :param pulumi.Input[bool] registration_allowed: When true, user registration will be enabled, and a link for registration will be displayed on the login page.
         :param pulumi.Input[bool] registration_email_as_username: When true, the user's email will be used as their username during registration.
         :param pulumi.Input[str] registration_flow: The desired flow for user registration. Defaults to `registration`.
         :param pulumi.Input[bool] remember_me: When true, a "remember me" checkbox will be displayed on the login page, and the user's session will not expire between browser restarts.
         :param pulumi.Input[str] reset_credentials_flow: The desired flow to use when a user attempts to reset their credentials. Defaults to `reset credentials`.
         :param pulumi.Input[bool] reset_password_allowed: When true, a "forgot password" link will be displayed on the login page.
         :param pulumi.Input[bool] revoke_refresh_token: If enabled a refresh token can only be used number of times specified in 'refresh_token_max_reuse' before they are revoked. If unspecified, refresh tokens can be reused.
@@ -119,14 +125,16 @@
         :param pulumi.Input[str] sso_session_idle_timeout: The amount of time a session can be idle before it expires.
         :param pulumi.Input[str] sso_session_idle_timeout_remember_me: Similar to `sso_session_idle_timeout`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_idle_timeout`.
         :param pulumi.Input[str] sso_session_max_lifespan: The maximum amount of time before a session expires regardless of activity.
         :param pulumi.Input[str] sso_session_max_lifespan_remember_me: Similar to `sso_session_max_lifespan`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_max_lifespan`.
         :param pulumi.Input[bool] user_managed_access: When `true`, users are allowed to manage their own resources. Defaults to `false`.
         :param pulumi.Input[bool] verify_email: When true, users are required to verify their email address after registration and after email address changes.
         :param pulumi.Input['RealmWebAuthnPasswordlessPolicyArgs'] web_authn_passwordless_policy: Configuration for WebAuthn Passwordless Policy authentication.
+               
+               Each of these attributes are blocks with the following attributes:
         :param pulumi.Input['RealmWebAuthnPolicyArgs'] web_authn_policy: Configuration for WebAuthn Policy authentication.
         """
         pulumi.set(__self__, "realm", realm)
         if access_code_lifespan is not None:
             pulumi.set(__self__, "access_code_lifespan", access_code_lifespan)
         if access_code_lifespan_login is not None:
             pulumi.set(__self__, "access_code_lifespan_login", access_code_lifespan_login)
@@ -589,14 +597,16 @@
         pulumi.set(self, "login_with_email_allowed", value)
 
     @property
     @pulumi.getter(name="oauth2DeviceCodeLifespan")
     def oauth2_device_code_lifespan(self) -> Optional[pulumi.Input[str]]:
         """
         The maximum amount of time a client has to finish the device code flow before it expires.
+
+        The attributes below should be specified in seconds.
         """
         return pulumi.get(self, "oauth2_device_code_lifespan")
 
     @oauth2_device_code_lifespan.setter
     def oauth2_device_code_lifespan(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oauth2_device_code_lifespan", value)
 
@@ -658,26 +668,30 @@
         pulumi.set(self, "otp_policy", value)
 
     @property
     @pulumi.getter(name="passwordPolicy")
     def password_policy(self) -> Optional[pulumi.Input[str]]:
         """
         The password policy for users within the realm.
+
+        The arguments below can be used to configure authentication flow bindings:
         """
         return pulumi.get(self, "password_policy")
 
     @password_policy.setter
     def password_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password_policy", value)
 
     @property
     @pulumi.getter(name="refreshTokenMaxReuse")
     def refresh_token_max_reuse(self) -> Optional[pulumi.Input[int]]:
         """
         Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+
+        The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         """
         return pulumi.get(self, "refresh_token_max_reuse")
 
     @refresh_token_max_reuse.setter
     def refresh_token_max_reuse(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "refresh_token_max_reuse", value)
 
@@ -868,14 +882,16 @@
         pulumi.set(self, "verify_email", value)
 
     @property
     @pulumi.getter(name="webAuthnPasswordlessPolicy")
     def web_authn_passwordless_policy(self) -> Optional[pulumi.Input['RealmWebAuthnPasswordlessPolicyArgs']]:
         """
         Configuration for WebAuthn Passwordless Policy authentication.
+
+        Each of these attributes are blocks with the following attributes:
         """
         return pulumi.get(self, "web_authn_passwordless_policy")
 
     @web_authn_passwordless_policy.setter
     def web_authn_passwordless_policy(self, value: Optional[pulumi.Input['RealmWebAuthnPasswordlessPolicyArgs']]):
         pulumi.set(self, "web_authn_passwordless_policy", value)
 
@@ -976,21 +992,27 @@
         :param pulumi.Input[bool] edit_username_allowed: When true, the username field is editable.
         :param pulumi.Input[str] email_theme: Used for emails that are sent by Keycloak.
         :param pulumi.Input[bool] enabled: When `false`, users and clients will not be able to access this realm. Defaults to `true`.
         :param pulumi.Input[str] internal_id: When specified, this will be used as the realm's internal ID within Keycloak. When not specified, the realm's internal ID will be set to the realm's name.
         :param pulumi.Input[str] login_theme: Used for the login, forgot password, and registration pages.
         :param pulumi.Input[bool] login_with_email_allowed: When true, users may log in with their email address.
         :param pulumi.Input[str] oauth2_device_code_lifespan: The maximum amount of time a client has to finish the device code flow before it expires.
+               
+               The attributes below should be specified in seconds.
         :param pulumi.Input[int] oauth2_device_polling_interval: The minimum amount of time in seconds that the client should wait between polling requests to the token endpoint.
         :param pulumi.Input[str] offline_session_idle_timeout: The amount of time an offline session can be idle before it expires.
         :param pulumi.Input[str] offline_session_max_lifespan: The maximum amount of time before an offline session expires regardless of activity.
         :param pulumi.Input[bool] offline_session_max_lifespan_enabled: Enable `offline_session_max_lifespan`.
         :param pulumi.Input[str] password_policy: The password policy for users within the realm.
+               
+               The arguments below can be used to configure authentication flow bindings:
         :param pulumi.Input[str] realm: The name of the realm. This is unique across Keycloak. This will also be used as the realm's internal ID within Keycloak.
         :param pulumi.Input[int] refresh_token_max_reuse: Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+               
+               The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         :param pulumi.Input[bool] registration_allowed: When true, user registration will be enabled, and a link for registration will be displayed on the login page.
         :param pulumi.Input[bool] registration_email_as_username: When true, the user's email will be used as their username during registration.
         :param pulumi.Input[str] registration_flow: The desired flow for user registration. Defaults to `registration`.
         :param pulumi.Input[bool] remember_me: When true, a "remember me" checkbox will be displayed on the login page, and the user's session will not expire between browser restarts.
         :param pulumi.Input[str] reset_credentials_flow: The desired flow to use when a user attempts to reset their credentials. Defaults to `reset credentials`.
         :param pulumi.Input[bool] reset_password_allowed: When true, a "forgot password" link will be displayed on the login page.
         :param pulumi.Input[bool] revoke_refresh_token: If enabled a refresh token can only be used number of times specified in 'refresh_token_max_reuse' before they are revoked. If unspecified, refresh tokens can be reused.
@@ -998,14 +1020,16 @@
         :param pulumi.Input[str] sso_session_idle_timeout: The amount of time a session can be idle before it expires.
         :param pulumi.Input[str] sso_session_idle_timeout_remember_me: Similar to `sso_session_idle_timeout`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_idle_timeout`.
         :param pulumi.Input[str] sso_session_max_lifespan: The maximum amount of time before a session expires regardless of activity.
         :param pulumi.Input[str] sso_session_max_lifespan_remember_me: Similar to `sso_session_max_lifespan`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_max_lifespan`.
         :param pulumi.Input[bool] user_managed_access: When `true`, users are allowed to manage their own resources. Defaults to `false`.
         :param pulumi.Input[bool] verify_email: When true, users are required to verify their email address after registration and after email address changes.
         :param pulumi.Input['RealmWebAuthnPasswordlessPolicyArgs'] web_authn_passwordless_policy: Configuration for WebAuthn Passwordless Policy authentication.
+               
+               Each of these attributes are blocks with the following attributes:
         :param pulumi.Input['RealmWebAuthnPolicyArgs'] web_authn_policy: Configuration for WebAuthn Policy authentication.
         """
         if access_code_lifespan is not None:
             pulumi.set(__self__, "access_code_lifespan", access_code_lifespan)
         if access_code_lifespan_login is not None:
             pulumi.set(__self__, "access_code_lifespan_login", access_code_lifespan_login)
         if access_code_lifespan_user_action is not None:
@@ -1457,14 +1481,16 @@
         pulumi.set(self, "login_with_email_allowed", value)
 
     @property
     @pulumi.getter(name="oauth2DeviceCodeLifespan")
     def oauth2_device_code_lifespan(self) -> Optional[pulumi.Input[str]]:
         """
         The maximum amount of time a client has to finish the device code flow before it expires.
+
+        The attributes below should be specified in seconds.
         """
         return pulumi.get(self, "oauth2_device_code_lifespan")
 
     @oauth2_device_code_lifespan.setter
     def oauth2_device_code_lifespan(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "oauth2_device_code_lifespan", value)
 
@@ -1526,14 +1552,16 @@
         pulumi.set(self, "otp_policy", value)
 
     @property
     @pulumi.getter(name="passwordPolicy")
     def password_policy(self) -> Optional[pulumi.Input[str]]:
         """
         The password policy for users within the realm.
+
+        The arguments below can be used to configure authentication flow bindings:
         """
         return pulumi.get(self, "password_policy")
 
     @password_policy.setter
     def password_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password_policy", value)
 
@@ -1550,14 +1578,16 @@
         pulumi.set(self, "realm", value)
 
     @property
     @pulumi.getter(name="refreshTokenMaxReuse")
     def refresh_token_max_reuse(self) -> Optional[pulumi.Input[int]]:
         """
         Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+
+        The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         """
         return pulumi.get(self, "refresh_token_max_reuse")
 
     @refresh_token_max_reuse.setter
     def refresh_token_max_reuse(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "refresh_token_max_reuse", value)
 
@@ -1748,14 +1778,16 @@
         pulumi.set(self, "verify_email", value)
 
     @property
     @pulumi.getter(name="webAuthnPasswordlessPolicy")
     def web_authn_passwordless_policy(self) -> Optional[pulumi.Input['RealmWebAuthnPasswordlessPolicyArgs']]:
         """
         Configuration for WebAuthn Passwordless Policy authentication.
+
+        Each of these attributes are blocks with the following attributes:
         """
         return pulumi.get(self, "web_authn_passwordless_policy")
 
     @web_authn_passwordless_policy.setter
     def web_authn_passwordless_policy(self, value: Optional[pulumi.Input['RealmWebAuthnPasswordlessPolicyArgs']]):
         pulumi.set(self, "web_authn_passwordless_policy", value)
 
@@ -1941,21 +1973,27 @@
         :param pulumi.Input[bool] edit_username_allowed: When true, the username field is editable.
         :param pulumi.Input[str] email_theme: Used for emails that are sent by Keycloak.
         :param pulumi.Input[bool] enabled: When `false`, users and clients will not be able to access this realm. Defaults to `true`.
         :param pulumi.Input[str] internal_id: When specified, this will be used as the realm's internal ID within Keycloak. When not specified, the realm's internal ID will be set to the realm's name.
         :param pulumi.Input[str] login_theme: Used for the login, forgot password, and registration pages.
         :param pulumi.Input[bool] login_with_email_allowed: When true, users may log in with their email address.
         :param pulumi.Input[str] oauth2_device_code_lifespan: The maximum amount of time a client has to finish the device code flow before it expires.
+               
+               The attributes below should be specified in seconds.
         :param pulumi.Input[int] oauth2_device_polling_interval: The minimum amount of time in seconds that the client should wait between polling requests to the token endpoint.
         :param pulumi.Input[str] offline_session_idle_timeout: The amount of time an offline session can be idle before it expires.
         :param pulumi.Input[str] offline_session_max_lifespan: The maximum amount of time before an offline session expires regardless of activity.
         :param pulumi.Input[bool] offline_session_max_lifespan_enabled: Enable `offline_session_max_lifespan`.
         :param pulumi.Input[str] password_policy: The password policy for users within the realm.
+               
+               The arguments below can be used to configure authentication flow bindings:
         :param pulumi.Input[str] realm: The name of the realm. This is unique across Keycloak. This will also be used as the realm's internal ID within Keycloak.
         :param pulumi.Input[int] refresh_token_max_reuse: Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+               
+               The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         :param pulumi.Input[bool] registration_allowed: When true, user registration will be enabled, and a link for registration will be displayed on the login page.
         :param pulumi.Input[bool] registration_email_as_username: When true, the user's email will be used as their username during registration.
         :param pulumi.Input[str] registration_flow: The desired flow for user registration. Defaults to `registration`.
         :param pulumi.Input[bool] remember_me: When true, a "remember me" checkbox will be displayed on the login page, and the user's session will not expire between browser restarts.
         :param pulumi.Input[str] reset_credentials_flow: The desired flow to use when a user attempts to reset their credentials. Defaults to `reset credentials`.
         :param pulumi.Input[bool] reset_password_allowed: When true, a "forgot password" link will be displayed on the login page.
         :param pulumi.Input[bool] revoke_refresh_token: If enabled a refresh token can only be used number of times specified in 'refresh_token_max_reuse' before they are revoked. If unspecified, refresh tokens can be reused.
@@ -1963,14 +2001,16 @@
         :param pulumi.Input[str] sso_session_idle_timeout: The amount of time a session can be idle before it expires.
         :param pulumi.Input[str] sso_session_idle_timeout_remember_me: Similar to `sso_session_idle_timeout`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_idle_timeout`.
         :param pulumi.Input[str] sso_session_max_lifespan: The maximum amount of time before a session expires regardless of activity.
         :param pulumi.Input[str] sso_session_max_lifespan_remember_me: Similar to `sso_session_max_lifespan`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_max_lifespan`.
         :param pulumi.Input[bool] user_managed_access: When `true`, users are allowed to manage their own resources. Defaults to `false`.
         :param pulumi.Input[bool] verify_email: When true, users are required to verify their email address after registration and after email address changes.
         :param pulumi.Input[pulumi.InputType['RealmWebAuthnPasswordlessPolicyArgs']] web_authn_passwordless_policy: Configuration for WebAuthn Passwordless Policy authentication.
+               
+               Each of these attributes are blocks with the following attributes:
         :param pulumi.Input[pulumi.InputType['RealmWebAuthnPolicyArgs']] web_authn_policy: Configuration for WebAuthn Policy authentication.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RealmArgs,
@@ -2291,21 +2331,27 @@
         :param pulumi.Input[bool] edit_username_allowed: When true, the username field is editable.
         :param pulumi.Input[str] email_theme: Used for emails that are sent by Keycloak.
         :param pulumi.Input[bool] enabled: When `false`, users and clients will not be able to access this realm. Defaults to `true`.
         :param pulumi.Input[str] internal_id: When specified, this will be used as the realm's internal ID within Keycloak. When not specified, the realm's internal ID will be set to the realm's name.
         :param pulumi.Input[str] login_theme: Used for the login, forgot password, and registration pages.
         :param pulumi.Input[bool] login_with_email_allowed: When true, users may log in with their email address.
         :param pulumi.Input[str] oauth2_device_code_lifespan: The maximum amount of time a client has to finish the device code flow before it expires.
+               
+               The attributes below should be specified in seconds.
         :param pulumi.Input[int] oauth2_device_polling_interval: The minimum amount of time in seconds that the client should wait between polling requests to the token endpoint.
         :param pulumi.Input[str] offline_session_idle_timeout: The amount of time an offline session can be idle before it expires.
         :param pulumi.Input[str] offline_session_max_lifespan: The maximum amount of time before an offline session expires regardless of activity.
         :param pulumi.Input[bool] offline_session_max_lifespan_enabled: Enable `offline_session_max_lifespan`.
         :param pulumi.Input[str] password_policy: The password policy for users within the realm.
+               
+               The arguments below can be used to configure authentication flow bindings:
         :param pulumi.Input[str] realm: The name of the realm. This is unique across Keycloak. This will also be used as the realm's internal ID within Keycloak.
         :param pulumi.Input[int] refresh_token_max_reuse: Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+               
+               The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         :param pulumi.Input[bool] registration_allowed: When true, user registration will be enabled, and a link for registration will be displayed on the login page.
         :param pulumi.Input[bool] registration_email_as_username: When true, the user's email will be used as their username during registration.
         :param pulumi.Input[str] registration_flow: The desired flow for user registration. Defaults to `registration`.
         :param pulumi.Input[bool] remember_me: When true, a "remember me" checkbox will be displayed on the login page, and the user's session will not expire between browser restarts.
         :param pulumi.Input[str] reset_credentials_flow: The desired flow to use when a user attempts to reset their credentials. Defaults to `reset credentials`.
         :param pulumi.Input[bool] reset_password_allowed: When true, a "forgot password" link will be displayed on the login page.
         :param pulumi.Input[bool] revoke_refresh_token: If enabled a refresh token can only be used number of times specified in 'refresh_token_max_reuse' before they are revoked. If unspecified, refresh tokens can be reused.
@@ -2313,14 +2359,16 @@
         :param pulumi.Input[str] sso_session_idle_timeout: The amount of time a session can be idle before it expires.
         :param pulumi.Input[str] sso_session_idle_timeout_remember_me: Similar to `sso_session_idle_timeout`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_idle_timeout`.
         :param pulumi.Input[str] sso_session_max_lifespan: The maximum amount of time before a session expires regardless of activity.
         :param pulumi.Input[str] sso_session_max_lifespan_remember_me: Similar to `sso_session_max_lifespan`, but used when a user clicks "Remember Me". If not set, Keycloak will default to the value of `sso_session_max_lifespan`.
         :param pulumi.Input[bool] user_managed_access: When `true`, users are allowed to manage their own resources. Defaults to `false`.
         :param pulumi.Input[bool] verify_email: When true, users are required to verify their email address after registration and after email address changes.
         :param pulumi.Input[pulumi.InputType['RealmWebAuthnPasswordlessPolicyArgs']] web_authn_passwordless_policy: Configuration for WebAuthn Passwordless Policy authentication.
+               
+               Each of these attributes are blocks with the following attributes:
         :param pulumi.Input[pulumi.InputType['RealmWebAuthnPolicyArgs']] web_authn_policy: Configuration for WebAuthn Policy authentication.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RealmState.__new__(_RealmState)
 
         __props__.__dict__["access_code_lifespan"] = access_code_lifespan
@@ -2605,14 +2653,16 @@
         return pulumi.get(self, "login_with_email_allowed")
 
     @property
     @pulumi.getter(name="oauth2DeviceCodeLifespan")
     def oauth2_device_code_lifespan(self) -> pulumi.Output[str]:
         """
         The maximum amount of time a client has to finish the device code flow before it expires.
+
+        The attributes below should be specified in seconds.
         """
         return pulumi.get(self, "oauth2_device_code_lifespan")
 
     @property
     @pulumi.getter(name="oauth2DevicePollingInterval")
     def oauth2_device_polling_interval(self) -> pulumi.Output[int]:
         """
@@ -2650,14 +2700,16 @@
         return pulumi.get(self, "otp_policy")
 
     @property
     @pulumi.getter(name="passwordPolicy")
     def password_policy(self) -> pulumi.Output[Optional[str]]:
         """
         The password policy for users within the realm.
+
+        The arguments below can be used to configure authentication flow bindings:
         """
         return pulumi.get(self, "password_policy")
 
     @property
     @pulumi.getter
     def realm(self) -> pulumi.Output[str]:
         """
@@ -2666,14 +2718,16 @@
         return pulumi.get(self, "realm")
 
     @property
     @pulumi.getter(name="refreshTokenMaxReuse")
     def refresh_token_max_reuse(self) -> pulumi.Output[Optional[int]]:
         """
         Maximum number of times a refresh token can be reused before they are revoked. If unspecified and 'revoke_refresh_token' is enabled the default value is 0 and refresh tokens can not be reused.
+
+        The arguments below should be specified as [Go duration strings](https://golang.org/pkg/time/#Duration.String). They will default to Keycloak's default settings.
         """
         return pulumi.get(self, "refresh_token_max_reuse")
 
     @property
     @pulumi.getter(name="registrationAllowed")
     def registration_allowed(self) -> pulumi.Output[bool]:
         """
@@ -2796,14 +2850,16 @@
         return pulumi.get(self, "verify_email")
 
     @property
     @pulumi.getter(name="webAuthnPasswordlessPolicy")
     def web_authn_passwordless_policy(self) -> pulumi.Output['outputs.RealmWebAuthnPasswordlessPolicy']:
         """
         Configuration for WebAuthn Passwordless Policy authentication.
+
+        Each of these attributes are blocks with the following attributes:
         """
         return pulumi.get(self, "web_authn_passwordless_policy")
 
     @property
     @pulumi.getter(name="webAuthnPolicy")
     def web_authn_policy(self) -> pulumi.Output['outputs.RealmWebAuthnPolicy']:
         """
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_events.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_aes_generated.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_aes_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_ecdsa_generated.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_ecdsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_hmac_generated.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_hmac_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_java_generated.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_java_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
                  active: Optional[pulumi.Input[bool]] = None,
                  algorithm: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a RealmKeystoreJavaGenerated resource.
-        :param pulumi.Input[str] key_alias: Alias for the private key
-        :param pulumi.Input[str] key_password: Password for the private key
+        :param pulumi.Input[str] key_alias: Alias for the private key.
+        :param pulumi.Input[str] key_password: Password for the private key.
         :param pulumi.Input[str] keystore: Path to keys file on keycloak instance.
-        :param pulumi.Input[str] keystore_password: Password for the private key.
+        :param pulumi.Input[str] keystore_password: Password for the keys.
         :param pulumi.Input[str] realm_id: The realm this keystore exists in.
         :param pulumi.Input[bool] active: When `false`, key in not used for signing. Defaults to `true`.
         :param pulumi.Input[str] algorithm: Intended algorithm for the key. Defaults to `RS256`
         :param pulumi.Input[bool] enabled: When `false`, key is not accessible in this realm. Defaults to `true`.
         :param pulumi.Input[str] name: Display name of provider when linked in admin console.
         :param pulumi.Input[int] priority: Priority for the provider. Defaults to `0`
         """
@@ -53,27 +53,27 @@
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
 
     @property
     @pulumi.getter(name="keyAlias")
     def key_alias(self) -> pulumi.Input[str]:
         """
-        Alias for the private key
+        Alias for the private key.
         """
         return pulumi.get(self, "key_alias")
 
     @key_alias.setter
     def key_alias(self, value: pulumi.Input[str]):
         pulumi.set(self, "key_alias", value)
 
     @property
     @pulumi.getter(name="keyPassword")
     def key_password(self) -> pulumi.Input[str]:
         """
-        Password for the private key
+        Password for the private key.
         """
         return pulumi.get(self, "key_password")
 
     @key_password.setter
     def key_password(self, value: pulumi.Input[str]):
         pulumi.set(self, "key_password", value)
 
@@ -89,15 +89,15 @@
     def keystore(self, value: pulumi.Input[str]):
         pulumi.set(self, "keystore", value)
 
     @property
     @pulumi.getter(name="keystorePassword")
     def keystore_password(self) -> pulumi.Input[str]:
         """
-        Password for the private key.
+        Password for the keys.
         """
         return pulumi.get(self, "keystore_password")
 
     @keystore_password.setter
     def keystore_password(self, value: pulumi.Input[str]):
         pulumi.set(self, "keystore_password", value)
 
@@ -188,18 +188,18 @@
                  priority: Optional[pulumi.Input[int]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RealmKeystoreJavaGenerated resources.
         :param pulumi.Input[bool] active: When `false`, key in not used for signing. Defaults to `true`.
         :param pulumi.Input[str] algorithm: Intended algorithm for the key. Defaults to `RS256`
         :param pulumi.Input[bool] enabled: When `false`, key is not accessible in this realm. Defaults to `true`.
-        :param pulumi.Input[str] key_alias: Alias for the private key
-        :param pulumi.Input[str] key_password: Password for the private key
+        :param pulumi.Input[str] key_alias: Alias for the private key.
+        :param pulumi.Input[str] key_password: Password for the private key.
         :param pulumi.Input[str] keystore: Path to keys file on keycloak instance.
-        :param pulumi.Input[str] keystore_password: Password for the private key.
+        :param pulumi.Input[str] keystore_password: Password for the keys.
         :param pulumi.Input[str] name: Display name of provider when linked in admin console.
         :param pulumi.Input[int] priority: Priority for the provider. Defaults to `0`
         :param pulumi.Input[str] realm_id: The realm this keystore exists in.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if algorithm is not None:
@@ -257,27 +257,27 @@
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="keyAlias")
     def key_alias(self) -> Optional[pulumi.Input[str]]:
         """
-        Alias for the private key
+        Alias for the private key.
         """
         return pulumi.get(self, "key_alias")
 
     @key_alias.setter
     def key_alias(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_alias", value)
 
     @property
     @pulumi.getter(name="keyPassword")
     def key_password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the private key
+        Password for the private key.
         """
         return pulumi.get(self, "key_password")
 
     @key_password.setter
     def key_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_password", value)
 
@@ -293,15 +293,15 @@
     def keystore(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keystore", value)
 
     @property
     @pulumi.getter(name="keystorePassword")
     def keystore_password(self) -> Optional[pulumi.Input[str]]:
         """
-        Password for the private key.
+        Password for the keys.
         """
         return pulumi.get(self, "keystore_password")
 
     @keystore_password.setter
     def keystore_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "keystore_password", value)
 
@@ -359,31 +359,50 @@
                  realm_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Allows for creating and managing `java-keystore` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_keycloak as keycloak
+
+        realm = keycloak.Realm("realm", realm="my-realm")
+        java_keystore = keycloak.RealmKeystoreJavaGenerated("javaKeystore",
+            realm_id=realm.id,
+            enabled=True,
+            active=True,
+            keystore="<path to your keystore>",
+            keystore_password="<password for keystore>",
+            key_alias="<alias for the private key>",
+            key_password="<password for the private key>",
+            priority=100,
+            algorithm="RS256")
+        ```
+
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI. Examplebash
 
         ```sh
          $ pulumi import keycloak:index/realmKeystoreJavaGenerated:RealmKeystoreJavaGenerated java_keystore my-realm/618cfba7-49aa-4c09-9a19-2f699b576f0b
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: When `false`, key in not used for signing. Defaults to `true`.
         :param pulumi.Input[str] algorithm: Intended algorithm for the key. Defaults to `RS256`
         :param pulumi.Input[bool] enabled: When `false`, key is not accessible in this realm. Defaults to `true`.
-        :param pulumi.Input[str] key_alias: Alias for the private key
-        :param pulumi.Input[str] key_password: Password for the private key
+        :param pulumi.Input[str] key_alias: Alias for the private key.
+        :param pulumi.Input[str] key_password: Password for the private key.
         :param pulumi.Input[str] keystore: Path to keys file on keycloak instance.
-        :param pulumi.Input[str] keystore_password: Password for the private key.
+        :param pulumi.Input[str] keystore_password: Password for the keys.
         :param pulumi.Input[str] name: Display name of provider when linked in admin console.
         :param pulumi.Input[int] priority: Priority for the provider. Defaults to `0`
         :param pulumi.Input[str] realm_id: The realm this keystore exists in.
         """
         ...
     @overload
     def __init__(__self__,
@@ -391,14 +410,33 @@
                  args: RealmKeystoreJavaGeneratedArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Allows for creating and managing `java-keystore` Realm keystores within Keycloak.
 
         A realm keystore manages generated key pairs that are used by Keycloak to perform cryptographic signatures and encryption.
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_keycloak as keycloak
+
+        realm = keycloak.Realm("realm", realm="my-realm")
+        java_keystore = keycloak.RealmKeystoreJavaGenerated("javaKeystore",
+            realm_id=realm.id,
+            enabled=True,
+            active=True,
+            keystore="<path to your keystore>",
+            keystore_password="<password for keystore>",
+            key_alias="<alias for the private key>",
+            key_password="<password for the private key>",
+            priority=100,
+            algorithm="RS256")
+        ```
+
         ## Import
 
         Realm keys can be imported using realm name and keystore id, you can find it in web UI. Examplebash
 
         ```sh
          $ pulumi import keycloak:index/realmKeystoreJavaGenerated:RealmKeystoreJavaGenerated java_keystore my-realm/618cfba7-49aa-4c09-9a19-2f699b576f0b
         ```
@@ -483,18 +521,18 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: When `false`, key in not used for signing. Defaults to `true`.
         :param pulumi.Input[str] algorithm: Intended algorithm for the key. Defaults to `RS256`
         :param pulumi.Input[bool] enabled: When `false`, key is not accessible in this realm. Defaults to `true`.
-        :param pulumi.Input[str] key_alias: Alias for the private key
-        :param pulumi.Input[str] key_password: Password for the private key
+        :param pulumi.Input[str] key_alias: Alias for the private key.
+        :param pulumi.Input[str] key_password: Password for the private key.
         :param pulumi.Input[str] keystore: Path to keys file on keycloak instance.
-        :param pulumi.Input[str] keystore_password: Password for the private key.
+        :param pulumi.Input[str] keystore_password: Password for the keys.
         :param pulumi.Input[str] name: Display name of provider when linked in admin console.
         :param pulumi.Input[int] priority: Priority for the provider. Defaults to `0`
         :param pulumi.Input[str] realm_id: The realm this keystore exists in.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RealmKeystoreJavaGeneratedState.__new__(_RealmKeystoreJavaGeneratedState)
@@ -535,23 +573,23 @@
         """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="keyAlias")
     def key_alias(self) -> pulumi.Output[str]:
         """
-        Alias for the private key
+        Alias for the private key.
         """
         return pulumi.get(self, "key_alias")
 
     @property
     @pulumi.getter(name="keyPassword")
     def key_password(self) -> pulumi.Output[str]:
         """
-        Password for the private key
+        Password for the private key.
         """
         return pulumi.get(self, "key_password")
 
     @property
     @pulumi.getter
     def keystore(self) -> pulumi.Output[str]:
         """
@@ -559,15 +597,15 @@
         """
         return pulumi.get(self, "keystore")
 
     @property
     @pulumi.getter(name="keystorePassword")
     def keystore_password(self) -> pulumi.Output[str]:
         """
-        Password for the private key.
+        Password for the keys.
         """
         return pulumi.get(self, "keystore_password")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_rsa.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_rsa.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_keystore_rsa_generated.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_keystore_rsa_generated.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/realm_user_profile.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/realm_user_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/required_action.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/required_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/role.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/__init__.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/_inputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/client.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/client_default_scope.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/client_default_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/client_scope.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/client_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/get_client.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/get_client_installation_provider.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/get_client_installation_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/identity_provider.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/identity_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                  enabled: Optional[pulumi.Input[bool]] = None,
                  extra_config: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  first_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  force_authn: Optional[pulumi.Input[bool]] = None,
                  gui_order: Optional[pulumi.Input[str]] = None,
                  hide_on_login_page: Optional[pulumi.Input[bool]] = None,
                  link_only: Optional[pulumi.Input[bool]] = None,
+                 login_hint: Optional[pulumi.Input[str]] = None,
                  name_id_policy_format: Optional[pulumi.Input[str]] = None,
                  post_binding_authn_request: Optional[pulumi.Input[bool]] = None,
                  post_binding_logout: Optional[pulumi.Input[bool]] = None,
                  post_binding_response: Optional[pulumi.Input[bool]] = None,
                  post_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  principal_attribute: Optional[pulumi.Input[str]] = None,
                  principal_type: Optional[pulumi.Input[str]] = None,
@@ -65,14 +66,15 @@
         :param pulumi.Input[str] display_name: The display name for the realm that is shown when logging in to the admin console.
         :param pulumi.Input[bool] enabled: When `false`, users and clients will not be able to access this realm. Defaults to `true`.
         :param pulumi.Input[str] first_broker_login_flow_alias: Alias of authentication flow, which is triggered after first login with this identity provider. Term 'First Login' means that there is not yet existing Keycloak account linked with the authenticated identity provider account. Defaults to `first broker login`.
         :param pulumi.Input[bool] force_authn: Indicates whether the identity provider must authenticate the presenter directly rather than rely on a previous security context.
         :param pulumi.Input[str] gui_order: A number defining the order of this identity provider in the GUI.
         :param pulumi.Input[bool] hide_on_login_page: If hidden, then login with this provider is possible only if requested explicitly, e.g. using the 'kc_idp_hint' parameter.
         :param pulumi.Input[bool] link_only: When `true`, users cannot login using this provider, but their existing accounts will be linked when possible. Defaults to `false`.
+        :param pulumi.Input[str] login_hint: Login Hint.
         :param pulumi.Input[str] name_id_policy_format: Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         :param pulumi.Input[bool] post_binding_authn_request: Indicates whether the AuthnRequest must be sent using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_logout: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_response: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used..
         :param pulumi.Input[str] post_broker_login_flow_alias: Alias of authentication flow, which is triggered after each login with this identity provider. Useful if you want additional verification of each user authenticated with this identity provider (for example OTP). Leave this empty if you don't want any additional authenticators to be triggered after login with this identity provider. Also note, that authenticator implementations must assume that user is already set in ClientSession as identity provider already set it. Defaults to empty.
         :param pulumi.Input[str] principal_attribute: The principal attribute.
         :param pulumi.Input[str] principal_type: The principal type. Can be one of `SUBJECT`, `ATTRIBUTE` or `FRIENDLY_ATTRIBUTE`.
@@ -116,14 +118,16 @@
             pulumi.set(__self__, "force_authn", force_authn)
         if gui_order is not None:
             pulumi.set(__self__, "gui_order", gui_order)
         if hide_on_login_page is not None:
             pulumi.set(__self__, "hide_on_login_page", hide_on_login_page)
         if link_only is not None:
             pulumi.set(__self__, "link_only", link_only)
+        if login_hint is not None:
+            pulumi.set(__self__, "login_hint", login_hint)
         if name_id_policy_format is not None:
             pulumi.set(__self__, "name_id_policy_format", name_id_policy_format)
         if post_binding_authn_request is not None:
             pulumi.set(__self__, "post_binding_authn_request", post_binding_authn_request)
         if post_binding_logout is not None:
             pulumi.set(__self__, "post_binding_logout", post_binding_logout)
         if post_binding_response is not None:
@@ -367,14 +371,26 @@
         return pulumi.get(self, "link_only")
 
     @link_only.setter
     def link_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "link_only", value)
 
     @property
+    @pulumi.getter(name="loginHint")
+    def login_hint(self) -> Optional[pulumi.Input[str]]:
+        """
+        Login Hint.
+        """
+        return pulumi.get(self, "login_hint")
+
+    @login_hint.setter
+    def login_hint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "login_hint", value)
+
+    @property
     @pulumi.getter(name="nameIdPolicyFormat")
     def name_id_policy_format(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         """
         return pulumi.get(self, "name_id_policy_format")
 
@@ -603,14 +619,15 @@
                  extra_config: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  first_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  force_authn: Optional[pulumi.Input[bool]] = None,
                  gui_order: Optional[pulumi.Input[str]] = None,
                  hide_on_login_page: Optional[pulumi.Input[bool]] = None,
                  internal_id: Optional[pulumi.Input[str]] = None,
                  link_only: Optional[pulumi.Input[bool]] = None,
+                 login_hint: Optional[pulumi.Input[str]] = None,
                  name_id_policy_format: Optional[pulumi.Input[str]] = None,
                  post_binding_authn_request: Optional[pulumi.Input[bool]] = None,
                  post_binding_logout: Optional[pulumi.Input[bool]] = None,
                  post_binding_response: Optional[pulumi.Input[bool]] = None,
                  post_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  principal_attribute: Optional[pulumi.Input[str]] = None,
                  principal_type: Optional[pulumi.Input[str]] = None,
@@ -641,14 +658,15 @@
         :param pulumi.Input[str] entity_id: The Entity ID that will be used to uniquely identify this SAML Service Provider.
         :param pulumi.Input[str] first_broker_login_flow_alias: Alias of authentication flow, which is triggered after first login with this identity provider. Term 'First Login' means that there is not yet existing Keycloak account linked with the authenticated identity provider account. Defaults to `first broker login`.
         :param pulumi.Input[bool] force_authn: Indicates whether the identity provider must authenticate the presenter directly rather than rely on a previous security context.
         :param pulumi.Input[str] gui_order: A number defining the order of this identity provider in the GUI.
         :param pulumi.Input[bool] hide_on_login_page: If hidden, then login with this provider is possible only if requested explicitly, e.g. using the 'kc_idp_hint' parameter.
         :param pulumi.Input[str] internal_id: Internal Identity Provider Id
         :param pulumi.Input[bool] link_only: When `true`, users cannot login using this provider, but their existing accounts will be linked when possible. Defaults to `false`.
+        :param pulumi.Input[str] login_hint: Login Hint.
         :param pulumi.Input[str] name_id_policy_format: Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         :param pulumi.Input[bool] post_binding_authn_request: Indicates whether the AuthnRequest must be sent using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_logout: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_response: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used..
         :param pulumi.Input[str] post_broker_login_flow_alias: Alias of authentication flow, which is triggered after each login with this identity provider. Useful if you want additional verification of each user authenticated with this identity provider (for example OTP). Leave this empty if you don't want any additional authenticators to be triggered after login with this identity provider. Also note, that authenticator implementations must assume that user is already set in ClientSession as identity provider already set it. Defaults to empty.
         :param pulumi.Input[str] principal_attribute: The principal attribute.
         :param pulumi.Input[str] principal_type: The principal type. Can be one of `SUBJECT`, `ATTRIBUTE` or `FRIENDLY_ATTRIBUTE`.
@@ -696,14 +714,16 @@
             pulumi.set(__self__, "gui_order", gui_order)
         if hide_on_login_page is not None:
             pulumi.set(__self__, "hide_on_login_page", hide_on_login_page)
         if internal_id is not None:
             pulumi.set(__self__, "internal_id", internal_id)
         if link_only is not None:
             pulumi.set(__self__, "link_only", link_only)
+        if login_hint is not None:
+            pulumi.set(__self__, "login_hint", login_hint)
         if name_id_policy_format is not None:
             pulumi.set(__self__, "name_id_policy_format", name_id_policy_format)
         if post_binding_authn_request is not None:
             pulumi.set(__self__, "post_binding_authn_request", post_binding_authn_request)
         if post_binding_logout is not None:
             pulumi.set(__self__, "post_binding_logout", post_binding_logout)
         if post_binding_response is not None:
@@ -939,14 +959,26 @@
         return pulumi.get(self, "link_only")
 
     @link_only.setter
     def link_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "link_only", value)
 
     @property
+    @pulumi.getter(name="loginHint")
+    def login_hint(self) -> Optional[pulumi.Input[str]]:
+        """
+        Login Hint.
+        """
+        return pulumi.get(self, "login_hint")
+
+    @login_hint.setter
+    def login_hint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "login_hint", value)
+
+    @property
     @pulumi.getter(name="nameIdPolicyFormat")
     def name_id_policy_format(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         """
         return pulumi.get(self, "name_id_policy_format")
 
@@ -1200,14 +1232,15 @@
                  entity_id: Optional[pulumi.Input[str]] = None,
                  extra_config: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  first_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  force_authn: Optional[pulumi.Input[bool]] = None,
                  gui_order: Optional[pulumi.Input[str]] = None,
                  hide_on_login_page: Optional[pulumi.Input[bool]] = None,
                  link_only: Optional[pulumi.Input[bool]] = None,
+                 login_hint: Optional[pulumi.Input[str]] = None,
                  name_id_policy_format: Optional[pulumi.Input[str]] = None,
                  post_binding_authn_request: Optional[pulumi.Input[bool]] = None,
                  post_binding_logout: Optional[pulumi.Input[bool]] = None,
                  post_binding_response: Optional[pulumi.Input[bool]] = None,
                  post_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  principal_attribute: Optional[pulumi.Input[str]] = None,
                  principal_type: Optional[pulumi.Input[str]] = None,
@@ -1275,14 +1308,15 @@
         :param pulumi.Input[bool] enabled: When `false`, users and clients will not be able to access this realm. Defaults to `true`.
         :param pulumi.Input[str] entity_id: The Entity ID that will be used to uniquely identify this SAML Service Provider.
         :param pulumi.Input[str] first_broker_login_flow_alias: Alias of authentication flow, which is triggered after first login with this identity provider. Term 'First Login' means that there is not yet existing Keycloak account linked with the authenticated identity provider account. Defaults to `first broker login`.
         :param pulumi.Input[bool] force_authn: Indicates whether the identity provider must authenticate the presenter directly rather than rely on a previous security context.
         :param pulumi.Input[str] gui_order: A number defining the order of this identity provider in the GUI.
         :param pulumi.Input[bool] hide_on_login_page: If hidden, then login with this provider is possible only if requested explicitly, e.g. using the 'kc_idp_hint' parameter.
         :param pulumi.Input[bool] link_only: When `true`, users cannot login using this provider, but their existing accounts will be linked when possible. Defaults to `false`.
+        :param pulumi.Input[str] login_hint: Login Hint.
         :param pulumi.Input[str] name_id_policy_format: Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         :param pulumi.Input[bool] post_binding_authn_request: Indicates whether the AuthnRequest must be sent using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_logout: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_response: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used..
         :param pulumi.Input[str] post_broker_login_flow_alias: Alias of authentication flow, which is triggered after each login with this identity provider. Useful if you want additional verification of each user authenticated with this identity provider (for example OTP). Leave this empty if you don't want any additional authenticators to be triggered after login with this identity provider. Also note, that authenticator implementations must assume that user is already set in ClientSession as identity provider already set it. Defaults to empty.
         :param pulumi.Input[str] principal_attribute: The principal attribute.
         :param pulumi.Input[str] principal_type: The principal type. Can be one of `SUBJECT`, `ATTRIBUTE` or `FRIENDLY_ATTRIBUTE`.
@@ -1370,14 +1404,15 @@
                  entity_id: Optional[pulumi.Input[str]] = None,
                  extra_config: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  first_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  force_authn: Optional[pulumi.Input[bool]] = None,
                  gui_order: Optional[pulumi.Input[str]] = None,
                  hide_on_login_page: Optional[pulumi.Input[bool]] = None,
                  link_only: Optional[pulumi.Input[bool]] = None,
+                 login_hint: Optional[pulumi.Input[str]] = None,
                  name_id_policy_format: Optional[pulumi.Input[str]] = None,
                  post_binding_authn_request: Optional[pulumi.Input[bool]] = None,
                  post_binding_logout: Optional[pulumi.Input[bool]] = None,
                  post_binding_response: Optional[pulumi.Input[bool]] = None,
                  post_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
                  principal_attribute: Optional[pulumi.Input[str]] = None,
                  principal_type: Optional[pulumi.Input[str]] = None,
@@ -1419,14 +1454,15 @@
             __props__.__dict__["entity_id"] = entity_id
             __props__.__dict__["extra_config"] = extra_config
             __props__.__dict__["first_broker_login_flow_alias"] = first_broker_login_flow_alias
             __props__.__dict__["force_authn"] = force_authn
             __props__.__dict__["gui_order"] = gui_order
             __props__.__dict__["hide_on_login_page"] = hide_on_login_page
             __props__.__dict__["link_only"] = link_only
+            __props__.__dict__["login_hint"] = login_hint
             __props__.__dict__["name_id_policy_format"] = name_id_policy_format
             __props__.__dict__["post_binding_authn_request"] = post_binding_authn_request
             __props__.__dict__["post_binding_logout"] = post_binding_logout
             __props__.__dict__["post_binding_response"] = post_binding_response
             __props__.__dict__["post_broker_login_flow_alias"] = post_broker_login_flow_alias
             __props__.__dict__["principal_attribute"] = principal_attribute
             __props__.__dict__["principal_type"] = principal_type
@@ -1471,14 +1507,15 @@
             extra_config: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             first_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
             force_authn: Optional[pulumi.Input[bool]] = None,
             gui_order: Optional[pulumi.Input[str]] = None,
             hide_on_login_page: Optional[pulumi.Input[bool]] = None,
             internal_id: Optional[pulumi.Input[str]] = None,
             link_only: Optional[pulumi.Input[bool]] = None,
+            login_hint: Optional[pulumi.Input[str]] = None,
             name_id_policy_format: Optional[pulumi.Input[str]] = None,
             post_binding_authn_request: Optional[pulumi.Input[bool]] = None,
             post_binding_logout: Optional[pulumi.Input[bool]] = None,
             post_binding_response: Optional[pulumi.Input[bool]] = None,
             post_broker_login_flow_alias: Optional[pulumi.Input[str]] = None,
             principal_attribute: Optional[pulumi.Input[str]] = None,
             principal_type: Optional[pulumi.Input[str]] = None,
@@ -1514,14 +1551,15 @@
         :param pulumi.Input[str] entity_id: The Entity ID that will be used to uniquely identify this SAML Service Provider.
         :param pulumi.Input[str] first_broker_login_flow_alias: Alias of authentication flow, which is triggered after first login with this identity provider. Term 'First Login' means that there is not yet existing Keycloak account linked with the authenticated identity provider account. Defaults to `first broker login`.
         :param pulumi.Input[bool] force_authn: Indicates whether the identity provider must authenticate the presenter directly rather than rely on a previous security context.
         :param pulumi.Input[str] gui_order: A number defining the order of this identity provider in the GUI.
         :param pulumi.Input[bool] hide_on_login_page: If hidden, then login with this provider is possible only if requested explicitly, e.g. using the 'kc_idp_hint' parameter.
         :param pulumi.Input[str] internal_id: Internal Identity Provider Id
         :param pulumi.Input[bool] link_only: When `true`, users cannot login using this provider, but their existing accounts will be linked when possible. Defaults to `false`.
+        :param pulumi.Input[str] login_hint: Login Hint.
         :param pulumi.Input[str] name_id_policy_format: Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         :param pulumi.Input[bool] post_binding_authn_request: Indicates whether the AuthnRequest must be sent using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_logout: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used.
         :param pulumi.Input[bool] post_binding_response: Indicates whether to respond to requests using HTTP-POST binding. If false, HTTP-REDIRECT binding will be used..
         :param pulumi.Input[str] post_broker_login_flow_alias: Alias of authentication flow, which is triggered after each login with this identity provider. Useful if you want additional verification of each user authenticated with this identity provider (for example OTP). Leave this empty if you don't want any additional authenticators to be triggered after login with this identity provider. Also note, that authenticator implementations must assume that user is already set in ClientSession as identity provider already set it. Defaults to empty.
         :param pulumi.Input[str] principal_attribute: The principal attribute.
         :param pulumi.Input[str] principal_type: The principal type. Can be one of `SUBJECT`, `ATTRIBUTE` or `FRIENDLY_ATTRIBUTE`.
@@ -1556,14 +1594,15 @@
         __props__.__dict__["extra_config"] = extra_config
         __props__.__dict__["first_broker_login_flow_alias"] = first_broker_login_flow_alias
         __props__.__dict__["force_authn"] = force_authn
         __props__.__dict__["gui_order"] = gui_order
         __props__.__dict__["hide_on_login_page"] = hide_on_login_page
         __props__.__dict__["internal_id"] = internal_id
         __props__.__dict__["link_only"] = link_only
+        __props__.__dict__["login_hint"] = login_hint
         __props__.__dict__["name_id_policy_format"] = name_id_policy_format
         __props__.__dict__["post_binding_authn_request"] = post_binding_authn_request
         __props__.__dict__["post_binding_logout"] = post_binding_logout
         __props__.__dict__["post_binding_response"] = post_binding_response
         __props__.__dict__["post_broker_login_flow_alias"] = post_broker_login_flow_alias
         __props__.__dict__["principal_attribute"] = principal_attribute
         __props__.__dict__["principal_type"] = principal_type
@@ -1712,14 +1751,22 @@
     def link_only(self) -> pulumi.Output[Optional[bool]]:
         """
         When `true`, users cannot login using this provider, but their existing accounts will be linked when possible. Defaults to `false`.
         """
         return pulumi.get(self, "link_only")
 
     @property
+    @pulumi.getter(name="loginHint")
+    def login_hint(self) -> pulumi.Output[Optional[str]]:
+        """
+        Login Hint.
+        """
+        return pulumi.get(self, "login_hint")
+
+    @property
     @pulumi.getter(name="nameIdPolicyFormat")
     def name_id_policy_format(self) -> pulumi.Output[Optional[str]]:
         """
         Specifies the URI reference corresponding to a name identifier format. Defaults to empty.
         """
         return pulumi.get(self, "name_id_policy_format")
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/outputs.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/script_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/script_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/user_attribute_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/user_attribute_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/saml/user_property_protocol_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/saml/user_property_protocol_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user_groups.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,19 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  exhaustive: Optional[pulumi.Input[bool]] = None,
                  group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Allows for managing a Keycloak user's groups.
+
+        If `exhaustive` is true, this resource attempts to be an **authoritative** source over user groups: groups that are manually added to the user will be removed, and groups that are manually removed from the user group will be added upon the next run of `pulumi up`.
+        If `exhaustive` is false, this resource is a partial assignation of groups to a user. As a result, you can get multiple `UserGroups` for the same `user_id`.
+
         ## Example Usage
         ### Exhaustive Groups)
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
@@ -220,14 +225,19 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserGroupsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Allows for managing a Keycloak user's groups.
+
+        If `exhaustive` is true, this resource attempts to be an **authoritative** source over user groups: groups that are manually added to the user will be removed, and groups that are manually removed from the user group will be added upon the next run of `pulumi up`.
+        If `exhaustive` is false, this resource is a partial assignation of groups to a user. As a result, you can get multiple `UserGroups` for the same `user_id`.
+
         ## Example Usage
         ### Exhaustive Groups)
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
         realm = keycloak.Realm("realm",
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user_roles.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user_roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,14 +159,23 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  exhaustive: Optional[pulumi.Input[bool]] = None,
                  realm_id: Optional[pulumi.Input[str]] = None,
                  role_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Allows you to manage roles assigned to a Keycloak user.
+
+        If `exhaustive` is true, this resource attempts to be an **authoritative** source over user roles: roles that are manually added to the user will be removed, and roles that are manually removed from the
+        user will be added upon the next run of `pulumi up`.
+        If `exhaustive` is false, this resource is a partial assignation of roles to a user. As a result, you can use multiple `UserRoles` for the same `user_id`.
+
+        Note that when assigning composite roles to a user, you may see a non-empty plan following a `pulumi up` if you assign
+        a role and a composite that includes that role to the same user.
+
         ## Example Usage
         ### Exhaustive Roles)
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
 
@@ -219,14 +228,23 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserRolesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Allows you to manage roles assigned to a Keycloak user.
+
+        If `exhaustive` is true, this resource attempts to be an **authoritative** source over user roles: roles that are manually added to the user will be removed, and roles that are manually removed from the
+        user will be added upon the next run of `pulumi up`.
+        If `exhaustive` is false, this resource is a partial assignation of roles to a user. As a result, you can use multiple `UserRoles` for the same `user_id`.
+
+        Note that when assigning composite roles to a user, you may see a non-empty plan following a `pulumi up` if you assign
+        a role and a composite that includes that role to the same user.
+
         ## Example Usage
         ### Exhaustive Roles)
 
         ```python
         import pulumi
         import pulumi_keycloak as keycloak
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/user_template_importer_identity_provider_mapper.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/user_template_importer_identity_provider_mapper.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak/users_permissions.py` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak/users_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/PKG-INFO` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-keycloak
-Version: 5.2.0a1685166531
+Version: 5.2.0a1686176633
 Summary: A Pulumi package for creating and managing keycloak cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-keycloak
 Keywords: pulumi keycloak
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-keycloak/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-keycloak/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fkeycloak.svg)](https://www.npmjs.com/package/@pulumi/keycloak)
 [![Python version](https://badge.fury.io/py/pulumi-keycloak.svg)](https://pypi.org/project/pulumi-keycloak)
 [![NuGet version](https://badge.fury.io/nu/pulumi.keycloak.svg)](https://badge.fury.io/nu/pulumi.keycloak)
```

### Comparing `pulumi_keycloak-5.2.0a1685166531/pulumi_keycloak.egg-info/SOURCES.txt` & `pulumi_keycloak-5.2.0a1686176633/pulumi_keycloak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_keycloak-5.2.0a1685166531/setup.py` & `pulumi_keycloak-5.2.0a1686176633/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.2.0a1685166531"
-PLUGIN_VERSION = "5.2.0-alpha.1685166531+f2c76df2"
+VERSION = "5.2.0a1686176633"
+PLUGIN_VERSION = "5.2.0-alpha.1686176633+55976244"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'keycloak', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "keycloak Pulumi Package - Development Version"
 
 
 setup(name='pulumi_keycloak',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing keycloak cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

