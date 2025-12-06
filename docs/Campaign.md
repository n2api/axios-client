# Campaign


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | **string** |  | [default to undefined]
**id** | **string** |  | [default to undefined]
**adAccount** | **string** |  | [default to undefined]
**channelKind** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**advertiser** | **string** |  | [default to undefined]
**lastUpdate** | **number** |  | [default to undefined]
**status** | **string** |  | [default to undefined]
**adSets** | [**Array&lt;AdSet&gt;**](AdSet.md) |  | [optional] [default to undefined]
**settings** | **Array&lt;object&gt;** |  | [default to undefined]
**targetings** | **Array&lt;object&gt;** |  | [optional] [default to undefined]
**kind** | **string** |  | [default to undefined]

## Example

```typescript
import { Campaign } from '@n2api/axios-client';

const instance: Campaign = {
    platform,
    id,
    adAccount,
    channelKind,
    name,
    advertiser,
    lastUpdate,
    status,
    adSets,
    settings,
    targetings,
    kind,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
