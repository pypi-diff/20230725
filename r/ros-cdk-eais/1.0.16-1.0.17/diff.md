# Comparing `tmp/ros-cdk-eais-1.0.16.tar.gz` & `tmp/ros-cdk-eais-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-eais-1.0.16.tar", last modified: Wed Jul 19 02:03:45 2023, max compression
+gzip compressed data, was "dist/ros-cdk-eais-1.0.17.tar", last modified: Tue Jul 25 07:07:30 2023, max compression
```

## Comparing `ros-cdk-eais-1.0.16.tar` & `ros-cdk-eais-1.0.17.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/
--rw-r--r--   0 root         (0) root         (0)    10279 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1881 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais/
--rw-r--r--   0 root         (0) root         (0)    44562 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais/_jsii/
--rw-r--r--   0 root         (0) root         (0)      408 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37994 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais/_jsii/ros-cdk-eais@1.0.16.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1296 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-19 02:03:44.000000 ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/
+-rw-r--r--   0 root         (0) root         (0)    10279 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/
+-rw-r--r--   0 root         (0) root         (0)    60913 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41964 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/_jsii/ros-cdk-eais@1.0.17.jsii.tgz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/datasource/
+-rw-r--r--   0 root         (0) root         (0)    21641 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/datasource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:07:30.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-25 07:07:29.000000 ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/top_level.txt
```

### Comparing `ros-cdk-eais-1.0.16/LICENSE` & `ros-cdk-eais-1.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-eais-1.0.16/PKG-INFO` & `ros-cdk-eais-1.0.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eais
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EAIS Construct Library
```

### Comparing `ros-cdk-eais-1.0.16/setup.py` & `ros-cdk-eais-1.0.17/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-eais",
-    "version": "1.0.16",
+    "version": "1.0.17",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -18,19 +18,20 @@
         "Source": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "ros_cdk_eais",
-        "ros_cdk_eais._jsii"
+        "ros_cdk_eais._jsii",
+        "ros_cdk_eais.datasource"
     ],
     "package_data": {
         "ros_cdk_eais._jsii": [
-            "ros-cdk-eais@1.0.16.jsii.tgz"
+            "ros-cdk-eais@1.0.17.jsii.tgz"
         ],
         "ros_cdk_eais": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `ros-cdk-eais-1.0.16/src/ros_cdk_eais/__init__.py` & `ros-cdk-eais-1.0.17/src/ros_cdk_eais/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,14 +20,125 @@
 from typeguard import check_type
 
 from ._jsii import *
 
 import ros_cdk_core as _ros_cdk_core_7adfd82f
 
 
+class ClientInstanceAttachment(
+    _ros_cdk_core_7adfd82f.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-eais.ClientInstanceAttachment",
+):
+    '''A ROS resource type:  ``ALIYUN::EAIS::ClientInstanceAttachment``.'''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["ClientInstanceAttachmentProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''Create a new ``ALIYUN::EAIS::ClientInstanceAttachment``.
+
+        Param scope - scope in which this resource is defined
+        Param id    - scoped id of the resource
+        Param props - resource properties
+
+        :param scope: -
+        :param id: -
+        :param props: -
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__04f77a20c52df2719b43947acfca5985d22fcc56e52ebb42f3c88bfc3f8766e3)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrClientInstanceId")
+    def attr_client_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute ClientInstanceId: The ID of the ECS or ECI instance bound to the EAIS instance.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrClientInstanceId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrInstanceId")
+    def attr_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute InstanceId: The EAIS instance ID.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrInstanceId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrVSwitchId")
+    def attr_v_switch_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''Attribute VSwitchId: Switch ID.'''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrVSwitchId"))
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-eais.ClientInstanceAttachmentProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "client_instance_id": "clientInstanceId",
+        "instance_id": "instanceId",
+    },
+)
+class ClientInstanceAttachmentProps:
+    def __init__(
+        self,
+        *,
+        client_instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        '''Properties for defining a ``ALIYUN::EAIS::ClientInstanceAttachment``.
+
+        :param client_instance_id: Property clientInstanceId: The ID of the ECS or ECI instance bound to the EAIS instance.
+        :param instance_id: Property instanceId: The EAIS instance ID.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1f28d8d88b24db2773265ca5ae6fc3b5845eeb9042cbf7f5a84e853cbb7bc3d8)
+            check_type(argname="argument client_instance_id", value=client_instance_id, expected_type=type_hints["client_instance_id"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "client_instance_id": client_instance_id,
+            "instance_id": instance_id,
+        }
+
+    @builtins.property
+    def client_instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property clientInstanceId: The ID of the ECS or ECI instance bound to the EAIS instance.'''
+        result = self._values.get("client_instance_id")
+        assert result is not None, "Required property 'client_instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''Property instanceId: The EAIS instance ID.'''
+        result = self._values.get("instance_id")
+        assert result is not None, "Required property 'instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ClientInstanceAttachmentProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class Instance(
     _ros_cdk_core_7adfd82f.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-eais.Instance",
 ):
     '''A ROS resource type:  ``ALIYUN::EAIS::Instance``.'''
 
@@ -269,14 +380,207 @@
 
     def __repr__(self) -> str:
         return "InstanceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosClientInstanceAttachment(
+    _ros_cdk_core_7adfd82f.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-eais.RosClientInstanceAttachment",
+):
+    '''A ROS template type:  ``ALIYUN::EAIS::ClientInstanceAttachment``.'''
+
+    def __init__(
+        self,
+        scope: _ros_cdk_core_7adfd82f.Construct,
+        id: builtins.str,
+        props: typing.Union["RosClientInstanceAttachmentProps", typing.Dict[builtins.str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''Create a new ``ALIYUN::EAIS::ClientInstanceAttachment``.
+
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c1daf1e89f956be520a1b05c675057195171b4db3f1270dbadbcfe48023cfcec)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @jsii.member(jsii_name="renderProperties")
+    def _render_properties(
+        self,
+        props: typing.Mapping[builtins.str, typing.Any],
+    ) -> typing.Mapping[builtins.str, typing.Any]:
+        '''
+        :param props: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cc085fef4fd1eec89b890d216623eb8c2264c2869cddcaf663909273163148da)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
+    def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
+        '''The resource type name for this resource class.'''
+        return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrClientInstanceId")
+    def attr_client_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: ClientInstanceId: The ID of the ECS or ECI instance bound to the EAIS instance.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrClientInstanceId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrInstanceId")
+    def attr_instance_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: InstanceId: The EAIS instance ID.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrInstanceId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrVSwitchId")
+    def attr_v_switch_id(self) -> _ros_cdk_core_7adfd82f.IResolvable:
+        '''
+        :Attribute: VSwitchId: Switch ID.
+        '''
+        return typing.cast(_ros_cdk_core_7adfd82f.IResolvable, jsii.get(self, "attrVSwitchId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rosProperties")
+    def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
+
+    @builtins.property
+    @jsii.member(jsii_name="clientInstanceId")
+    def client_instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: clientInstanceId: The ID of the ECS or ECI instance bound to the EAIS instance.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "clientInstanceId"))
+
+    @client_instance_id.setter
+    def client_instance_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d26b3b29d1fd660eefc8f77f28d48708e6a9519f9e022e0d474bfd132b864667)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "clientInstanceId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @enable_resource_property_constraint.setter
+    def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b526a9254b8288853917020c3396bff2173055c1d8bb61150cd6af68b8b85a7f)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="instanceId")
+    def instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: instanceId: The EAIS instance ID.
+        '''
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], jsii.get(self, "instanceId"))
+
+    @instance_id.setter
+    def instance_id(
+        self,
+        value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cf3f4b07719d58b8d5159929ce87048a4ae458d4545aeff7663b7f3811127bbc)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "instanceId", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-eais.RosClientInstanceAttachmentProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "client_instance_id": "clientInstanceId",
+        "instance_id": "instanceId",
+    },
+)
+class RosClientInstanceAttachmentProps:
+    def __init__(
+        self,
+        *,
+        client_instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+        instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    ) -> None:
+        '''Properties for defining a ``ALIYUN::EAIS::ClientInstanceAttachment``.
+
+        :param client_instance_id: 
+        :param instance_id: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8cd50513c4779db7d0ddcaedad0e012bbf753241a5df1b3bc8369d6842417268)
+            check_type(argname="argument client_instance_id", value=client_instance_id, expected_type=type_hints["client_instance_id"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "client_instance_id": client_instance_id,
+            "instance_id": instance_id,
+        }
+
+    @builtins.property
+    def client_instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: clientInstanceId: The ID of the ECS or ECI instance bound to the EAIS instance.
+        '''
+        result = self._values.get("client_instance_id")
+        assert result is not None, "Required property 'client_instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    @builtins.property
+    def instance_id(
+        self,
+    ) -> typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]:
+        '''
+        :Property: instanceId: The EAIS instance ID.
+        '''
+        result = self._values.get("instance_id")
+        assert result is not None, "Required property 'instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosClientInstanceAttachmentProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class RosInstance(
     _ros_cdk_core_7adfd82f.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-eais.RosInstance",
 ):
     '''A ROS template type:  ``ALIYUN::EAIS::Instance``.'''
 
@@ -808,22 +1112,47 @@
     def __repr__(self) -> str:
         return "RosInstanceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
+    "ClientInstanceAttachment",
+    "ClientInstanceAttachmentProps",
     "Instance",
     "InstanceProps",
+    "RosClientInstanceAttachment",
+    "RosClientInstanceAttachmentProps",
     "RosInstance",
     "RosInstanceProps",
+    "datasource",
 ]
 
 publication.publish()
 
+# Loading modules to ensure their types are registered with the jsii runtime library
+from . import datasource
+
+def _typecheckingstub__04f77a20c52df2719b43947acfca5985d22fcc56e52ebb42f3c88bfc3f8766e3(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[ClientInstanceAttachmentProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1f28d8d88b24db2773265ca5ae6fc3b5845eeb9042cbf7f5a84e853cbb7bc3d8(
+    *,
+    client_instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__94fccfcf7819241315e3d89601d4efbc48c9a24ada6a1e8f6d9f8857d82b6199(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[InstanceProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
@@ -839,14 +1168,55 @@
     instance_name: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     payment_type: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
     resource_group_id: typing.Optional[typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__c1daf1e89f956be520a1b05c675057195171b4db3f1270dbadbcfe48023cfcec(
+    scope: _ros_cdk_core_7adfd82f.Construct,
+    id: builtins.str,
+    props: typing.Union[RosClientInstanceAttachmentProps, typing.Dict[builtins.str, typing.Any]],
+    enable_resource_property_constraint: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cc085fef4fd1eec89b890d216623eb8c2264c2869cddcaf663909273163148da(
+    props: typing.Mapping[builtins.str, typing.Any],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d26b3b29d1fd660eefc8f77f28d48708e6a9519f9e022e0d474bfd132b864667(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b526a9254b8288853917020c3396bff2173055c1d8bb61150cd6af68b8b85a7f(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cf3f4b07719d58b8d5159929ce87048a4ae458d4545aeff7663b7f3811127bbc(
+    value: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8cd50513c4779db7d0ddcaedad0e012bbf753241a5df1b3bc8369d6842417268(
+    *,
+    client_instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+    instance_id: typing.Union[builtins.str, _ros_cdk_core_7adfd82f.IResolvable],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__d01e5dcce647be05207c5def57a92e83466e5d0e1b82ae072f644056f23f9783(
     scope: _ros_cdk_core_7adfd82f.Construct,
     id: builtins.str,
     props: typing.Union[RosInstanceProps, typing.Dict[builtins.str, typing.Any]],
     enable_resource_property_constraint: builtins.bool,
 ) -> None:
     """Type checking stubs"""
```

### Comparing `ros-cdk-eais-1.0.16/src/ros_cdk_eais.egg-info/PKG-INFO` & `ros-cdk-eais-1.0.17/src/ros_cdk_eais.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eais
-Version: 1.0.16
+Version: 1.0.17
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EAIS Construct Library
```

