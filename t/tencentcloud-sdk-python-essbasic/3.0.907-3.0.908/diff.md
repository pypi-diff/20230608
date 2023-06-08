# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.907.tar", last modified: Tue Jun  6 02:26:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.908.tar", last modified: Wed Jun  7 00:24:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.907.tar` & `tencentcloud-sdk-python-essbasic-3.0.908.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16533 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51478 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   232146 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:26:52.000000 tencentcloud-sdk-python-essbasic-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51478 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   233553 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:24:17.000000 tencentcloud-sdk-python-essbasic-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.907'
+__version__ = '3.0.908'
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20210526/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,21 +87,21 @@
 class ApproverRestriction(AbstractModel):
     """指定签署人限制项
 
     """
 
     def __init__(self):
         r"""
-        :param Name: 指定签署人名字
+        :param Name: 指定签署人姓名
         :type Name: str
-        :param Mobile: 指定签署人手机号
+        :param Mobile: 指定签署人手机号，11位数字
         :type Mobile: str
-        :param IdCardType: 指定签署人证件类型
+        :param IdCardType: 指定签署人证件类型，ID_CARD-身份证，HONGKONG_AND_MACAO-港澳居民来往内地通行证，HONGKONG_MACAO_AND_TAIWAN-港澳台居民居住证
         :type IdCardType: str
-        :param IdCardNumber: 指定签署人证件号码
+        :param IdCardNumber: 指定签署人证件号码，其中字母大写
         :type IdCardNumber: str
         """
         self.Name = None
         self.Mobile = None
         self.IdCardType = None
         self.IdCardNumber = None
 
@@ -123,17 +123,17 @@
 class AuthFailMessage(AbstractModel):
     """授权出错信息
 
     """
 
     def __init__(self):
         r"""
-        :param ProxyOrganizationOpenId: 合作企业Id
+        :param ProxyOrganizationOpenId: 第三方应用平台的子客企业OpenId
         :type ProxyOrganizationOpenId: str
-        :param Message: 出错信息
+        :param Message: 错误信息
         :type Message: str
         """
         self.ProxyOrganizationOpenId = None
         self.Message = None
 
 
     def _deserialize(self, params):
@@ -151,15 +151,15 @@
 class AuthorizedUser(AbstractModel):
     """授权用户
 
     """
 
     def __init__(self):
         r"""
-        :param OpenId: 用户openid
+        :param OpenId: 第三方应用平台的用户openid
         :type OpenId: str
         """
         self.OpenId = None
 
 
     def _deserialize(self, params):
         self.OpenId = params.get("OpenId")
@@ -181,23 +181,23 @@
         r"""
         :param FlowName: 合同流程名称
         :type FlowName: str
         :param FlowType: 合同流程类型
         :type FlowType: str
         :param FlowDescription: 合同流程描述信息
         :type FlowDescription: str
-        :param Deadline: 合同流程截止时间，unix时间戳
+        :param Deadline: 合同流程截止时间，unix时间戳，单位秒
         :type Deadline: int
         :param Unordered: 是否顺序签署(true:无序签,false:顺序签)
         :type Unordered: bool
-        :param IntelligentStatus: 打开智能添加填写区(默认开启，打开:"OPEN" 关闭："CLOSE")
+        :param IntelligentStatus: 是否打开智能添加填写区(默认开启，打开:"OPEN" 关闭："CLOSE")
         :type IntelligentStatus: str
         :param FormFields: 填写控件内容
         :type FormFields: list of FormField
-        :param NeedSignReview: 本企业(发起方企业)是否需要签署审批，true：开启本企业签署审批
+        :param NeedSignReview: 本企业(发起方企业)是否需要签署审批，true：开启本企业签署审批。使用ChannelCreateFlowSignReview接口提交审批结果，才能继续完成签署
         :type NeedSignReview: bool
         :param UserData: 用户流程自定义数据参数
         :type UserData: str
         :param CcInfos: 抄送人信息
         :type CcInfos: list of CcInfo
         :param NeedCreateReview: 是否需要发起前审核，当指定NeedCreateReview=true，则发起后，需要使用接口：ChannelCreateFlowSignReview，来完成发起前审核，审核通过后，可以继续查看，签署合同
         :type NeedCreateReview: bool
@@ -2762,15 +2762,15 @@
 class CreateFlowOption(AbstractModel):
     """创建合同配置信息
 
     """
 
     def __init__(self):
         r"""
-        :param CanEditFlow: 是否允许修改合同信息
+        :param CanEditFlow: 是否允许修改合同信息，true-是，false-否
         :type CanEditFlow: bool
         """
         self.CanEditFlow = None
 
 
     def _deserialize(self, params):
         self.CanEditFlow = params.get("CanEditFlow")
@@ -3583,26 +3583,26 @@
     def __init__(self):
         r"""
         :param Type: 扩展服务类型
   AUTO_SIGN             企业静默签（自动签署）
   OVERSEA_SIGN          企业与港澳台居民*签署合同
   MOBILE_CHECK_APPROVER 使用手机号验证签署方身份
   PAGING_SEAL           骑缝章
-  DOWNLOAD_FLOW         授权渠道下载合同 
+  DOWNLOAD_FLOW         授权平台企业下载合同 
         :type Type: str
         :param Name: 扩展服务名称 
         :type Name: str
         :param Status: 服务状态 
 ENABLE 开启 
 DISABLE 关闭
         :type Status: str
-        :param OperatorOpenId: 最近操作人openid（经办人openid）
+        :param OperatorOpenId: 最近操作人第三方应用平台的用户openid
 注意：此字段可能返回 null，表示取不到有效值。
         :type OperatorOpenId: str
-        :param OperateOn: 最近操作时间
+        :param OperateOn: 最近操作时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type OperateOn: int
         """
         self.Type = None
         self.Name = None
         self.Status = None
         self.OperatorOpenId = None
@@ -3721,15 +3721,15 @@
 RELIEVED 已经解除
 
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveStatus: str
         :param ApproveMessage: 签署人信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveMessage: str
-        :param ApproveTime: 签署人签署时间
+        :param ApproveTime: 签署人签署时间戳，单位秒
         :type ApproveTime: int
         :param ApproveType: 参与者类型 (ORGANIZATION企业/PERSON个人)
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApproveType: str
         """
         self.ReceiptId = None
         self.ProxyOrganizationOpenId = None
@@ -3807,26 +3807,26 @@
 PERSON-个人/自然人；
 PERSON_AUTO_SIGN-个人自动签（定制化场景下使用）；
 ORGANIZATION-企业（企业签署方或模板发起时的企业静默签）；
 ENTERPRISESERVER-企业静默签（文件发起时的企业静默签字）。
         :type ApproverType: str
         :param RecipientId: 签署流程签署人在模板中对应的签署人Id；在非单方签署、以及非B2C签署的场景下必传，用于指定当前签署方在签署流程中的位置；
         :type RecipientId: str
-        :param Deadline: 签署截止时间，默认一年
+        :param Deadline: 签署截止时间戳，默认一年
         :type Deadline: int
         :param CallbackUrl: 签署完回调url，最大长度1000个字符
         :type CallbackUrl: str
         :param SignComponents: 使用PDF文件直接发起合同时，签署人指定的签署控件
         :type SignComponents: list of Component
         :param ComponentLimitType: 个人签署方指定签署控件类型，目前支持：OCR_ESIGN -AI智慧手写签名
 HANDWRITE -手写签名
         :type ComponentLimitType: list of str
         :param PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
-        :param JumpUrl: 签署完前端跳转的url，暂未使用
+        :param JumpUrl: 签署完前端跳转的url，此字段的用法场景请联系客户经理确认
         :type JumpUrl: str
         :param ApproverOption: 签署人个性化能力值
         :type ApproverOption: :class:`tencentcloud.essbasic.v20210526.models.ApproverOption`
         :param ApproverNeedSignReview: 当前签署方进行签署操作是否需要企业内部审批，true 则为需要
         :type ApproverNeedSignReview: bool
         :param ApproverVerifyTypes: 签署人查看合同时认证方式, 1-实名查看 2-短信验证码查看(企业签署方不支持该方式) 如果不传默认为1
 查看合同的认证方式 Flow层级的优先于approver层级的
@@ -3957,17 +3957,17 @@
 DEADLINE 流签
 CANCEL 取消
 RELIEVED 解除
  
         :type FlowStatus: str
         :param FlowMessage: 合同(流程)的信息
         :type FlowMessage: str
-        :param CreateOn: 合同(流程)的创建时间戳
+        :param CreateOn: 合同(流程)的创建时间戳，单位秒
         :type CreateOn: int
-        :param DeadLine: 合同(流程)的签署截止时间戳
+        :param DeadLine: 合同(流程)的签署截止时间戳，单位秒
         :type DeadLine: int
         :param CustomData: 用户自定义数据
         :type CustomData: str
         :param FlowApproverInfos: 合同(流程)的签署人数组
         :type FlowApproverInfos: list of FlowApproverDetail
         :param CcInfos: 合同(流程)关注方信息列表
         :type CcInfos: list of FlowApproverDetail
@@ -4338,15 +4338,15 @@
         r"""
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
 SELECTOR - 选项值
-DYNAMIC_TABLE - 传入json格式的表格内容，具体见数据结构FlowInfo：https://cloud.tencent.com/document/api/1420/61525#FlowInfo
+DYNAMIC_TABLE - 传入json格式的表格内容，具体见数据结构FlowInfo
         :type ComponentValue: str
         :param ComponentId: 表单域或控件的ID，跟ComponentName二选一，不能全为空；
 CreateFlowsByTemplates 接口不使用此字段。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ComponentId: str
         :param ComponentName: 控件的名字，跟ComponentId二选一，不能全为空
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4507,28 +4507,28 @@
 
     def __init__(self):
         r"""
         :param SealId: 电子印章编号
         :type SealId: str
         :param SealName: 电子印章名称
         :type SealName: str
-        :param CreateOn: 电子印章授权时间戳
+        :param CreateOn: 电子印章授权时间戳，单位秒
         :type CreateOn: int
-        :param Creator: 电子印章授权人
+        :param Creator: 电子印章授权人，电子签的UserId
         :type Creator: str
         :param SealPolicyId: 电子印章策略Id
         :type SealPolicyId: str
         :param SealStatus: 印章状态，有以下六种：CHECKING（审核中）SUCCESS（已启用）FAIL（审核拒绝）CHECKING-SADM（待超管审核）DISABLE（已停用）STOPPED（已终止）
         :type SealStatus: str
         :param FailReason: 审核失败原因
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailReason: str
         :param Url: 印章图片url，5分钟内有效
         :type Url: str
-        :param SealType: 印章类型
+        :param SealType: 印章类型，OFFICIAL-企业公章，CONTRACT-合同专用章，LEGAL_PERSON_SEAL-法人章
         :type SealType: str
         :param IsAllTime: 用印申请是否为永久授权
         :type IsAllTime: bool
         :param AuthorizedUsers: 授权人列表
         :type AuthorizedUsers: list of AuthorizedUser
         """
         self.SealId = None
@@ -4675,36 +4675,36 @@
 
     """
 
     def __init__(self):
         r"""
         :param OrganizationOpenId: 用户在渠道的机构编号
         :type OrganizationOpenId: str
-        :param ClientIp: 用户真实的IP
-        :type ClientIp: str
-        :param ProxyIp: 机构的代理IP
-        :type ProxyIp: str
         :param OrganizationId: 机构在平台的编号
         :type OrganizationId: str
         :param Channel: 用户渠道
         :type Channel: str
+        :param ClientIp: 用户真实的IP
+        :type ClientIp: str
+        :param ProxyIp: 机构的代理IP
+        :type ProxyIp: str
         """
         self.OrganizationOpenId = None
-        self.ClientIp = None
-        self.ProxyIp = None
         self.OrganizationId = None
         self.Channel = None
+        self.ClientIp = None
+        self.ProxyIp = None
 
 
     def _deserialize(self, params):
         self.OrganizationOpenId = params.get("OrganizationOpenId")
-        self.ClientIp = params.get("ClientIp")
-        self.ProxyIp = params.get("ProxyIp")
         self.OrganizationId = params.get("OrganizationId")
         self.Channel = params.get("Channel")
+        self.ClientIp = params.get("ClientIp")
+        self.ProxyIp = params.get("ProxyIp")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4719,35 +4719,35 @@
         r"""
         :param VerifyResult: 验签结果。0-签名域未签名；1-验签成功； 3-验签失败；4-未找到签名域：文件内没有签名域；5-签名值格式不正确。
         :type VerifyResult: int
         :param SignPlatform: 签署平台，如果文件是在腾讯电子签平台签署，则返回腾讯电子签，如果文件不在腾讯电子签平台签署，则返回其他平台。
         :type SignPlatform: str
         :param SignerName: 签署人名称
         :type SignerName: str
-        :param SignTime: 签署时间
+        :param SignTime: 签署时间戳，单位秒
         :type SignTime: int
         :param SignAlgorithm: 签名算法
         :type SignAlgorithm: str
         :param CertSn: 签名证书序列号
         :type CertSn: str
-        :param CertNotBefore: 证书起始时间
+        :param CertNotBefore: 证书起始时间戳，单位秒
         :type CertNotBefore: int
-        :param CertNotAfter: 证书过期时间
+        :param CertNotAfter: 证书过期时间戳，单位秒
         :type CertNotAfter: int
         :param SignType: 签名类型
         :type SignType: int
-        :param ComponentPosX: 签名域横坐标
+        :param ComponentPosX: 签名域横坐标，单位px
         :type ComponentPosX: float
-        :param ComponentPosY: 签名域纵坐标
+        :param ComponentPosY: 签名域纵坐标，单位px
         :type ComponentPosY: float
-        :param ComponentWidth: 签名域宽度
+        :param ComponentWidth: 签名域宽度，单位px
         :type ComponentWidth: float
-        :param ComponentHeight: 签名域高度
+        :param ComponentHeight: 签名域高度，单位px
         :type ComponentHeight: float
-        :param ComponentPage: 签名域所在页码
+        :param ComponentPage: 签名域所在页码，1～N
         :type ComponentPage: int
         """
         self.VerifyResult = None
         self.SignPlatform = None
         self.SignerName = None
         self.SignTime = None
         self.SignAlgorithm = None
@@ -4905,25 +4905,25 @@
 class Recipient(AbstractModel):
     """签署参与者信息
 
     """
 
     def __init__(self):
         r"""
-        :param RecipientId: 签署人唯一标识
+        :param RecipientId: 签署人唯一标识，在通过模板发起合同的时候对应签署方Id
         :type RecipientId: str
         :param RecipientType: 参与者类型。默认为空。ENTERPRISE-企业；INDIVIDUAL-个人；PROMOTER-发起方
         :type RecipientType: str
         :param Description: 描述
         :type Description: str
-        :param RoleName: 签署方备注信息
+        :param RoleName: 签署方备注角色名
         :type RoleName: str
-        :param RequireValidation: 是否需要校验
+        :param RequireValidation: 是否需要校验，true-是，false-否
         :type RequireValidation: bool
-        :param RequireSign: 是否必须填写
+        :param RequireSign: 是否必须填写，true-是，false-否
         :type RequireSign: bool
         :param SignType: 签署类型
         :type SignType: int
         :param RoutingOrder: 签署顺序：数字越小优先级越高
         :type RoutingOrder: int
         :param IsPromoter: 是否是发起方
         :type IsPromoter: bool
@@ -4974,14 +4974,15 @@
         r"""
         :param OrganizationName: 企业签署方工商营业执照上的企业名称，签署方为非发起方企业场景下必传，最大长度64个字符
         :type OrganizationName: str
         :param ApproverNumber: 签署人在原流程中的签署人列表中的顺序序号（从0开始，按顺序依次递增），如果不清楚原流程中的签署人列表，可以通过DescribeFlows接口查看
         :type ApproverNumber: int
         :param ApproverType: 签署人类型，目前仅支持
 ORGANIZATION-企业
+ENTERPRISESERVER-企业静默签
         :type ApproverType: str
         :param Name: 签署人姓名，最大长度50个字符
         :type Name: str
         :param IdCardType: 签署人身份证件类型
 1.ID_CARD 居民身份证
 2.HONGKONG_MACAO_AND_TAIWAN 港澳台居民居住证
 3.HONGKONG_AND_MACAO 港澳居民来往内地通行证
@@ -5069,19 +5070,19 @@
 class RemindFlowRecords(AbstractModel):
     """催办接口返回详细信息
 
     """
 
     def __init__(self):
         r"""
-        :param CanRemind: 是否能够催办
+        :param CanRemind: 是否能够催办，true-是，false-否
         :type CanRemind: bool
         :param FlowId: 合同id
         :type FlowId: str
-        :param RemindMessage: 催办详情
+        :param RemindMessage: 催办详情信息
         :type RemindMessage: str
         """
         self.CanRemind = None
         self.FlowId = None
         self.RemindMessage = None
 
 
@@ -5203,15 +5204,15 @@
     """
 
     def __init__(self):
         r"""
         :param SignUrl: 签署链接，过期时间为30天
 注意：此字段可能返回 null，表示取不到有效值。
         :type SignUrl: str
-        :param Deadline: 合同过期时间
+        :param Deadline: 合同过期时间戳，单位秒
 注意：此字段可能返回 null，表示取不到有效值。
         :type Deadline: int
         :param SignOrder: 当流程为顺序签署此参数有效时，数字越小优先级越高，暂不支持并行签署 可选
 注意：此字段可能返回 null，表示取不到有效值。
         :type SignOrder: int
         :param SignId: 签署人编号
 注意：此字段可能返回 null，表示取不到有效值。
@@ -5287,37 +5288,37 @@
 class Staff(AbstractModel):
     """企业员工信息
 
     """
 
     def __init__(self):
         r"""
-        :param UserId: 员工在电子签平台的id
+        :param UserId: 员工在电子签平台的用户ID
         :type UserId: str
         :param DisplayName: 显示的员工名
         :type DisplayName: str
         :param Mobile: 员工手机号
         :type Mobile: str
         :param Email: 员工邮箱
 注意：此字段可能返回 null，表示取不到有效值。
         :type Email: str
-        :param OpenId: 员工在第三方平台id
+        :param OpenId: 员工在第三方应用平台的用户ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type OpenId: str
         :param Roles: 员工角色
 注意：此字段可能返回 null，表示取不到有效值。
         :type Roles: list of StaffRole
         :param Department: 员工部门
 注意：此字段可能返回 null，表示取不到有效值。
         :type Department: :class:`tencentcloud.essbasic.v20210526.models.Department`
         :param Verified: 员工是否实名
         :type Verified: bool
-        :param CreatedOn: 员工创建时间戳
+        :param CreatedOn: 员工创建时间戳，单位秒
         :type CreatedOn: int
-        :param VerifiedOn: 员工实名时间戳
+        :param VerifiedOn: 员工实名时间戳，单位秒
         :type VerifiedOn: int
         :param QuiteJob: 员工是否离职：0-未离职，1-离职
         :type QuiteJob: int
         """
         self.UserId = None
         self.DisplayName = None
         self.Mobile = None
@@ -5392,15 +5393,15 @@
 class SyncFailReason(AbstractModel):
     """同步经办人失败原因
 
     """
 
     def __init__(self):
         r"""
-        :param Id: 经办人Id
+        :param Id: 对应Agent-ProxyOperator-OpenId。第三方应用平台自定义，对子客企业员的唯一标识。一个OpenId在一个子客企业内唯一对应一个真实员工，不可在其他子客企业内重复使用。（例如，可以使用经办人企业名+员工身份证的hash值，需要第三方应用平台保存），最大64位字符串
         :type Id: str
         :param Message: 失败原因
 例如：Id不符合规范、证件号码不合法等
 注意：此字段可能返回 null，表示取不到有效值。
         :type Message: str
         """
         self.Id = None
@@ -5603,37 +5604,37 @@
         r"""
         :param TemplateId: 模板ID
         :type TemplateId: str
         :param TemplateName: 模板名字
         :type TemplateName: str
         :param Description: 模板描述信息
         :type Description: str
-        :param Components: 模板控件信息结构
+        :param Components: 模板的填充控件信息结构
         :type Components: list of Component
         :param Recipients: 模板中的流程参与人信息
         :type Recipients: list of Recipient
-        :param SignComponents: 签署区模板信息结构
+        :param SignComponents: 模板中的签署控件信息结构
         :type SignComponents: list of Component
         :param TemplateType: 模板类型：1-静默签；3-普通模板
         :type TemplateType: int
         :param IsPromoter: 是否是发起人 ,已弃用
         :type IsPromoter: bool
-        :param Creator: 模板的创建者信息
+        :param Creator: 模板的创建者信息，电子签系统用户ID
         :type Creator: str
-        :param CreatedOn: 模板创建的时间戳（精确到秒）
+        :param CreatedOn: 模板创建的时间戳，单位秒
         :type CreatedOn: int
-        :param PreviewUrl: 模板的H5预览链接,可以通过浏览器打开此链接预览模板，或者嵌入到iframe中预览模板。
+        :param PreviewUrl: 模板的H5预览链接,可以通过浏览器打开此链接预览模板，或者嵌入到iframe中预览模板。请求参数WithPreviewUrl=true时返回，有效期5分钟。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PreviewUrl: str
-        :param PdfUrl: 第三方应用集成-模板PDF文件链接
+        :param PdfUrl: 第三方应用集成-模板PDF文件链接。请求参数WithPdfUrl=true时返回（此功能开放需要联系客户经理），有效期5分钟。
 注意：此字段可能返回 null，表示取不到有效值。
         :type PdfUrl: str
-        :param ChannelTemplateId: 关联的平台企业模板ID
+        :param ChannelTemplateId: 关联的第三方应用平台企业模板ID
         :type ChannelTemplateId: str
-        :param ChannelTemplateName: 关联的平台企业模板名称
+        :param ChannelTemplateName: 关联的三方应用平台平台企业模板名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChannelTemplateName: str
         :param ChannelAutoSave: 0-需要子客企业手动领取平台企业的模板(默认); 1-平台自动设置子客模板
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChannelAutoSave: int
         :param TemplateVersion: 模板版本，全数字字符。默认为空，初始版本为yyyyMMdd001。
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.908/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.908/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.907/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.908/setup.py`

 * *Files identical despite different names*

