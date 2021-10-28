---
title: "Update extensionProperty"
description: "Update the properties of an extensionProperty object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update extensionProperty
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [extensionProperty](../resources/extensionproperty.md) object.

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
PATCH /applications/{applicationsId}/extensionProperties/{extensionPropertyId}
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
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|appDisplayName|String|**TODO: Add Description** Optional.|
|name|String|**TODO: Add Description** Required.|
|dataType|String|**TODO: Add Description** Required.|
|isSyncedFromOnPremises|Boolean|**TODO: Add Description** Optional.|
|targetObjects|String collection|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `200 OK` response code and an updated [extensionProperty](../resources/extensionproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_extensionproperty"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/extensionProperties/{extensionPropertyId}
Content-Type: application/json
Content-length: 262

{
  "@odata.type": "#microsoft.graph.extensionProperty",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": "Boolean",
  "targetObjects": [
    "String"
  ]
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
  "@odata.type": "#microsoft.graph.extensionProperty",
  "id": "0ced73ca-73ca-0ced-ca73-ed0cca73ed0c",
  "deletedDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "name": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": "Boolean",
  "targetObjects": [
    "String"
  ]
}
```

