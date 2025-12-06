# ReportingApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**reportingControllerGetReportIxk9wf**](#reportingcontrollergetreportixk9wf) | **GET** /reporting | |

# **reportingControllerGetReportIxk9wf**
> object reportingControllerGetReportIxk9wf()


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


let granularity: string; //  (default to undefined)
let dimensions: string; //  (default to undefined)
let fields: string; //  (default to undefined)
let platform: 'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest'; //  (default to undefined)
let start: string; // Start date of the report. This is the \"earlier\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (optional) (default to undefined)
let end: string; // End date of the report. This is the \"later\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (optional) (default to undefined)
let filters: string; //  (optional) (default to undefined)
let callCounter: boolean; //  (optional) (default to undefined)

const { status, data } = await client.reporting.reportingControllerGetReportIxk9wf(
    granularity,
    dimensions,
    fields,
    platform,
    start,
    end,
    filters,
    callCounter
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **granularity** | [**string**] |  | defaults to undefined|
| **dimensions** | [**string**] |  | defaults to undefined|
| **fields** | [**string**] |  | defaults to undefined|
| **platform** | [**&#39;ActiveAgent&#39; | &#39;Facebook&#39; | &#39;GoogleAds&#39; | &#39;TheTradeDesk&#39; | &#39;Pinterest&#39;**]**Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39;>** |  | defaults to undefined|
| **start** | [**string**] | Start date of the report. This is the \&quot;earlier\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | (optional) defaults to undefined|
| **end** | [**string**] | End date of the report. This is the \&quot;later\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | (optional) defaults to undefined|
| **filters** | [**string**] |  | (optional) defaults to undefined|
| **callCounter** | [**boolean**] |  | (optional) defaults to undefined|


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

