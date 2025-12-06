# FacebookApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adAccountsControllerFindAll0549lm**](#adaccountscontrollerfindall0549lm) | **GET** /facebook/adaccounts | |
|[**adAccountsControllerSyncCustomerKpkzo2**](#adaccountscontrollersynccustomerkpkzo2) | **PUT** /facebook/adaccounts/customer | |
|[**adSetsControllerFindAllGeus8d**](#adsetscontrollerfindallgeus8d) | **GET** /facebook/adsets | |
|[**adSetsControllerFindOne7d8j59**](#adsetscontrollerfindone7d8j59) | **GET** /facebook/adsets/{id} | |
|[**adSetsControllerRemoveQpjoni**](#adsetscontrollerremoveqpjoni) | **DELETE** /facebook/adsets/{id} | |
|[**adSetsControllerUpdate505b7c**](#adsetscontrollerupdate505b7c) | **PATCH** /facebook/adsets/{id} | |
|[**authControllerGetAccessTokenT41rff**](#authcontrollergetaccesstokent41rff) | **POST** /facebook/auth | |
|[**campaignsControllerFindAllZ5jbts**](#campaignscontrollerfindallz5jbts) | **GET** /facebook/campaigns | |
|[**credentialsControllerCreateCustomerLqwsc5**](#credentialscontrollercreatecustomerlqwsc5) | **POST** /facebook/credentials/customer | |
|[**credentialsControllerDeleteCustomerGkcpsz**](#credentialscontrollerdeletecustomergkcpsz) | **DELETE** /facebook/credentials/{customerId} | |
|[**credentialsControllerFindAllUrmvrv**](#credentialscontrollerfindallurmvrv) | **GET** /facebook/credentials | |
|[**credentialsControllerIsConnectedTfvw6f**](#credentialscontrollerisconnectedtfvw6f) | **GET** /facebook/credentials/isConnected | |
|[**rawControllerRawRequest1fu5v3Put**](#rawcontrollerrawrequest1fu5v3put) | **PUT** /facebook/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequest2tg1shGet**](#rawcontrollerrawrequest2tg1shget) | **GET** /facebook/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestF1g1cgPost**](#rawcontrollerrawrequestf1g1cgpost) | **POST** /facebook/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestG9ig2bPatch**](#rawcontrollerrawrequestg9ig2bpatch) | **PATCH** /facebook/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestHkcfxtDelete**](#rawcontrollerrawrequesthkcfxtdelete) | **DELETE** /facebook/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestU28fawOptions**](#rawcontrollerrawrequestu28fawoptions) | **OPTIONS** /facebook/{customerId}/raw/{externalPath} | |
|[**rawControllerRawRequestUdhoymHead**](#rawcontrollerrawrequestudhoymhead) | **HEAD** /facebook/{customerId}/raw/{externalPath} | |

# **adAccountsControllerFindAll0549lm**
> Array<FacebookAdAccountWrapper> adAccountsControllerFindAll0549lm()


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


const { status, data } = await client.facebook.adAccountsControllerFindAll0549lm();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<FacebookAdAccountWrapper>**

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

# **adAccountsControllerSyncCustomerKpkzo2**
> adAccountsControllerSyncCustomerKpkzo2()


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


const { status, data } = await client.facebook.adAccountsControllerSyncCustomerKpkzo2();
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

# **adSetsControllerFindAllGeus8d**
> Array<AdSet> adSetsControllerFindAllGeus8d()


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

const { status, data } = await client.facebook.adSetsControllerFindAllGeus8d(
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

# **adSetsControllerFindOne7d8j59**
> string adSetsControllerFindOne7d8j59()


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

const { status, data } = await client.facebook.adSetsControllerFindOne7d8j59(
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

# **adSetsControllerRemoveQpjoni**
> string adSetsControllerRemoveQpjoni()


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

const { status, data } = await client.facebook.adSetsControllerRemoveQpjoni(
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

# **adSetsControllerUpdate505b7c**
> string adSetsControllerUpdate505b7c(body)


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

const { status, data } = await client.facebook.adSetsControllerUpdate505b7c(
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

# **authControllerGetAccessTokenT41rff**
> object authControllerGetAccessTokenT41rff(createFacebookAuthDto)


### Example

```typescript
import {
    Client,
    Configuration,
    CreateFacebookAuthDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let createFacebookAuthDto: CreateFacebookAuthDto; // 

const { status, data } = await client.facebook.authControllerGetAccessTokenT41rff(
    createFacebookAuthDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createFacebookAuthDto** | **CreateFacebookAuthDto**|  | |


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

# **campaignsControllerFindAllZ5jbts**
> Array<Campaign> campaignsControllerFindAllZ5jbts()


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

const { status, data } = await client.facebook.campaignsControllerFindAllZ5jbts(
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

# **credentialsControllerCreateCustomerLqwsc5**
> credentialsControllerCreateCustomerLqwsc5(facebookCreateCredentialDto)


### Example

```typescript
import {
    Client,
    Configuration,
    FacebookCreateCredentialDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let facebookCreateCredentialDto: FacebookCreateCredentialDto; // 

const { status, data } = await client.facebook.credentialsControllerCreateCustomerLqwsc5(
    facebookCreateCredentialDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **facebookCreateCredentialDto** | **FacebookCreateCredentialDto**|  | |


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

# **credentialsControllerDeleteCustomerGkcpsz**
> credentialsControllerDeleteCustomerGkcpsz()


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

const { status, data } = await client.facebook.credentialsControllerDeleteCustomerGkcpsz(
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

# **credentialsControllerFindAllUrmvrv**
> Array<object> credentialsControllerFindAllUrmvrv()


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


const { status, data } = await client.facebook.credentialsControllerFindAllUrmvrv();
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

# **credentialsControllerIsConnectedTfvw6f**
> credentialsControllerIsConnectedTfvw6f()


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


const { status, data } = await client.facebook.credentialsControllerIsConnectedTfvw6f();
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

# **rawControllerRawRequest1fu5v3Put**
> rawControllerRawRequest1fu5v3Put()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequest1fu5v3Put(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

# **rawControllerRawRequest2tg1shGet**
> rawControllerRawRequest2tg1shGet()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequest2tg1shGet(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestF1g1cgPost**
> rawControllerRawRequestF1g1cgPost()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequestF1g1cgPost(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestG9ig2bPatch**
> rawControllerRawRequestG9ig2bPatch()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequestG9ig2bPatch(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestHkcfxtDelete**
> rawControllerRawRequestHkcfxtDelete()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequestHkcfxtDelete(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestU28fawOptions**
> rawControllerRawRequestU28fawOptions()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequestU28fawOptions(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

# **rawControllerRawRequestUdhoymHead**
> rawControllerRawRequestUdhoymHead()


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
let externalPath: string; // The external path for the Facebook Ads API request. (default to undefined)

const { status, data } = await client.facebook.rawControllerRawRequestUdhoymHead(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Facebook Ads API request. | defaults to undefined|


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

