# CreateTargetingDtoTargetingsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**targetingKind** | **string** |  | [default to TargetingKindEnum_UrlTargeting]
**zipcodes** | [**Array&lt;ZipcodeDto&gt;**](ZipcodeDto.md) |  | [default to undefined]
**time** | **number** |  | [default to undefined]
**requests** | **number** |  | [default to undefined]
**urls** | **Array&lt;string&gt;** |  | [default to undefined]

## Example

```typescript
import { CreateTargetingDtoTargetingsInner } from '@n2api/axios-client';

const instance: CreateTargetingDtoTargetingsInner = {
    targetingKind,
    zipcodes,
    time,
    requests,
    urls,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
