---
title: "Create subscribedSku"
description: "Create a new subscribedSku object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create subscribedSku
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [subscribedSku](../resources/subscribedsku.md) object.

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
POST /subscribedSkus
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [subscribedSku](../resources/subscribedsku.md) object.

You can specify the following properties when creating a **subscribedSku**.

|Property|Type|Description|
|:---|:---|:---|
|capabilityStatus|String|**TODO: Add Description** Optional.|
|consumedUnits|Int32|**TODO: Add Description** Optional.|
|prepaidUnits|[Microsoft.DirectoryServices.licenseUnitsDetail](../resources/licenseunitsdetail.md)|**TODO: Add Description** Optional.|
|servicePlans|[Microsoft.DirectoryServices.servicePlanInfo](../resources/serviceplaninfo.md) collection|**TODO: Add Description** Required.|
|skuId|Guid|**TODO: Add Description** Optional.|
|skuPartNumber|String|**TODO: Add Description** Optional.|
|appliesTo|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [subscribedSku](../resources/subscribedsku.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_subscribedsku_from_subscribedskus"
}
-->
``` http
POST https://graph.microsoft.com/beta/subscribedSkus
Content-Type: application/json
Content-length: 388

{
  "@odata.type": "#Microsoft.DirectoryServices.subscribedSku",
  "capabilityStatus": "String",
  "consumedUnits": "Integer",
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String",
  "appliesTo": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.subscribedSku"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.subscribedSku",
  "capabilityStatus": "String",
  "consumedUnits": "Integer",
  "id": "55418c11-8c11-5541-118c-4155118c4155",
  "prepaidUnits": {
    "@odata.type": "microsoft.graph.licenseUnitsDetail"
  },
  "servicePlans": [
    {
      "@odata.type": "microsoft.graph.servicePlanInfo"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String",
  "appliesTo": "String"
}
```

