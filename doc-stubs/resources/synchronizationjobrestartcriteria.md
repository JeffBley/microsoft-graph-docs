---
title: "synchronizationJobRestartCriteria resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationJobRestartCriteria resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|resetScope|synchronizationJobRestartScope|**TODO: Add Description**. The possible values are: `None`, `ConnectorDataStore`, `Escrows`, `Watermark`, `QuarantineState`, `Full`, `ForceDeletes`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobRestartCriteria",
  "resetScope": "String"
}
```

