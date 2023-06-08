# Comparing `tmp/aliyun-python-sdk-oceanbasepro-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-oceanbasepro-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-oceanbasepro-1.0.8.tar", last modified: Fri May 19 06:28:30 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-oceanbasepro-1.0.9.tar", last modified: Thu Jun  8 02:43:22 2023, max compression
```

## Comparing `aliyun-python-sdk-oceanbasepro-1.0.8.tar` & `aliyun-python-sdk-oceanbasepro-1.0.9.tar`

### file list

```diff
@@ -1,93 +1,105 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1582 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1582 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5720 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/
--rw-r--r--   0 root         (0) root         (0)     2618 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3388 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     3486 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1880 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2384 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py
--rw-r--r--   0 root         (0) root         (0)     4110 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2968 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py
--rw-r--r--   0 root         (0) root         (0)     2410 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     4108 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/KillProcessListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 06:28:30.000000 aliyun-python-sdk-oceanbasepro-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2497 2023-05-19 06:28:29.000000 aliyun-python-sdk-oceanbasepro-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6612 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3388 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4302 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOasAnomalySQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOasSQLDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOasSQLHistoryListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOasSQLPlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3954 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOasSlowSQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOasTopSQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLSamplesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityIpGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/KillProcessListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantSecurityIpGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/SwitchoverInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-06-08 02:43:22.000000 aliyun-python-sdk-oceanbasepro-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/LICENSE` & `aliyun-python-sdk-oceanbasepro-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/PKG-INFO` & `aliyun-python-sdk-oceanbasepro-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-oceanbasepro
-Version: 1.0.8
+Version: 1.0.9
 Summary: The oceanbasepro module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-oceanbasepro
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/README.rst` & `aliyun-python-sdk-oceanbasepro-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-oceanbasepro
-Version: 1.0.8
+Version: 1.0.9
 Summary: The oceanbasepro module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-oceanbasepro
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyun_python_sdk_oceanbasepro.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py
+aliyunsdkoceanbasepro/request/v20190901/CreateTenantSecurityIpGroupRequest.py
 aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DeleteTenantSecurityIpGroupRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py
@@ -34,29 +36,37 @@
 aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeOasAnomalySQLListRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeOasSQLDetailsRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeOasSQLHistoryListRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeOasSQLPlansRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeOasSlowSQLListRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeOasTopSQLListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeSQLSamplesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py
+aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityIpGroupsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py
@@ -68,20 +78,22 @@
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py
+aliyunsdkoceanbasepro/request/v20190901/ModifyTenantSecurityIpGroupRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py
 aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py
 aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py
 aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py
+aliyunsdkoceanbasepro/request/v20190901/SwitchoverInstanceRequest.py
 aliyunsdkoceanbasepro/request/v20190901/__init__.py
```

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/endpoint.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateDatabaseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateOmsMysqlDataSourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateSecurityIpGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantReadOnlyConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/CreateTenantUserRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteDatabasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteSecurityIpGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DeleteTenantsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeAnomalySQLListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableCpuResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeAvailableMemResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeCharsetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeDatabasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceCreatableZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceSecurityConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTenantModesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstanceTopologyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeNodeMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOmsOpenAPIProjectStepsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeOutlineBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeRecommendIndexRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLDetailsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLHistoryListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSQLPlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSecurityIpGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLHistoryListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeSlowSQLListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantSecurityConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUserRolesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantUsersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantZonesReadRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTenantsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTimeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeTopSQLListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/KillProcessListRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/KillProcessListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyDatabaseUserRolesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceNodeNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceSpecRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyInstanceTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifySecurityIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantPrimaryZoneRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantResourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserRolesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ModifyTenantUserStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ReleaseOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ResetOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/ResumeOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIMonitorMetricRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/SearchOmsOpenAPIProjectsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/StartOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/aliyunsdkoceanbasepro/request/v20190901/StopOmsOpenAPIProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-oceanbasepro-1.0.8/setup.py` & `aliyun-python-sdk-oceanbasepro-1.0.9/setup.py`

 * *Files identical despite different names*

