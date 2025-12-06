# CreateFacebookAuthDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | The Facebook auth code returned from the redirect. | [default to undefined]
**redirect_uri** | **string** | The Facebook redirect uri. | [default to undefined]

## Example

```typescript
import { CreateFacebookAuthDto } from '@n2api/axios-client';

const instance: CreateFacebookAuthDto = {
    code,
    redirect_uri,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
