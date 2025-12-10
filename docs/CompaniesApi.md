# CompaniesApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCompany**](#getcompany) | **GET** /companies | |
|[**getRedirectUri**](#getredirecturi) | **GET** /companies/redirect_uri | |
|[**setRedirectUri**](#setredirecturi) | **PUT** /companies/redirect_uri | |

# **getCompany**
> getCompany()


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


const { status, data } = await client.companies.getCompany();
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

# **getRedirectUri**
> getRedirectUri()


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


const { status, data } = await client.companies.getRedirectUri();
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

# **setRedirectUri**
> setRedirectUri(redirectUriDTO)


### Example

```typescript
import {
    Client,
    Configuration,
    RedirectUriDTO
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let redirectUriDTO: RedirectUriDTO; // 

const { status, data } = await client.companies.setRedirectUri(
    redirectUriDTO
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **redirectUriDTO** | **RedirectUriDTO**|  | |


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
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

