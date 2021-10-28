---
title: "unifiedRbacResourceAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unifiedRbacResourceAction resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRbacResourceActions](../api/unifiedrbacresourceaction-list.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) collection|Get a list of the [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) objects and their properties.|
|[Create unifiedRbacResourceAction](../api/unifiedrbacresourcenamespace-post-resourceactions.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Create a new [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) object.|
|[Get unifiedRbacResourceAction](../api/unifiedrbacresourceaction-get.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Read the properties and relationships of an [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) object.|
|[Update unifiedRbacResourceAction](../api/unifiedrbacresourceaction-update.md)|[unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md)|Update the properties of an [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) object.|
|[Delete unifiedRbacResourceAction](../api/unifiedrbacresourceaction-delete.md)|None|Deletes an [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) object.|
|[List unifiedRbacResourceScope](../api/unifiedrbacresourceaction-list-resourcescope.md)|[unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md) collection|Get the unifiedRbacResourceScope resources from the resourceScope navigation property.|
|[Create unifiedRbacResourceScope](../api/unifiedrbacresourceaction-post-resourcescope.md)|[unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md)|Create a new unifiedRbacResourceScope object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionVerb|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isEnabledForCustomRole|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|resourceScopeId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resourceScope|[unifiedRbacResourceScope](../resources/unifiedrbacresourcescope.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRbacResourceAction",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceAction",
  "id": "String (identifier)",
  "actionVerb": "String",
  "description": "String",
  "isEnabledForCustomRole": "Boolean",
  "name": "String",
  "resourceScopeId": "String"
}
```

