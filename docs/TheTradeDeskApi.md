# TheTradeDeskApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**rawRequest**](#rawrequest) | **GET** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**rawRequest_0**](#rawrequest_0) | **HEAD** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**rawRequest_1**](#rawrequest_1) | **PUT** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**rawRequest_2**](#rawrequest_2) | **POST** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**rawRequest_3**](#rawrequest_3) | **DELETE** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**rawRequest_4**](#rawrequest_4) | **PATCH** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**rawRequest_5**](#rawrequest_5) | **OPTIONS** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API|
|[**storeCustomerCredentials**](#storecustomercredentials) | **POST** /thetradedesk/credentials/customer | Login to The Trade Desk|

# **rawRequest**
> object rawRequest()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **rawRequest_0**
> object rawRequest_0()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest_0(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **rawRequest_1**
> object rawRequest_1()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest_1(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **rawRequest_2**
> object rawRequest_2()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest_2(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **rawRequest_3**
> object rawRequest_3()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest_3(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **rawRequest_4**
> object rawRequest_4()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest_4(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **rawRequest_5**
> object rawRequest_5()

This route proxies raw requests to the The Trade Desk API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // External API path (default to undefined)

const { status, data } = await client.theTradeDesk.rawRequest_5(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | External API path | defaults to undefined|


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

# **storeCustomerCredentials**
> storeCustomerCredentials(theTradeDeskCreateCredentialsDto)

Log in a customer to The Trade Desk using their *login* and *password*. This will store their credentials securely for future use.

### Example

```typescript
import {
    Client,
    Configuration,
    TheTradeDeskCreateCredentialsDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let theTradeDeskCreateCredentialsDto: TheTradeDeskCreateCredentialsDto; // 

const { status, data } = await client.theTradeDesk.storeCustomerCredentials(
    theTradeDeskCreateCredentialsDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **theTradeDeskCreateCredentialsDto** | **TheTradeDeskCreateCredentialsDto**|  | |


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

