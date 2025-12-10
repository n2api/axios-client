# AdAccountsApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**findAll**](#findall) | **GET** /adaccounts | |

# **findAll**
> findAll()


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


let platforms: Array<PlatformName>; // List of platforms to include in the response. (default to undefined)
let customers: Array<string>; // List of Customer IDs whose AdAccounts to include in the response. (default to undefined)

const { status, data } = await client.adAccounts.findAll(
    platforms,
    customers
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **platforms** | **Array&lt;PlatformName&gt;** | List of platforms to include in the response. | defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose AdAccounts to include in the response. | defaults to undefined|


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

