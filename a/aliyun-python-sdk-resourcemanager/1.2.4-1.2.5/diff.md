# Comparing `tmp/aliyun-python-sdk-resourcemanager-1.2.4.tar.gz` & `tmp/aliyun-python-sdk-resourcemanager-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-resourcemanager-1.2.4.tar", last modified: Wed Feb 22 02:17:05 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-resourcemanager-1.2.5.tar", last modified: Thu Jun  8 10:02:37 2023, max compression
```

## Comparing `aliyun-python-sdk-resourcemanager-1.2.4.tar` & `aliyun-python-sdk-resourcemanager-1.2.5.tar`

### file list

```diff
@@ -1,112 +1,111 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1597 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1597 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7279 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/
--rw-r--r--   0 root         (0) root         (0)     1522 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2340 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2340 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupListAclModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2722 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py
--rw-r--r--   0 root         (0) root         (0)     2286 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3327 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2650 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2555 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1932 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2260 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1769 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-02-22 02:17:05.000000 aliyun-python-sdk-resourcemanager-1.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2512 2023-02-22 02:17:04.000000 aliyun-python-sdk-resourcemanager-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-08 10:02:37.000000 aliyun-python-sdk-resourcemanager-1.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-06-08 10:02:36.000000 aliyun-python-sdk-resourcemanager-1.2.5/setup.py
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/LICENSE` & `aliyun-python-sdk-resourcemanager-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/PKG-INFO` & `aliyun-python-sdk-resourcemanager-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-resourcemanager
-Version: 1.2.4
+Version: 1.2.5
 Summary: The resourcemanager module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-resourcemanager
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/README.rst` & `aliyun-python-sdk-resourcemanager-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-resourcemanager
-Version: 1.2.4
+Version: 1.2.5
 Summary: The resourcemanager module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-resourcemanager
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyun_python_sdk_resourcemanager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py
-aliyunsdkresourcemanager/request/v20200331/GetResourceGroupListAclModeRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py
 aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py
 aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py
 aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py
 aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py
 aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/AcceptHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class AcceptHandshakeRequest(RpcRequest):
+class GetHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AcceptHandshake')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetHandshake','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachControlPolicyRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class AttachControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/AttachPolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class AttachPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'AttachPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/BindSecureMobilePhoneRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class BindSecureMobilePhoneRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'BindSecureMobilePhone')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'BindSecureMobilePhone','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class CancelChangeAccountEmailRequest(RpcRequest):
+class GetAccountDeletionStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelChangeAccountEmail')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionStatus','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelCreateCloudAccountRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CancelCreateCloudAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelCreateCloudAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelCreateCloudAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelHandshakeRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CancelHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelHandshake')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelHandshake','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelPromoteResourceAccountRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CancelPromoteResourceAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelPromoteResourceAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelPromoteResourceAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ChangeAccountEmailRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ChangeAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ChangeAccountEmail')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ChangeAccountEmail','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CheckAccountDeleteRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CheckAccountDeleteRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CheckAccountDelete')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CheckAccountDelete','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateCloudAccountRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateCloudAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateCloudAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateCloudAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateControlPolicyRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateFolderRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateFolder')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateFolder','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreatePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreatePolicyVersionRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreatePolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicyVersion')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreatePolicyVersion','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceAccountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateResourceAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateResourceGroupRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceGroup')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateResourceGroup','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateRoleRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateRole')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateRole','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CreateServiceLinkedRoleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class CreateServiceLinkedRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateServiceLinkedRole')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CreateServiceLinkedRole','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeclineHandshakeRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeclineHandshakeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeclineHandshake')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeclineHandshake','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteAccountRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 import json
 
 class DeleteAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteControlPolicyRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class DeleteFolderRequest(RpcRequest):
+class GetFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteFolder')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetFolder','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeletePolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeletePolicyVersionRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeletePolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicyVersion')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeletePolicyVersion','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteResourceGroupRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteResourceGroup')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteResourceGroup','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteRoleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteRole')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteRole','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteServiceLinkedRoleRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeleteServiceLinkedRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteServiceLinkedRole')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteServiceLinkedRole','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeregisterDelegatedAdministratorRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DeregisterDelegatedAdministratorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeregisterDelegatedAdministrator')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeregisterDelegatedAdministrator','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DestroyResourceDirectoryRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DestroyResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DestroyResourceDirectory')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DestroyResourceDirectory','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachControlPolicyRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DetachControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DetachPolicyRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DetachPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DetachPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DisableControlPolicyRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class DisableControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DisableControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DisableControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableControlPolicyRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class EnableControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/EnableResourceDirectoryRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class EnableResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableResourceDirectory')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'EnableResourceDirectory','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionCheckResultRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetAccountDeletionCheckResultRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionCheckResult')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionCheckResult','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetAccountDeletionStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetAccountDeletionStatusRequest(RpcRequest):
+class GetPayerForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccountDeletionStatus')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPayerForAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetAccountRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyEnablementStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetControlPolicyEnablementStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicyEnablementStatus')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicyEnablementStatus','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetControlPolicyRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetFolderRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/DeleteFolderRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetFolderRequest(RpcRequest):
+class DeleteFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetFolder')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'DeleteFolder','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetHandshakeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetHandshakeRequest(RpcRequest):
+class SetMemberDeletionPermissionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetHandshake')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetMemberDeletionPermission','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_HandshakeId(self): # String
-		return self.get_query_params().get('HandshakeId')
+	def get_Status(self): # String
+		return self.get_query_params().get('Status')
 
-	def set_HandshakeId(self, HandshakeId):  # String
-		self.add_query_param('HandshakeId', HandshakeId)
+	def set_Status(self, Status):  # String
+		self.add_query_param('Status', Status)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetPayerForAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/CancelChangeAccountEmailRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetPayerForAccountRequest(RpcRequest):
+class CancelChangeAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPayerForAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'CancelChangeAccountEmail','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,31 +16,26 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetPolicyVersionRequest(RpcRequest):
+class SetDefaultPolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicyVersion')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetDefaultPolicyVersion','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_PolicyType(self): # String
-		return self.get_query_params().get('PolicyType')
-
-	def set_PolicyType(self, PolicyType):  # String
-		self.add_query_param('PolicyType', PolicyType)
 	def get_VersionId(self): # String
 		return self.get_query_params().get('VersionId')
 
 	def set_VersionId(self, VersionId):  # String
 		self.add_query_param('VersionId', VersionId)
 	def get_PolicyName(self): # String
 		return self.get_query_params().get('PolicyName')
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceDirectoryRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceDirectory')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceDirectory','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupListAclModeRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class GetResourceGroupListAclModeRequest(RpcRequest):
+class InitResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceGroupListAclMode')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InitResourceDirectory','resourcemanager')
+		self.set_protocol_type('https')
+		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetResourceGroupRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceGroup')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetResourceGroup','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetRoleRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetRole')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetRole','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetServiceLinkedRoleDeletionStatusRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class GetServiceLinkedRoleDeletionStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetServiceLinkedRoleDeletionStatus')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetServiceLinkedRoleDeletionStatus','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/InitResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,19 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class InitResourceDirectoryRequest(RpcRequest):
+class ResendCreateCloudAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InitResourceDirectory')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendCreateCloudAccountEmail','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_RecordId(self): # String
+		return self.get_query_params().get('RecordId')
+
+	def set_RecordId(self, RecordId):  # String
+		self.add_query_param('RecordId', RecordId)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/InviteAccountToResourceDirectoryRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class InviteAccountToResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InviteAccountToResourceDirectory')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'InviteAccountToResourceDirectory','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsForParentRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListAccountsForParentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccountsForParent')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccountsForParent','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAccountsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListAccountsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccounts')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAccounts','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListAncestorsRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListAncestorsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAncestors')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListAncestors','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListControlPoliciesRequest(RpcRequest):
+class ListPoliciesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicies')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicies','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPolicyAttachmentsForTargetRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListControlPolicyAttachmentsForTargetRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicyAttachmentsForTarget')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicyAttachmentsForTarget','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedAdministratorsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListDelegatedAdministratorsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedAdministrators')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedAdministrators','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListDelegatedServicesForAccountRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListDelegatedServicesForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedServicesForAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListDelegatedServicesForAccount','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListFoldersForParentRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListFoldersForParentRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListFoldersForParent')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListFoldersForParent','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForAccountRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListHandshakesForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListHandshakesForResourceDirectoryRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListHandshakesForResourceDirectoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForResourceDirectory')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListHandshakesForResourceDirectory','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListPoliciesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListControlPoliciesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListPoliciesRequest(RpcRequest):
+class ListControlPoliciesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicies')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListControlPolicies','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyAttachmentsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListPolicyAttachmentsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyAttachments')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyAttachments','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/GetPolicyVersionRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ListPolicyVersionsRequest(RpcRequest):
+class GetPolicyVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyVersions')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'GetPolicyVersion','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_PolicyType(self): # String
 		return self.get_query_params().get('PolicyType')
 
 	def set_PolicyType(self, PolicyType):  # String
 		self.add_query_param('PolicyType', PolicyType)
+	def get_VersionId(self): # String
+		return self.get_query_params().get('VersionId')
+
+	def set_VersionId(self, VersionId):  # String
+		self.add_query_param('VersionId', VersionId)
 	def get_PolicyName(self): # String
 		return self.get_query_params().get('PolicyName')
 
 	def set_PolicyName(self, PolicyName):  # String
 		self.add_query_param('PolicyName', PolicyName)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourceGroupsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListResourceGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResourceGroups')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResourceGroups','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListResourcesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResources')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListResources','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListRolesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListRolesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListRoles')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListRoles','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagKeysRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTagKeysRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagKeys')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagKeys','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagResourcesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagResources')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagResources','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTagValuesRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTagValuesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagValues')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTagValues','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTargetAttachmentsForControlPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTargetAttachmentsForControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTargetAttachmentsForControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTargetAttachmentsForControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListTrustedServiceStatusRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class ListTrustedServiceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTrustedServiceStatus')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListTrustedServiceStatus','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveAccountRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class MoveAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/MoveResourcesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class MoveResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveResources')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'MoveResources','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/PromoteResourceAccountRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class PromoteResourceAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'PromoteResourceAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'PromoteResourceAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RegisterDelegatedAdministratorRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class RegisterDelegatedAdministratorRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RegisterDelegatedAdministrator')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RegisterDelegatedAdministrator','resourcemanager')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RemoveCloudAccountRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class RemoveCloudAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RemoveCloudAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RemoveCloudAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ResendCreateCloudAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ResendCreateCloudAccountEmailRequest(RpcRequest):
+class ResendPromoteResourceAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendCreateCloudAccountEmail')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendPromoteResourceAccountEmail','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/ResendPromoteResourceAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class ResendPromoteResourceAccountEmailRequest(RpcRequest):
+class RetryChangeAccountEmailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ResendPromoteResourceAccountEmail')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RetryChangeAccountEmail','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_RecordId(self): # String
-		return self.get_query_params().get('RecordId')
+	def get_AccountId(self): # String
+		return self.get_query_params().get('AccountId')
 
-	def set_RecordId(self, RecordId):  # String
-		self.add_query_param('RecordId', RecordId)
+	def set_AccountId(self, AccountId):  # String
+		self.add_query_param('AccountId', AccountId)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/RetryChangeAccountEmailRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,24 +16,34 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class RetryChangeAccountEmailRequest(RpcRequest):
+class UpdateAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'RetryChangeAccountEmail')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateAccount','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_NewDisplayName(self): # String
+		return self.get_query_params().get('NewDisplayName')
+
+	def set_NewDisplayName(self, NewDisplayName):  # String
+		self.add_query_param('NewDisplayName', NewDisplayName)
+	def get_NewAccountType(self): # String
+		return self.get_query_params().get('NewAccountType')
+
+	def set_NewAccountType(self, NewAccountType):  # String
+		self.add_query_param('NewAccountType', NewAccountType)
 	def get_AccountId(self): # String
 		return self.get_query_params().get('AccountId')
 
 	def set_AccountId(self, AccountId):  # String
 		self.add_query_param('AccountId', AccountId)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForBindSecureMobilePhoneRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class SendVerificationCodeForBindSecureMobilePhoneRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForBindSecureMobilePhone')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForBindSecureMobilePhone','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/SendVerificationCodeForEnableRDRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class SendVerificationCodeForEnableRDRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForEnableRD')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SendVerificationCodeForEnableRD','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SetDefaultPolicyVersionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/ListPolicyVersionsRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class SetDefaultPolicyVersionRequest(RpcRequest):
+class ListPolicyVersionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetDefaultPolicyVersion')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'ListPolicyVersions','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_VersionId(self): # String
-		return self.get_query_params().get('VersionId')
+	def get_PolicyType(self): # String
+		return self.get_query_params().get('PolicyType')
 
-	def set_VersionId(self, VersionId):  # String
-		self.add_query_param('VersionId', VersionId)
+	def set_PolicyType(self, PolicyType):  # String
+		self.add_query_param('PolicyType', PolicyType)
 	def get_PolicyName(self): # String
 		return self.get_query_params().get('PolicyName')
 
 	def set_PolicyName(self, PolicyName):  # String
 		self.add_query_param('PolicyName', PolicyName)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/SetMemberDeletionPermissionRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateFolderRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class SetMemberDeletionPermissionRequest(RpcRequest):
+class UpdateFolderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'SetMemberDeletionPermission')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateFolder','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Status(self): # String
-		return self.get_query_params().get('Status')
+	def get_FolderId(self): # String
+		return self.get_query_params().get('FolderId')
 
-	def set_Status(self, Status):  # String
-		self.add_query_param('Status', Status)
+	def set_FolderId(self, FolderId):  # String
+		self.add_query_param('FolderId', FolderId)
+	def get_NewFolderName(self): # String
+		return self.get_query_params().get('NewFolderName')
+
+	def set_NewFolderName(self, NewFolderName):  # String
+		self.add_query_param('NewFolderName', NewFolderName)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/TagResourcesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'TagResources')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'TagResources','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UntagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UntagResources')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UntagResources','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateAccountRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,34 +16,29 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class UpdateAccountRequest(RpcRequest):
+class UpdateResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateAccount')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateResourceGroup','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_NewDisplayName(self): # String
 		return self.get_query_params().get('NewDisplayName')
 
 	def set_NewDisplayName(self, NewDisplayName):  # String
 		self.add_query_param('NewDisplayName', NewDisplayName)
-	def get_NewAccountType(self): # String
-		return self.get_query_params().get('NewAccountType')
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
 
-	def set_NewAccountType(self, NewAccountType):  # String
-		self.add_query_param('NewAccountType', NewAccountType)
-	def get_AccountId(self): # String
-		return self.get_query_params().get('AccountId')
-
-	def set_AccountId(self, AccountId):  # String
-		self.add_query_param('AccountId', AccountId)
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateControlPolicyRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
 class UpdateControlPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateControlPolicy')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateControlPolicy','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/aliyunsdkresourcemanager/request/v20200331/UpdateResourceGroupRequest.py` & `aliyun-python-sdk-resourcemanager-1.2.5/aliyunsdkresourcemanager/request/v20200331/UpdateRoleRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,29 +16,39 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkresourcemanager.endpoint import endpoint_data
 
-class UpdateResourceGroupRequest(RpcRequest):
+class UpdateRoleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateResourceGroup')
+		RpcRequest.__init__(self, 'ResourceManager', '2020-03-31', 'UpdateRole','resourcemanager')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_NewDisplayName(self): # String
-		return self.get_query_params().get('NewDisplayName')
+	def get_NewAssumeRolePolicyDocument(self): # String
+		return self.get_query_params().get('NewAssumeRolePolicyDocument')
 
-	def set_NewDisplayName(self, NewDisplayName):  # String
-		self.add_query_param('NewDisplayName', NewDisplayName)
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
+	def set_NewAssumeRolePolicyDocument(self, NewAssumeRolePolicyDocument):  # String
+		self.add_query_param('NewAssumeRolePolicyDocument', NewAssumeRolePolicyDocument)
+	def get_RoleName(self): # String
+		return self.get_query_params().get('RoleName')
 
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def set_RoleName(self, RoleName):  # String
+		self.add_query_param('RoleName', RoleName)
+	def get_NewMaxSessionDuration(self): # Long
+		return self.get_query_params().get('NewMaxSessionDuration')
+
+	def set_NewMaxSessionDuration(self, NewMaxSessionDuration):  # Long
+		self.add_query_param('NewMaxSessionDuration', NewMaxSessionDuration)
+	def get_NewDescription(self): # String
+		return self.get_query_params().get('NewDescription')
+
+	def set_NewDescription(self, NewDescription):  # String
+		self.add_query_param('NewDescription', NewDescription)
```

### Comparing `aliyun-python-sdk-resourcemanager-1.2.4/setup.py` & `aliyun-python-sdk-resourcemanager-1.2.5/setup.py`

 * *Files identical despite different names*

