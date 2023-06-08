# Comparing `tmp/pyakamai-1.0-py3-none-any.whl.zip` & `tmp/pyakamai-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 24717 bytes, number of entries: 19
+Zip file size: 24775 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      454 b- defN 23-May-01 03:11 pyakamai/__init__.py
 -rw-r--r--  2.0 unx     3821 b- defN 23-May-01 03:18 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     2332 b- defN 23-Apr-30 11:30 pyakamai/akamaicps.py
--rw-r--r--  2.0 unx     9215 b- defN 23-Apr-30 10:33 pyakamai/akamaidatastream.py
+-rw-r--r--  2.0 unx     9439 b- defN 23-Jun-08 00:37 pyakamai/akamaidatastream.py
 -rw-r--r--  2.0 unx     4408 b- defN 23-Apr-30 10:57 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     2843 b- defN 23-Apr-30 15:28 pyakamai/akamaiehn.py
 -rw-r--r--  2.0 unx    14193 b- defN 23-May-01 03:54 pyakamai/akamaiksd1.py
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Apr-30 11:42 pyakamai/akamailds.py
--rw-r--r--  2.0 unx     3850 b- defN 23-Apr-30 08:40 pyakamai/akamaimsl.py
--rw-r--r--  2.0 unx    27989 b- defN 23-Apr-30 08:41 pyakamai/akamaiproperty.py
+-rw-r--r--  2.0 unx     3878 b- defN 23-Jun-08 00:38 pyakamai/akamaimsl.py
+-rw-r--r--  2.0 unx    28281 b- defN 23-Jun-08 00:35 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
--rw-r--r--  2.0 unx     8058 b- defN 23-Apr-30 11:25 pyakamai/http_calls.py
--rw-r--r--  2.0 unx     2624 b- defN 23-May-01 03:12 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx      492 b- defN 23-May-02 04:32 pyakamai-1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 04:32 pyakamai-1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-02 04:32 pyakamai-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1493 b- defN 23-May-02 04:32 pyakamai-1.0.dist-info/RECORD
-19 files, 94984 bytes uncompressed, 22313 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx     8058 b- defN 23-May-12 02:25 pyakamai/http_calls.py
+-rw-r--r--  2.0 unx     2624 b- defN 23-Jun-08 00:08 pyakamai/pyakamai.py
+-rw-r--r--  2.0 unx      492 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1493 b- defN 23-Jun-08 00:38 pyakamai-1.1.dist-info/RECORD
+19 files, 95528 bytes uncompressed, 22371 bytes compressed:  76.6%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-1.0.dist-info/METADATA
+Filename: pyakamai-1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-1.0.dist-info/WHEEL
+Filename: pyakamai-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-1.0.dist-info/top_level.txt
+Filename: pyakamai-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-1.0.dist-info/RECORD
+Filename: pyakamai-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyakamai/akamaidatastream.py

```diff
@@ -35,183 +35,183 @@
         return None
     
     def listGroups(self):
         """ List the groups associated with the account """
         listGroupEndpoint = '/datastream-config-api/v1/log/groups'
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            groupList = self._prdHttpCaller.getResult(listGroupEndpoint,params)
+            status,groupList = self._prdHttpCaller.getResult(listGroupEndpoint,params)
         else:
-            groupList = self._prdHttpCaller.getResult(listGroupEndpoint)
+            status,groupList = self._prdHttpCaller.getResult(listGroupEndpoint)
         return(groupList)
 
     def listConnectors(self):
         """ List the type of connectors available with the datastream .
         Can use one of the connector types as a destination for log delivery in a data stream configuration"""
 
         listConnectorEndpoint = 'datastream-config-api/v1/log/connectors'
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            connectorList = self._prdHttpCaller.getResult(listConnectorEndpoint,params)
+            status,connectorList = self._prdHttpCaller.getResult(listConnectorEndpoint,params)
         else:
-            connectorList = self._prdHttpCaller.getResult(listConnectorEndpoint)
+            status,connectorList = self._prdHttpCaller.getResult(listConnectorEndpoint)
         return(connectorList)
 
     def listProducts(self):
         listProductEndpoint = 'datastream-config-api/v1/log/products'
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            productsList = self._prdHttpCaller.getResult(listProductEndpoint,params)
+            status,productsList = self._prdHttpCaller.getResult(listProductEndpoint,params)
         else:
-            productsList = self._prdHttpCaller.getResult(listProductEndpoint)
+            status,productsList = self._prdHttpCaller.getResult(listProductEndpoint)
         return(productsList)
 
     def listStreamTypes(self):
         """ List the type of streams available with the datastream."""
 
         listStreamTypeEndpoint = 'datastream-config-api/v1/log/streamTypes'
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            streamTypeList = self._prdHttpCaller.getResult(listStreamTypeEndpoint,params)
+            status,streamTypeList = self._prdHttpCaller.getResult(listStreamTypeEndpoint,params)
         else:
-            streamTypeList = self._prdHttpCaller.getResult(listStreamTypeEndpoint)
+            status,streamTypeList = self._prdHttpCaller.getResult(listStreamTypeEndpoint)
         return(streamTypeList)
 
     def listStreams(self,groupId):
         """ List the type of Streams available with the Group """
 
         listStreamsEndpoint = 'datastream-config-api/v1/log/streams'
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey,
                     'groupId':int(groupId)
                     }
-            streamList = self._prdHttpCaller.getResult(listStreamsEndpoint,params)
+            status,streamList = self._prdHttpCaller.getResult(listStreamsEndpoint,params)
         else:
-            streamList = self._prdHttpCaller.getResult(listStreamsEndpoint)
+            status,streamList = self._prdHttpCaller.getResult(listStreamsEndpoint)
         return(streamList)
 
     def listProperties(self,groupId,productId):
         """ List the type of Properties available with the Group """
 
         listPropertiesEndpoint = 'datastream-config-api/v1/log/properties/product/'+str(productId)+'/group/'+str(groupId)
 
         if self.accountSwitchKey:
             params = {
                         'accountSwitchKey':self.accountSwitchKey
                     }
-            propertiesList = self._prdHttpCaller.getResult(listPropertiesEndpoint,params)
+            status,propertiesList = self._prdHttpCaller.getResult(listPropertiesEndpoint,params)
         else:
-            propertiesList = self._prdHttpCaller.getResult(listPropertiesEndpoint)
+            status,propertiesList = self._prdHttpCaller.getResult(listPropertiesEndpoint)
         return(propertiesList)
 
 
     def listErrorStreams(self,groupId):
         """ List the type of Error Streams available with the Group """
         listErrorStreamsEndpoint = 'datastream-config-api/v1/log/error-streams/groups/' + str(groupId)
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            errorstreamList = self._prdHttpCaller.getResult(listErrorStreamsEndpoint,params)
+            status,errorstreamList = self._prdHttpCaller.getResult(listErrorStreamsEndpoint,params)
         else:
-            errorstreamList = self._prdHttpCaller.getResult(listErrorStreamsEndpoint)
+            status,errorstreamList = self._prdHttpCaller.getResult(listErrorStreamsEndpoint)
         return(errorstreamList)
 
     def getStream(self,streamId,version=None):
         """Get the Details of the Stream """
 
         if version:
             getStreamDetailEndpoint = '/datastream-config-api/v1/log/streams/' + str(streamId) + '/version/' + str(config.version)
         else:
             getStreamDetailEndpoint = '/datastream-config-api/v1/log/streams/' + str(streamId)
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            streamDetail = self._prdHttpCaller.getResult(getStreamDetailEndpoint,params)
+            status,streamDetail = self._prdHttpCaller.getResult(getStreamDetailEndpoint,params)
         else:
-            streamDetail = self._prdHttpCaller.getResult(getStreamDetailEndpoint)
+            status,streamDetail = self._prdHttpCaller.getResult(getStreamDetailEndpoint)
         return(streamDetail)
 
     def getStreamActHistory(self,streamId):
         streamActHistoryEndpoint = '/datastream-config-api/v1/log/streams/'+ str(streamId) + '/activationHistory'
 
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            streamActHistory = self._prdHttpCaller.getResult(streamActHistoryEndpoint,params)
+            status,streamActHistory = self._prdHttpCaller.getResult(streamActHistoryEndpoint,params)
         else:
-            streamActHistory = self._prdHttpCaller.getResult(streamActHistoryEndpoint)
+            status,streamActHistory = self._prdHttpCaller.getResult(streamActHistoryEndpoint)
         return(streamActHistory)
 
 
     def getStreamHistory(self,streamId):
         streamHistoryEndpoint = '/datastream-config-api/v1/log/streams/'+ str(streamId) + '/history'
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            streamHistory = self._prdHttpCaller.getResult(streamHistoryEndpoint,params)
+            status,streamHistory = self._prdHttpCaller.getResult(streamHistoryEndpoint,params)
         else:
-            streamHistory = self._prdHttpCaller.getResult(streamHistoryEndpoint)
+            status,streamHistory = self._prdHttpCaller.getResult(streamHistoryEndpoint)
         return(streamHistory)
 
     def getDatasets(self,templatename):
         datasetsEndpoint = '/datastream-config-api/v1/log/datasets/template/'+ templatename
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            datasetList = self._prdHttpCaller.getResult(datasetsEndpoint,params)
+            status,datasetList = self._prdHttpCaller.getResult(datasetsEndpoint,params)
         else:
-            datasetList = self._prdHttpCaller.getResult(datasetsEndpoint)
+            status,datasetList = self._prdHttpCaller.getResult(datasetsEndpoint)
         return(datasetList)
 
 
     def createStream(self,data):
         """ Create a Stream"""
         createEndpoint = '/datastream-config-api/v1/log/streams'
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            createResponse = self._prdHttpCaller.postResult(createEndpoint,data,params)
+            cstatus,reateResponse = self._prdHttpCaller.postResult(createEndpoint,data,params)
         else:
-            createResponse = self._prdHttpCaller.postResult(createEndpoint,data)
+            status,createResponse = self._prdHttpCaller.postResult(createEndpoint,data)
         return(createResponse)
 
     def updateStream(self,data,streamid):
         """ Update a Stream"""
         updateEndpoint = '/datastream-config-api/v1/log/streams/' + str(streamid)
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            updateResponse = self._prdHttpCaller.putResult(updateEndpoint,data,params)
+            status,updateResponse = self._prdHttpCaller.putResult(updateEndpoint,data,params)
         else:
-            updateResponse = self._prdHttpCaller.putResult(updateEndpoint,data)
+            status,updateResponse = self._prdHttpCaller.putResult(updateEndpoint,data)
         return(updateResponse)
 
 
     def activateStream(self,streamId):
         """ Activate a particular Datastream"""
         activateEndpoint = '/datastream-config-api/v1/log/streams/' + str(streamId) +'/activate/'
         data = {}
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            activateResponse = self._prdHttpCaller.putResult(activateEndpoint,data,params)
+            status,activateResponse = self._prdHttpCaller.putResult(activateEndpoint,data,params)
         else:
-            activateResponse = self._prdHttpCaller.putResult(activateEndpoint,data)
+            status,activateResponse = self._prdHttpCaller.putResult(activateEndpoint,data)
         return(activateResponse)
 
     def deActivateStream(self,streamId):
         """ Deactivate a particular stream"""
         deactivateEndpoint = '/datastream-config-api/v1/log/streams/' + str(streamId) +'/deactivate/'
         data = {}
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            deactivateResponse = self._prdHttpCaller.putResult(deactivateEndpoint,data,params)
+            status,deactivateResponse = self._prdHttpCaller.putResult(deactivateEndpoint,data,params)
         else:
-            deactivateResponse = self._prdHttpCaller.putResult(deactivateEndpoint,data)
+            status,deactivateResponse = self._prdHttpCaller.putResult(deactivateEndpoint,data)
         return(deactivateResponse)
 
     def deleteStream(self,streamId):
         """ Delete a particular stream"""
         deleteEndpoint = '/datastream-config-api/v1/log/streams/' + str(streamId)
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            deleteResponse = self._prdHttpCaller.deleteResult(deleteEndpoint,params)
+            status,deleteResponse = self._prdHttpCaller.deleteResult(deleteEndpoint,params)
         else:
-            deleteResponse = self._prdHttpCaller.deleteResult(deleteEndpoint)
+            status,deleteResponse = self._prdHttpCaller.deleteResult(deleteEndpoint)
         return(deleteResponse)
```

## pyakamai/akamaimsl.py

```diff
@@ -55,17 +55,17 @@
 
 
     def stream(self,streamId):
         self.id =  streamId
         mslInfoEndPoint = "/config-media-live/v2/msl-origin/streams/" + str(streamId)
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
-            msl_info = self._prdHttpCaller.getResult(mslInfoEndPoint,params)
+            status,msl_info = self._prdHttpCaller.getResult(mslInfoEndPoint,params)
         else:
-            msl_info = self._prdHttpCaller.getResult(mslInfoEndPoint)
+            status,msl_info = self._prdHttpCaller.getResult(mslInfoEndPoint)
         self.name = msl_info['name']
         self.format = msl_info['format']
         self.cpcode = msl_info['cpcode']
         self.ingestAccelerated = msl_info['ingestAccelerated']
         if 'dvrWindow' in msl_info:
             self.dvrWindow = msl_info['dvrWindow']
         self.encoderZone = msl_info['encoderZone']
@@ -94,12 +94,12 @@
 
     def updateStream(self,jsondata):
         if self.provisionStatus == 'PROVISIONED':
             streamUpdateEndpoint = '/config-media-live/v2/msl-origin/streams/' + str(self.id)
             if self.accountSwitchKey:
                 params = {}
                 params["accountSwitchKey"] = self.accountSwitchKey
-                updateStreamJson = self._prdHttpCaller.putResult(streamUpdateEndpoint,jsondata,params)
+                status,updateStreamJson = self._prdHttpCaller.putResult(streamUpdateEndpoint,jsondata,params)
             else:
-                updateStreamJson = self._prdHttpCaller.putResult(streamUpdateEndpoint,jsondata)
+                status,updateStreamJson = self._prdHttpCaller.putResult(streamUpdateEndpoint,jsondata)
             print(updateStreamJson)
```

## pyakamai/akamaiproperty.py

```diff
@@ -64,19 +64,22 @@
     
     def config(self,name):
         self.name = name
         data = {}
         data['propertyName'] = name
         json_data = json.dumps(data)
         propertyInfoEndPoint = "/papi/v1/search/find-by-value"
+        print(json_data)
         if self.accountSwitchKey:
             params = {'accountSwitchKey':self.accountSwitchKey}
+            print(params)
             status,prop_info = self._prdHttpCaller.postResult(propertyInfoEndPoint,json_data,params)
         else:
             status,prop_info = self._prdHttpCaller.postResult(propertyInfoEndPoint,json_data)
+        #print(status,prop_info)
         if prop_info:
             if 'versions' in prop_info and 'items' in prop_info['versions'] and len(prop_info['versions']['items']) !=0:
                 self.propertyId = prop_info['versions']['items'][0]['propertyId']
                 self.contractId = prop_info['versions']['items'][0]['contractId']
                 self.groupId = prop_info['versions']['items'][0]['groupId']
                 for item in prop_info['versions']['items']:
                     if item["productionStatus"] == "ACTIVE":
@@ -86,20 +89,21 @@
 
                 propertyVersionEndPoint = "/papi/v1/properties/{}".format(self.propertyId)
                 newparams = {}
                 if self.accountSwitchKey:
                     newparams["accountSwitchKey"] = self.accountSwitchKey
 
                 if newparams:
-                    getpropInfoJson = self._prdHttpCaller.getResult(propertyVersionEndPoint,params)
+                    status,getpropInfoJson = self._prdHttpCaller.getResult(propertyVersionEndPoint,params)
                 else:
-                    getpropInfoJson = self._prdHttpCaller.getResult(propertyVersionEndPoint)
+                    status,getpropInfoJson = self._prdHttpCaller.getResult(propertyVersionEndPoint)
                 
                 if getpropInfoJson :
-                    self.latestVersion = getpropInfoJson['properties']['items'][0]['latestVersion']
+                    if 'latestVersion' in getpropInfoJson['properties']['items'][0].keys():
+                        self.latestVersion = getpropInfoJson['properties']['items'][0]['latestVersion']
                     self.assetId = getpropInfoJson['properties']['items'][0]['assetId']
 
             else:
                 print("No Configuration with {} Found".format(name))
                 self._invalidconfig = True
         return None
 
@@ -138,15 +142,15 @@
                     'validateRules': 'false',
                     'validateMode': 'false',
                     'dryRun': 'true'
                     }
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
 
-        ruleTree = self._prdHttpCaller.getResult(ruleTreeEndPoint,params)
+        status,ruleTree = self._prdHttpCaller.getResult(ruleTreeEndPoint,params)
         return ruleTree
 
     def updateRuleTree(self,version,jsondata):
         if self._invalidconfig == True:
             print("No Configuration Found")
             return False
         updateRuleTreeEndPoint = '/papi/v1/properties/' + self.propertyId + '/versions/' + str(version) + '/rules'
@@ -171,15 +175,15 @@
         params = {}
         params["contractId"] =self.contractId
         params["groupId"] = self.groupId
 
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
 
-        getHostnameJson = self._prdHttpCaller.getResult(getHostNameEndPoint,params)
+        status,getHostnameJson = self._prdHttpCaller.getResult(getHostNameEndPoint,params)
         hostNameList = []
         for hostname in  getHostnameJson["hostnames"]["items"]:
             hostNameList.append(hostname["cnameFrom"])
         return hostNameList
 
 
     def createVersion(self,baseVersion):
@@ -316,17 +320,17 @@
             return []
 
         behaviorList = []
         getAvailableFeaturesEndPoint = "/papi/v1/properties/{propertyId}/versions/{propertyVersion}/available-behaviors".format(propertyId=self.propertyId,propertyVersion=version)
         params = {}
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
-            getFeaturesjson = self._prdHttpCaller.getResult(getAvailableFeaturesEndPoint,params)
+            status,getFeaturesjson = self._prdHttpCaller.getResult(getAvailableFeaturesEndPoint,params)
         else:
-            getFeaturesjson = self._prdHttpCaller.getResult(getAvailableFeaturesEndPoint)
+            status,getFeaturesjson = self._prdHttpCaller.getResult(getAvailableFeaturesEndPoint)
         for behaviors in getFeaturesjson["behaviors"]["items"]:
             behaviorList.append(behaviors["name"])
         return behaviorList
 
     def getUnusedBehaviors(self,version):
         if self._invalidconfig == True:
             print("No Configuration Found")
@@ -438,17 +442,17 @@
             return []
         version = self.getVersionofConfig()
 
         getVersionEP = "/papi/v1/properties/{propertyId}/versions".format(propertyId=self.propertyId)
         params = {}
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
-            getVersionsJson = self._prdHttpCaller.getResult(getVersionEP,params)
+            status,getVersionsJson = self._prdHttpCaller.getResult(getVersionEP,params)
         else:
-            getVersionsJson = self._prdHttpCaller.getResult(getVersionEP)
+            status,getVersionsJson = self._prdHttpCaller.getResult(getVersionEP)
         for versionItem in getVersionsJson["versions"]["items"]:
             if versionItem['propertyVersion'] == version:
                 return self.getMappings(versionItem['productId'])
         return 'Unknown Product'
 
 
     def insertRule(self,version,rule_dict,pos=0):
@@ -604,45 +608,45 @@
 
     def getGroups(self):
         groupsList = []
         ep = "/papi/v1/groups"
         params = {}
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
-            getgroupJson = self._prdHttpCaller.getResult(ep,params)
+            status,getgroupJson = self._prdHttpCaller.getResult(ep,params)
         else:
-            getgroupJson = self._prdHttpCaller.getResult(ep)
+            status,getgroupJson = self._prdHttpCaller.getResult(ep)
         print(getgroupJson)
         for items in getgroupJson["groups"]["items"]:
             groupsList.append(items["groupId"])
         return groupsList
 
     def getContracts(self):
         contractsList = []
         ep = "/papi/v1/contracts"
         params = {}
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
-            getcontractJson = self._prdHttpCaller.getResult(ep,params)
+            status,getcontractJson = self._prdHttpCaller.getResult(ep,params)
         else:
-            getcontractJson = self._prdHttpCaller.getResult(ep)
+            status,getcontractJson = self._prdHttpCaller.getResult(ep)
         for items in getcontractJson["contracts"]["items"]:
             contractsList.append(items["contractId"])
         return contractsList
 
     def listCPCodes(self,contract_id,group_id):
         cpCodeList = []
         ep = '/papi/v1/cpcodes'
         params = {}
         params['contractId'] = contract_id
         params['groupId'] = group_id
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
         try:
-            getcpCodesJson = self._prdHttpCaller.getResult(ep,parameters=params)
+            status,getcpCodesJson = self._prdHttpCaller.getResult(ep,parameters=params)
             for items in getcpCodesJson["cpcodes"]["items"]:
                 cpCodeList.append(items["cpcodeId"])
         except Exception as e:
             return []
         return cpCodeList
 
     def getPropertiesofGroup(self,contractid,groupid):
@@ -650,15 +654,15 @@
         params = {}
         params['contractId'] = contractid
         params['groupId'] = groupid
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
         
         try: 
-            getpropertiesJson = self._prdHttpCaller.getResult(ep,parameters=params)
+            status,getpropertiesJson = self._prdHttpCaller.getResult(ep,parameters=params)
             propList = []
             if len(getpropertiesJson['properties']['items']) != 0:
                 for prop in getpropertiesJson['properties']['items']:
                     propList.append(prop['propertyName'])
             return propList
 
         except Exception as e:
@@ -709,15 +713,15 @@
     def getCustomBehaviors(self):
         cbList = {}
         ep = '/papi/v1/custom-behaviors'
         params = {}
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
         try:
-            getcbJson = self._prdHttpCaller.getResult(ep,parameters=params)
+            status,getcbJson = self._prdHttpCaller.getResult(ep,parameters=params)
             for item in getcbJson["customBehaviors"]["items"]:                
                 cbList[item['name']] =  item['behaviorId']
             return cbList
         except Exception as e:
             print('Exception:',e)
             return []
 
@@ -725,15 +729,15 @@
     def getCustomOverrides(self):
         coList = {}
         ep = '/papi/v1/custom-overrides'
         params = {}
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
         try:
-            getcoJson = self._prdHttpCaller.getResult(ep,parameters=params)
+            status,getcoJson = self._prdHttpCaller.getResult(ep,parameters=params)
             for items in getcoJson["customOverrides"]["items"]:
                 coList[items['name']] =  items['overrideId']
             return coList
         except Exception as e:
             print('Exception:',e)
             return []
```

## pyakamai/http_calls.py

```diff
@@ -48,18 +48,19 @@
         if self.verbose: print (">>>\n" + json.dumps(endpoint_result.json(), indent=2) + "\n<<<\n")
         status = endpoint_result.status_code
         if self.verbose: print( "LOG: GET %s %s %s" % (endpoint,status,endpoint_result.headers["content-type"]))
         self.httpErrors(endpoint_result.status_code, path, endpoint_result.json())
         return status,endpoint_result.json()
 
 
-    def postResult(self, endpoint, body, headers=None,params=None):
+    def postResult(self, endpoint, body,params=None,headers=None):
         """ Executes a GET API call and returns the JSON output """
         if headers == None:
             headers = {'content-type': 'application/json'}
+
         path = endpoint
         endpoint_result = self.session.post(parse.urljoin(self.baseurl, path), data=body, headers=headers, params=params)
         status = endpoint_result.status_code
         if self.verbose:
             print("LOG: POST %s %s %s" % (path, status, endpoint_result.headers["content-type"]))
         if status == 204:
             return status,{}
```

## Comparing `pyakamai-1.0.dist-info/RECORD` & `pyakamai-1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 pyakamai/__init__.py,sha256=JER0abqNyr-F_5XlBsXxh3NEbppAZa4pygHLoBmtMEU,454
 pyakamai/akamaicasemanagement.py,sha256=DcNQenKNSNpW4buRbb6kQPMMymyteiKTbBT165i12SE,3821
 pyakamai/akamaicpcode.py,sha256=yQ31HE7krGBo_7tn8iGBwt0UtBHMM-wnTP33hwsamiI,1473
 pyakamai/akamaicps.py,sha256=6WOARWxWlkauMawOH4BE2-VJKdMgpqKdtcX8TXLKIgs,2332
-pyakamai/akamaidatastream.py,sha256=Y4Jxda5yMeUGr_fgUmGUt2fg-Ieqz1XgKUpYg1feXW4,9215
+pyakamai/akamaidatastream.py,sha256=TaU8glzaoiZMdwk3n1vdzsOKAP1nWhfEBQSz0lki9F8,9439
 pyakamai/akamaiedns.py,sha256=ROh3xQjOxalGnya97FyxE-iYZgZniD8GAGH1mhwjvRs,4408
 pyakamai/akamaiehn.py,sha256=aZ2U6YG54IKP5vuQPd5GygalsJqVuEzvCnALjjszRFI,2843
 pyakamai/akamaiksd1.py,sha256=7RslIDB6oR3KA4nyC7infxXqH4Jr7dM0t3znyDfCUPI,14193
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
-pyakamai/akamaimsl.py,sha256=vhs1DOuooLTdCZIiZTdmVE1Vmtc3fWCPtHn8YHnIapk,3850
-pyakamai/akamaiproperty.py,sha256=Kq4ota0auspXf75HAxLnFS1x4Y_OohtEN1HkZ9-ifRE,27989
+pyakamai/akamaimsl.py,sha256=ykRv_yy-qVWs37Wu2auDddX4IEuSWiO-1g9p59LTYww,3878
+pyakamai/akamaiproperty.py,sha256=mUgCU9GJ-o3A1um8T55_ihS37K9DrIgqLI-RxD-PANo,28281
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
-pyakamai/http_calls.py,sha256=yWCk3NZMJtjSFfiiswwyOA9nCAT-cwQCuHoUlQCkWE4,8058
+pyakamai/http_calls.py,sha256=vH5oWXTuMtSq64crAycijH5EFQC-9QAQf--Da-qlS-I,8058
 pyakamai/pyakamai.py,sha256=xqX5Ms9Rcl4qTxkvpI5tm_AUI0qgIEyf0Jda6b-gP9c,2624
-pyakamai-1.0.dist-info/METADATA,sha256=6nc2xVhqB26LallyOFXK2HvMmd7iMq_C_2-m6h_4lx8,492
-pyakamai-1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyakamai-1.0.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-1.0.dist-info/RECORD,,
+pyakamai-1.1.dist-info/METADATA,sha256=it82c6r3vdR2hfuJtwR0LbjxC3FsqNjLyHJPVtK2_Wk,492
+pyakamai-1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyakamai-1.1.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-1.1.dist-info/RECORD,,
```

