# ReportingApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getReport**](#getreport) | **GET** /reporting | |

# **getReport**
> getReport()


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


let start: string; // Start date of the report. This is the \"earlier\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (default to undefined)
let end: string; // End date of the report. This is the \"later\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (default to undefined)
let platform: PlatformName; // The platform for which to generate the report. (default to undefined)

const { status, data } = await client.reporting.getReport(
    start,
    end,
    platform
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **start** | [**string**] | Start date of the report. This is the \&quot;earlier\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | defaults to undefined|
| **end** | [**string**] | End date of the report. This is the \&quot;later\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | defaults to undefined|
| **platform** | **PlatformName** | The platform for which to generate the report. | defaults to undefined|


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

