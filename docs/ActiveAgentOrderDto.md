# ActiveAgentOrderDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [default to undefined]
**advertiserId** | **number** |  | [default to undefined]
**networkId** | **number** |  | [default to undefined]
**campaignIds** | **Array&lt;number&gt;** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**runtimeBudgets** | [**Array&lt;RuntimeBudget&gt;**](RuntimeBudget.md) |  | [default to undefined]
**lastUpdate** | **number** |  | [default to undefined]
**deleted** | **boolean** |  | [default to undefined]
**advertiserMarginId** | **number** |  | [optional] [default to undefined]
**agencyId** | **number** |  | [optional] [default to undefined]
**calculatedDailyBudget** | **number** |  | [optional] [default to undefined]
**calculatedDailyImpressions** | **number** |  | [optional] [default to undefined]
**dailyBudget** | **number** |  | [optional] [default to undefined]
**dailyClicks** | **number** |  | [optional] [default to undefined]
**dailyImpressions** | **number** |  | [optional] [default to undefined]
**dailyPacing** | **boolean** |  | [optional] [default to undefined]
**footfallStoreConfigId** | **number** |  | [optional] [default to undefined]
**pace** | **number** |  | [optional] [default to undefined]
**runtimePacing** | **boolean** |  | [optional] [default to undefined]
**runtimePacingFactor** | **number** |  | [optional] [default to undefined]
**totalBudget** | **number** |  | [optional] [default to undefined]
**totalClicks** | **number** |  | [optional] [default to undefined]
**totalImpressions** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { ActiveAgentOrderDto } from '@n2api/axios-client';

const instance: ActiveAgentOrderDto = {
    id,
    advertiserId,
    networkId,
    campaignIds,
    name,
    runtimeBudgets,
    lastUpdate,
    deleted,
    advertiserMarginId,
    agencyId,
    calculatedDailyBudget,
    calculatedDailyImpressions,
    dailyBudget,
    dailyClicks,
    dailyImpressions,
    dailyPacing,
    footfallStoreConfigId,
    pace,
    runtimePacing,
    runtimePacingFactor,
    totalBudget,
    totalClicks,
    totalImpressions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
