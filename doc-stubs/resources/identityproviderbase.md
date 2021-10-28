---
title: "identityProviderBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# identityProviderBase resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**
This is an abstract type.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List identityProviderBases](../api/identityproviderbase-list.md)|[identityProviderBase](../resources/identityproviderbase.md) collection|Get a list of the [identityProviderBase](../resources/identityproviderbase.md) objects and their properties.|
|[Create identityProviderBase](../api/directory-post-federationconfigurations.md)|[identityProviderBase](../resources/identityproviderbase.md)|Create a new [identityProviderBase](../resources/identityproviderbase.md) object.|
|[Get identityProviderBase](../api/identityproviderbase-get.md)|[identityProviderBase](../resources/identityproviderbase.md)|Read the properties and relationships of an [identityProviderBase](../resources/identityproviderbase.md) object.|
|[Update identityProviderBase](../api/identityproviderbase-update.md)|[identityProviderBase](../resources/identityproviderbase.md)|Update the properties of an [identityProviderBase](../resources/identityproviderbase.md) object.|
|[Delete identityProviderBase](../api/identityproviderbase-delete.md)|None|Deletes an [identityProviderBase](../resources/identityproviderbase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityProviderBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identityProviderBase",
  "id": "String (identifier)",
  "displayName": "String"
}
```

