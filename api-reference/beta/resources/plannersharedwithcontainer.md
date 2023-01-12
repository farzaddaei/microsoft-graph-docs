---
title: "plannerSharedWithContainer resource type"
description: "Represents a container for a plannerPlan. The container is a resource that specifies authorization rules and the lifetime of the plan."
author: "FarzadDaei"
ms.localizationpriority: medium
ms.prod: "planner"
doc_type: resourcePageType
---

# plannerSharedWithContainer resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the relationship of a planner Plan to a planner Container. Plans can be shared with containers that are not the original container the plan belongs to. When the plan is verifying a user's access to it, the plan will additionally check the authorization logic of the containers is it shared with.

Inherits from [plannerPlanContainer](plannerplancontainer.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessLevel|plannerPlanAccessLevel|The maxmimum access level the shared container can provide to the plan.|
|containerId|String|The identifier of the resource that contains the plan. Optional. Inherited from [plannerPlanContainer](plannerplancontainer.md).|
|type|plannerContainerType|The type of the resource that contains the plan. For supported types, see the previous table. Possible values are: `group`, `unknownFutureValue`, `roster`, `project`, and `driveItem`. Note that you must use the `Prefer: include-unknown-enum-members` request header to get the following value in this [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `roster`, `project`, `driveItem`. Optional. Inherited from [plannerPlanContainer](plannerplancontainer.md).|
|url|String|The full canonical URL of the container. Optional. Inherited from [plannerPlanContainer](plannerplancontainer.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerSharedWithContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerSharedWithContainer",
  "url": "String",
  "containerId": "String",
  "type": "String",
  "accessLevel": "String"
}
```

