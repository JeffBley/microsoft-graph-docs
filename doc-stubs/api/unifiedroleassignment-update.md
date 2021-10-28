---
title: "Update unifiedRoleAssignment"
description: "Update the properties of an unifiedRoleAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRoleAssignment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

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
PATCH /me/transitiveRoleAssignments
PATCH /users/{usersId}/transitiveRoleAssignments
PATCH /groups/{groupsId}/transitiveRoleAssignments
PATCH /servicePrincipals/{servicePrincipalsId}/transitiveRoleAssignments
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
|appScopeId|String|**TODO: Add Description** Optional.|
|condition|String|**TODO: Add Description** Optional.|
|directoryScopeId|String|**TODO: Add Description** Optional.|
|principalId|String|**TODO: Add Description** Optional.|
|principalOrganizationId|String|**TODO: Add Description** Optional.|
|resourceScope|String|**TODO: Add Description** Optional.|
|roleDefinitionId|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/transitiveRoleAssignments
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "appScopeId": "String",
  "condition": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "principalOrganizationId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
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
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "37ed2c59-2c59-37ed-592c-ed37592ced37",
  "appScopeId": "String",
  "condition": "String",
  "directoryScopeId": "String",
  "principalId": "String",
  "principalOrganizationId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

