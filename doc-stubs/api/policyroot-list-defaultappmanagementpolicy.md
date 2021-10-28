---
title: "List tenantAppManagementPolicy"
description: "Get the tenantAppManagementPolicy resources from the defaultAppManagementPolicy navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List tenantAppManagementPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the tenantAppManagementPolicy resources from the defaultAppManagementPolicy navigation property.

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
GET /policyRoot/defaultAppManagementPolicy
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [tenantAppManagementPolicy](../resources/tenantappmanagementpolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_tenantappmanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policyRoot/defaultAppManagementPolicy
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.tenantAppManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
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
  ]
}
```

