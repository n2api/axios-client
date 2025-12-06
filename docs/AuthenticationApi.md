# AuthenticationApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**authControllerCreateCompanyTokenK3gngq**](#authcontrollercreatecompanytokenk3gngq) | **POST** /auth/company_token | |
|[**authControllerDeleteCompanyTokenU6zccl**](#authcontrollerdeletecompanytokenu6zccl) | **DELETE** /auth/company_token | |
|[**authControllerGetCompanyToken8bpz6u**](#authcontrollergetcompanytoken8bpz6u) | **GET** /auth/company_token | |
|[**authControllerGetHelloR0h1ua**](#authcontrollergethellor0h1ua) | **GET** /auth/user | |
|[**authControllerGetSessionTokenRbwd43**](#authcontrollergetsessiontokenrbwd43) | **POST** /auth/session_token | |
|[**authControllerLogin4otw64**](#authcontrollerlogin4otw64) | **POST** /auth/login | Login|
|[**authControllerRefreshHq9r5i**](#authcontrollerrefreshhq9r5i) | **POST** /auth/refresh | |
|[**authControllerVerifySessionTokenQkbht6**](#authcontrollerverifysessiontokenqkbht6) | **POST** /auth/session_token/verify | |

# **authControllerCreateCompanyTokenK3gngq**
> authControllerCreateCompanyTokenK3gngq()


### Example

```typescript
import {
    Client,
    Configuration
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


const { status, data } = await client.authentication.authControllerCreateCompanyTokenK3gngq();
```

### Parameters
This endpoint does not have any parameters.


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerDeleteCompanyTokenU6zccl**
> authControllerDeleteCompanyTokenU6zccl()


### Example

```typescript
import {
    Client,
    Configuration
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


const { status, data } = await client.authentication.authControllerDeleteCompanyTokenU6zccl();
```

### Parameters
This endpoint does not have any parameters.


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerGetCompanyToken8bpz6u**
> authControllerGetCompanyToken8bpz6u()


### Example

```typescript
import {
    Client,
    Configuration
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


const { status, data } = await client.authentication.authControllerGetCompanyToken8bpz6u();
```

### Parameters
This endpoint does not have any parameters.


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerGetHelloR0h1ua**
> object authControllerGetHelloR0h1ua()


### Example

```typescript
import {
    Client,
    Configuration
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


const { status, data } = await client.authentication.authControllerGetHelloR0h1ua();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**object**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerGetSessionTokenRbwd43**
> authControllerGetSessionTokenRbwd43(sessionTokenDto)


### Example

```typescript
import {
    Client,
    Configuration,
    SessionTokenDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let sessionTokenDto: SessionTokenDto; // 

const { status, data } = await client.authentication.authControllerGetSessionTokenRbwd43(
    sessionTokenDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionTokenDto** | **SessionTokenDto**|  | |


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerLogin4otw64**
> object authControllerLogin4otw64(loginDto)

Login with *username* and *password*. Returns an access token.

### Example

```typescript
import {
    Client,
    Configuration,
    LoginDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let loginDto: LoginDto; // 

const { status, data } = await client.authentication.authControllerLogin4otw64(
    loginDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **loginDto** | **LoginDto**|  | |


### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerRefreshHq9r5i**
> object authControllerRefreshHq9r5i()


### Example

```typescript
import {
    Client,
    Configuration
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


const { status, data } = await client.authentication.authControllerRefreshHq9r5i();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**object**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **authControllerVerifySessionTokenQkbht6**
> object authControllerVerifySessionTokenQkbht6(sessionTokenVerifyDto)


### Example

```typescript
import {
    Client,
    Configuration,
    SessionTokenVerifyDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let sessionTokenVerifyDto: SessionTokenVerifyDto; // 

const { status, data } = await client.authentication.authControllerVerifySessionTokenQkbht6(
    sessionTokenVerifyDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sessionTokenVerifyDto** | **SessionTokenVerifyDto**|  | |


### Return type

**object**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

