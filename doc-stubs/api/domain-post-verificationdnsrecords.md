---
title: "Create domainDnsRecord"
description: "Create a new domainDnsRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create domainDnsRecord
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new domainDnsRecord object.

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
POST /domains/{domainsId}/verificationDnsRecords
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [domainDnsRecord](../resources/domaindnsrecord.md) object.

You can specify the following properties when creating a **domainDnsRecord**.

|Property|Type|Description|
|:---|:---|:---|
|isOptional|Boolean|**TODO: Add Description** Required.|
|label|String|**TODO: Add Description** Required.|
|recordType|String|**TODO: Add Description** Optional.|
|supportedService|String|**TODO: Add Description** Required.|
|ttl|Int32|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `201 Created` response code and a [domainDnsRecord](../resources/domaindnsrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_domaindnsrecord_from_domaindnsrecords"
}
-->
``` http
POST https://graph.microsoft.com/beta/domains/{domainsId}/verificationDnsRecords
Content-Type: application/json
Content-length: 200

{
  "@odata.type": "#Microsoft.DirectoryServices.domainDnsRecord",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.domainDnsRecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.domainDnsRecord",
  "id": "7616c12e-c12e-7616-2ec1-16762ec11676",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer"
}
```

