# ActiveAgentApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**_delete**](#_delete) | **DELETE** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | |
|[**_delete_0**](#_delete_0) | **DELETE** /activeagent/credentials | |
|[**create**](#create) | **POST** /activeagent/campaigns | |
|[**createCustomer**](#createcustomer) | **POST** /activeagent/credentials/customer | |
|[**create_0**](#create_0) | **POST** /activeagent/{resource}/{resourceId}/targeting | |
|[**create_1**](#create_1) | **POST** /activeagent/adsets | |
|[**find**](#find) | **GET** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | |
|[**findAll**](#findall) | **GET** /activeagent/campaigns | |
|[**findAll_0**](#findall_0) | **GET** /activeagent/adsets | |
|[**findAll_1**](#findall_1) | **GET** /activeagent/ads | |
|[**findAll_2**](#findall_2) | **GET** /activeagent/credentials | |
|[**findOne**](#findone) | **GET** /activeagent/campaigns/{id} | |
|[**findOne_0**](#findone_0) | **GET** /activeagent/adsets/{id} | |
|[**findOne_1**](#findone_1) | **GET** /activeagent/ads/{id} | |
|[**getReport**](#getreport) | **GET** /activeagent/campaigns/{id}/report | |
|[**getReport_0**](#getreport_0) | **GET** /activeagent/reporting | |
|[**rawRequestDelete**](#rawrequestdelete) | **DELETE** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawRequestGet**](#rawrequestget) | **GET** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawRequestHead**](#rawrequesthead) | **HEAD** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawRequestOptions**](#rawrequestoptions) | **OPTIONS** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawRequestPatch**](#rawrequestpatch) | **PATCH** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawRequestPost**](#rawrequestpost) | **POST** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawRequestPut**](#rawrequestput) | **PUT** /activeagent/{customerId}/raw/{externalPath} | |
|[**remove**](#remove) | **DELETE** /activeagent/campaigns/{id} | |
|[**remove_0**](#remove_0) | **DELETE** /activeagent/adsets/{id} | |
|[**sync**](#sync) | **PUT** /activeagent/adaccounts | |
|[**syncCustomer**](#synccustomer) | **PUT** /activeagent/adaccounts/customer | |
|[**translate**](#translate) | **POST** /activeagent/campaigns/translate | |
|[**update**](#update) | **PATCH** /activeagent/campaigns/{id} | |
|[**updateOrCreate**](#updateorcreate) | **PUT** /activeagent/{resource}/{resourceId}/targeting | |
|[**update_0**](#update_0) | **PATCH** /activeagent/adsets/{id} | |
|[**update_1**](#update_1) | **PUT** /activeagent/credentials | |
|[**update_2**](#update_2) | **PUT** /activeagent/{resource}/{resourceId}/settings | |

# **_delete**
> _delete()


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


let resource: string; //  (default to undefined)
let resourceId: string; //  (default to undefined)
let targetingKind: Array<string>; //  (default to undefined)

const { status, data } = await client.activeAgent._delete(
    resource,
    resourceId,
    targetingKind
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **resource** | [**string**] |  | defaults to undefined|
| **resourceId** | [**string**] |  | defaults to undefined|
| **targetingKind** | **Array&lt;string&gt;** |  | defaults to undefined|


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

# **_delete_0**
> _delete_0()


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


const { status, data } = await client.activeAgent._delete_0();
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

# **create**
> object create(body)


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


let body: object; // 

const { status, data } = await client.activeAgent.create(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |


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
|**201** | Campaign created successfuly. The created campaign is returned in the response body. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createCustomer**
> createCustomer(activeAgentCreateCredentialDto)


### Example

```typescript
import {
    Client,
    Configuration,
    ActiveAgentCreateCredentialDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let activeAgentCreateCredentialDto: ActiveAgentCreateCredentialDto; // 

const { status, data } = await client.activeAgent.createCustomer(
    activeAgentCreateCredentialDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **activeAgentCreateCredentialDto** | **ActiveAgentCreateCredentialDto**|  | |


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

# **create_0**
> object create_0(createTargetingDto)


### Example

```typescript
import {
    Client,
    Configuration,
    CreateTargetingDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let resource: string; //  (default to undefined)
let resourceId: string; //  (default to undefined)
let createTargetingDto: CreateTargetingDto; // 

const { status, data } = await client.activeAgent.create_0(
    resource,
    resourceId,
    createTargetingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTargetingDto** | **CreateTargetingDto**|  | |
| **resource** | [**string**] |  | defaults to undefined|
| **resourceId** | [**string**] |  | defaults to undefined|


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
|**201** | Targeting created successfully. The created targeting is returned in the response body. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_1**
> create_1(body)


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


let body: object; // 

const { status, data } = await client.activeAgent.create_1(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |


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

# **find**
> find()


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


let resource: string; //  (default to undefined)
let resourceId: string; //  (default to undefined)
let targetingKind: Array<string>; //  (default to undefined)

const { status, data } = await client.activeAgent.find(
    resource,
    resourceId,
    targetingKind
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **resource** | [**string**] |  | defaults to undefined|
| **resourceId** | [**string**] |  | defaults to undefined|
| **targetingKind** | **Array&lt;string&gt;** |  | defaults to undefined|


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


let childResources: Array<ResourceKind>; // List of child resources to include in the response. Example: set childResources to Targeting and AdSet to get a list of Campaigns with their Targetings and AdSets (and the AdSets Targetings) (default to undefined)
let status: Status; // Status of the Campaigns to return. Example: set status to Running to get a list of running Campaigns. (default to undefined)
let platforms: Array<PlatformName>; // List of platforms to include in the response. (default to undefined)
let customers: Array<string>; // List of Customer IDs whose campaigns to include in the response. (default to undefined)
let ids: Array<string>; // List of Campaign IDs to include in the response. Requires platform and customer to be set to a single value. (default to undefined)

const { status, data } = await client.activeAgent.findAll(
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

# **findAll_0**
> findAll_0()


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

const { status, data } = await client.activeAgent.findAll_0(
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

# **findAll_1**
> findAll_1()


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


let childResources: Array<ResourceKind>; // List of child resources to include in the response. Example: set childResources to Targeting to get a list of Ads with their Targetings (default to undefined)
let status: Status; // Status of the Ads to return. Example: set status to Running to get a list of running Ads (default to undefined)
let platforms: Array<PlatformName>; // List of platforms to include in the response. (default to undefined)
let customers: Array<string>; // List of Customer IDs whose Ads to include in the response. (default to undefined)
let ids: Array<string>; // List of Ad IDs to include in the response. Requires platform and customer to be set to a single value. (default to undefined)

const { status, data } = await client.activeAgent.findAll_1(
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
| **childResources** | **Array&lt;ResourceKind&gt;** | List of child resources to include in the response. Example: set childResources to Targeting to get a list of Ads with their Targetings | defaults to undefined|
| **status** | **Status** | Status of the Ads to return. Example: set status to Running to get a list of running Ads | defaults to undefined|
| **platforms** | **Array&lt;PlatformName&gt;** | List of platforms to include in the response. | defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose Ads to include in the response. | defaults to undefined|
| **ids** | **Array&lt;string&gt;** | List of Ad IDs to include in the response. Requires platform and customer to be set to a single value. | defaults to undefined|


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

# **findAll_2**
> findAll_2()


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


const { status, data } = await client.activeAgent.findAll_2();
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

# **findOne**
> findOne()


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


let id: string; //  (default to undefined)
let childResources: string; // Comma separated list of child resources to include in the response. Possible values: Campaign, AdSet, Ad, Targeting (default to undefined)
let countCalls: boolean; // If true, the number of calls made to the API is returned in the response body. (optional) (default to undefined)

const { status, data } = await client.activeAgent.findOne(
    id,
    childResources,
    countCalls
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **childResources** | [**string**] | Comma separated list of child resources to include in the response. Possible values: Campaign, AdSet, Ad, Targeting | defaults to undefined|
| **countCalls** | [**boolean**] | If true, the number of calls made to the API is returned in the response body. | (optional) defaults to undefined|


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

# **findOne_0**
> findOne_0()


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


let id: string; //  (default to undefined)
let childResources: string; //  (default to undefined)

const { status, data } = await client.activeAgent.findOne_0(
    id,
    childResources
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **childResources** | [**string**] |  | defaults to undefined|


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

# **findOne_1**
> findOne_1()


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


let id: string; //  (default to undefined)
let childResources: string; // Comma separated list of child resources to include in the response. Possible values: Campaign, AdSet, Ad, Targeting (default to undefined)
let countCalls: boolean; // If true, the number of calls made to the API is returned in the response body. (optional) (default to undefined)

const { status, data } = await client.activeAgent.findOne_1(
    id,
    childResources,
    countCalls
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **childResources** | [**string**] | Comma separated list of child resources to include in the response. Possible values: Campaign, AdSet, Ad, Targeting | defaults to undefined|
| **countCalls** | [**boolean**] | If true, the number of calls made to the API is returned in the response body. | (optional) defaults to undefined|


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


let id: string; //  (default to undefined)
let start: string; // Start date of the report. This is the \"earlier\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (default to undefined)
let end: string; // End date of the report. This is the \"later\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (default to undefined)

const { status, data } = await client.activeAgent.getReport(
    id,
    start,
    end
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **start** | [**string**] | Start date of the report. This is the \&quot;earlier\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | defaults to undefined|
| **end** | [**string**] | End date of the report. This is the \&quot;later\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | defaults to undefined|


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

# **getReport_0**
> getReport_0()


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

const { status, data } = await client.activeAgent.getReport_0(
    start,
    end
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **start** | [**string**] | Start date of the report. This is the \&quot;earlier\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | defaults to undefined|
| **end** | [**string**] | End date of the report. This is the \&quot;later\&quot; of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. | defaults to undefined|


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

# **rawRequestDelete**
> rawRequestDelete()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestDelete(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **rawRequestGet**
> rawRequestGet()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestGet(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **rawRequestHead**
> rawRequestHead()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestHead(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **rawRequestOptions**
> rawRequestOptions()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestOptions(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **rawRequestPatch**
> rawRequestPatch()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestPatch(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **rawRequestPost**
> rawRequestPost()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestPost(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **rawRequestPut**
> rawRequestPut()


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


let customerId: string; // Customer UUID (default to undefined)
let externalPath: string; // The external path for the ActiveAgent API request. (default to undefined)

const { status, data } = await client.activeAgent.rawRequestPut(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the ActiveAgent API request. | defaults to undefined|


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

# **remove**
> remove()


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


let id: string; //  (default to undefined)

const { status, data } = await client.activeAgent.remove(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


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

# **remove_0**
> remove_0()


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


let id: string; //  (default to undefined)

const { status, data } = await client.activeAgent.remove_0(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


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

# **sync**
> sync()


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


const { status, data } = await client.activeAgent.sync();
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

# **syncCustomer**
> syncCustomer()


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


const { status, data } = await client.activeAgent.syncCustomer();
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

# **translate**
> translate(body)


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


let childResources: string; //  (default to undefined)
let body: object; // 

const { status, data } = await client.activeAgent.translate(
    childResources,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |
| **childResources** | [**string**] |  | defaults to undefined|


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

# **update**
> update(body)


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


let id: string; //  (default to undefined)
let body: object; // 

const { status, data } = await client.activeAgent.update(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |
| **id** | [**string**] |  | defaults to undefined|


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

# **updateOrCreate**
> updateOrCreate(createTargetingDto)


### Example

```typescript
import {
    Client,
    Configuration,
    CreateTargetingDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let resource: string; //  (default to undefined)
let resourceId: string; //  (default to undefined)
let createTargetingDto: CreateTargetingDto; // 

const { status, data } = await client.activeAgent.updateOrCreate(
    resource,
    resourceId,
    createTargetingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTargetingDto** | **CreateTargetingDto**|  | |
| **resource** | [**string**] |  | defaults to undefined|
| **resourceId** | [**string**] |  | defaults to undefined|


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

# **update_0**
> update_0(body)


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


let id: string; //  (default to undefined)
let body: object; // 

const { status, data } = await client.activeAgent.update_0(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |
| **id** | [**string**] |  | defaults to undefined|


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

# **update_1**
> update_1(activeAgentCreateCredentialDto)


### Example

```typescript
import {
    Client,
    Configuration,
    ActiveAgentCreateCredentialDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let activeAgentCreateCredentialDto: ActiveAgentCreateCredentialDto; // 

const { status, data } = await client.activeAgent.update_1(
    activeAgentCreateCredentialDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **activeAgentCreateCredentialDto** | **ActiveAgentCreateCredentialDto**|  | |


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

# **update_2**
> update_2(createSettingDto)


### Example

```typescript
import {
    Client,
    Configuration,
    CreateSettingDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let resource: string; //  (default to undefined)
let resourceId: string; //  (default to undefined)
let createSettingDto: CreateSettingDto; // 

const { status, data } = await client.activeAgent.update_2(
    resource,
    resourceId,
    createSettingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createSettingDto** | **CreateSettingDto**|  | |
| **resource** | [**string**] |  | defaults to undefined|
| **resourceId** | [**string**] |  | defaults to undefined|


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

