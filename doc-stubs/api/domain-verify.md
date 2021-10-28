---
title: "domain: verify"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# domain: verify
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
POST /domains/{domainsId}/verify
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `200 OK` response code and a [domain](../resources/domain.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}
-->
``` http
POST https://graph.microsoft.com/beta/domains/{domainsId}/verify
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.domain"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.domain",
    "authenticationType": "String",
    "availabilityStatus": "String",
    "isAdminManaged": "Boolean",
    "isDefault": "Boolean",
    "isInitial": "Boolean",
    "isRoot": "Boolean",
    "isVerified": "Boolean",
    "id": "String (identifier)",
    "passwordNotificationWindowInDays": "Integer",
    "passwordValidityPeriodInDays": "Integer",
    "supportedServices": [
      "String"
    ],
    "state": {
      "@odata.type": "microsoft.graph.domainState"
    }
  }
}
```

