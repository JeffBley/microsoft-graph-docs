---
title: "Create permissionGrantPolicy"
description: "Create a new permissionGrantPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create permissionGrantPolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.

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
POST /policyRoot/permissionGrantPolicies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.

You can specify the following properties when creating a **permissionGrantPolicy**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|



## Response

If successful, this method returns a `201 Created` response code and a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_permissiongrantpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/policyRoot/permissionGrantPolicies
Content-Type: application/json
Content-length: 175

{
  "@odata.type": "#Microsoft.DirectoryServices.permissionGrantPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.permissionGrantPolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.permissionGrantPolicy",
  "id": "1f921e86-1e86-1f92-861e-921f861e921f",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```

