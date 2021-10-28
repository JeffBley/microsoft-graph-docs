---
title: "Create delegatedPermissionClassification"
description: "Create a new delegatedPermissionClassification object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create delegatedPermissionClassification
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

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
POST /servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.

You can specify the following properties when creating a **delegatedPermissionClassification**.

|Property|Type|Description|
|:---|:---|:---|
|permissionId|String|**TODO: Add Description** Optional.|
|permissionName|String|**TODO: Add Description** Optional.|
|classification|permissionClassificationType|**TODO: Add Description**. The possible values are: `low`, `medium`, `high`, `unknownFutureValue`. Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_delegatedpermissionclassification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/delegatedPermissionClassifications
Content-Type: application/json
Content-length: 178

{
  "@odata.type": "#Microsoft.DirectoryServices.delegatedPermissionClassification",
  "permissionId": "String",
  "permissionName": "String",
  "classification": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.delegatedPermissionClassification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.delegatedPermissionClassification",
  "id": "baaa6467-6467-baaa-6764-aaba6764aaba",
  "permissionId": "String",
  "permissionName": "String",
  "classification": "String"
}
```

