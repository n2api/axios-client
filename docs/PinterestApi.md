# PinterestApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**convertAuthCode**](#convertauthcode) | **POST** /pinterest/auth | Convert Pinterest auth code|
|[**deletePinterestCustomerCredentials**](#deletepinterestcustomercredentials) | **DELETE** /pinterest/credentials/{customerId} | Delete Pinterest credentials for a customer|
|[**rawRequest**](#rawrequest) | **GET** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequest_0**](#rawrequest_0) | **HEAD** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequest_1**](#rawrequest_1) | **PUT** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequest_2**](#rawrequest_2) | **POST** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequest_3**](#rawrequest_3) | **DELETE** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequest_4**](#rawrequest_4) | **PATCH** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequest_5**](#rawrequest_5) | **OPTIONS** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**storePinterestCustomerCredentials**](#storepinterestcustomercredentials) | **POST** /pinterest/credentials/customer | Store Pinterest credentials for a customer|

# **convertAuthCode**
> object convertAuthCode(createPinterestAuthDto)

Convert a Pinterest authorization code into access and refresh tokens. This route requires a customer session token for authentication. Requests will fail with a regular token.

### Example

```typescript
import {
    Client,
    Configuration,
    CreatePinterestAuthDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let createPinterestAuthDto: CreatePinterestAuthDto; // 

const { status, data } = await client.pinterest.convertAuthCode(
    createPinterestAuthDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPinterestAuthDto** | **CreatePinterestAuthDto**|  | |


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

# **deletePinterestCustomerCredentials**
> deletePinterestCustomerCredentials()

Delete all Pinterest credentials for a given customer and its related synced ad accounts data. Calling this method will not delete data on Pinterest itself.

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


let customerId: string; // The ID of the customer whose credentials are to be deleted. (default to undefined)

const { status, data } = await client.pinterest.deletePinterestCustomerCredentials(
    customerId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | The ID of the customer whose credentials are to be deleted. | defaults to undefined|


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
|**204** | Customer credentials deleted successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **rawRequest**
> rawRequest()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **rawRequest_0**
> rawRequest_0()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest_0(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **rawRequest_1**
> rawRequest_1()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest_1(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **rawRequest_2**
> rawRequest_2()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest_2(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **rawRequest_3**
> rawRequest_3()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest_3(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **rawRequest_4**
> rawRequest_4()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest_4(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **rawRequest_5**
> rawRequest_5()

This route proxies raw requests to the Pinterest API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the Pinterest Ads API request. (default to undefined)

const { status, data } = await client.pinterest.rawRequest_5(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the Pinterest Ads API request. | defaults to undefined|


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

# **storePinterestCustomerCredentials**
> storePinterestCustomerCredentials(pinterestCreateCredentialDto)

Store Pinterest credentials for a customer. This requires a customer session token for authentication. Using a regular token will fail.

### Example

```typescript
import {
    Client,
    Configuration,
    PinterestCreateCredentialDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let pinterestCreateCredentialDto: PinterestCreateCredentialDto; // 

const { status, data } = await client.pinterest.storePinterestCustomerCredentials(
    pinterestCreateCredentialDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pinterestCreateCredentialDto** | **PinterestCreateCredentialDto**|  | |


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

