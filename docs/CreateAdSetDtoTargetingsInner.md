# CreateAdSetDtoTargetingsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**targetingKind** | **string** |  | [default to TargetingKindEnum_UserFrequencyCapping]
**zipcodes** | [**Array&lt;ZipcodeDto&gt;**](ZipcodeDto.md) |  | [default to undefined]
**time** | **number** |  | [default to undefined]
**requests** | **number** |  | [default to undefined]

## Example

```typescript
import { CreateAdSetDtoTargetingsInner } from '@n2api/axios-client';

const instance: CreateAdSetDtoTargetingsInner = {
    targetingKind,
    zipcodes,
    time,
    requests,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
