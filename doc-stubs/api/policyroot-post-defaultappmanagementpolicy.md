---
title: "Create tenantAppManagementPolicy"
description: "Create a new tenantAppManagementPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create tenantAppManagementPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for Microsoft.DirectoryServices.tenantAppManagementPolicy not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) object.

You can specify the following properties when creating a **tenantAppManagementPolicy**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|isEnabled|Boolean|**TODO: Add Description** Required.|
|applicationRestrictions|[Microsoft.DirectoryServices.appManagementConfiguration](../resources/appmanagementconfiguration.md)|**TODO: Add Description** Optional.|
|servicePrincipalRestrictions|[Microsoft.DirectoryServices.appManagementConfiguration](../resources/appmanagementconfiguration.md)|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_tenantappmanagementpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for Microsoft.DirectoryServices.tenantAppManagementPolicy not found
Content-Type: application/json
Content-length: 417

{
  "@odata.type": "#Microsoft.DirectoryServices.tenantAppManagementPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "applicationRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.tenantAppManagementPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.tenantAppManagementPolicy",
  "id": "1c3cc936-c936-1c3c-36c9-3c1c36c93c1c",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "applicationRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  },
  "servicePrincipalRestrictions": {
    "@odata.type": "microsoft.graph.appManagementConfiguration"
  }
}
```

