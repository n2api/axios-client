# CreateAdSetDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**targetings** | [**Array&lt;CreateAdSetDtoTargetingsInner&gt;**](CreateAdSetDtoTargetingsInner.md) |  | [optional] [default to undefined]
**settings** | [**Array&lt;CreateAdSetDtoSettingsInner&gt;**](CreateAdSetDtoSettingsInner.md) |  | [optional] [default to undefined]
**channelKind** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**ads** | **Array&lt;object&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateAdSetDto } from '@n2api/axios-client';

const instance: CreateAdSetDto = {
    targetings,
    settings,
    channelKind,
    name,
    ads,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
