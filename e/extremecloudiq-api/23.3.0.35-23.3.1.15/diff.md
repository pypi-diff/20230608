# Comparing `tmp/extremecloudiq-api-23.3.0.35.tar.gz` & `tmp/extremecloudiq-api-23.3.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmpfsmo7khp/extremecloudiq-api-23.3.0.35.tar", last modified: Tue May 23 15:38:14 2023, max compression
+gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmpmwfnz94c/extremecloudiq-api-23.3.1.15.tar", last modified: Thu Jun  8 17:56:21 2023, max compression
```

## Comparing `extremecloudiq-api-23.3.0.35.tar` & `extremecloudiq-api-23.3.1.15.tar`

### file list

```diff
@@ -1,802 +1,806 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32863 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/account_api.py
--rw-r--r--   0 root         (0) root         (0)    16607 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/alert_api.py
--rw-r--r--   0 root         (0) root         (0)    24696 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/application_api.py
--rw-r--r--   0 root         (0) root         (0)    11075 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    26155 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/authorization_api.py
--rw-r--r--   0 root         (0) root         (0)    47344 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/client_api.py
--rw-r--r--   0 root         (0) root         (0)   171865 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    34020 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)     7036 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)    16188 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)   292853 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)   133458 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)    56032 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)    96669 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)   261168 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/device_api.py
--rw-r--r--   0 root         (0) root         (0)    56015 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/hiq_api.py
--rw-r--r--   0 root         (0) root         (0)    67518 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/location_api.py
--rw-r--r--   0 root         (0) root         (0)    45962 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/log_api.py
--rw-r--r--   0 root         (0) root         (0)    49087 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)    15845 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/notification_api.py
--rw-r--r--   0 root         (0) root         (0)    16819 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/operation_api.py
--rw-r--r--   0 root         (0) root         (0)    59448 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/
--rw-r--r--   0 root         (0) root         (0)    31266 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3762 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/inline_object.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     7549 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     7198 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     7171 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     7414 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     7684 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     7495 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     7198 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     7171 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     7522 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7252 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     7333 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     7468 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     7387 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     7225 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     7414 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)    14244 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)    30789 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)    21694 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)    10200 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     2914 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     2885 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
--rw-r--r--   0 root         (0) root         (0)    11942 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     4638 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)    12035 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)    11007 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)    11341 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     2983 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     7297 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     4918 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     5034 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assurance_scans_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     6191 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     4744 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_device_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     8778 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_packet_counts_entity.py
--rw-r--r--   0 root         (0) root         (0)     4777 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_packet_counts_response.py
--rw-r--r--   0 root         (0) root         (0)     9992 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_audit_log_sort_field.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     5200 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_data.py
--rw-r--r--   0 root         (0) root         (0)     4360 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_request.py
--rw-r--r--   0 root         (0) root         (0)     3453 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_response.py
--rw-r--r--   0 root         (0) root         (0)     8803 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     9740 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)    10481 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     5521 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     4513 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)    10385 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     9147 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     5160 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     3850 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)    36439 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     3460 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     2981 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)    13090 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3007 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     8602 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)    10453 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     8904 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     5501 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6858 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5895 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)    13025 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    11803 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)    11600 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    32293 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    19021 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4577 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4470 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)    18200 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    15074 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     5736 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    13170 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     7343 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    15880 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     7692 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5113 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7193 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     6441 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     6707 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     7369 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     6913 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     4443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     3465 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     8692 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    29777 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     8199 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     5363 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     4314 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     3237 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)    11915 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_installation_report.py
--rw-r--r--   0 root         (0) root         (0)     5440 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     4958 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_lldp_cdp_info.py
--rw-r--r--   0 root         (0) root         (0)    14407 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     6912 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_null_field.py
--rw-r--r--   0 root         (0) root         (0)     2839 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     5419 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)    29253 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_wifi_interface.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
--rw-r--r--   0 root         (0) root         (0)     4607 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     5838 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     6152 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_device.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_devices.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_make.py
--rw-r--r--   0 root         (0) root         (0)     4453 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_model.py
--rw-r--r--   0 root         (0) root         (0)     6350 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     5412 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_duplex_data_rate_entity.py
--rw-r--r--   0 root         (0) root         (0)     8666 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)    13081 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)    19289 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     5520 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     2919 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     8373 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     3012 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     9136 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)    13976 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     8960 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)    15643 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     5508 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     6363 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)    15300 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     9830 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     6609 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5022 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4704 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     9688 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)    34397 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     3181 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)    10731 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     9191 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     7344 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     2855 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)    18840 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)    11043 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     4526 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     5819 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     2854 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     9805 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     3378 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     5598 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)    12064 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     8615 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)    10248 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     3938 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     6202 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)    10513 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     9629 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     9871 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     5442 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4002 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_port_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     7190 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)    24027 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     6104 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    17441 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     6149 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     3059 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)    13997 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     6301 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2924 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)    31140 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)    11299 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     8920 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)    12894 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)    50568 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     8501 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     4445 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     3773 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     9306 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)    13069 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)    10197 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)    14921 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)    11003 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)    10607 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_speed_duplex_entity.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     3387 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     2881 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     6385 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     5031 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6860 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5263 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     6261 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)    10733 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10502 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     5313 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10459 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    29855 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    16312 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4264 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)    18046 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6338 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    13979 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6535 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    11163 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)    31687 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     7034 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5657 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    10884 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)    58066 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     5908 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    11172 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    15880 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6941 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5113 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7193 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    14730 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user.py
--rw-r--r--   0 root         (0) root         (0)    19134 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7058 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     7244 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     5800 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     6384 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     7742 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     5243 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     7921 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)    13204 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)    10999 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)    11215 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     3683 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     8403 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     7174 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     7145 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     4028 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     8514 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     5775 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)    13566 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    33207 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26261 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/api_client.py
--rw-r--r--   0 root         (0) root         (0)    12886 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3802 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12334 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/extremecloudiq/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35650 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/test/
--rw-r--r--   0 root         (0) root         (0)     1913 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_account_api.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_alert_api.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_application_api.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_authorization_api.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_client_api.py
--rw-r--r--   0 root         (0) root         (0)     6222 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     9451 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)     4802 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)     8486 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_device_api.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_hiq_api.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_inline_object.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_location_api.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_log_api.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)     1226 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_notification_api.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_operation_api.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     3020 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     4078 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     2063 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     3938 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-05-03 18:58:15.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2321 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     6282 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4819 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     4285 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomalies_count_vo_entity.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)     2372 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_assurance_scans_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_atp_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_atp_device_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_atp_packet_counts_entity.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_atp_packet_counts_response.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_audit_log_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_data.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_request.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_response.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)     2243 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_client_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)     2349 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2609 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2100 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     5097 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2003 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     2081 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     3187 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     3430 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_installation_report.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_lldp_cdp_info.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_null_field.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_device_wifi_interface.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_channel_changes_entity.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_channel_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_recurence_channel_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_recurence_count_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_device.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_devices.py
--rw-r--r--   0 root         (0) root         (0)     1443 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_make.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_model.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_duplex_data_rate_entity.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2315 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-05-03 18:58:16.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     5133 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     5513 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)     2745 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)     3475 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)     2382 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3239 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1870 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_port_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)     4358 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)     2214 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)     2187 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1375 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_speed_duplex_entity.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1467 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     1531 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2036 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2376 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     3387 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2078 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)     3372 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     9060 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     1790 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     1796 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     1546 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     3276 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)     3941 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     1538 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2044 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     1641 2023-05-03 18:58:17.000000 extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    67875 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1125 2023-05-03 18:58:19.000000 extremecloudiq-api-23.3.0.35/setup.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-23 15:38:14.000000 extremecloudiq-api-23.3.0.35/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32863 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/account_api.py
+-rw-r--r--   0 root         (0) root         (0)    16607 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/alert_api.py
+-rw-r--r--   0 root         (0) root         (0)    24696 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/application_api.py
+-rw-r--r--   0 root         (0) root         (0)    11075 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    26155 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)    47344 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/client_api.py
+-rw-r--r--   0 root         (0) root         (0)   171865 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    34020 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)     7036 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)    16188 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)   292853 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)   133458 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    56032 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)    96669 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)   261168 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/device_api.py
+-rw-r--r--   0 root         (0) root         (0)    56015 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)    67518 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/location_api.py
+-rw-r--r--   0 root         (0) root         (0)    45962 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/log_api.py
+-rw-r--r--   0 root         (0) root         (0)    49087 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/notification_api.py
+-rw-r--r--   0 root         (0) root         (0)    16819 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/operation_api.py
+-rw-r--r--   0 root         (0) root         (0)    59448 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/
+-rw-r--r--   0 root         (0) root         (0)    31442 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     7549 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     7414 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     7684 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     7495 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7252 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     7225 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7414 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)    14244 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)    30789 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)    21694 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10200 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)    11942 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)    12035 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)    11007 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)    11341 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     7297 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     4918 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     5034 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     8778 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_response.py
+-rw-r--r--   0 root         (0) root         (0)     9992 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     8803 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     9740 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)    10481 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     9147 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     5160 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)    36439 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     5122 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)    13090 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)    10453 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6858 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5895 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)    13025 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    11803 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    32293 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    19021 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4577 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4470 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)    18200 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    15074 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    13170 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     7343 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    15880 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     7692 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7193 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     6441 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     6707 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     6913 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     8692 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)    29777 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     8199 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)    11915 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)    14407 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_null_field.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     5419 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)    29253 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_device.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_devices.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_feat_license.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_make.py
+-rw-r--r--   0 root         (0) root         (0)     4453 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_model.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_vim_module.py
+-rw-r--r--   0 root         (0) root         (0)     5412 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     8666 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)    13081 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)    19289 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     8960 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     8373 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     9136 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)    13976 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)    15643 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6363 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)    15300 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     9830 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4704 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     9688 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)    34397 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)    10731 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     9191 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)    18840 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)    11043 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     9805 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)    12064 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     8615 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)    10248 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     6202 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)    10513 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     9629 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     9871 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     5442 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     7190 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)    24027 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     6104 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    17441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     6149 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)    13997 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     6301 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)    31140 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)    11299 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     8920 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    50568 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     8501 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     9306 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)    13069 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)    10197 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)    14921 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)    11003 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)    10607 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     6385 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)    10733 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10502 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     5313 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    29855 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    16312 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4264 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6338 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    13979 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6535 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    11163 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)    31687 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     7034 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5657 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)    58066 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    11172 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    15880 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6941 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7193 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    14730 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)    19134 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7058 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6384 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     7921 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)    13204 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)    11215 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3683 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     8403 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     7174 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     7145 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5775 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    33383 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26261 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    12886 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12334 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/extremecloudiq/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35842 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/test/
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_account_api.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_alert_api.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_application_api.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_client_api.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     9451 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)     8486 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_device_api.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_location_api.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_log_api.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_notification_api.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_operation_api.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4078 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     6282 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4285 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-06-06 21:24:44.000000 extremecloudiq-api-23.3.1.15/test/test_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_response.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-06-06 21:24:41.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_null_field.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_device.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_feat_license.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_make.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_model.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_vim_module.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     5133 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)     3475 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     4358 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-06 21:24:42.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     9060 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3941 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-06-06 21:24:43.000000 extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    68003 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/README.md
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-06 21:24:45.000000 extremecloudiq-api-23.3.1.15/setup.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-08 17:56:21.000000 extremecloudiq-api-23.3.1.15/PKG-INFO
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/__init__.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/__init__.py`

 * *Files identical despite different names*

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/account_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/alert_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/alert_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/application_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/application_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/authentication_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/authorization_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/authorization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/client_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/client_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___authentication_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___basic_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___basic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___certificate_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___certificate_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___deployment_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___deployment_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___policy_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/configuration___user_management_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/configuration___user_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/copilot___anomalies_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___anomalies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/copilot___connectivity_experience_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/device_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/device_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/hiq_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/hiq_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/location_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/location_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/log_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/log_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/network_policy_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/network_policy_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/notification_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/operation_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/operation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api/user_api.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/__init__.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -183,17 +183,19 @@
 from extremecloudiq.models.xiq_device_wifi_interface import XiqDeviceWifiInterface
 from extremecloudiq.models.xiq_dfs_channel_changes_entity import XiqDfsChannelChangesEntity
 from extremecloudiq.models.xiq_dfs_channel_stats_entity import XiqDfsChannelStatsEntity
 from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
 from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
 from extremecloudiq.models.xiq_digital_twin_device import XiqDigitalTwinDevice
 from extremecloudiq.models.xiq_digital_twin_devices import XiqDigitalTwinDevices
+from extremecloudiq.models.xiq_digital_twin_feat_license import XiqDigitalTwinFeatLicense
 from extremecloudiq.models.xiq_digital_twin_make import XiqDigitalTwinMake
 from extremecloudiq.models.xiq_digital_twin_model import XiqDigitalTwinModel
 from extremecloudiq.models.xiq_digital_twin_products import XiqDigitalTwinProducts
+from extremecloudiq.models.xiq_digital_twin_vim_module import XiqDigitalTwinVimModule
 from extremecloudiq.models.xiq_duplex_data_rate_entity import XiqDuplexDataRateEntity
 from extremecloudiq.models.xiq_email_log import XiqEmailLog
 from extremecloudiq.models.xiq_email_template import XiqEmailTemplate
 from extremecloudiq.models.xiq_end_user import XiqEndUser
 from extremecloudiq.models.xiq_entitlement_type import XiqEntitlementType
 from extremecloudiq.models.xiq_error import XiqError
 from extremecloudiq.models.xiq_exos_devices import XiqExosDevices
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/inline_object.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_accounting_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_accounting_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_alert.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_application.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_audit_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_auth_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_certificate.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_classification_rule.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_client.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cloud_config_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_connectivity_experience_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_copilot_wireless_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_credential_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_cwp.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_device.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_device_alarm.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_digital_twin_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_email_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_end_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_external_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_external_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_ldap_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_network_policy.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_radio_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_client_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_sms_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_sms_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_ssid.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_user_group.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_user_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/paged_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_account.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_account_mode.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_account_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_account_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_accounting_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_active_directory_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_category.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_group_query.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_group_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_severity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_severity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_source.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_alert_source_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_alert_source_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomalies_count_vo_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomalies_count_vo_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_device_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_location_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_severity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_severity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_anomaly_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_anomaly_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_api_token_info.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_api_token_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_detection_protocol.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_detection_rule.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_detection_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_detection_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_application_top_clients_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_country_code_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assign_devices_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_assurance_scans_overview_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_assurance_scans_overview_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_device_stats_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_device_stats_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_device_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_packet_counts_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_atp_packet_counts_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_atp_packet_counts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_audit_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_audit_log_category.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_audit_log_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_audit_log_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_auth_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_data.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_operation_result.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_operation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_bounce_device_port_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_bounce_device_port_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_building.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_certificate.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_certificate_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_certificate_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_ibeacon_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_change_devices_os_mode_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_check_permission_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_check_permission_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_check_permission_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_classification.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_classification_rule.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_classification_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_classification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cli_output.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cli_response_code.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cli_response_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_sort_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_summary.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_usage.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_client_view.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_client_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cloud_config_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_connectivity_experience_view_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wired_events_score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_country_code.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_country_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_building_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_classification_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_end_user_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_floor_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_location_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_organization_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_client.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_user_group_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_user_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_user_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_create_webhook_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_credential_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_cwp.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_cwp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_data_point.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_date_time_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_date_time_unit_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_date_time_unit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_default_device_password.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_default_device_password.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_delivery_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_delivery_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dell_devices.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dell_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_overview.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_policy.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_deployment_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_deployment_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_admin_state.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_admin_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_alarm.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_cpu_memory_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_filter.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_function.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_ibeacon.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_ibeacon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_installation_report.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_installation_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_level_ssid.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_lldp_cdp_info.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_lldp_cdp_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_location.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_location_assignment.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_location_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_null_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_null_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_stats.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_view.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_device_wifi_interface.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_device_wifi_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_channel_changes_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_changes_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_channel_stats_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_channel_stats_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_device.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_products.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,167 +1,171 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqDigitalTwinDevice(object):
+class XiqDigitalTwinProducts(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'make': 'XiqDigitalTwinMake',
-        'model': 'XiqDigitalTwinModel',
+        'make': 'str',
+        'model': 'str',
         'os_type': 'str',
-        'os_version': 'str'
+        'os_versions': 'list[str]'
     }
 
     attribute_map = {
         'make': 'make',
         'model': 'model',
         'os_type': 'os_type',
-        'os_version': 'os_version'
+        'os_versions': 'os_versions'
     }
 
-    def __init__(self, make=None, model=None, os_type=None, os_version=None, local_vars_configuration=None):  # noqa: E501
-        """XiqDigitalTwinDevice - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, make=None, model=None, os_type=None, os_versions=None, local_vars_configuration=None):  # noqa: E501
+        """XiqDigitalTwinProducts - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._make = None
         self._model = None
         self._os_type = None
-        self._os_version = None
+        self._os_versions = None
         self.discriminator = None
 
         self.make = make
         self.model = model
         if os_type is not None:
             self.os_type = os_type
-        self.os_version = os_version
+        self.os_versions = os_versions
 
     @property
     def make(self):
-        """Gets the make of this XiqDigitalTwinDevice.  # noqa: E501
+        """Gets the make of this XiqDigitalTwinProducts.  # noqa: E501
 
+        The Digital Twin device make.  # noqa: E501
 
-        :return: The make of this XiqDigitalTwinDevice.  # noqa: E501
-        :rtype: XiqDigitalTwinMake
+        :return: The make of this XiqDigitalTwinProducts.  # noqa: E501
+        :rtype: str
         """
         return self._make
 
     @make.setter
     def make(self, make):
-        """Sets the make of this XiqDigitalTwinDevice.
+        """Sets the make of this XiqDigitalTwinProducts.
 
+        The Digital Twin device make.  # noqa: E501
 
-        :param make: The make of this XiqDigitalTwinDevice.  # noqa: E501
-        :type: XiqDigitalTwinMake
+        :param make: The make of this XiqDigitalTwinProducts.  # noqa: E501
+        :type: str
         """
         if self.local_vars_configuration.client_side_validation and make is None:  # noqa: E501
             raise ValueError("Invalid value for `make`, must not be `None`")  # noqa: E501
 
         self._make = make
 
     @property
     def model(self):
-        """Gets the model of this XiqDigitalTwinDevice.  # noqa: E501
+        """Gets the model of this XiqDigitalTwinProducts.  # noqa: E501
 
+        The Digital Twin device model.  # noqa: E501
 
-        :return: The model of this XiqDigitalTwinDevice.  # noqa: E501
-        :rtype: XiqDigitalTwinModel
+        :return: The model of this XiqDigitalTwinProducts.  # noqa: E501
+        :rtype: str
         """
         return self._model
 
     @model.setter
     def model(self, model):
-        """Sets the model of this XiqDigitalTwinDevice.
+        """Sets the model of this XiqDigitalTwinProducts.
 
+        The Digital Twin device model.  # noqa: E501
 
-        :param model: The model of this XiqDigitalTwinDevice.  # noqa: E501
-        :type: XiqDigitalTwinModel
+        :param model: The model of this XiqDigitalTwinProducts.  # noqa: E501
+        :type: str
         """
         if self.local_vars_configuration.client_side_validation and model is None:  # noqa: E501
             raise ValueError("Invalid value for `model`, must not be `None`")  # noqa: E501
 
         self._model = model
 
     @property
     def os_type(self):
-        """Gets the os_type of this XiqDigitalTwinDevice.  # noqa: E501
+        """Gets the os_type of this XiqDigitalTwinProducts.  # noqa: E501
 
         The Digital Twin device OS type.  # noqa: E501
 
-        :return: The os_type of this XiqDigitalTwinDevice.  # noqa: E501
+        :return: The os_type of this XiqDigitalTwinProducts.  # noqa: E501
         :rtype: str
         """
         return self._os_type
 
     @os_type.setter
     def os_type(self, os_type):
-        """Sets the os_type of this XiqDigitalTwinDevice.
+        """Sets the os_type of this XiqDigitalTwinProducts.
 
         The Digital Twin device OS type.  # noqa: E501
 
-        :param os_type: The os_type of this XiqDigitalTwinDevice.  # noqa: E501
+        :param os_type: The os_type of this XiqDigitalTwinProducts.  # noqa: E501
         :type: str
         """
 
         self._os_type = os_type
 
     @property
-    def os_version(self):
-        """Gets the os_version of this XiqDigitalTwinDevice.  # noqa: E501
+    def os_versions(self):
+        """Gets the os_versions of this XiqDigitalTwinProducts.  # noqa: E501
 
-        The Digital Twin device OS version.  # noqa: E501
+        The Digital Twin device OS versions.  # noqa: E501
 
-        :return: The os_version of this XiqDigitalTwinDevice.  # noqa: E501
-        :rtype: str
+        :return: The os_versions of this XiqDigitalTwinProducts.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._os_version
+        return self._os_versions
 
-    @os_version.setter
-    def os_version(self, os_version):
-        """Sets the os_version of this XiqDigitalTwinDevice.
+    @os_versions.setter
+    def os_versions(self, os_versions):
+        """Sets the os_versions of this XiqDigitalTwinProducts.
 
-        The Digital Twin device OS version.  # noqa: E501
+        The Digital Twin device OS versions.  # noqa: E501
 
-        :param os_version: The os_version of this XiqDigitalTwinDevice.  # noqa: E501
-        :type: str
+        :param os_versions: The os_versions of this XiqDigitalTwinProducts.  # noqa: E501
+        :type: list[str]
         """
-        if self.local_vars_configuration.client_side_validation and os_version is None:  # noqa: E501
-            raise ValueError("Invalid value for `os_version`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and os_versions is None:  # noqa: E501
+            raise ValueError("Invalid value for `os_versions`, must not be `None`")  # noqa: E501
 
-        self._os_version = os_version
+        self._os_versions = os_versions
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -189,18 +193,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqDigitalTwinDevice):
+        if not isinstance(other, XiqDigitalTwinProducts):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqDigitalTwinDevice):
+        if not isinstance(other, XiqDigitalTwinProducts):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_devices.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_make.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_make.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_model.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,143 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqDigitalTwinProducts(object):
+class XiqInitKeyBasedPcgNetworkPolicyRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'make': 'str',
-        'model': 'str',
-        'os_type': 'str',
-        'os_versions': 'list[str]'
+        'policy_name': 'str',
+        'ssid_name': 'str',
+        'users': 'list[XiqKeyBasedPcgUserBaseInfo]'
     }
 
     attribute_map = {
-        'make': 'make',
-        'model': 'model',
-        'os_type': 'os_type',
-        'os_versions': 'os_versions'
+        'policy_name': 'policy_name',
+        'ssid_name': 'ssid_name',
+        'users': 'users'
     }
 
-    def __init__(self, make=None, model=None, os_type=None, os_versions=None, local_vars_configuration=None):  # noqa: E501
-        """XiqDigitalTwinProducts - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, policy_name=None, ssid_name=None, users=None, local_vars_configuration=None):  # noqa: E501
+        """XiqInitKeyBasedPcgNetworkPolicyRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._make = None
-        self._model = None
-        self._os_type = None
-        self._os_versions = None
+        self._policy_name = None
+        self._ssid_name = None
+        self._users = None
         self.discriminator = None
 
-        self.make = make
-        self.model = model
-        if os_type is not None:
-            self.os_type = os_type
-        self.os_versions = os_versions
+        self.policy_name = policy_name
+        self.ssid_name = ssid_name
+        self.users = users
 
     @property
-    def make(self):
-        """Gets the make of this XiqDigitalTwinProducts.  # noqa: E501
+    def policy_name(self):
+        """Gets the policy_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
 
-        The Digital Twin device make.  # noqa: E501
+        The network policy name  # noqa: E501
 
-        :return: The make of this XiqDigitalTwinProducts.  # noqa: E501
+        :return: The policy_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
         :rtype: str
         """
-        return self._make
+        return self._policy_name
 
-    @make.setter
-    def make(self, make):
-        """Sets the make of this XiqDigitalTwinProducts.
+    @policy_name.setter
+    def policy_name(self, policy_name):
+        """Sets the policy_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.
 
-        The Digital Twin device make.  # noqa: E501
+        The network policy name  # noqa: E501
 
-        :param make: The make of this XiqDigitalTwinProducts.  # noqa: E501
+        :param policy_name: The policy_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and make is None:  # noqa: E501
-            raise ValueError("Invalid value for `make`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and policy_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `policy_name`, must not be `None`")  # noqa: E501
 
-        self._make = make
+        self._policy_name = policy_name
 
     @property
-    def model(self):
-        """Gets the model of this XiqDigitalTwinProducts.  # noqa: E501
+    def ssid_name(self):
+        """Gets the ssid_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
 
-        The Digital Twin device model.  # noqa: E501
+        The SSID name  # noqa: E501
 
-        :return: The model of this XiqDigitalTwinProducts.  # noqa: E501
+        :return: The ssid_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
         :rtype: str
         """
-        return self._model
+        return self._ssid_name
 
-    @model.setter
-    def model(self, model):
-        """Sets the model of this XiqDigitalTwinProducts.
+    @ssid_name.setter
+    def ssid_name(self, ssid_name):
+        """Sets the ssid_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.
 
-        The Digital Twin device model.  # noqa: E501
+        The SSID name  # noqa: E501
 
-        :param model: The model of this XiqDigitalTwinProducts.  # noqa: E501
+        :param ssid_name: The ssid_name of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and model is None:  # noqa: E501
-            raise ValueError("Invalid value for `model`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and ssid_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `ssid_name`, must not be `None`")  # noqa: E501
 
-        self._model = model
+        self._ssid_name = ssid_name
 
     @property
-    def os_type(self):
-        """Gets the os_type of this XiqDigitalTwinProducts.  # noqa: E501
+    def users(self):
+        """Gets the users of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
 
-        The Digital Twin device OS type.  # noqa: E501
+        The Key-based PCG users  # noqa: E501
 
-        :return: The os_type of this XiqDigitalTwinProducts.  # noqa: E501
-        :rtype: str
-        """
-        return self._os_type
-
-    @os_type.setter
-    def os_type(self, os_type):
-        """Sets the os_type of this XiqDigitalTwinProducts.
-
-        The Digital Twin device OS type.  # noqa: E501
-
-        :param os_type: The os_type of this XiqDigitalTwinProducts.  # noqa: E501
-        :type: str
-        """
-
-        self._os_type = os_type
-
-    @property
-    def os_versions(self):
-        """Gets the os_versions of this XiqDigitalTwinProducts.  # noqa: E501
-
-        The Digital Twin device OS versions.  # noqa: E501
-
-        :return: The os_versions of this XiqDigitalTwinProducts.  # noqa: E501
-        :rtype: list[str]
+        :return: The users of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
+        :rtype: list[XiqKeyBasedPcgUserBaseInfo]
         """
-        return self._os_versions
+        return self._users
 
-    @os_versions.setter
-    def os_versions(self, os_versions):
-        """Sets the os_versions of this XiqDigitalTwinProducts.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this XiqInitKeyBasedPcgNetworkPolicyRequest.
 
-        The Digital Twin device OS versions.  # noqa: E501
+        The Key-based PCG users  # noqa: E501
 
-        :param os_versions: The os_versions of this XiqDigitalTwinProducts.  # noqa: E501
-        :type: list[str]
+        :param users: The users of this XiqInitKeyBasedPcgNetworkPolicyRequest.  # noqa: E501
+        :type: list[XiqKeyBasedPcgUserBaseInfo]
         """
-        if self.local_vars_configuration.client_side_validation and os_versions is None:  # noqa: E501
-            raise ValueError("Invalid value for `os_versions`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and users is None:  # noqa: E501
+            raise ValueError("Invalid value for `users`, must not be `None`")  # noqa: E501
 
-        self._os_versions = os_versions
+        self._users = users
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -193,18 +165,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqDigitalTwinProducts):
+        if not isinstance(other, XiqInitKeyBasedPcgNetworkPolicyRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqDigitalTwinProducts):
+        if not isinstance(other, XiqInitKeyBasedPcgNetworkPolicyRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_duplex_data_rate_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_duplex_data_rate_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_email_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_email_template.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_email_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_end_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_entitlement_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_entitlement_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_error.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_exos_devices.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_exos_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_expiration_action_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_action_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_expiration_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_expiration_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_expiration_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_account.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_radius_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user_directory.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_external_user_directory_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_external_user_directory_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_measurement_unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqExternalUserDirectoryType(object):
+class XiqMeasurementUnit(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    OPEN_LDAP = "OPEN_LDAP"
-    ACTIVE_DIRECTORY = "ACTIVE_DIRECTORY"
+    FEET = "FEET"
+    METERS = "METERS"
 
-    allowable_values = [OPEN_LDAP, ACTIVE_DIRECTORY]  # noqa: E501
+    allowable_values = [FEET, METERS]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqExternalUserDirectoryType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqMeasurementUnit - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqExternalUserDirectoryType):
+        if not isinstance(other, XiqMeasurementUnit):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqExternalUserDirectoryType):
+        if not isinstance(other, XiqMeasurementUnit):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_extreme_devices.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_extreme_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_firmware_activate_option.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_activate_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_firmware_upgrade_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_flap_count_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_flap_count_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_floor.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_forensic_bucket.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_forensic_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_generate_api_token_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_generate_api_token_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_generate_api_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_get_port_assignment_details_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_grant_external_user_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_grant_external_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_hiq_context.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_hiq_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_hiq_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_initialize_location_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_initialize_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_key_based_pcg.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_l3_address_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_l3_address_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_l3_address_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_protocol_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ldap_server.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ldap_server_verification_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_license_mode.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_license_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_license_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_location.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_location_legend.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_legend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_location_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_location_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_login_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_login_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_measurement_unit.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqMeasurementUnit(object):
+class XiqRadioMode(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    FEET = "FEET"
-    METERS = "METERS"
+    B_G = "B_G"
+    G_N = "G_N"
+    A = "A"
+    A_N = "A_N"
+    AC = "AC"
+    AX_2_4_GHZ = "AX_2_4_GHZ"
+    AX_5_GHZ = "AX_5_GHZ"
+    AX_6_GHZ = "AX_6_GHZ"
 
-    allowable_values = [FEET, METERS]  # noqa: E501
+    allowable_values = [B_G, G_N, A, A_N, AC, AX_2_4_GHZ, AX_5_GHZ, AX_6_GHZ]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +50,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqMeasurementUnit - a model defined in OpenAPI"""  # noqa: E501
+        """XiqRadioMode - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +90,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqMeasurementUnit):
+        if not isinstance(other, XiqRadioMode):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqMeasurementUnit):
+        if not isinstance(other, XiqRadioMode):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_network_policy_view.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_network_policy_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_onboard_device_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_operation_metadata.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_operation_object.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_operation_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_operation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_organization.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_organization_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_organization_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_character_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_character_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_db_location.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_db_location.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_password_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_password_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_assign_ports_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_pcg_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_pcg_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_permission.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_poe_flapping_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_port_efficiency_stats_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_port_efficiency_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_post_expiration_action.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_post_expiration_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_psk_generation_method.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_psk_generation_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radio_mode.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_key_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqRadioMode(object):
+class XiqSsidKeyType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    B_G = "B_G"
-    G_N = "G_N"
-    A = "A"
-    A_N = "A_N"
-    AC = "AC"
-    AX_2_4_GHZ = "AX_2_4_GHZ"
-    AX_5_GHZ = "AX_5_GHZ"
-    AX_6_GHZ = "AX_6_GHZ"
+    ASCII = "ASCII"
+    HEX = "HEX"
 
-    allowable_values = [B_G, G_N, A, A_N, AC, AX_2_4_GHZ, AX_5_GHZ, AX_6_GHZ]  # noqa: E501
+    allowable_values = [ASCII, HEX]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -50,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqRadioMode - a model defined in OpenAPI"""  # noqa: E501
+        """XiqSsidKeyType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -90,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqRadioMode):
+        if not isinstance(other, XiqSsidKeyType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqRadioMode):
+        if not isinstance(other, XiqSsidKeyType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radio_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client_object.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_client_object_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_client_object_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_proxy.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_format_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_radius_server_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_radius_server_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_regenerate_end_user_password_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rf_environment_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rf_environment_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_channel_selection.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_channel_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_miscellaneous_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_sensor_scan_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_rp_wmm_qos_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_send_cli_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_send_cli_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_send_cli_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_server_role.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_server_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sms_log.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sms_log_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_log_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sms_template.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sms_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sort_field.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_sort_order.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_sort_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_speed_duplex_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_speed_duplex_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_dot1x_key_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_key_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_encryption_method.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqSsidKeyType(object):
+class XiqSsidWepEncryptionMethod(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    ASCII = "ASCII"
-    HEX = "HEX"
+    WEP40 = "WEP40"
+    WEP104 = "WEP104"
 
-    allowable_values = [ASCII, HEX]  # noqa: E501
+    allowable_values = [WEP40, WEP104]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqSsidKeyType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqSsidWepEncryptionMethod - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqSsidKeyType):
+        if not isinstance(other, XiqSsidWepEncryptionMethod):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqSsidKeyType):
+        if not isinstance(other, XiqSsidWepEncryptionMethod):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_ppsk_key_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_encryption_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_psk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_sae_group.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_sae_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_default_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_if_name.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqSsidWepEncryptionMethod(object):
+class XiqWirelessIfName(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    WEP40 = "WEP40"
-    WEP104 = "WEP104"
+    WIFI0 = "WIFI0"
+    WIFI1 = "WIFI1"
 
-    allowable_values = [WEP40, WEP104]  # noqa: E501
+    allowable_values = [WIFI0, WIFI1]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqSsidWepEncryptionMethod - a model defined in OpenAPI"""  # noqa: E501
+        """XiqWirelessIfName - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqSsidWepEncryptionMethod):
+        if not isinstance(other, XiqWirelessIfName):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqSsidWepEncryptionMethod):
+        if not isinstance(other, XiqWirelessIfName):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_ssid_wep_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_subscription_data_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_data_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_subscription_message_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_message_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_subscription_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_subscription_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_top_applications_usage.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_top_applications_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_trend_indicator.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_trend_indicator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_building_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_classification_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_device_level_ssid_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_end_user_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_external_user_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_external_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_floor_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_floor_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_location_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radio_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_client.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_client_object_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_channel_selection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_user_group_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_user_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_profile_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_user_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_update_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user_group.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_user_role.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_user_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_daily_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_daily_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_during_date_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_for_time_period_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_first_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_valid_time_period_after_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_viq.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_viq_license.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_viq_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_object_classified_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_vlan_profile.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_vlan_profile_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_voss_devices.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_voss_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_webhook_subscription.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_webhook_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wing_devices.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wing_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_event_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_hardware_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_hardware_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_quality_index_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wired_view_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wired_view_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_apps_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_apps_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_event_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_if_name.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_list_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqWirelessIfName(object):
+class XiqWirelessViewsListType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    WIFI0 = "WIFI0"
-    WIFI1 = "WIFI1"
+    SSID = "SSID"
+    OS = "OS"
 
-    allowable_values = [WIFI0, WIFI1]  # noqa: E501
+    allowable_values = [SSID, OS]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqWirelessIfName - a model defined in OpenAPI"""  # noqa: E501
+        """XiqWirelessViewsListType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqWirelessIfName):
+        if not isinstance(other, XiqWirelessViewsListType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqWirelessIfName):
+        if not isinstance(other, XiqWirelessViewsListType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_performance_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_quality_index_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_time_to_connect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_digital_twin_vim_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqWirelessViewsListType(object):
+class XiqDigitalTwinVimModule(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    SSID = "SSID"
-    OS = "OS"
+    _5520_VIM_4X = "DT_5520_VIM_4X"
+    _5520_VIM_4XE = "DT_5520_VIM_4XE"
+    _5520_VIM_4YE = "DT_5520_VIM_4YE"
+    _5720_VIM_2CE = "DT_5720_VIM_2CE"
+    _5720_VIM_6YE = "DT_5720_VIM_6YE"
 
-    allowable_values = [SSID, OS]  # noqa: E501
+    allowable_values = [_5520_VIM_4X, _5520_VIM_4XE, _5520_VIM_4YE, _5720_VIM_2CE, _5720_VIM_6YE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +47,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqWirelessViewsListType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqDigitalTwinVimModule - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +87,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqWirelessViewsListType):
+        if not isinstance(other, XiqDigitalTwinVimModule):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqWirelessViewsListType):
+        if not isinstance(other, XiqDigitalTwinVimModule):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/models/xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/models/xiq_wireless_views_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/__init__.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "23.3.0.35"
+__version__ = "23.3.1.15"
 
 # import apis into sdk package
 from extremecloudiq.api.account_api import AccountApi
 from extremecloudiq.api.alert_api import AlertApi
 from extremecloudiq.api.application_api import ApplicationApi
 from extremecloudiq.api.authentication_api import AuthenticationApi
 from extremecloudiq.api.authorization_api import AuthorizationApi
@@ -218,17 +218,19 @@
 from extremecloudiq.models.xiq_device_wifi_interface import XiqDeviceWifiInterface
 from extremecloudiq.models.xiq_dfs_channel_changes_entity import XiqDfsChannelChangesEntity
 from extremecloudiq.models.xiq_dfs_channel_stats_entity import XiqDfsChannelStatsEntity
 from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
 from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
 from extremecloudiq.models.xiq_digital_twin_device import XiqDigitalTwinDevice
 from extremecloudiq.models.xiq_digital_twin_devices import XiqDigitalTwinDevices
+from extremecloudiq.models.xiq_digital_twin_feat_license import XiqDigitalTwinFeatLicense
 from extremecloudiq.models.xiq_digital_twin_make import XiqDigitalTwinMake
 from extremecloudiq.models.xiq_digital_twin_model import XiqDigitalTwinModel
 from extremecloudiq.models.xiq_digital_twin_products import XiqDigitalTwinProducts
+from extremecloudiq.models.xiq_digital_twin_vim_module import XiqDigitalTwinVimModule
 from extremecloudiq.models.xiq_duplex_data_rate_entity import XiqDuplexDataRateEntity
 from extremecloudiq.models.xiq_email_log import XiqEmailLog
 from extremecloudiq.models.xiq_email_template import XiqEmailTemplate
 from extremecloudiq.models.xiq_end_user import XiqEndUser
 from extremecloudiq.models.xiq_entitlement_type import XiqEntitlementType
 from extremecloudiq.models.xiq_error import XiqError
 from extremecloudiq.models.xiq_exos_devices import XiqExosDevices
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/api_client.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/23.3.0.35/python'
+        self.user_agent = 'OpenAPI-Generator/23.3.1.15/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/configuration.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -333,16 +333,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.3.0.35\n"\
-               "SDK Package Version: 23.3.0.35".\
+               "Version of the API: 23.3.1.15\n"\
+               "SDK Package Version: 23.3.1.15".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/exceptions.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq/rest.py` & `extremecloudiq-api-23.3.1.15/extremecloudiq/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/extremecloudiq_api.egg-info/SOURCES.txt` & `extremecloudiq-api-23.3.1.15/extremecloudiq_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -198,17 +198,19 @@
 extremecloudiq/models/xiq_device_wifi_interface.py
 extremecloudiq/models/xiq_dfs_channel_changes_entity.py
 extremecloudiq/models/xiq_dfs_channel_stats_entity.py
 extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
 extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
 extremecloudiq/models/xiq_digital_twin_device.py
 extremecloudiq/models/xiq_digital_twin_devices.py
+extremecloudiq/models/xiq_digital_twin_feat_license.py
 extremecloudiq/models/xiq_digital_twin_make.py
 extremecloudiq/models/xiq_digital_twin_model.py
 extremecloudiq/models/xiq_digital_twin_products.py
+extremecloudiq/models/xiq_digital_twin_vim_module.py
 extremecloudiq/models/xiq_duplex_data_rate_entity.py
 extremecloudiq/models/xiq_email_log.py
 extremecloudiq/models/xiq_email_template.py
 extremecloudiq/models/xiq_end_user.py
 extremecloudiq/models/xiq_entitlement_type.py
 extremecloudiq/models/xiq_error.py
 extremecloudiq/models/xiq_exos_devices.py
@@ -593,17 +595,19 @@
 test/test_xiq_device_wifi_interface.py
 test/test_xiq_dfs_channel_changes_entity.py
 test/test_xiq_dfs_channel_stats_entity.py
 test/test_xiq_dfs_recurence_channel_stats_response.py
 test/test_xiq_dfs_recurence_count_stats_response.py
 test/test_xiq_digital_twin_device.py
 test/test_xiq_digital_twin_devices.py
+test/test_xiq_digital_twin_feat_license.py
 test/test_xiq_digital_twin_make.py
 test/test_xiq_digital_twin_model.py
 test/test_xiq_digital_twin_products.py
+test/test_xiq_digital_twin_vim_module.py
 test/test_xiq_duplex_data_rate_entity.py
 test/test_xiq_email_log.py
 test/test_xiq_email_template.py
 test/test_xiq_end_user.py
 test/test_xiq_entitlement_type.py
 test/test_xiq_error.py
 test/test_xiq_exos_devices.py
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_account_api.py` & `extremecloudiq-api-23.3.1.15/test/test_account_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_alert_api.py` & `extremecloudiq-api-23.3.1.15/test/test_alert_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_application_api.py` & `extremecloudiq-api-23.3.1.15/test/test_application_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_authentication_api.py` & `extremecloudiq-api-23.3.1.15/test/test_authentication_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_authorization_api.py` & `extremecloudiq-api-23.3.1.15/test/test_authorization_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_client_api.py` & `extremecloudiq-api-23.3.1.15/test/test_client_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_configuration___authentication_api.py` & `extremecloudiq-api-23.3.1.15/test/test_configuration___authentication_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_configuration___basic_api.py` & `extremecloudiq-api-23.3.1.15/test/test_configuration___basic_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_configuration___certificate_api.py` & `extremecloudiq-api-23.3.1.15/test/test_configuration___certificate_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_configuration___deployment_api.py` & `extremecloudiq-api-23.3.1.15/test/test_configuration___deployment_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_configuration___policy_api.py` & `extremecloudiq-api-23.3.1.15/test/test_configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_configuration___user_management_api.py` & `extremecloudiq-api-23.3.1.15/test/test_configuration___user_management_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_copilot___anomalies_api.py` & `extremecloudiq-api-23.3.1.15/test/test_copilot___anomalies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.3.1.15/test/test_copilot___connectivity_experience_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_device_api.py` & `extremecloudiq-api-23.3.1.15/test/test_device_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_hiq_api.py` & `extremecloudiq-api-23.3.1.15/test/test_hiq_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_inline_object.py` & `extremecloudiq-api-23.3.1.15/test/test_inline_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_location_api.py` & `extremecloudiq-api-23.3.1.15/test/test_location_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_log_api.py` & `extremecloudiq-api-23.3.1.15/test/test_log_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_network_policy_api.py` & `extremecloudiq-api-23.3.1.15/test/test_network_policy_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_notification_api.py` & `extremecloudiq-api-23.3.1.15/test/test_notification_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_operation_api.py` & `extremecloudiq-api-23.3.1.15/test/test_operation_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_accounting_log.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_accounting_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_active_directory_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_alert.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_application.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_audit_log.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_audit_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_auth_log.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_auth_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_certificate.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_classification_rule.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_client.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cloud_config_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_connectivity_experience_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_credential_log.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_cwp.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_cwp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_device.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_device_alarm.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_digital_twin_products.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_email_log.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_email_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_end_user.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_radius_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_external_user.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_external_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_internal_radius_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_ldap_server.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ldap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_network_policy.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_radio_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_radius_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_rp_mac_oui_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_sms_log.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_ssid.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_ssid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_user.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_user_group.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_user_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_vlan_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_paged_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_user_api.py` & `extremecloudiq-api-23.3.1.15/test/test_user_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_account.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_account_mode.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_account_mode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_account_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_account_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_accounting_log.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_accounting_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_active_directory_server.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_alert.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_alert_category.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_category.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_alert_group_query.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_group_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_alert_severity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_severity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_alert_source.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_alert_source_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_alert_source_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomalies_count_vo_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomalies_count_vo_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_device_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_devices_by_location_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_location_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_severity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField  # noqa: E501
+from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqAnomalySortField(unittest.TestCase):
-    """XiqAnomalySortField unit test stubs"""
+class TestXiqAnomalyType(unittest.TestCase):
+    """XiqAnomalyType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqAnomalySortField
+        """Test XiqAnomalyType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_anomaly_sort_field.XiqAnomalySortField()  # noqa: E501
+        # model = extremecloudiq.models.xiq_anomaly_type.XiqAnomalyType()  # noqa: E501
         if include_optional :
-            return XiqAnomalySortField(
+            return XiqAnomalyType(
             )
         else :
-            return XiqAnomalySortField(
+            return XiqAnomalyType(
         )
 
-    def testXiqAnomalySortField(self):
-        """Test XiqAnomalySortField"""
+    def testXiqAnomalyType(self):
+        """Test XiqAnomalyType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_anomaly_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_stats.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType  # noqa: E501
+from extremecloudiq.models.xiq_device_stats import XiqDeviceStats  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqAnomalyType(unittest.TestCase):
-    """XiqAnomalyType unit test stubs"""
+class TestXiqDeviceStats(unittest.TestCase):
+    """XiqDeviceStats unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqAnomalyType
+        """Test XiqDeviceStats
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_anomaly_type.XiqAnomalyType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_device_stats.XiqDeviceStats()  # noqa: E501
         if include_optional :
-            return XiqAnomalyType(
+            return XiqDeviceStats(
+                total_device_count = 56, 
+                managed_device_count = 56, 
+                connected_device_count = 56
             )
         else :
-            return XiqAnomalyType(
+            return XiqDeviceStats(
         )
 
-    def testXiqAnomalyType(self):
-        """Test XiqAnomalyType"""
+    def testXiqDeviceStats(self):
+        """Test XiqDeviceStats"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_api_token_info.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_api_token_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_application.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_application_detection_protocol.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_application_detection_rule.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_application_detection_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_application_detection_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_application_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_application_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_application_top_clients_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_country_code_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_audit_log.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_location_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_assign_devices_network_policy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_assurance_scans_overview_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_assurance_scans_overview_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_atp_device_stats_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_atp_device_stats_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_device_stats_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_atp_packet_counts_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_atp_packet_counts_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_atp_packet_counts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_audit_log_category.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_category.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_audit_log_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_audit_log_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_auth_log.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_auth_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_data.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_operation_result.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_operation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_bounce_device_port_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_bounce_device_port_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_building.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_certificate.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_certificate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_certificate_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_certificate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_ibeacon_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_change_devices_os_mode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_check_permission_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_check_permission_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_check_permission_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_classification.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_classification_rule.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_classification_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_classification_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_cli_output.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_cli_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_cli_response_code.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_cli_response_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_client.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_client_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_client_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_client_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_client_sort_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_client_summary.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_client_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_client_usage.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_client_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_client_view.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_client_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_cloud_config_group.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_cloud_config_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_connectivity_experience_view_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wired_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_events_wireless_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wired_events_score_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_copilot_wireless_events_score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_country_code.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_country_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_building_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_building_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_classification_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_classification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_cloud_config_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_end_user_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_end_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_external_radius_server_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_floor_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_internal_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_key_based_pcg_users_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_ldap_server_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_location_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_organization_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radio_profile_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_client.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_radius_proxy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_user_group_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_user_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_user_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_object_classified_entry_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_create_vlan_object_classified_entry_request import XiqCreateVlanObjectClassifiedEntryRequest  # noqa: E501
+from extremecloudiq.models.xiq_update_vlan_object_classified_entry_request import XiqUpdateVlanObjectClassifiedEntryRequest  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqCreateVlanObjectClassifiedEntryRequest(unittest.TestCase):
-    """XiqCreateVlanObjectClassifiedEntryRequest unit test stubs"""
+class TestXiqUpdateVlanObjectClassifiedEntryRequest(unittest.TestCase):
+    """XiqUpdateVlanObjectClassifiedEntryRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqCreateVlanObjectClassifiedEntryRequest
+        """Test XiqUpdateVlanObjectClassifiedEntryRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_create_vlan_object_classified_entry_request.XiqCreateVlanObjectClassifiedEntryRequest()  # noqa: E501
+        # model = extremecloudiq.models.xiq_update_vlan_object_classified_entry_request.XiqUpdateVlanObjectClassifiedEntryRequest()  # noqa: E501
         if include_optional :
-            return XiqCreateVlanObjectClassifiedEntryRequest(
+            return XiqUpdateVlanObjectClassifiedEntryRequest(
                 vlan_id = 56, 
                 classification_rule_id = 56
             )
         else :
-            return XiqCreateVlanObjectClassifiedEntryRequest(
+            return XiqUpdateVlanObjectClassifiedEntryRequest(
                 vlan_id = 56,
                 classification_rule_id = 56,
         )
 
-    def testXiqCreateVlanObjectClassifiedEntryRequest(self):
-        """Test XiqCreateVlanObjectClassifiedEntryRequest"""
+    def testXiqUpdateVlanObjectClassifiedEntryRequest(self):
+        """Test XiqUpdateVlanObjectClassifiedEntryRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_profile_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_webhook_subscription_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_credential_log.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_credential_log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_cwp.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_cwp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_data_point.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_data_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_date_time_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_date_time_unit_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_date_time_unit_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_default_device_password.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_default_device_password.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_delete_key_based_pcg_users_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_delivery_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_delivery_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_dell_devices.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_dell_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_overview.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_overview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_policy.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_deployment_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_deployment_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_admin_state.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_admin_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_alarm.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_cpu_memory_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_filter.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_function.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_ibeacon.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_ibeacon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_installation_report.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_installation_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_level_ssid.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_lldp_cdp_info.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_lldp_cdp_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_location.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_location_assignment.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_location_assignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_null_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_null_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_stats.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_device_stats import XiqDeviceStats  # noqa: E501
+from extremecloudiq.models.xiq_network_policy_type import XiqNetworkPolicyType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqDeviceStats(unittest.TestCase):
-    """XiqDeviceStats unit test stubs"""
+class TestXiqNetworkPolicyType(unittest.TestCase):
+    """XiqNetworkPolicyType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqDeviceStats
+        """Test XiqNetworkPolicyType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_device_stats.XiqDeviceStats()  # noqa: E501
+        # model = extremecloudiq.models.xiq_network_policy_type.XiqNetworkPolicyType()  # noqa: E501
         if include_optional :
-            return XiqDeviceStats(
-                total_device_count = 56, 
-                managed_device_count = 56, 
-                connected_device_count = 56
+            return XiqNetworkPolicyType(
             )
         else :
-            return XiqDeviceStats(
+            return XiqNetworkPolicyType(
         )
 
-    def testXiqDeviceStats(self):
-        """Test XiqDeviceStats"""
+    def testXiqNetworkPolicyType(self):
+        """Test XiqNetworkPolicyType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_view.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_device_wifi_interface.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_device_wifi_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_channel_changes_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_changes_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_channel_stats_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_channel_stats_entity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_recurence_channel_stats_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_channel_stats_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_dfs_recurence_count_stats_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_dfs_recurence_count_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_device.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_make.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_digital_twin_device import XiqDigitalTwinDevice  # noqa: E501
+from extremecloudiq.models.xiq_digital_twin_make import XiqDigitalTwinMake  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqDigitalTwinDevice(unittest.TestCase):
-    """XiqDigitalTwinDevice unit test stubs"""
+class TestXiqDigitalTwinMake(unittest.TestCase):
+    """XiqDigitalTwinMake unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqDigitalTwinDevice
+        """Test XiqDigitalTwinMake
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_digital_twin_device.XiqDigitalTwinDevice()  # noqa: E501
+        # model = extremecloudiq.models.xiq_digital_twin_make.XiqDigitalTwinMake()  # noqa: E501
         if include_optional :
-            return XiqDigitalTwinDevice(
-                make = 'SWITCH_ENGINE', 
-                model = 'DT_5320_16P_4XE', 
-                os_type = '0', 
-                os_version = '0'
+            return XiqDigitalTwinMake(
             )
         else :
-            return XiqDigitalTwinDevice(
-                make = 'SWITCH_ENGINE',
-                model = 'DT_5320_16P_4XE',
-                os_version = '0',
+            return XiqDigitalTwinMake(
         )
 
-    def testXiqDigitalTwinDevice(self):
-        """Test XiqDigitalTwinDevice"""
+    def testXiqDigitalTwinMake(self):
+        """Test XiqDigitalTwinMake"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_devices.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -38,15 +38,21 @@
         if include_optional :
             return XiqDigitalTwinDevices(
                 dts = [
                     extremecloudiq.models.xiq_digital_twin_device.XiqDigitalTwinDevice(
                         make = 'SWITCH_ENGINE', 
                         model = 'DT_5320_16P_4XE', 
                         os_type = '0', 
-                        os_version = '0', )
+                        os_version = '0', 
+                        vim_modules = [
+                            'DT_5520_VIM_4X'
+                            ], 
+                        feat_licenses = [
+                            'PRD_5000_PRMR'
+                            ], )
                     ]
             )
         else :
             return XiqDigitalTwinDevices(
         )
 
     def testXiqDigitalTwinDevices(self):
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_make.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_vim_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_digital_twin_make import XiqDigitalTwinMake  # noqa: E501
+from extremecloudiq.models.xiq_digital_twin_vim_module import XiqDigitalTwinVimModule  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqDigitalTwinMake(unittest.TestCase):
-    """XiqDigitalTwinMake unit test stubs"""
+class TestXiqDigitalTwinVimModule(unittest.TestCase):
+    """XiqDigitalTwinVimModule unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqDigitalTwinMake
+        """Test XiqDigitalTwinVimModule
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_digital_twin_make.XiqDigitalTwinMake()  # noqa: E501
+        # model = extremecloudiq.models.xiq_digital_twin_vim_module.XiqDigitalTwinVimModule()  # noqa: E501
         if include_optional :
-            return XiqDigitalTwinMake(
+            return XiqDigitalTwinVimModule(
             )
         else :
-            return XiqDigitalTwinMake(
+            return XiqDigitalTwinVimModule(
         )
 
-    def testXiqDigitalTwinMake(self):
-        """Test XiqDigitalTwinMake"""
+    def testXiqDigitalTwinVimModule(self):
+        """Test XiqDigitalTwinVimModule"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_model.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_digital_twin_products.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_digital_twin_products.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_duplex_data_rate_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_duplex_data_rate_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_email_log.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_email_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_email_template.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_email_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_end_user.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_end_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_entitlement_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_entitlement_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_error.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_exos_devices.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_exos_devices.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_expiration_action_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_action_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_expiration_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_expiration_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_expiration_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_external_account.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_external_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_external_radius_server.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_external_user.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_external_user_directory.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_external_user_directory_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_external_user_directory_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_extreme_devices.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_extreme_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_firmware_activate_option.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_activate_option.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_firmware_upgrade_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_flap_count_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_flap_count_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_floor.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_forensic_bucket.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_forensic_bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_generate_api_token_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_generate_api_token_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_generate_api_token_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_get_port_assignment_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_grant_external_user_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_grant_external_user_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_hiq_context.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_hiq_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_hiq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_initialize_location_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_initialize_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_device.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_server.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_internal_radius_server_authentication_method_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_key_based_pcg.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_key_based_pcg_user_base_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_l3_address_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_l3_address_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_l3_address_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_protocol_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ldap_server.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ldap_server_verification_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_license_mode.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_license_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_license_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_license_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_location.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_location_legend.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_location_legend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_location_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_location_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_login_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_login_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_login_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_measurement_unit.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_measurement_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_network_policy_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_network_policy_type import XiqNetworkPolicyType  # noqa: E501
+from extremecloudiq.models.xiq_network_policy_view import XiqNetworkPolicyView  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqNetworkPolicyType(unittest.TestCase):
-    """XiqNetworkPolicyType unit test stubs"""
+class TestXiqNetworkPolicyView(unittest.TestCase):
+    """XiqNetworkPolicyView unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqNetworkPolicyType
+        """Test XiqNetworkPolicyView
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_network_policy_type.XiqNetworkPolicyType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_network_policy_view.XiqNetworkPolicyView()  # noqa: E501
         if include_optional :
-            return XiqNetworkPolicyType(
+            return XiqNetworkPolicyView(
             )
         else :
-            return XiqNetworkPolicyType(
+            return XiqNetworkPolicyView(
         )
 
-    def testXiqNetworkPolicyType(self):
-        """Test XiqNetworkPolicyType"""
+    def testXiqNetworkPolicyView(self):
+        """Test XiqNetworkPolicyView"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_network_policy_view.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_password_character_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_network_policy_view import XiqNetworkPolicyView  # noqa: E501
+from extremecloudiq.models.xiq_password_character_type import XiqPasswordCharacterType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqNetworkPolicyView(unittest.TestCase):
-    """XiqNetworkPolicyView unit test stubs"""
+class TestXiqPasswordCharacterType(unittest.TestCase):
+    """XiqPasswordCharacterType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqNetworkPolicyView
+        """Test XiqPasswordCharacterType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_network_policy_view.XiqNetworkPolicyView()  # noqa: E501
+        # model = extremecloudiq.models.xiq_password_character_type.XiqPasswordCharacterType()  # noqa: E501
         if include_optional :
-            return XiqNetworkPolicyView(
+            return XiqPasswordCharacterType(
             )
         else :
-            return XiqNetworkPolicyView(
+            return XiqPasswordCharacterType(
         )
 
-    def testXiqNetworkPolicyView(self):
-        """Test XiqNetworkPolicyView"""
+    def testXiqPasswordCharacterType(self):
+        """Test XiqPasswordCharacterType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_onboard_device_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_device_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -59,15 +59,21 @@
                         }, ), 
                 dt = extremecloudiq.models.xiq_digital_twin_devices.XiqDigitalTwinDevices(
                     dts = [
                         extremecloudiq.models.xiq_digital_twin_device.XiqDigitalTwinDevice(
                             make = 'SWITCH_ENGINE', 
                             model = 'DT_5320_16P_4XE', 
                             os_type = '0', 
-                            os_version = '0', )
+                            os_version = '0', 
+                            vim_modules = [
+                                'DT_5520_VIM_4X'
+                                ], 
+                            feat_licenses = [
+                                'PRD_5000_PRMR'
+                                ], )
                         ], )
             )
         else :
             return XiqOnboardDeviceRequest(
         )
 
     def testXiqOnboardDeviceRequest(self):
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_onboard_key_based_pcg_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_operation_metadata.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_operation_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_operation_object.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_operation_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_operation_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_organization.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_organization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_organization_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_organization_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_password_character_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_password_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_password_character_type import XiqPasswordCharacterType  # noqa: E501
+from extremecloudiq.models.xiq_password_type import XiqPasswordType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqPasswordCharacterType(unittest.TestCase):
-    """XiqPasswordCharacterType unit test stubs"""
+class TestXiqPasswordType(unittest.TestCase):
+    """XiqPasswordType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqPasswordCharacterType
+        """Test XiqPasswordType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_password_character_type.XiqPasswordCharacterType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_password_type.XiqPasswordType()  # noqa: E501
         if include_optional :
-            return XiqPasswordCharacterType(
+            return XiqPasswordType(
             )
         else :
-            return XiqPasswordCharacterType(
+            return XiqPasswordType(
         )
 
-    def testXiqPasswordCharacterType(self):
-        """Test XiqPasswordCharacterType"""
+    def testXiqPasswordType(self):
+        """Test XiqPasswordType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_password_db_location.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_password_db_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_password_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_password_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_password_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radio_mode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_password_type import XiqPasswordType  # noqa: E501
+from extremecloudiq.models.xiq_radio_mode import XiqRadioMode  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqPasswordType(unittest.TestCase):
-    """XiqPasswordType unit test stubs"""
+class TestXiqRadioMode(unittest.TestCase):
+    """XiqRadioMode unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqPasswordType
+        """Test XiqRadioMode
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_password_type.XiqPasswordType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_radio_mode.XiqRadioMode()  # noqa: E501
         if include_optional :
-            return XiqPasswordType(
+            return XiqRadioMode(
             )
         else :
-            return XiqPasswordType(
+            return XiqRadioMode(
         )
 
-    def testXiqPasswordType(self):
-        """Test XiqPasswordType"""
+    def testXiqRadioMode(self):
+        """Test XiqRadioMode"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_assign_ports_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_pcg_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_pcg_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_permission.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_poe_flapping_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_port_efficiency_speed_duplex_stats_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_speed_duplex_stats_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_port_efficiency_stats_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_port_efficiency_stats_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_post_expiration_action.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_post_expiration_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_psk_generation_method.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_psk_generation_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radio_mode.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_sort_order.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_radio_mode import XiqRadioMode  # noqa: E501
+from extremecloudiq.models.xiq_sort_order import XiqSortOrder  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqRadioMode(unittest.TestCase):
-    """XiqRadioMode unit test stubs"""
+class TestXiqSortOrder(unittest.TestCase):
+    """XiqSortOrder unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqRadioMode
+        """Test XiqSortOrder
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_radio_mode.XiqRadioMode()  # noqa: E501
+        # model = extremecloudiq.models.xiq_sort_order.XiqSortOrder()  # noqa: E501
         if include_optional :
-            return XiqRadioMode(
+            return XiqSortOrder(
             )
         else :
-            return XiqRadioMode(
+            return XiqSortOrder(
         )
 
-    def testXiqRadioMode(self):
-        """Test XiqRadioMode"""
+    def testXiqSortOrder(self):
+        """Test XiqSortOrder"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radio_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client_object.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_client_object_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_client_object_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_proxy.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_format_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_radius_server_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_radius_server_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_regenerate_end_user_password_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rf_environment_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rf_environment_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_channel_selection.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_channel_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_miscellaneous_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_sensor_scan_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_rp_wmm_qos_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_send_cli_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_send_cli_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_send_cli_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_server_role.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_server_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_dot1x_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_ppsk_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_psk_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_set_ssid_mode_wep_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_sms_log.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_sms_log_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_sms_log_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_sms_template.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_sms_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_sort_field.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_sort_order.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_anomaly_sort_field.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_sort_order import XiqSortOrder  # noqa: E501
+from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqSortOrder(unittest.TestCase):
-    """XiqSortOrder unit test stubs"""
+class TestXiqAnomalySortField(unittest.TestCase):
+    """XiqAnomalySortField unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqSortOrder
+        """Test XiqAnomalySortField
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_sort_order.XiqSortOrder()  # noqa: E501
+        # model = extremecloudiq.models.xiq_anomaly_sort_field.XiqAnomalySortField()  # noqa: E501
         if include_optional :
-            return XiqSortOrder(
+            return XiqAnomalySortField(
             )
         else :
-            return XiqSortOrder(
+            return XiqAnomalySortField(
         )
 
-    def testXiqSortOrder(self):
-        """Test XiqSortOrder"""
+    def testXiqAnomalySortField(self):
+        """Test XiqAnomalySortField"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_speed_duplex_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_speed_duplex_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_dot1x_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_key_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_key_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_ppsk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_encryption_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_psk_key_management.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_sae_group.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_sae_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_default_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_ssid_wep_key_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_subscription_data_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_data_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_subscription_message_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_message_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_subscription_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_subscription_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_top_applications_usage.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_top_applications_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_trend_indicator.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_trend_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_building_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_building_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_classification_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_end_user_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_end_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_radius_server_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_user.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_external_user_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_external_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_floor_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_floor_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_key_based_pcg_users_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_ldap_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_location_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_network_policy_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radio_profile_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_client.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_client_object_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_radius_proxy_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_channel_selection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_mac_oui_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_user_group_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_user_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_user_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_create_vlan_object_classified_entry_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_update_vlan_object_classified_entry_request import XiqUpdateVlanObjectClassifiedEntryRequest  # noqa: E501
+from extremecloudiq.models.xiq_create_vlan_object_classified_entry_request import XiqCreateVlanObjectClassifiedEntryRequest  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqUpdateVlanObjectClassifiedEntryRequest(unittest.TestCase):
-    """XiqUpdateVlanObjectClassifiedEntryRequest unit test stubs"""
+class TestXiqCreateVlanObjectClassifiedEntryRequest(unittest.TestCase):
+    """XiqCreateVlanObjectClassifiedEntryRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqUpdateVlanObjectClassifiedEntryRequest
+        """Test XiqCreateVlanObjectClassifiedEntryRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_update_vlan_object_classified_entry_request.XiqUpdateVlanObjectClassifiedEntryRequest()  # noqa: E501
+        # model = extremecloudiq.models.xiq_create_vlan_object_classified_entry_request.XiqCreateVlanObjectClassifiedEntryRequest()  # noqa: E501
         if include_optional :
-            return XiqUpdateVlanObjectClassifiedEntryRequest(
+            return XiqCreateVlanObjectClassifiedEntryRequest(
                 vlan_id = 56, 
                 classification_rule_id = 56
             )
         else :
-            return XiqUpdateVlanObjectClassifiedEntryRequest(
+            return XiqCreateVlanObjectClassifiedEntryRequest(
                 vlan_id = 56,
                 classification_rule_id = 56,
         )
 
-    def testXiqUpdateVlanObjectClassifiedEntryRequest(self):
-        """Test XiqUpdateVlanObjectClassifiedEntryRequest"""
+    def testXiqCreateVlanObjectClassifiedEntryRequest(self):
+        """Test XiqCreateVlanObjectClassifiedEntryRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_update_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_user_group.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_user_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_user_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_user_role.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_user_role.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_valid_daily_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_daily_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_during_date_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_for_time_period_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_first_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_id_creation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_valid_time_period_after_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_viq.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_viq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_viq_license.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_viq_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_object_classified_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_vlan_profile.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_vlan_profile_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_voss_devices.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_voss_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_webhook_subscription.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_webhook_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wing_devices.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wing_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wired_event_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wired_hardware_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_hardware_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_quality_index_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wired_view_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wired_view_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_apps_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_apps_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_connectivity_performance_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_event_retries_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_if_name.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_if_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_performance_retries_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_quality_index_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_time_to_connect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_list_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/test/test_xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.3.1.15/test/test_xiq_wireless_views_type_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.0.35/README.md` & `extremecloudiq-api-23.3.1.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # extremecloudiq-api
 ExtremeCloud IQ RESTful API for external and internal applications.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 23.3.0.35
-- Package version: 23.3.0.35
+- API version: 23.3.1.15
+- Package version: 23.3.1.15
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.extremenetworks.com/support](https://www.extremenetworks.com/support)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -520,17 +520,19 @@
  - [XiqDeviceWifiInterface](docs/XiqDeviceWifiInterface.md)
  - [XiqDfsChannelChangesEntity](docs/XiqDfsChannelChangesEntity.md)
  - [XiqDfsChannelStatsEntity](docs/XiqDfsChannelStatsEntity.md)
  - [XiqDfsRecurenceChannelStatsResponse](docs/XiqDfsRecurenceChannelStatsResponse.md)
  - [XiqDfsRecurenceCountStatsResponse](docs/XiqDfsRecurenceCountStatsResponse.md)
  - [XiqDigitalTwinDevice](docs/XiqDigitalTwinDevice.md)
  - [XiqDigitalTwinDevices](docs/XiqDigitalTwinDevices.md)
+ - [XiqDigitalTwinFeatLicense](docs/XiqDigitalTwinFeatLicense.md)
  - [XiqDigitalTwinMake](docs/XiqDigitalTwinMake.md)
  - [XiqDigitalTwinModel](docs/XiqDigitalTwinModel.md)
  - [XiqDigitalTwinProducts](docs/XiqDigitalTwinProducts.md)
+ - [XiqDigitalTwinVimModule](docs/XiqDigitalTwinVimModule.md)
  - [XiqDuplexDataRateEntity](docs/XiqDuplexDataRateEntity.md)
  - [XiqEmailLog](docs/XiqEmailLog.md)
  - [XiqEmailTemplate](docs/XiqEmailTemplate.md)
  - [XiqEndUser](docs/XiqEndUser.md)
  - [XiqEntitlementType](docs/XiqEntitlementType.md)
  - [XiqError](docs/XiqError.md)
  - [XiqExosDevices](docs/XiqExosDevices.md)
```

### Comparing `extremecloudiq-api-23.3.0.35/setup.py` & `extremecloudiq-api-23.3.1.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.0.35
+    The version of the OpenAPI document: 23.3.1.15
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "extremecloudiq-api"
-VERSION = "23.3.0.35"
+VERSION = "23.3.1.15"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

