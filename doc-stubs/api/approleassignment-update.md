---
title: "Update appRoleAssignment"
description: "Update the properties of an appRoleAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update appRoleAssignment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [appRoleAssignment](../resources/approleassignment.md) object.

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
PATCH /appRoleAssignments/{appRoleAssignmentsId}
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
|appRoleId|Guid|**TODO: Add Description** Required.|
|creationTimestamp|DateTimeOffset|**TODO: Add Description** Optional.|
|principalDisplayName|String|**TODO: Add Description** Optional.|
|principalId|Guid|**TODO: Add Description** Optional.|
|principalType|String|**TODO: Add Description** Optional.|
|resourceDisplayName|String|**TODO: Add Description** Optional.|
|resourceId|Guid|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{appRoleAssignmentsId}
Content-Type: application/json
Content-length: 283

{
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "Guid",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
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
  "@odata.type": "#microsoft.graph.appRoleAssignment",
  "appRoleId": "Guid",
  "creationTimestamp": "String (timestamp)",
  "id": "ee737201-7201-ee73-0172-73ee017273ee",
  "principalDisplayName": "String",
  "principalId": "Guid",
  "principalType": "String",
  "resourceDisplayName": "String",
  "resourceId": "Guid"
}
```

