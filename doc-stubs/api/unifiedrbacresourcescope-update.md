---
title: "Update unifiedRbacResourceScope"
description: "Update the properties of an unifiedRbacResourceScope object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRbacResourceScope
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md) object.

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
PATCH /unifiedRbacResourceNamespace/resourceActions/{unifiedRbacResourceActionId}/resourceScope
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Optional.|
|scope|String|**TODO: Add Description** Required.|
|type|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedrbacresourcescope"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/unifiedRbacResourceNamespace/resourceActions/{unifiedRbacResourceActionId}/resourceScope
Content-Type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceScope",
  "displayName": "String",
  "scope": "String",
  "type": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceScope",
  "id": "e0c7c65b-c65b-e0c7-5bc6-c7e05bc6c7e0",
  "displayName": "String",
  "scope": "String",
  "type": "String"
}
```

