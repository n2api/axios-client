# LinkedInApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCustomer**](#createcustomer) | **POST** /linkedin/credentials/customer | Store LinkedIn credentials for a customer|
|[**deleteCustomer**](#deletecustomer) | **DELETE** /linkedin/credentials/{customerId} | Delete LinkedIn credentials for a customer|
|[**getAccessToken**](#getaccesstoken) | **POST** /linkedin/auth | Convert LinkedIn auth code|
|[**rawRequestDelete**](#rawrequestdelete) | **DELETE** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|
|[**rawRequestGet**](#rawrequestget) | **GET** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|
|[**rawRequestHead**](#rawrequesthead) | **HEAD** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|
|[**rawRequestOptions**](#rawrequestoptions) | **OPTIONS** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|
|[**rawRequestPatch**](#rawrequestpatch) | **PATCH** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|
|[**rawRequestPost**](#rawrequestpost) | **POST** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|
|[**rawRequestPut**](#rawrequestput) | **PUT** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API|

# **createCustomer**
> createCustomer(linkedInCreateCredentialDto)

Store LinkedIn credentials for a customer. This requires a customer session token for authentication. Using a regular token will fail.

### Example

```typescript
import {
    Client,
    Configuration,
    LinkedInCreateCredentialDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let linkedInCreateCredentialDto: LinkedInCreateCredentialDto; // 

const { status, data } = await client.linkedIn.createCustomer(
    linkedInCreateCredentialDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **linkedInCreateCredentialDto** | **LinkedInCreateCredentialDto**|  | |


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

# **deleteCustomer**
> deleteCustomer()

Delete all LinkedIn credentials for a given customer and its related synced ad accounts data. Calling this method will not delete data on LinkedIn itself, but will revoke the permissions granted to the app.

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

const { status, data } = await client.linkedIn.deleteCustomer(
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
|**404** | Customer credentials not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAccessToken**
> object getAccessToken(createAuthDto)

Convert a LinkedIn authorization code into access and refresh tokens. This route requires a customer session token for authentication. Requests will fail with a regular token.

### Example

```typescript
import {
    Client,
    Configuration,
    CreateAuthDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let createAuthDto: CreateAuthDto; // 

const { status, data } = await client.linkedIn.getAccessToken(
    createAuthDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAuthDto** | **CreateAuthDto**|  | |


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

# **rawRequestDelete**
> rawRequestDelete()

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestDelete(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestGet(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestHead(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestOptions(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestPatch(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestPost(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

This route proxies raw requests to the LinkedIn API, allowing for dynamic endpoints and parameters.

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
let externalPath: string; // The external path for the LinkedIn API request. (default to undefined)

const { status, data } = await client.linkedIn.rawRequestPut(
    customerId,
    externalPath
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customerId** | [**string**] | Customer UUID | defaults to undefined|
| **externalPath** | [**string**] | The external path for the LinkedIn API request. | defaults to undefined|


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

