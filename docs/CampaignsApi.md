# CampaignsApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**campaignsControllerGetCampaigns2qcanu**](#campaignscontrollergetcampaigns2qcanu) | **GET** /campaigns | |

# **campaignsControllerGetCampaigns2qcanu**
> Array<Campaign> campaignsControllerGetCampaigns2qcanu()


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


let childResources: Array<'Campaign' | 'AdSet' | 'Ad' | 'Targeting' | 'AdAccount'>; // List of child resources to include in the response. Example: set childResources to Targeting and AdSet to get a list of Campaigns with their Targetings and AdSets (and the AdSets Targetings) (optional) (default to undefined)
let status: 'ACTIVE' | 'RUNNING' | 'PAUSED' | 'UNKNOWN'; // Status of the Campaigns to return. Example: set status to Running to get a list of running Campaigns. (optional) (default to undefined)
let platforms: Array<'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest'>; // List of platforms to include in the response. (optional) (default to undefined)
let customers: Array<string>; // List of Customer IDs whose campaigns to include in the response. (optional) (default to undefined)
let ids: Array<string>; // List of Campaign IDs to include in the response. Requires platform and customer to be set to a single value. (optional) (default to undefined)

const { status, data } = await client.campaigns.campaignsControllerGetCampaigns2qcanu(
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
| **childResources** | **Array<&#39;Campaign&#39; &#124; &#39;AdSet&#39; &#124; &#39;Ad&#39; &#124; &#39;Targeting&#39; &#124; &#39;AdAccount&#39;>** | List of child resources to include in the response. Example: set childResources to Targeting and AdSet to get a list of Campaigns with their Targetings and AdSets (and the AdSets Targetings) | (optional) defaults to undefined|
| **status** | [**&#39;ACTIVE&#39; | &#39;RUNNING&#39; | &#39;PAUSED&#39; | &#39;UNKNOWN&#39;**]**Array<&#39;ACTIVE&#39; &#124; &#39;RUNNING&#39; &#124; &#39;PAUSED&#39; &#124; &#39;UNKNOWN&#39;>** | Status of the Campaigns to return. Example: set status to Running to get a list of running Campaigns. | (optional) defaults to undefined|
| **platforms** | **Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39;>** | List of platforms to include in the response. | (optional) defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose campaigns to include in the response. | (optional) defaults to undefined|
| **ids** | **Array&lt;string&gt;** | List of Campaign IDs to include in the response. Requires platform and customer to be set to a single value. | (optional) defaults to undefined|


### Return type

**Array<Campaign>**

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

