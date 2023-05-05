---
title: "continuousAccessEvaluationSessionControl resource type"
description: "Session control to define the Continuous Access Evaluation behavior."
ms.localizationpriority: medium
author: "elijaholasunkanmi"
ms.prod: "identity-and-sign-in"
doc_type: "resourcePageType"
---

# continuousAccessEvaluationSessionControl resource type

Namespace: microsoft.graph

Session control to define the Continuous Access Evaluation behavior. Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).

## Properties
| Property | Type                                             | Description                                                                   | Read-Only |
| :------- | :----------------------------------------------- | :---------------------------------------------------------------------------- | :-------: |
| `mode`   | `microsoft.graph.continuousAccessEvaluationMode` | Type of Continuous Access Evaluation mode (e.g. disabled, unknownFutureValue, strictLocation). |           |

| Modes    | Description |
|:-------------|:------------|
| `disabled`   | Continuous Access Evaluation is disabled. Disablement can only be applied to all applications, with no other conditions.|
| `unknownFutureValue`| Evolvable enum sentinel value. |
| `strictLocation`    | Continuous Access Evaluation strict location is enabled. IP location policy will be strictly enforced on IP seen by Resource provider as well.|

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.continuousAccessEvaluationSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "mode": "String"
}
```