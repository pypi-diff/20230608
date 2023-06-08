# Comparing `tmp/sdc11073-2.0.0a1.tar.gz` & `tmp/sdc11073-2.0.0a2.tar.gz`

## Comparing `sdc11073-2.0.0a1.tar` & `sdc11073-2.0.0a2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/CHANGELOG.md
--rw-r--r--   0        0        0   347063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/docs/sdc_social_preview.jpg
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/__init__.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/certloader.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/commlog.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/definitions_base.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/definitions_sdc.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/etc.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/exceptions.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/location.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/loghelper.py
--rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/multikey.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/namespaces.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/schema_resolver.py
--rw-r--r--   0        0        0    51437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/wsdiscovery.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/dispatch/__init__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/dispatch/dispatchkey.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/dispatch/messageconverter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/dispatch/pathelementregistry.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/dispatch/request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/httpserver/__init__.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/httpserver/compression.py
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/httpserver/httpreader.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/httpserver/httprequesthandler.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/httpserver/httpserverimpl.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/__init__.py
--rw-r--r--   0        0        0    34886 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/clientmdib.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/clientmdibxtra.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/containerbase.py
--rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/descriptorcontainers.py
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/devicemdib.py
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/devicemdibxtra.py
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/devicewaveform.py
--rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/mdibbase.py
--rw-r--r--   0        0        0    24434 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/statecontainers.py
--rw-r--r--   0        0        0    36856 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/mdib/transactions.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/netconn/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/observableproperties/__init__.py
--rw-r--r--   0        0        0     8027 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/observableproperties/observables.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/observableproperties/valuecollector.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/__init__.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/msgfactory.py
--rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/msgreader.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/soapclient.py
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/soapclient_async.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/soapclientpool.py
--rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/pysoap/soapenvelope.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/__init__.py
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/alarmprovider.py
--rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/audiopauseprovider.py
--rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/clockprovider.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/contextprovider.py
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/metricprovider.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/nomenclature.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/operationprovider.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/patientcontextprovider.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/product.py
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/roles/providerbase.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/__init__.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/components.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/manipulator.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/operations.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/request_handler_deferred.py
--rw-r--r--   0        0        0    31894 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/sdcclientimpl.py
--rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/__init__.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/contextservice.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/descriptioneventservice.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/getservice.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/localizationservice.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/setservice.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/stateeventservice.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/waveformservice.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/__init__.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/components.py
--rw-r--r--   0        0        0     9462 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/dpwshostedservice.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/intervaltimer.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/operations.py
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/periodicreports.py
--rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/sco.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/scopesfactory.py
--rw-r--r--   0        0        0    24489 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/sdcdeviceimpl.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/servicesfactory.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/subscriptionmgr.py
--rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/subscriptionmgr_async.py
--rw-r--r--   0        0        0    24603 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/subscriptionmgr_base.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/waveforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py
--rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py
--rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py
--rw-r--r--   0        0        0    12513 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/localizationservice.py
--rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/porttypebase.py
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/actions.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/addressing_types.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/basetypes.py
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/dataconverters.py
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/dpws_types.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/eventing_types.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/ext_qnames.py
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/isoduration.py
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/mex_types.py
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/msg_qnames.py
--rw-r--r--   0        0        0    27781 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/msg_types.py
--rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/pm_qnames.py
--rw-r--r--   0        0        0    58377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/pm_types.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/wsd_types.py
--rw-r--r--   0        0        0    50747 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xml_types/xml_structure.py
--rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/BICEPS_MessageModel.xsd
--rw-r--r--   0        0        0   205547 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/ExtensionPoint.xsd
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/MetadataExchange.xsd
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/SafetyInformation.xsd
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/addressing.xsd
--rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/eventing.xsd
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/soap-envelope.xsd
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/ws-addr.xsd
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd
--rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/wsdl.xsd
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/src/sdc11073/xsd/xml.xsd
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/tutorial/README.rst
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/README.rst
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0   347063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/docs/sdc_social_preview.jpg
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/certloader.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/commlog.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/definitions_base.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/definitions_sdc.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/etc.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/exceptions.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/location.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/loghelper.py
+-rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/multikey.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/namespaces.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/schema_resolver.py
+-rw-r--r--   0        0        0    51437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/wsdiscovery.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/dispatch/__init__.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/dispatch/dispatchkey.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/dispatch/messageconverter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/dispatch/pathelementregistry.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/dispatch/request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/httpserver/__init__.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/httpserver/compression.py
+-rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/httpserver/httpreader.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/httpserver/httprequesthandler.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/httpserver/httpserverimpl.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/__init__.py
+-rw-r--r--   0        0        0    35169 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/clientmdib.py
+-rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/clientmdibxtra.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/containerbase.py
+-rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/descriptorcontainers.py
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/devicemdib.py
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/devicemdibxtra.py
+-rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/devicewaveform.py
+-rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/mdibbase.py
+-rw-r--r--   0        0        0    24434 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/statecontainers.py
+-rw-r--r--   0        0        0    36856 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/mdib/transactions.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/netconn/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/observableproperties/__init__.py
+-rw-r--r--   0        0        0     8027 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/observableproperties/observables.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/observableproperties/valuecollector.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/__init__.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/msgfactory.py
+-rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/msgreader.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/soapclient.py
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/soapclient_async.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/soapclientpool.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/pysoap/soapenvelope.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/__init__.py
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/alarmprovider.py
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/audiopauseprovider.py
+-rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/clockprovider.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/contextprovider.py
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/metricprovider.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/nomenclature.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/operationprovider.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/patientcontextprovider.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/product.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/roles/providerbase.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/__init__.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/components.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/manipulator.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/operations.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/request_handler_deferred.py
+-rw-r--r--   0        0        0    31894 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/sdcclientimpl.py
+-rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/subscription.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/contextservice.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/descriptioneventservice.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/getservice.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/localizationservice.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/setservice.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/stateeventservice.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/waveformservice.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/__init__.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/components.py
+-rw-r--r--   0        0        0     9462 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/dpwshostedservice.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/intervaltimer.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/operations.py
+-rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/periodicreports.py
+-rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/sco.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/scopesfactory.py
+-rw-r--r--   0        0        0    24489 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/sdcdeviceimpl.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/servicesfactory.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/subscriptionmgr.py
+-rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/subscriptionmgr_async.py
+-rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/subscriptionmgr_base.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/waveforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py
+-rw-r--r--   0        0        0     8063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py
+-rw-r--r--   0        0        0     9209 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py
+-rw-r--r--   0        0        0    12513 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/localizationservice.py
+-rw-r--r--   0        0        0    11775 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/porttypebase.py
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/__init__.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/actions.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/addressing_types.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/basetypes.py
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/dataconverters.py
+-rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/dpws_types.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/eventing_types.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/ext_qnames.py
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/isoduration.py
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/mex_types.py
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/msg_qnames.py
+-rw-r--r--   0        0        0    27781 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/msg_types.py
+-rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/pm_qnames.py
+-rw-r--r--   0        0        0    58377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/pm_types.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/wsd_types.py
+-rw-r--r--   0        0        0    50747 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xml_types/xml_structure.py
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/BICEPS_MessageModel.xsd
+-rw-r--r--   0        0        0   205547 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/ExtensionPoint.xsd
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/MetadataExchange.xsd
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/SafetyInformation.xsd
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/addressing.xsd
+-rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/eventing.xsd
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/soap-envelope.xsd
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/ws-addr.xsd
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd
+-rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/wsdl.xsd
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/src/sdc11073/xsd/xml.xsd
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/tutorial/README.rst
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/README.rst
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a2/PKG-INFO
```

### Comparing `sdc11073-2.0.0a1/CHANGELOG.md` & `sdc11073-2.0.0a2/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 All notable changes to the sdc11073 module will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [master]
 
+## [2.0.0a2] - 2023-06-07
+
+### Fixed
+- fixed bug that mk_scopes only created a scope if a location was associated.
+- fixed broken fault message generation in subscriptionsmanager_base. A previously removed method of 
+namespace helper was still used. 
+- fixed bug in constructor of dpws_types.ThisDeviceType. This could cause an invalid xml:lang attribute. 
+- fixed bug that ContainerBase.node was not set in update_from_node
+
 ## [2.0.0a1] - 2023-06-01
 
 ### Changed
 - Code follows PEP8 style (mostly)
 - Using dependency injection, classes are defined in sdcdevice/components.py and sdcclients/components.py.
 This allows users to replace components withs own ones and modify the behavior of client and device.
 - All QNames of BICEPS participant model, message model and extension are predefined in
```

### Comparing `sdc11073-2.0.0a1/docs/sdc_social_preview.jpg` & `sdc11073-2.0.0a2/docs/sdc_social_preview.jpg`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/certloader.py` & `sdc11073-2.0.0a2/src/sdc11073/certloader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/commlog.py` & `sdc11073-2.0.0a2/src/sdc11073/commlog.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/definitions_base.py` & `sdc11073-2.0.0a2/src/sdc11073/definitions_base.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/definitions_sdc.py` & `sdc11073-2.0.0a2/src/sdc11073/definitions_sdc.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/etc.py` & `sdc11073-2.0.0a2/src/sdc11073/etc.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/exceptions.py` & `sdc11073-2.0.0a2/src/sdc11073/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/location.py` & `sdc11073-2.0.0a2/src/sdc11073/location.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/loghelper.py` & `sdc11073-2.0.0a2/src/sdc11073/loghelper.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/multikey.py` & `sdc11073-2.0.0a2/src/sdc11073/multikey.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/namespaces.py` & `sdc11073-2.0.0a2/src/sdc11073/namespaces.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/schema_resolver.py` & `sdc11073-2.0.0a2/src/sdc11073/schema_resolver.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/wsdiscovery.py` & `sdc11073-2.0.0a2/src/sdc11073/wsdiscovery.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/dispatch/dispatchkey.py` & `sdc11073-2.0.0a2/src/sdc11073/dispatch/dispatchkey.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/dispatch/messageconverter.py` & `sdc11073-2.0.0a2/src/sdc11073/dispatch/messageconverter.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/dispatch/pathelementregistry.py` & `sdc11073-2.0.0a2/src/sdc11073/dispatch/pathelementregistry.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/dispatch/request.py` & `sdc11073-2.0.0a2/src/sdc11073/dispatch/request.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/httpserver/compression.py` & `sdc11073-2.0.0a2/src/sdc11073/httpserver/compression.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/httpserver/httpreader.py` & `sdc11073-2.0.0a2/src/sdc11073/httpserver/httpreader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/httpserver/httprequesthandler.py` & `sdc11073-2.0.0a2/src/sdc11073/httpserver/httprequesthandler.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/httpserver/httpserverimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/httpserver/httpserverimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/clientmdib.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/clientmdib.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,28 @@
     """Contains a single Value"""
     value_string: str
     determination_time: float
     validity: Enum
     annotations: list
 
     @property
-    def value(self):
+    def value(self) -> float:
+        """Returns the value of the Sample as float"""
         return float(self.value_string)
 
     @property
-    def dec_value(self):
+    def dec_value(self) -> Decimal:
+        """Returns the value of the Sample as Decimal"""
         return Decimal(self.value_string)
 
+    @property
+    def age(self) -> float:
+        """Returns the age of the Sample in seconds"""
+        return time.time() - self.determination_time
+
     def __repr__(self):
         return f'RtSample value="{self.value_string}" validity="{self.validity}" time={self.determination_time}'
 
 
 class ClientRtBuffer:
     """Collects data of one real time stream."""
```

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/clientmdibxtra.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/clientmdibxtra.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/containerbase.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/containerbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import inspect
-from typing import Optional, List
+from typing import Optional, List, Union
 
 from lxml import etree as etree_
 
 from .. import observableproperties as properties
 from ..namespaces import QN_TYPE, NamespaceHelper
 
 
@@ -16,19 +16,19 @@
     # every class with container properties must provide a list of property names.
     # this list is needed to create sub elements in a certain order.
     # rule is : elements are sorted from this root class to derived class. Last derived class comes last.
     # Initialization is from left to right
     # This is according to the inheritance in BICEPS xml schema
 
     def __init__(self):
-        self.node = None
+        self.node: Optional[etree_.Element] = None  # set in update_from_node
         for dummy_name, cprop in self.sorted_container_properties():
             cprop.init_instance_data(self)
 
-    def get_actual_value(self, attr_name):
+    def get_actual_value(self, attr_name: str):
         """ ignores default value and implied value, e.g. returns None if value is not present in xml"""
         return getattr(self.__class__, attr_name).get_actual_value(self)
 
     def mk_node(self, tag:etree_.QName, ns_helper: NamespaceHelper, set_xsi_type: bool=False):
         """
         create an etree node from instance data
         :param tag: tag of the newly created node
@@ -53,20 +53,21 @@
         """
         if set_xsi_type and self.NODETYPE is not None:
             node.set(QN_TYPE, ns_helper.doc_name_from_qname(self.NODETYPE))
         for dummy_name, prop in self.sorted_container_properties():
             prop.update_xml_value(self, node)
         return node
 
-    def update_from_node(self, node):
+    def update_from_node(self, node: etree_.Element):
         """ update members.
         :param node: node to be updated
         """
         for dummy_name, cprop in self.sorted_container_properties():
             cprop.update_from_node(self, node)
+        self.node = node
 
     def _update_from_other(self, other_container, skipped_properties):
         # update all ContainerProperties
         if skipped_properties is None:
             skipped_properties = []
         for prop_name, _ in self.sorted_container_properties():
             if prop_name not in skipped_properties:
@@ -75,15 +76,15 @@
 
     def mk_copy(self, copy_node=True):
         copied = copy.copy(self)
         if copy_node:
             copied.node = copy.deepcopy(self.node)
         return copied
 
-    def sorted_container_properties(self):
+    def sorted_container_properties(self) -> list:
         """
         :return: a list of (name, object) tuples of all GenericProperties ( and subclasses), base class properties first.
         """
         ret = []
         all_classes = inspect.getmro(self.__class__)
         for cls in reversed(all_classes):
             try:
@@ -92,15 +93,15 @@
                 continue
             for name in names:
                 obj = getattr(cls, name)
                 if obj is not None:
                     ret.append((name, obj))
         return ret
 
-    def diff(self, other, ignore_property_names: Optional[List[str]]=None):
+    def diff(self, other, ignore_property_names: Optional[List[str]]=None) -> Union[None, str]:
         """ compares all properties (except to be ignored ones).
         :param other: the object to compare with
         :param ignore_property_names: list of properties that shall be excluded from diff calculation
         :return: textual representation of differences or None if equal
         """
         ret = []
         ignore_list = ignore_property_names or []
@@ -128,9 +129,9 @@
         my_property_names = {p[0] for p in my_properties}  # set comprehension
         other_property_names = {p[0] for p in other.sorted_container_properties()}
         surplus_names = other_property_names - my_property_names
         if surplus_names:
             ret.append(f'other has more data elements:{surplus_names}')
         return None if len(ret) == 0 else ret
 
-    def is_equal(self, other):
+    def is_equal(self, other) -> bool:
         return len(self.diff(other)) == 0
```

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/descriptorcontainers.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/descriptorcontainers.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/devicemdib.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/devicemdib.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/devicemdibxtra.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/devicemdibxtra.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/devicewaveform.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/devicewaveform.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/mdibbase.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/mdibbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/statecontainers.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/statecontainers.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/mdib/transactions.py` & `sdc11073-2.0.0a2/src/sdc11073/mdib/transactions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/netconn/__init__.py` & `sdc11073-2.0.0a2/src/sdc11073/netconn/__init__.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/observableproperties/observables.py` & `sdc11073-2.0.0a2/src/sdc11073/observableproperties/observables.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/observableproperties/valuecollector.py` & `sdc11073-2.0.0a2/src/sdc11073/observableproperties/valuecollector.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/pysoap/msgfactory.py` & `sdc11073-2.0.0a2/src/sdc11073/pysoap/msgfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/pysoap/msgreader.py` & `sdc11073-2.0.0a2/src/sdc11073/pysoap/msgreader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/pysoap/soapclient.py` & `sdc11073-2.0.0a2/src/sdc11073/pysoap/soapclient.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/pysoap/soapclient_async.py` & `sdc11073-2.0.0a2/src/sdc11073/pysoap/soapclient_async.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/pysoap/soapclientpool.py` & `sdc11073-2.0.0a2/src/sdc11073/pysoap/soapclientpool.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/pysoap/soapenvelope.py` & `sdc11073-2.0.0a2/src/sdc11073/pysoap/soapenvelope.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/alarmprovider.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/alarmprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/audiopauseprovider.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/audiopauseprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/clockprovider.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/clockprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/contextprovider.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/contextprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/metricprovider.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/metricprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/nomenclature.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/nomenclature.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/patientcontextprovider.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/patientcontextprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/product.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/product.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/roles/providerbase.py` & `sdc11073-2.0.0a2/src/sdc11073/roles/providerbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/components.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/components.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/manipulator.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/manipulator.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/operations.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/operations.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/request_handler_deferred.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/request_handler_deferred.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/sdcclientimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/sdcclientimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/subscription.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/subscription.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/contextservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/contextservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/getservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/getservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/localizationservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/localizationservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/setservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/setservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcclient/serviceclients/stateeventservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcclient/serviceclients/stateeventservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/components.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/components.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/dpwshostedservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/dpwshostedservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/intervaltimer.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/intervaltimer.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/operations.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/operations.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/periodicreports.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/periodicreports.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/sco.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/sco.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/scopesfactory.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/scopesfactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,38 +8,39 @@
     """ scopes factory
     This method creates the scopes for publishing in wsdiscovery.
     :param mdib:
     :return: wsdiscovery.Scope
     """
     pm_types = mdib.data_model.pm_types
     pm_names = mdib.data_model.pm_names
+    scope = ScopesType()
     locations = mdib.context_states.NODETYPE.get(pm_names.LocationContextState, [])
     assoc_loc = [l for l in locations if l.ContextAssociation == pm_types.ContextAssociation.ASSOCIATED]
     if len(assoc_loc) == 1:
         loc = assoc_loc[0]
         det = loc.LocationDetail
         dr_loc = SdcLocation(fac=det.Facility, poc=det.PoC, bed=det.Bed, bld=det.Building,
                              flr=det.Floor, rm=det.Room)
-        scope = ScopesType(dr_loc.scope_string)
+        scope.text.append(dr_loc.scope_string)
 
-        for nodetype, scheme in ((pm_names.OperatorContextDescriptor, 'sdc.ctxt.opr'),
-                                 (pm_names.EnsembleContextDescriptor, 'sdc.ctxt.ens'),
-                                 (pm_names.WorkflowContextDescriptor, 'sdc.ctxt.wfl'),
-                                 (pm_names.MeansContextDescriptor, 'sdc.ctxt.mns')):
-            descriptors = mdib.descriptions.NODETYPE.get(nodetype, [])
-            for descriptor in descriptors:
-                states = mdib.context_states.descriptorHandle.get(descriptor.Handle, [])
-                assoc_st = [s for s in states if s.ContextAssociation == pm_types.ContextAssociation.ASSOCIATED]
-                for state in assoc_st:
-                    for ident in state.Identification:
-                        scope.text.append(f'{scheme}:/{quote_plus(ident.Root)}/{quote_plus(ident.Extension)}')
+    for nodetype, scheme in ((pm_names.OperatorContextDescriptor, 'sdc.ctxt.opr'),
+                             (pm_names.EnsembleContextDescriptor, 'sdc.ctxt.ens'),
+                             (pm_names.WorkflowContextDescriptor, 'sdc.ctxt.wfl'),
+                             (pm_names.MeansContextDescriptor, 'sdc.ctxt.mns')):
+        descriptors = mdib.descriptions.NODETYPE.get(nodetype, [])
+        for descriptor in descriptors:
+            states = mdib.context_states.descriptorHandle.get(descriptor.Handle, [])
+            assoc_st = [s for s in states if s.ContextAssociation == pm_types.ContextAssociation.ASSOCIATED]
+            for state in assoc_st:
+                for ident in state.Identification:
+                    scope.text.append(f'{scheme}:/{quote_plus(ident.Root)}/{quote_plus(ident.Extension)}')
 
-        scope.text.extend(_get_device_component_based_scopes(mdib))
-        scope.text.append('sdc.mds.pkp:1.2.840.10004.20701.1.1')  # key purpose Service provider
-        return scope
+    scope.text.extend(_get_device_component_based_scopes(mdib))
+    scope.text.append('sdc.mds.pkp:1.2.840.10004.20701.1.1')  # key purpose Service provider
+    return scope
 
 
 def _get_device_component_based_scopes(mdib):
     """
     SDC: For every instance derived from pm:AbstractComplexDeviceComponentDescriptor in the MDIB an
     SDC SERVICE PROVIDER SHOULD include a URI-encoded pm:AbstractComplexDeviceComponentDescriptor/pm:Type
     as dpws:Scope of the MDPWS discovery messages. The URI encoding conforms to the given Extended Backus-Naur Form.
```

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/sdcdeviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/sdcdeviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/servicesfactory.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/servicesfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/subscriptionmgr.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/subscriptionmgr.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/subscriptionmgr_async.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/subscriptionmgr_async.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/subscriptionmgr_base.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/subscriptionmgr_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
     def on_unsubscribe_request(self, request_data: RequestData) -> CreatedMessage:
         subscription: SubscriptionBase = self._get_subscription_for_request(request_data)
         nsh = self.sdc_definitions.data_model.ns_helper
         if subscription is None:
             fault = Fault()
             fault.Code.Value = faultcodeEnum.RECEIVER
-            fault.set_sub_code(nsh.wseTag('InvalidMessage'))
+            fault.set_sub_code(nsh.WSE.tag('InvalidMessage'))
             fault.add_reason_text('unknown Subscription identifier')
             response = self._msg_factory.mk_reply_soap_message(request_data, fault, ns_map=[nsh.WSE])
         else:
             subscription.close()
             with self._subscriptions.lock:
                 self._subscriptions.remove_object(subscription)
             self._logger.info('unsubscribe: subscription found and removed {})', str(subscription))
@@ -387,15 +387,15 @@
         nsh = data_model.ns_helper
 
         self._logger.debug('on_get_status_request {}', lambda: request_data.message_data.p_msg.raw_data)
         subscription: SubscriptionBase = self._get_subscription_for_request(request_data)
         if subscription is None:
             fault = Fault()
             fault.Code.Value = faultcodeEnum.RECEIVER
-            fault.set_sub_code(nsh.wseTag('InvalidMessage'))
+            fault.set_sub_code(nsh.WSE.tag('InvalidMessage'))
             fault.add_reason_text('unknown Subscription identifier')
             response = self._msg_factory.mk_reply_soap_message(request_data, fault)
         else:
             get_status_response = evt_types.GetStatusResponse()
             get_status_response.Expires = subscription.remaining_seconds
             response = self._msg_factory.mk_reply_soap_message(request_data,
                                                                get_status_response)
@@ -406,15 +406,15 @@
         nsh = data_model.ns_helper
         renew = evt_types.Renew.from_node(request_data.message_data.p_msg.msg_node)
         expires = renew.Expires
         subscription: SubscriptionBase = self._get_subscription_for_request(request_data)
         if subscription is None:
             fault = Fault()
             fault.Code.Value = faultcodeEnum.RECEIVER
-            fault.set_sub_code(nsh.wseTag('InvalidMessage'))
+            fault.set_sub_code(nsh.WSE.tag('InvalidMessage'))
             fault.add_reason_text('unknown Subscription identifier')
             response = self._msg_factory.mk_reply_soap_message(request_data, fault)
         else:
             subscription.renew(expires)
             renew_response = evt_types.RenewResponse()
             renew_response.Expires = subscription.remaining_seconds
             response = self._msg_factory.mk_reply_soap_message(request_data, renew_response)
```

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/waveforms.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/waveforms.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/localizationservice.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/localizationservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/porttypebase.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/porttypebase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py` & `sdc11073-2.0.0a2/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/actions.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/actions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/addressing_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/addressing_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/basetypes.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/basetypes.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/dataconverters.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/dataconverters.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/dpws_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/dpws_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,21 @@
 
 
 class LocalizedStringType(ElementWithText):
     lang = cp.StringAttributeProperty(default_ns_helper.XML.tag('lang'))
     _props = ['lang']
 
     @classmethod
-    def init(cls, lang, text):
+    def init(cls, text: str, lang: Optional[str] = None):
+        """
+        This class represents the LocalizedStringType in DPWS.
+        :param text: the text
+        :param lang: if given, the actual language
+        :return:
+        """
         instance = cls()
         instance.lang = lang
         instance.text = text
         return instance
 
 
 class ThisDeviceType(XMLTypeBase):
@@ -91,18 +97,18 @@
                               If argument is a dictionary, it is expected to be key=language, value=name.
                               None as key marks the default name.
         :param firmware_version: any string
         :param serial_number: any string
         """
         super().__init__()
         if isinstance(friendly_name, str):
-            self.FriendlyName.append(LocalizedStringType.init('', friendly_name))
+            self.FriendlyName.append(LocalizedStringType.init(friendly_name))
         elif isinstance(friendly_name, LocalizedStringTypeDict):
             for lang, text in friendly_name.items():
-                self.FriendlyName.append(LocalizedStringType.init(lang, text))
+                self.FriendlyName.append(LocalizedStringType.init(text, lang))
         self.FirmwareVersion = firmware_version
         self.SerialNumber = serial_number
 
 
 class ThisModelType(XMLTypeBase):
     Manufacturer = cp.SubElementListProperty(default_ns_helper.DPWS.tag('Manufacturer'),
                                              value_class=LocalizedStringType)
@@ -119,21 +125,21 @@
                  manufacturer_url: Optional[str] = None,
                  model_name: Union[str, LocalizedStringTypeDict, None] = None,
                  model_number: Optional[str] = None,
                  model_url: Optional[str] = None,
                  presentation_url: Optional[str] = None):
         super().__init__()
         if isinstance(manufacturer, str):
-            self.Manufacturer.append(LocalizedStringType.init(None, manufacturer))
+            self.Manufacturer.append(LocalizedStringType.init(manufacturer))
         elif isinstance(manufacturer, LocalizedStringTypeDict):
-            for lang, value in manufacturer.items():
-                self.Manufacturer.append(LocalizedStringType.init(lang, value))
+            for lang, text in manufacturer.items():
+                self.Manufacturer.append(LocalizedStringType.init(text, lang))
         self.ManufacturerUrl = manufacturer_url
         if isinstance(model_name, str):
-            self.ModelName.append(LocalizedStringType.init(None, model_name))
+            self.ModelName.append(LocalizedStringType.init(model_name))
         elif isinstance(model_name, LocalizedStringTypeDict):
-            for lang, value in model_name.items():
-                self.ModelName.append(LocalizedStringType.init(lang, value))
+            for lang, text in model_name.items():
+                self.ModelName.append(LocalizedStringType.init(text, lang))
         self.ModelNumber = model_number
         self.ModelUrl = model_url
         self.PresentationUrl = presentation_url
```

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/eventing_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/eventing_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/isoduration.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/isoduration.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/mex_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/mex_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/msg_qnames.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/msg_qnames.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/msg_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/msg_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/pm_qnames.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/pm_qnames.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/pm_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/pm_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/wsd_types.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/wsd_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from . import xml_structure as struct
 from .basetypes import XMLTypeBase, MessageType, ElementWithTextList
 from .addressing_types import EndpointReferenceType
 from ..namespaces import default_ns_helper
+from typing import Optional
 
 ########## Meta Data Exchange #########
 wsa_tag = default_ns_helper.WSA.tag  # shortcut
 wsd_tag = default_ns_helper.WSD.tag  # shortcut
 
 class QNameListType(struct.NodeTextQNameListProperty):
     pass
 
 class ScopesType(ElementWithTextList):
     # text is a URI list
     MatchBy = struct.AnyURIAttributeProperty('MatchBy')
     _props = ['MatchBy']
 
-    def __init__(self, value=None, match_by=None):
+    def __init__(self, value: Optional[str] = None, match_by: Optional[str] = None):
         super().__init__()
-        if isinstance(value, str):
-            self.text = [value]
-        else:
-            self.text = value
+        if value is not None:
+            self.text.append(value)
         self.MatchBy = match_by
 
 
 class HelloType(MessageType):
     NODETYPE = wsd_tag('Hello')
     action = f'{default_ns_helper.WSD.namespace}/Hello'
     EndpointReference = struct.SubElementProperty(wsa_tag('EndpointReference'),
```

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xml_types/xml_structure.py` & `sdc11073-2.0.0a2/src/sdc11073/xml_types/xml_structure.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/BICEPS_MessageModel.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/BICEPS_MessageModel.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/ExtensionPoint.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/ExtensionPoint.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/MetadataExchange.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/MetadataExchange.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/SafetyInformation.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/SafetyInformation.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/addressing.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/addressing.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/eventing.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/eventing.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/soap-envelope.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/ws-addr.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/wsdl.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/src/sdc11073/xsd/xml.xsd` & `sdc11073-2.0.0a2/src/sdc11073/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/tutorial/README.rst` & `sdc11073-2.0.0a2/tutorial/README.rst`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/.gitignore` & `sdc11073-2.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/LICENSE` & `sdc11073-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/README.rst` & `sdc11073-2.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/pyproject.toml` & `sdc11073-2.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a1/PKG-INFO` & `sdc11073-2.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc11073
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Pure python implementation of IEEE11073 SDC protocol
 Project-URL: Homepage, https://github.com/Draegerwerk/sdc11073
 Project-URL: Bug Tracker, https://github.com/Draegerwerk/sdc11073/issues
 Author-email: Bernd Deichmann <bernd.deichmann@draeger.com>, Leon Budnick <leon.budnick@draeger.com>
 License-File: LICENSE
 Keywords: IEEE11073,SDC
 Classifier: Development Status :: 5 - Production/Stable
```

