---
title: "servicePrincipal: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# servicePrincipal: delta
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
GET /servicePrincipals/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/servicePrincipals/delta
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.servicePrincipal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.servicePrincipal",
      "id": "String (identifier)",
      "deletedDateTime": "String (timestamp)",
      "accountEnabled": "Boolean",
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn"
        }
      ],
      "alternativeNames": [
        "String"
      ],
      "api": {
        "@odata.type": "microsoft.graph.apiServicePrincipal"
      },
      "appData": "String",
      "appDescription": "String",
      "appDisplayName": "String",
      "appId": "String",
      "appMetadata": {
        "@odata.type": "microsoft.graph.appMetadata"
      },
      "applicationTemplateId": "String",
      "appOwnerOrganizationId": "Guid",
      "appRoleAssignmentRequired": "Boolean",
      "appRoles": [
        {
          "@odata.type": "microsoft.graph.appRole"
        }
      ],
      "customSecurityAttributes": {
        "@odata.type": "microsoft.graph.customSecurityAttributeValue"
      },
      "description": "String",
      "disabledByMicrosoftStatus": "String",
      "displayName": "String",
      "errorUrl": "String",
      "hasPermissionClassifications": "Boolean",
      "homepage": "String",
      "info": {
        "@odata.type": "microsoft.graph.informationalUrl"
      },
      "isManagementRestricted": "Boolean",
      "keyCredentials": [
        {
          "@odata.type": "microsoft.graph.keyCredential"
        }
      ],
      "loginUrl": "String",
      "logoutUrl": "String",
      "managedIdentityResourceId": "String",
      "microsoftPolicyGroup": "Boolean",
      "notes": "String",
      "notificationEmailAddresses": [
        "String"
      ],
      "publishedPermissionScopes": [
        {
          "@odata.type": "microsoft.graph.permissionScope"
        }
      ],
      "passwordCredentials": [
        {
          "@odata.type": "microsoft.graph.passwordCredential"
        }
      ],
      "preferredTokenSigningKeyEndDateTime": "String (timestamp)",
      "preferredTokenSigningKeyThumbprint": "String",
      "preferredSingleSignOnMode": "String",
      "publisherName": "String",
      "replyUrls": [
        "String"
      ],
      "resourceSpecificApplicationPermissions": [
        {
          "@odata.type": "microsoft.graph.resourceSpecificPermission"
        }
      ],
      "samlMetadataUrl": "String",
      "samlSingleSignOnSettings": {
        "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
      },
      "servicePrincipalNames": [
        "String"
      ],
      "servicePrincipalType": "String",
      "signInAudience": "String",
      "tags": [
        "String"
      ],
      "tokenEncryptionKeyId": "Guid"
    }
  ]
}
```

