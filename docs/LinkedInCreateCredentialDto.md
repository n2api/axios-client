# LinkedInCreateCredentialDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accessToken** | **string** | The accessToken of the credential. | [default to undefined]
**expiresIn** | **number** | The number in seconds until the access token expires. | [default to undefined]
**refreshToken** | **string** | The refreshToken of the credential. | [default to undefined]
**refreshTokenExpiresIn** | **number** | The number in seconds until the refresh token expires. | [default to undefined]

## Example

```typescript
import { LinkedInCreateCredentialDto } from '@n2api/axios-client';

const instance: LinkedInCreateCredentialDto = {
    accessToken,
    expiresIn,
    refreshToken,
    refreshTokenExpiresIn,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
