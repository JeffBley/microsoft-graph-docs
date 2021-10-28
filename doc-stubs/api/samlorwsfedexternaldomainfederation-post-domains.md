---
title: "Create externalDomainName"
description: "Create a new externalDomainName object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create externalDomainName
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [externalDomainName](../resources/externaldomainname.md) object.

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
POST /samlOrWsFedExternalDomainFederation/domains
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [externalDomainName](../resources/externaldomainname.md) object.

You can specify the following properties when creating an **externalDomainName**.

|Property|Type|Description|
|:---|:---|:---|



## Response

If successful, this method returns a `201 Created` response code and an [externalDomainName](../resources/externaldomainname.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_externaldomainname_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/samlOrWsFedExternalDomainFederation/domains
Content-Type: application/json
Content-length: 72

{
  "@odata.type": "#Microsoft.DirectoryServices.externalDomainName"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.externalDomainName"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.externalDomainName",
  "id": "e762ac24-ac24-e762-24ac-62e724ac62e7"
}
```

