# CreateAdSetDtoSettingsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**settingType** | **string** |  | [default to SettingTypeEnum_MaximumDailyImpressions]
**maximumCpm** | **number** |  | [default to undefined]
**realtimeBiddingStrategy** | **string** |  | [default to undefined]
**pacingType** | **string** |  | [default to undefined]
**dailyBudget** | **number** |  | [default to undefined]
**maximumDailyImpressions** | **number** |  | [default to undefined]

## Example

```typescript
import { CreateAdSetDtoSettingsInner } from '@n2api/axios-client';

const instance: CreateAdSetDtoSettingsInner = {
    settingType,
    maximumCpm,
    realtimeBiddingStrategy,
    pacingType,
    dailyBudget,
    maximumDailyImpressions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
