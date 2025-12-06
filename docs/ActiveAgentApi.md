# ActiveAgentApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adAccountsControllerSyncCustomerQ7yxiw**](#adaccountscontrollersynccustomerq7yxiw) | **PUT** /activeagent/adaccounts/customer | |
|[**adAccountsControllerSyncR5ln7z**](#adaccountscontrollersyncr5ln7z) | **PUT** /activeagent/adaccounts | |
|[**adsControllerFindAllV0i00i**](#adscontrollerfindallv0i00i) | **GET** /activeagent/ads | |
|[**adsControllerFindOneKx2rz2**](#adscontrollerfindonekx2rz2) | **GET** /activeagent/ads/{id} | |
|[**adsetsControllerCreate7ajntd**](#adsetscontrollercreate7ajntd) | **POST** /activeagent/adsets | |
|[**adsetsControllerFindAll48b5vs**](#adsetscontrollerfindall48b5vs) | **GET** /activeagent/adsets | |
|[**adsetsControllerFindOneFfcces**](#adsetscontrollerfindoneffcces) | **GET** /activeagent/adsets/{id} | |
|[**adsetsControllerRemoveJnaag7**](#adsetscontrollerremovejnaag7) | **DELETE** /activeagent/adsets/{id} | |
|[**adsetsControllerUpdate31j4du**](#adsetscontrollerupdate31j4du) | **PATCH** /activeagent/adsets/{id} | |
|[**campaignsControllerCreateLsx4bk**](#campaignscontrollercreatelsx4bk) | **POST** /activeagent/campaigns | |
|[**campaignsControllerFindAllVkjjqn**](#campaignscontrollerfindallvkjjqn) | **GET** /activeagent/campaigns | |
|[**campaignsControllerFindOne32heet**](#campaignscontrollerfindone32heet) | **GET** /activeagent/campaigns/{id} | |
|[**campaignsControllerGetReport11en29**](#campaignscontrollergetreport11en29) | **GET** /activeagent/campaigns/{id}/report | |
|[**campaignsControllerRemoveWx2dfy**](#campaignscontrollerremovewx2dfy) | **DELETE** /activeagent/campaigns/{id} | |
|[**campaignsControllerTranslateEcvpl4**](#campaignscontrollertranslateecvpl4) | **POST** /activeagent/campaigns/translate | |
|[**campaignsControllerUpdate058yv3**](#campaignscontrollerupdate058yv3) | **PATCH** /activeagent/campaigns/{id} | |
|[**credentialsControllerCreateCustomer6ix19k**](#credentialscontrollercreatecustomer6ix19k) | **POST** /activeagent/credentials/customer | |
|[**credentialsControllerDeleteLt023k**](#credentialscontrollerdeletelt023k) | **DELETE** /activeagent/credentials | |
|[**credentialsControllerFindAllHu0kra**](#credentialscontrollerfindallhu0kra) | **GET** /activeagent/credentials | |
|[**credentialsControllerUpdateU7kaen**](#credentialscontrollerupdateu7kaen) | **PUT** /activeagent/credentials | |
|[**rawControllerRawRequest2jfj97Post**](#rawcontrollerrawrequest2jfj97post) | **POST** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequest5ryooeGet**](#rawcontrollerrawrequest5ryooeget) | **GET** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequest7bmyr4Patch**](#rawcontrollerrawrequest7bmyr4patch) | **PATCH** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequest7qnyhrHead**](#rawcontrollerrawrequest7qnyhrhead) | **HEAD** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestGpk4z6Put**](#rawcontrollerrawrequestgpk4z6put) | **PUT** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestO6zyiqDelete**](#rawcontrollerrawrequesto6zyiqdelete) | **DELETE** /activeagent/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestT080myOptions**](#rawcontrollerrawrequestt080myoptions) | **OPTIONS** /activeagent/{customerId}/raw/{externalPath} | |
|[**reportingControllerGetReportOj3kae**](#reportingcontrollergetreportoj3kae) | **GET** /activeagent/reporting | |
|[**settingsControllerUpdate6xv72v**](#settingscontrollerupdate6xv72v) | **PUT** /activeagent/{resource}/{resourceId}/settings | |
|[**targetingControllerCreate36thcg**](#targetingcontrollercreate36thcg) | **POST** /activeagent/{resource}/{resourceId}/targeting | |
|[**targetingControllerDelete3swtka**](#targetingcontrollerdelete3swtka) | **DELETE** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | |
|[**targetingControllerFind5148tb**](#targetingcontrollerfind5148tb) | **GET** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | |
|[**targetingControllerUpdateOrCreate2h20li**](#targetingcontrollerupdateorcreate2h20li) | **PUT** /activeagent/{resource}/{resourceId}/targeting | |

# **adAccountsControllerSyncCustomerQ7yxiw**
> adAccountsControllerSyncCustomerQ7yxiw()


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


const { status, data } = await client.activeAgent.adAccountsControllerSyncCustomerQ7yxiw();
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

# **adAccountsControllerSyncR5ln7z**
> adAccountsControllerSyncR5ln7z()


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


const { status, data } = await client.activeAgent.adAccountsControllerSyncR5ln7z();
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

# **adsControllerFindAllV0i00i**
> Array<Ad> adsControllerFindAllV0i00i()


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


let childResources: Array<'Campaign' | 'AdSet' | 'Ad' | 'Targeting' | 'AdAccount'>; // List of child resources to include in the response. Example: set childResources to Targeting to get a list of Ads with their Targetings (optional) (default to undefined)
let status: 'ACTIVE' | 'RUNNING' | 'PAUSED' | 'UNKNOWN'; // Status of the Ads to return. Example: set status to Running to get a list of running Ads (optional) (default to undefined)
let platforms: Array<'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest'>; // List of platforms to include in the response. (optional) (default to undefined)
let customers: Array<string>; // List of Customer IDs whose Ads to include in the response. (optional) (default to undefined)
let ids: Array<string>; // List of Ad IDs to include in the response. Requires platform and customer to be set to a single value. (optional) (default to undefined)

const { status, data } = await client.activeAgent.adsControllerFindAllV0i00i(
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
| **childResources** | **Array<&#39;Campaign&#39; &#124; &#39;AdSet&#39; &#124; &#39;Ad&#39; &#124; &#39;Targeting&#39; &#124; &#39;AdAccount&#39;>** | List of child resources to include in the response. Example: set childResources to Targeting to get a list of Ads with their Targetings | (optional) defaults to undefined|
| **status** | [**&#39;ACTIVE&#39; | &#39;RUNNING&#39; | &#39;PAUSED&#39; | &#39;UNKNOWN&#39;**]**Array<&#39;ACTIVE&#39; &#124; &#39;RUNNING&#39; &#124; &#39;PAUSED&#39; &#124; &#39;UNKNOWN&#39;>** | Status of the Ads to return. Example: set status to Running to get a list of running Ads | (optional) defaults to undefined|
| **platforms** | **Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39;>** | List of platforms to include in the response. | (optional) defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose Ads to include in the response. | (optional) defaults to undefined|
| **ids** | **Array&lt;string&gt;** | List of Ad IDs to include in the response. Requires platform and customer to be set to a single value. | (optional) defaults to undefined|


### Return type

**Array<Ad>**

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

# **adsControllerFindOneKx2rz2**
> object adsControllerFindOneKx2rz2()


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

const { status, data } = await client.activeAgent.adsControllerFindOneKx2rz2(
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

# **adsetsControllerCreate7ajntd**
> object adsetsControllerCreate7ajntd(body)


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

const { status, data } = await client.activeAgent.adsetsControllerCreate7ajntd(
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
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **adsetsControllerFindAll48b5vs**
> Array<AdSet> adsetsControllerFindAll48b5vs()


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


let childResources: Array<'Campaign' | 'AdSet' | 'Ad' | 'Targeting' | 'AdAccount'>; //  (optional) (default to undefined)
let platforms: Array<'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest'>; // List of platforms to include in the response. (optional) (default to undefined)
let customers: Array<string>; // List of Customer IDs whose AdSets to include in the response. (optional) (default to undefined)
let ids: Array<string>; // List of AdSet IDs to include in the response. Requires platform and customer to be set to a single value. (optional) (default to undefined)
let status: 'ACTIVE' | 'RUNNING' | 'PAUSED' | 'UNKNOWN'; //  (optional) (default to undefined)

const { status, data } = await client.activeAgent.adsetsControllerFindAll48b5vs(
    childResources,
    platforms,
    customers,
    ids,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **childResources** | **Array<&#39;Campaign&#39; &#124; &#39;AdSet&#39; &#124; &#39;Ad&#39; &#124; &#39;Targeting&#39; &#124; &#39;AdAccount&#39;>** |  | (optional) defaults to undefined|
| **platforms** | **Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39;>** | List of platforms to include in the response. | (optional) defaults to undefined|
| **customers** | **Array&lt;string&gt;** | List of Customer IDs whose AdSets to include in the response. | (optional) defaults to undefined|
| **ids** | **Array&lt;string&gt;** | List of AdSet IDs to include in the response. Requires platform and customer to be set to a single value. | (optional) defaults to undefined|
| **status** | [**&#39;ACTIVE&#39; | &#39;RUNNING&#39; | &#39;PAUSED&#39; | &#39;UNKNOWN&#39;**]**Array<&#39;ACTIVE&#39; &#124; &#39;RUNNING&#39; &#124; &#39;PAUSED&#39; &#124; &#39;UNKNOWN&#39;>** |  | (optional) defaults to undefined|


### Return type

**Array<AdSet>**

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

# **adsetsControllerFindOneFfcces**
> AdSet adsetsControllerFindOneFfcces()


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

const { status, data } = await client.activeAgent.adsetsControllerFindOneFfcces(
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

**AdSet**

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

# **adsetsControllerRemoveJnaag7**
> object adsetsControllerRemoveJnaag7()


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

const { status, data } = await client.activeAgent.adsetsControllerRemoveJnaag7(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


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

# **adsetsControllerUpdate31j4du**
> string adsetsControllerUpdate31j4du(body)


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

const { status, data } = await client.activeAgent.adsetsControllerUpdate31j4du(
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

**string**

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

# **campaignsControllerCreateLsx4bk**
> object campaignsControllerCreateLsx4bk(body)


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

const { status, data } = await client.activeAgent.campaignsControllerCreateLsx4bk(
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

# **campaignsControllerFindAllVkjjqn**
> Array<Campaign> campaignsControllerFindAllVkjjqn()


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

const { status, data } = await client.activeAgent.campaignsControllerFindAllVkjjqn(
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

# **campaignsControllerFindOne32heet**
> object campaignsControllerFindOne32heet()


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

const { status, data } = await client.activeAgent.campaignsControllerFindOne32heet(
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

# **campaignsControllerGetReport11en29**
> object campaignsControllerGetReport11en29()


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
let granularity: string; //  (default to undefined)
let dimensions: string; //  (default to undefined)
let fields: string; //  (default to undefined)
let start: string; // Start date of the report. This is the \"earlier\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (optional) (default to undefined)
let end: string; // End date of the report. This is the \"later\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (optional) (default to undefined)
let filters: string; //  (optional) (default to undefined)
let callCounter: boolean; //  (optional) (default to undefined)

const { status, data } = await client.activeAgent.campaignsControllerGetReport11en29(
    id,
    granularity,
    dimensions,
    fields,
    start,
    end,
    filters,
    callCounter
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **granularity** | [**string**] |  | defaults to undefined|
| **dimensions** | [**string**] |  | defaults to undefined|
| **fields** | [**string**] |  | defaults to undefined|
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

# **campaignsControllerRemoveWx2dfy**
> object campaignsControllerRemoveWx2dfy()


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

const { status, data } = await client.activeAgent.campaignsControllerRemoveWx2dfy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


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

# **campaignsControllerTranslateEcvpl4**
> Campaign campaignsControllerTranslateEcvpl4(activeAgentOrderDto)


### Example

```typescript
import {
    Client,
    Configuration,
    ActiveAgentOrderDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let childResources: string; //  (default to undefined)
let activeAgentOrderDto: ActiveAgentOrderDto; // 

const { status, data } = await client.activeAgent.campaignsControllerTranslateEcvpl4(
    childResources,
    activeAgentOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **activeAgentOrderDto** | **ActiveAgentOrderDto**|  | |
| **childResources** | [**string**] |  | defaults to undefined|


### Return type

**Campaign**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **campaignsControllerUpdate058yv3**
> Campaign campaignsControllerUpdate058yv3(body)


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

const { status, data } = await client.activeAgent.campaignsControllerUpdate058yv3(
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

**Campaign**

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

# **credentialsControllerCreateCustomer6ix19k**
> credentialsControllerCreateCustomer6ix19k(activeAgentCreateCredentialDto)


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

const { status, data } = await client.activeAgent.credentialsControllerCreateCustomer6ix19k(
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

# **credentialsControllerDeleteLt023k**
> credentialsControllerDeleteLt023k()


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


const { status, data } = await client.activeAgent.credentialsControllerDeleteLt023k();
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

# **credentialsControllerFindAllHu0kra**
> Array<object> credentialsControllerFindAllHu0kra()


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


const { status, data } = await client.activeAgent.credentialsControllerFindAllHu0kra();
```

### Parameters
This endpoint does not have any parameters.


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

# **credentialsControllerUpdateU7kaen**
> credentialsControllerUpdateU7kaen(activeAgentCreateCredentialDto)


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

const { status, data } = await client.activeAgent.credentialsControllerUpdateU7kaen(
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

# **rawControllerRawRequest2jfj97Post**
> rawControllerRawRequest2jfj97Post()


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

const { status, data } = await client.activeAgent.rawControllerRawRequest2jfj97Post(
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

# **rawControllerRawRequest5ryooeGet**
> rawControllerRawRequest5ryooeGet()


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

const { status, data } = await client.activeAgent.rawControllerRawRequest5ryooeGet(
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

# **rawControllerRawRequest7bmyr4Patch**
> rawControllerRawRequest7bmyr4Patch()


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

const { status, data } = await client.activeAgent.rawControllerRawRequest7bmyr4Patch(
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

# **rawControllerRawRequest7qnyhrHead**
> rawControllerRawRequest7qnyhrHead()


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

const { status, data } = await client.activeAgent.rawControllerRawRequest7qnyhrHead(
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

# **rawControllerRawRequestGpk4z6Put**
> rawControllerRawRequestGpk4z6Put()


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

const { status, data } = await client.activeAgent.rawControllerRawRequestGpk4z6Put(
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

# **rawControllerRawRequestO6zyiqDelete**
> rawControllerRawRequestO6zyiqDelete()


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

const { status, data } = await client.activeAgent.rawControllerRawRequestO6zyiqDelete(
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

# **rawControllerRawRequestT080myOptions**
> rawControllerRawRequestT080myOptions()


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

const { status, data } = await client.activeAgent.rawControllerRawRequestT080myOptions(
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

# **reportingControllerGetReportOj3kae**
> object reportingControllerGetReportOj3kae()


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
let start: string; // Start date of the report. This is the \"earlier\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (optional) (default to undefined)
let end: string; // End date of the report. This is the \"later\" of the two dates. Example: set start to 2021-01-01 and end to 2021-01-31 to get a report for the month of January 2021. (optional) (default to undefined)
let filters: string; //  (optional) (default to undefined)
let callCounter: boolean; //  (optional) (default to undefined)

const { status, data } = await client.activeAgent.reportingControllerGetReportOj3kae(
    granularity,
    dimensions,
    fields,
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

# **settingsControllerUpdate6xv72v**
> Array<object> settingsControllerUpdate6xv72v(createSettingDto)


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

const { status, data } = await client.activeAgent.settingsControllerUpdate6xv72v(
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

**Array<object>**

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

# **targetingControllerCreate36thcg**
> ZipcodeGeoTargetingDto targetingControllerCreate36thcg(createTargetingDto)


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

const { status, data } = await client.activeAgent.targetingControllerCreate36thcg(
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

**ZipcodeGeoTargetingDto**

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

# **targetingControllerDelete3swtka**
> number targetingControllerDelete3swtka()


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

const { status, data } = await client.activeAgent.targetingControllerDelete3swtka(
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

**number**

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

# **targetingControllerFind5148tb**
> Array<object> targetingControllerFind5148tb()


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

const { status, data } = await client.activeAgent.targetingControllerFind5148tb(
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

# **targetingControllerUpdateOrCreate2h20li**
> object targetingControllerUpdateOrCreate2h20li(createTargetingDto)


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

const { status, data } = await client.activeAgent.targetingControllerUpdateOrCreate2h20li(
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
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

