---
title: "Get domainDnsMxRecord"
description: "Read the properties and relationships of a domainDnsMxRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get domainDnsMxRecord
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.

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
GET /domainDnsMxRecord
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

If successful, this method returns a `200 OK` response code and a [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domaindnsmxrecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/domainDnsMxRecord
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.domainDnsMxRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.domainDnsMxRecord",
    "id": "f9ac104f-104f-f9ac-4f10-acf94f10acf9",
    "isOptional": "Boolean",
    "label": "String",
    "recordType": "String",
    "supportedService": "String",
    "ttl": "Integer",
    "mailExchange": "String",
    "preference": "Integer"
  }
}
```

