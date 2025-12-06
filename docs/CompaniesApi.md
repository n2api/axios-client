# CompaniesApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**companiesControllerGetCompany2lyej4**](#companiescontrollergetcompany2lyej4) | **GET** /companies | |
|[**companiesControllerGetRedirectUriF0i71s**](#companiescontrollergetredirecturif0i71s) | **GET** /companies/redirect_uri | |
|[**companiesControllerSetRedirectUriFcrzml**](#companiescontrollersetredirecturifcrzml) | **PUT** /companies/redirect_uri | |

# **companiesControllerGetCompany2lyej4**
> companiesControllerGetCompany2lyej4()


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


const { status, data } = await client.companies.companiesControllerGetCompany2lyej4();
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

# **companiesControllerGetRedirectUriF0i71s**
> RedirectUriDTO companiesControllerGetRedirectUriF0i71s()


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


const { status, data } = await client.companies.companiesControllerGetRedirectUriF0i71s();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**RedirectUriDTO**

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

# **companiesControllerSetRedirectUriFcrzml**
> RedirectUriDTO companiesControllerSetRedirectUriFcrzml(redirectUriDTO)


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

const { status, data } = await client.companies.companiesControllerSetRedirectUriFcrzml(
    redirectUriDTO
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **redirectUriDTO** | **RedirectUriDTO**|  | |


### Return type

**RedirectUriDTO**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

