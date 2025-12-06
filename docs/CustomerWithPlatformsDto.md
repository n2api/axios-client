# CustomerWithPlatformsDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The unique identifier (UUID) of the customer. | [default to undefined]
**name** | **string** | The name of the customer. | [default to undefined]
**company** | **string** | The company UUID the customer belongs to. | [default to undefined]
**created_at** | **string** | The timestamp when the customer was created. | [default to undefined]
**platforms** | **Array&lt;string&gt;** | List of connected platforms for this customer. | [default to undefined]

## Example

```typescript
import { CustomerWithPlatformsDto } from '@n2api/axios-client';

const instance: CustomerWithPlatformsDto = {
    id,
    name,
    company,
    created_at,
    platforms,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
