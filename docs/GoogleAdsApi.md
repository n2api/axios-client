# GoogleAdsApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adAccountsControllerFindAllMln5nd**](#adaccountscontrollerfindallmln5nd) | **GET** /googleads/adaccounts | |
|[**adAccountsControllerSyncCustomer2j6xn9**](#adaccountscontrollersynccustomer2j6xn9) | **PUT** /googleads/{customerId}/adaccounts | |
|[**adsControllerCreate5j1f9u**](#adscontrollercreate5j1f9u) | **POST** /googleads/ads | |
|[**adsControllerFindAllErdkms**](#adscontrollerfindallerdkms) | **GET** /googleads/ads | |
|[**adsControllerFindOneNutbxl**](#adscontrollerfindonenutbxl) | **GET** /googleads/ads/{id} | |
|[**adsControllerRemoveAhonpn**](#adscontrollerremoveahonpn) | **DELETE** /googleads/ads/{id} | |
|[**adsControllerUpdateT99o7f**](#adscontrollerupdatet99o7f) | **PATCH** /googleads/ads/{id} | |
|[**adsetsControllerCreateX8svw5**](#adsetscontrollercreatex8svw5) | **POST** /googleads/adsets | |
|[**adsetsControllerFindAll9d7h31**](#adsetscontrollerfindall9d7h31) | **GET** /googleads/adsets | |
|[**adsetsControllerFindOne3q406b**](#adsetscontrollerfindone3q406b) | **GET** /googleads/adsets/{id} | |
|[**adsetsControllerRemoveIariyn**](#adsetscontrollerremoveiariyn) | **DELETE** /googleads/adsets/{id} | |
|[**adsetsControllerUpdateQb6632**](#adsetscontrollerupdateqb6632) | **PATCH** /googleads/adsets/{id} | |
|[**authControllerGetAccessToken69qgkv**](#authcontrollergetaccesstoken69qgkv) | **POST** /googleads/auth | |
|[**campaignsControllerCreateWi0t68**](#campaignscontrollercreatewi0t68) | **POST** /googleads/campaigns | |
|[**campaignsControllerFindAllJazafv**](#campaignscontrollerfindalljazafv) | **GET** /googleads/campaigns | |
|[**campaignsControllerFindOneU27hua**](#campaignscontrollerfindoneu27hua) | **GET** /googleads/campaigns/{id} | |
|[**campaignsControllerRemoveWvf99p**](#campaignscontrollerremovewvf99p) | **DELETE** /googleads/campaigns/{id} | |
|[**campaignsControllerUpdate40ll7r**](#campaignscontrollerupdate40ll7r) | **PATCH** /googleads/campaigns/{id} | |
|[**credentialsControllerCreateCustomer8qpv6w**](#credentialscontrollercreatecustomer8qpv6w) | **POST** /googleads/credentials/customer | |
|[**credentialsControllerDeleteCustomerCredentialsSiel2b**](#credentialscontrollerdeletecustomercredentialssiel2b) | **DELETE** /googleads/{customerId}/credentials | |
|[**credentialsControllerFindAll9quhk2**](#credentialscontrollerfindall9quhk2) | **GET** /googleads/credentials | |
|[**rawControllerRawRequest60eqvdPost**](#rawcontrollerrawrequest60eqvdpost) | **POST** /googleads/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequest7vtbrnGet**](#rawcontrollerrawrequest7vtbrnget) | **GET** /googleads/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestAfsh4hDelete**](#rawcontrollerrawrequestafsh4hdelete) | **DELETE** /googleads/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestD0r8raHead**](#rawcontrollerrawrequestd0r8rahead) | **HEAD** /googleads/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestF0ip1pOptions**](#rawcontrollerrawrequestf0ip1poptions) | **OPTIONS** /googleads/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestH2cub1Put**](#rawcontrollerrawrequesth2cub1put) | **PUT** /googleads/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestWg2qdkPatch**](#rawcontrollerrawrequestwg2qdkpatch) | **PATCH** /googleads/{customerId}/raw/{externalPath} | |

# **adAccountsControllerFindAllMln5nd**
> Array<GoogleAdsAdAccountWrapper> adAccountsControllerFindAllMln5nd()


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


const { status, data } = await client.googleAds.adAccountsControllerFindAllMln5nd();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<GoogleAdsAdAccountWrapper>**

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

# **adAccountsControllerSyncCustomer2j6xn9**
> adAccountsControllerSyncCustomer2j6xn9()


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


let customerId: string; //  (default to undefined)

const { status, data } = await client.googleAds.adAccountsControllerSyncCustomer2j6xn9(
    customerId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] |  | defaults to undefined|


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

# **adsControllerCreate5j1f9u**
> string adsControllerCreate5j1f9u(body)


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

const { status, data } = await client.googleAds.adsControllerCreate5j1f9u(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |


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
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **adsControllerFindAllErdkms**
> Array<Ad> adsControllerFindAllErdkms()


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

const { status, data } = await client.googleAds.adsControllerFindAllErdkms(
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

# **adsControllerFindOneNutbxl**
> string adsControllerFindOneNutbxl()


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

const { status, data } = await client.googleAds.adsControllerFindOneNutbxl(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **adsControllerRemoveAhonpn**
> string adsControllerRemoveAhonpn()


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

const { status, data } = await client.googleAds.adsControllerRemoveAhonpn(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **adsControllerUpdateT99o7f**
> string adsControllerUpdateT99o7f(body)


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

const { status, data } = await client.googleAds.adsControllerUpdateT99o7f(
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

# **adsetsControllerCreateX8svw5**
> string adsetsControllerCreateX8svw5(body)


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

const { status, data } = await client.googleAds.adsetsControllerCreateX8svw5(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |


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
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **adsetsControllerFindAll9d7h31**
> Array<AdSet> adsetsControllerFindAll9d7h31()


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

const { status, data } = await client.googleAds.adsetsControllerFindAll9d7h31(
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

# **adsetsControllerFindOne3q406b**
> string adsetsControllerFindOne3q406b()


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

const { status, data } = await client.googleAds.adsetsControllerFindOne3q406b(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **adsetsControllerRemoveIariyn**
> string adsetsControllerRemoveIariyn()


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

const { status, data } = await client.googleAds.adsetsControllerRemoveIariyn(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **adsetsControllerUpdateQb6632**
> string adsetsControllerUpdateQb6632(body)


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

const { status, data } = await client.googleAds.adsetsControllerUpdateQb6632(
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

# **authControllerGetAccessToken69qgkv**
> object authControllerGetAccessToken69qgkv(createGoogleAdsAuthDto)


### Example

```typescript
import {
    Client,
    Configuration,
    CreateGoogleAdsAuthDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let createGoogleAdsAuthDto: CreateGoogleAdsAuthDto; // 

const { status, data } = await client.googleAds.authControllerGetAccessToken69qgkv(
    createGoogleAdsAuthDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createGoogleAdsAuthDto** | **CreateGoogleAdsAuthDto**|  | |


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

# **campaignsControllerCreateWi0t68**
> string campaignsControllerCreateWi0t68(body)


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

const { status, data } = await client.googleAds.campaignsControllerCreateWi0t68(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |


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
|**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **campaignsControllerFindAllJazafv**
> campaignsControllerFindAllJazafv()


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

const { status, data } = await client.googleAds.campaignsControllerFindAllJazafv(
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

# **campaignsControllerFindOneU27hua**
> string campaignsControllerFindOneU27hua()


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

const { status, data } = await client.googleAds.campaignsControllerFindOneU27hua(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **campaignsControllerRemoveWvf99p**
> string campaignsControllerRemoveWvf99p()


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

const { status, data } = await client.googleAds.campaignsControllerRemoveWvf99p(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**string**

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

# **campaignsControllerUpdate40ll7r**
> string campaignsControllerUpdate40ll7r(body)


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

const { status, data } = await client.googleAds.campaignsControllerUpdate40ll7r(
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

# **credentialsControllerCreateCustomer8qpv6w**
> credentialsControllerCreateCustomer8qpv6w(googleAdsCreateCredentialDto)


### Example

```typescript
import {
    Client,
    Configuration,
    GoogleAdsCreateCredentialDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let googleAdsCreateCredentialDto: GoogleAdsCreateCredentialDto; // 

const { status, data } = await client.googleAds.credentialsControllerCreateCustomer8qpv6w(
    googleAdsCreateCredentialDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **googleAdsCreateCredentialDto** | **GoogleAdsCreateCredentialDto**|  | |


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

# **credentialsControllerDeleteCustomerCredentialsSiel2b**
> credentialsControllerDeleteCustomerCredentialsSiel2b()


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


let customerId: string; // The id (UUID) of the customer whose credentials should be deleted. (default to undefined)

const { status, data } = await client.googleAds.credentialsControllerDeleteCustomerCredentialsSiel2b(
    customerId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | The id (UUID) of the customer whose credentials should be deleted. | defaults to undefined|


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

# **credentialsControllerFindAll9quhk2**
> Array<object> credentialsControllerFindAll9quhk2()


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


const { status, data } = await client.googleAds.credentialsControllerFindAll9quhk2();
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

# **rawControllerRawRequest60eqvdPost**
> rawControllerRawRequest60eqvdPost()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequest60eqvdPost(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

# **rawControllerRawRequest7vtbrnGet**
> rawControllerRawRequest7vtbrnGet()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequest7vtbrnGet(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestAfsh4hDelete**
> rawControllerRawRequestAfsh4hDelete()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequestAfsh4hDelete(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestD0r8raHead**
> rawControllerRawRequestD0r8raHead()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequestD0r8raHead(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestF0ip1pOptions**
> rawControllerRawRequestF0ip1pOptions()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequestF0ip1pOptions(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestH2cub1Put**
> rawControllerRawRequestH2cub1Put()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequestH2cub1Put(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestWg2qdkPatch**
> rawControllerRawRequestWg2qdkPatch()


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
let externalPath: string; // The external path for the Google Ads API request. (default to undefined)

const { status, data } = await client.googleAds.rawControllerRawRequestWg2qdkPatch(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Google Ads API request. | defaults to undefined|


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

