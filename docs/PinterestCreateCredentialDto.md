# PinterestCreateCredentialDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_token** | **string** | The access token of the credential. | [default to undefined]
**refresh_token** | **string** | The refresh token of the credential. | [default to undefined]
**response_type** | **string** | The response type of the credential. | [default to undefined]
**token_type** | **string** | The token type of the credential. | [default to undefined]
**expires_in** | **number** | The expiration time of the access token. | [default to undefined]
**refresh_token_expires_in** | **number** | The expiration time of the refresh token. | [default to undefined]
**refresh_token_expires_at** | **number** | The expiration timestamp of the refresh token. | [default to undefined]
**scope** | **string** | The scope of the credential. | [default to undefined]

## Example

```typescript
import { PinterestCreateCredentialDto } from '@n2api/axios-client';

const instance: PinterestCreateCredentialDto = {
    access_token,
    refresh_token,
    response_type,
    token_type,
    expires_in,
    refresh_token_expires_in,
    refresh_token_expires_at,
    scope,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
