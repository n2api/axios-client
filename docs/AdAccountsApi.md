# AdAccountsApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adAccountsControllerFindAll1f63wu**](#adaccountscontrollerfindall1f63wu) | **GET** /adaccounts | |

# **adAccountsControllerFindAll1f63wu**
> Array<object> adAccountsControllerFindAll1f63wu()


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


let platforms: Array<'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest'>; // List of platforms to include in the response. (optional) (default to undefined)
let customers: Array<string>; // List of Customer IDs whose AdAccounts to include in the response. (optional) (default to undefined)

const { status, data } = await client.adAccounts.adAccountsControllerFindAll1f63wu(
    platforms,
    customers
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **platforms** | **Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39;>** | List of platforms to include in the response. | (optional) defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose AdAccounts to include in the response. | (optional) defaults to undefined|


### Return type

**Array<object>**

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

