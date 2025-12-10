# PinterestApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCustomer**](#createcustomer) | **POST** /pinterest/credentials/customer | Store Pinterest credentials for a customer|
|[**deleteCustomerCredentials**](#deletecustomercredentials) | **DELETE** /pinterest/credentials/{customerId} | Delete Pinterest credentials for a customer|
|[**getAccessToken**](#getaccesstoken) | **POST** /pinterest/auth | Convert Pinterest auth code|
|[**rawRequestDelete**](#rawrequestdelete) | **DELETE** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequestGet**](#rawrequestget) | **GET** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequestHead**](#rawrequesthead) | **HEAD** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequestOptions**](#rawrequestoptions) | **OPTIONS** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequestPatch**](#rawrequestpatch) | **PATCH** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequestPost**](#rawrequestpost) | **POST** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|
|[**rawRequestPut**](#rawrequestput) | **PUT** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API|

# **createCustomer**
> createCustomer(pinterestCreateCredentialDto)

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

const { status, data } = await client.pinterest.createCustomer(
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

# **deleteCustomerCredentials**
> deleteCustomerCredentials()

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

const { status, data } = await client.pinterest.deleteCustomerCredentials(
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

# **getAccessToken**
> getAccessToken(createPinterestAuthDto)

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

const { status, data } = await client.pinterest.getAccessToken(
    createPinterestAuthDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPinterestAuthDto** | **CreatePinterestAuthDto**|  | |


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

# **rawRequestDelete**
> rawRequestDelete()

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

const { status, data } = await client.pinterest.rawRequestDelete(
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

# **rawRequestGet**
> rawRequestGet()

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

const { status, data } = await client.pinterest.rawRequestGet(
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

# **rawRequestHead**
> rawRequestHead()

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

const { status, data } = await client.pinterest.rawRequestHead(
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

# **rawRequestOptions**
> rawRequestOptions()

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

const { status, data } = await client.pinterest.rawRequestOptions(
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

# **rawRequestPatch**
> rawRequestPatch()

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

const { status, data } = await client.pinterest.rawRequestPatch(
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

# **rawRequestPost**
> rawRequestPost()

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

const { status, data } = await client.pinterest.rawRequestPost(
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

# **rawRequestPut**
> rawRequestPut()

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

const { status, data } = await client.pinterest.rawRequestPut(
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

