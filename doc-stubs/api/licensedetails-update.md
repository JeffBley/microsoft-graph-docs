---
title: "Update licenseDetails"
description: "Update the properties of a licenseDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update licenseDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [licenseDetails](../resources/licensedetails.md) object.

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
PATCH /me/licenseDetails/{licenseDetailsId}
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
|servicePlans|[Microsoft.DirectoryServices.servicePlanInfo](../resources/serviceplaninfo.md) collection|**TODO: Add Description** Required.|
|skuId|Guid|**TODO: Add Description** Optional.|
|skuPartNumber|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [licenseDetails](../resources/licensedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_licensedetails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/licenseDetails/{licenseDetailsId}
Content-Type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.licenseDetails",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
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
  "@odata.type": "#microsoft.graph.licenseDetails",
  "id": "bd02028e-028e-bd02-8e02-02bd8e0202bd",
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
```

