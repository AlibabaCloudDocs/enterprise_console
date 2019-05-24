# 使用 ActionTrail 记录资源组操作 {#concept_qsx_yjm_4fb .concept}

ActionTrail 可以记录主账号或 RAM 用户进行的操作，通过 ActionTrail 可以查看所有用户对资源实例进行操作的记录。

## 前提条件 {#section_a5m_mf4_tgb .section}

资源组已经与 ActionTrail 服务进行了集成，可以联合使用。

## 使用 ActionTrail 查看 资源组操作记录的步骤 {#section_hyp_ll4_tgb .section}

1.  登录 [ActionTrail 控制台](https://actiontrail.console.aliyun.com)。
2.  在**历史事件查询**页签下，使用**过滤器**进行搜索。
3.  输入相关的用户名，选择**事件类型**和**时间**后，单击**搜索**。

    **说明：** 您也可以通过**事件名称**、**资源类型**、**资源名称**、**AccessKeyId**等进行搜索。

4.  单击需要查看的事件，单击**查看事件**。

## ActionTrail 记录的操作 {#section_qkm_4f4_tgb .section}

ActionTrail 可以记录资源组控制台的操作，例如：

```language-json

{

  "eventId": "B1CFCA37-83FA-4288-B623-01994CF8BDD2",
  "eventVersion": "1",
  "requestParameters": {
  "RequestId": "B1CFCA37-83FA-4288-B623-01994CF8BDD2",
  "DisplayName": "actiontrail",
  "HostId": "resourcemanager-share.aliyuncs.com",
  "Name": "action"
},
  "eventSource": "resourcemanager-share.aliyuncs.com",
  "sourceIpAddress": "42.120.75.152",
  "userIdentity": {
  "sessionContext": {
  "attributes": {
  "mfaAuthenticated": "false",
  "creationDate": "2019-03-08T07:00:04Z"
}
},
  "accountId": "1117495088180940",
  "principalId": "1117495088180940",
  "userName": "root",
  "type": "root-account"
},
  "eventType": "ApiCall",
  "serviceName": "ResourceManager",
  "apiVersion": "2016-11-11",
  "requestId": "B1CFCA37-83FA-4288-B623-01994CF8BDD2",
  "eventTime": "2019-03-08T07:00:04Z",
  "acsRegion": "cn-hangzhou",
  "eventName": "CreateResourceGroup"
}

```

## 更多信息 {#section_qqw_pf4_tgb .section}

关于操作记录的详细信息，请参考[操作事件\(Event\)结构定义](../../../../cn.zh-CN/用户指南/操作事件(Event)结构定义.md#)。

