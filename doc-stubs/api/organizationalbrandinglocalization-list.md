---
title: "List organizationalBrandingLocalizations"
description: "Get a list of the organizationalBrandingLocalization objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List organizationalBrandingLocalizations
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) objects and their properties.

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
GET /organization/{organizationId}/branding/localizations
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

If successful, this method returns a `200 OK` response code and a collection of [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_organizationalbrandinglocalization"
}
-->
``` http
GET https://graph.microsoft.com/beta/organization/{organizationId}/branding/localizations
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.DirectoryServices.organizationalBrandingLocalization)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.organizationalBrandingLocalization",
      "id": "946a4faa-4faa-946a-aa4f-6a94aa4f6a94",
      "backgroundColor": "String",
      "backgroundImage": "Stream",
      "backgroundImageRelativeUrl": "String",
      "bannerLogo": "Stream",
      "bannerLogoRelativeUrl": "String",
      "cdnList": [
        "String"
      ],
      "signInPageText": "String",
      "squareLogo": "Stream",
      "squareLogoRelativeUrl": "String",
      "usernameHintText": "String",
      "customAccountResetCredentialsUrl": "String",
      "customCannotAccessYourAccountText": "String",
      "customCannotAccessYourAccountUrl": "String",
      "customForgotMyPasswordText": "String",
      "customPrivacyAndCookiesText": "String",
      "customPrivacyAndCookiesUrl": "String",
      "customResetItNowText": "String",
      "customTermsOfUseText": "String",
      "customTermsOfUseUrl": "String",
      "favicon": "Stream",
      "faviconRelativeUrl": "String",
      "headerBackgroundColor": "String",
      "loginPageTextVisibilitySettings": {
        "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
      }
    }
  ]
}
```

