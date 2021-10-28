---
title: "List resourceSpecificPermissionGrants"
description: "Get a list of the resourceSpecificPermissionGrant objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List resourceSpecificPermissionGrants
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects and their properties.

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
GET /permissionGrants
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

If successful, this method returns a `200 OK` response code and a collection of [resourceSpecificPermissionGrant](../resources/resourcespecificpermissiongrant.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_resourcespecificpermissiongrant"
}
-->
``` http
GET https://graph.microsoft.com/beta/permissionGrants
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.resourceSpecificPermissionGrant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.resourceSpecificPermissionGrant",
      "id": "2d6d0be5-0be5-2d6d-e50b-6d2de50b6d2d",
      "deletedDateTime": "String (timestamp)",
      "clientId": "String",
      "clientAppId": "String",
      "resourceAppId": "String",
      "permissionType": "String",
      "permission": "String"
    }
  ]
}
```

