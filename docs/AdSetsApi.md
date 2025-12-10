# AdSetsApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAdsets**](#getadsets) | **GET** /adsets | |

# **getAdsets**
> getAdsets()


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


let childResources: Array<ResourceKind>; //  (default to undefined)
let status: Status; // Status of the AdSets to return. Example: set status to Running to get a list of running AdSets. (default to undefined)
let platforms: Array<PlatformName>; // List of platforms to include in the response. (default to undefined)
let customers: Array<string>; // List of Customer IDs whose AdSets to include in the response. (default to undefined)
let ids: Array<string>; // List of AdSet IDs to include in the response. Requires platform and customer to be set to a single value. (default to undefined)

const { status, data } = await client.adSets.getAdsets(
    childResources,
    status,
    platforms,
    customers,
    ids
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **childResources** | **Array&lt;ResourceKind&gt;** |  | defaults to undefined|
| **status** | **Status** | Status of the AdSets to return. Example: set status to Running to get a list of running AdSets. | defaults to undefined|
| **platforms** | **Array&lt;PlatformName&gt;** | List of platforms to include in the response. | defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose AdSets to include in the response. | defaults to undefined|
| **ids** | **Array&lt;string&gt;** | List of AdSet IDs to include in the response. Requires platform and customer to be set to a single value. | defaults to undefined|


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

