---
title: "Add tokenIssuancePolicy"
description: "Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add tokenIssuancePolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.

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
POST /servicePrincipals/{servicePrincipalsId}/tokenIssuancePolicies/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.

You can specify the following properties when creating a **tokenIssuancePolicy**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md). Required.|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md). Required.|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md). Optional.|



## Response

If successful, this method returns a `204 No Content` response code and a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/tokenIssuancePolicies/$ref
Content-Type: application/json
Content-length: 251

{
  "@odata.type": "#Microsoft.DirectoryServices.tokenIssuancePolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.tokenIssuancePolicy"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.tokenIssuancePolicy",
  "id": "ac8246c5-46c5-ac82-c546-82acc54682ac",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

