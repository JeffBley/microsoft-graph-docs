---
title: "Update directoryObjectPartnerReference"
description: "Update the properties of a directoryObjectPartnerReference object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update directoryObjectPartnerReference
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object.

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
PATCH /directoryObjectPartnerReference
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
|description|String|**TODO: Add Description** Optional.|
|displayName|String|**TODO: Add Description** Optional.|
|externalPartnerTenantId|Guid|**TODO: Add Description** Optional.|
|objectType|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [directoryObjectPartnerReference](../resources/directoryobjectpartnerreference.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_directoryobjectpartnerreference"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directoryObjectPartnerReference
Content-Type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalPartnerTenantId": "Guid",
  "objectType": "String"
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
  "@odata.type": "#microsoft.graph.directoryObjectPartnerReference",
  "id": "edeec3a1-c3a1-edee-a1c3-eeeda1c3eeed",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "externalPartnerTenantId": "Guid",
  "objectType": "String"
}
```

