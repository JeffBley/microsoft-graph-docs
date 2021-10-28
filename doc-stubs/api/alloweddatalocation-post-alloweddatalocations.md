---
title: "Create allowedDataLocation"
description: "Create a new allowedDataLocation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create allowedDataLocation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [allowedDataLocation](../resources/alloweddatalocation.md) object.

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
POST /allowedDataLocations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [allowedDataLocation](../resources/alloweddatalocation.md) object.

You can specify the following properties when creating an **allowedDataLocation**.

|Property|Type|Description|
|:---|:---|:---|
|appId|String|**TODO: Add Description** Optional.|
|location|String|**TODO: Add Description** Optional.|
|isDefault|Boolean|**TODO: Add Description** Optional.|
|domain|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [allowedDataLocation](../resources/alloweddatalocation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_alloweddatalocation_from_alloweddatalocations"
}
-->
``` http
POST https://graph.microsoft.com/beta/allowedDataLocations
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#Microsoft.DirectoryServices.allowedDataLocation",
  "appId": "String",
  "location": "String",
  "isDefault": "Boolean",
  "domain": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.allowedDataLocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.allowedDataLocation",
  "id": "0e95559a-559a-0e95-9a55-950e9a55950e",
  "appId": "String",
  "location": "String",
  "isDefault": "Boolean",
  "domain": "String"
}
```

