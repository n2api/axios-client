# CampaignsApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCampaigns**](#getcampaigns) | **GET** /campaigns | |

# **getCampaigns**
> getCampaigns()


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


let childResources: Array<ResourceKind>; // List of child resources to include in the response. Example: set childResources to Targeting and AdSet to get a list of Campaigns with their Targetings and AdSets (and the AdSets Targetings) (default to undefined)
let status: Status; // Status of the Campaigns to return. Example: set status to Running to get a list of running Campaigns. (default to undefined)
let platforms: Array<PlatformName>; // List of platforms to include in the response. (default to undefined)
let customers: Array<string>; // List of Customer IDs whose campaigns to include in the response. (default to undefined)
let ids: Array<string>; // List of Campaign IDs to include in the response. Requires platform and customer to be set to a single value. (default to undefined)

const { status, data } = await client.campaigns.getCampaigns(
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
| **childResources** | **Array&lt;ResourceKind&gt;** | List of child resources to include in the response. Example: set childResources to Targeting and AdSet to get a list of Campaigns with their Targetings and AdSets (and the AdSets Targetings) | defaults to undefined|
| **status** | **Status** | Status of the Campaigns to return. Example: set status to Running to get a list of running Campaigns. | defaults to undefined|
| **platforms** | **Array&lt;PlatformName&gt;** | List of platforms to include in the response. | defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose campaigns to include in the response. | defaults to undefined|
| **ids** | **Array&lt;string&gt;** | List of Campaign IDs to include in the response. Requires platform and customer to be set to a single value. | defaults to undefined|


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

