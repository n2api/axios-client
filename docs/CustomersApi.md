# CustomersApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**customersControllerCreateCustomer2cjlz2**](#customerscontrollercreatecustomer2cjlz2) | **POST** /customers | |
|[**customersControllerDeleteCustomer00kwoh**](#customerscontrollerdeletecustomer00kwoh) | **DELETE** /customers/{id} | |
|[**customersControllerFindAllKggoor**](#customerscontrollerfindallkggoor) | **GET** /customers | |
|[**customersControllerFindAllWithPlatformsXzeg6k**](#customerscontrollerfindallwithplatformsxzeg6k) | **GET** /customers/platforms | |
|[**customersControllerFindOneV9u2yc**](#customerscontrollerfindonev9u2yc) | **GET** /customers/{id} | |
|[**getConnectCustomerUrl**](#getconnectcustomerurl) | **GET** /customers/{id}/connect | Generate connect URL for a customer|

# **customersControllerCreateCustomer2cjlz2**
> customersControllerCreateCustomer2cjlz2(createCustomerDto)


### Example

```typescript
import {
    Client,
    Configuration,
    CreateCustomerDto
} from '@n2api/axios-client';

const configuration = new Configuration({
    accessToken: 'YOUR_ACCESS_TOKEN',
});
const client = new Client(configuration);


let createCustomerDto: CreateCustomerDto; // 

const { status, data } = await client.customers.customersControllerCreateCustomer2cjlz2(
    createCustomerDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCustomerDto** | **CreateCustomerDto**|  | |


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

# **customersControllerDeleteCustomer00kwoh**
> customersControllerDeleteCustomer00kwoh()


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


let id: string; // The id of the customer to delete. (default to undefined)

const { status, data } = await client.customers.customersControllerDeleteCustomer00kwoh(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The id of the customer to delete. | defaults to undefined|


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

# **customersControllerFindAllKggoor**
> customersControllerFindAllKggoor()


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


const { status, data } = await client.customers.customersControllerFindAllKggoor();
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

# **customersControllerFindAllWithPlatformsXzeg6k**
> customersControllerFindAllWithPlatformsXzeg6k()


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


let customers: Array<string>; // The ids of the customers to fetch. (optional) (default to undefined)

const { status, data } = await client.customers.customersControllerFindAllWithPlatformsXzeg6k(
    customers
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customers** | **Array&lt;string&gt;** | The ids of the customers to fetch. | (optional) defaults to undefined|


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

# **customersControllerFindOneV9u2yc**
> customersControllerFindOneV9u2yc()


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

const { status, data } = await client.customers.customersControllerFindOneV9u2yc(
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

# **getConnectCustomerUrl**
> object getConnectCustomerUrl()

Generate a connect URL for a customer. This URL will redirect the customer to the platform\'s authentication page. If no platform is specified, the user will be presented with a list of platforms to choose from.

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


let id: string; // The id (UUID) of the customer to connect. (default to undefined)
let platform: 'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest'; // The platform to connect the customer to. If undefined, users will be presented with a list of platforms to choose from. (optional) (default to undefined)

const { status, data } = await client.customers.getConnectCustomerUrl(
    id,
    platform
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The id (UUID) of the customer to connect. | defaults to undefined|
| **platform** | [**&#39;ActiveAgent&#39; | &#39;Facebook&#39; | &#39;GoogleAds&#39; | &#39;TheTradeDesk&#39; | &#39;Pinterest&#39;**]**Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39;>** | The platform to connect the customer to. If undefined, users will be presented with a list of platforms to choose from. | (optional) defaults to undefined|


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

