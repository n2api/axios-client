# CustomersApi

All URIs are relative to *https://api.n2api.io*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCustomer**](#createcustomer) | **POST** /customers | Create customer|
|[**deleteCustomer**](#deletecustomer) | **DELETE** /customers/{id} | Delete customer|
|[**generateConnectCustomerUrl**](#generateconnectcustomerurl) | **GET** /customers/{id}/connect | Generate connect URL for a customer|
|[**getAllCustomers**](#getallcustomers) | **GET** /customers | Get all customers|
|[**getAllCustomersWithPlatforms**](#getallcustomerswithplatforms) | **GET** /customers/platforms | Get all customers with platforms|
|[**getCustomer**](#getcustomer) | **GET** /customers/{id} | Get customer by id|
|[**getCustomerWithPlatforms**](#getcustomerwithplatforms) | **GET** /customers/{id}/platforms | Get customer with platforms|

# **createCustomer**
> CustomerDto createCustomer(createCustomerDto)

Create a new customer.

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

const { status, data } = await client.customers.createCustomer(
    createCustomerDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCustomerDto** | **CreateCustomerDto**|  | |


### Return type

**CustomerDto**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Customer created successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteCustomer**
> deleteCustomer()

Delete a customer by their id.

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

const { status, data } = await client.customers.deleteCustomer(
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
|**200** | Customer deleted successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **generateConnectCustomerUrl**
> generateConnectCustomerUrl()

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
let platform: 'ActiveAgent' | 'Facebook' | 'GoogleAds' | 'TheTradeDesk' | 'Pinterest' | 'LinkedIn'; // The platform to connect the customer to. If undefined, users will be presented with a list of platforms to choose from. (optional) (default to undefined)

const { status, data } = await client.customers.generateConnectCustomerUrl(
    id,
    platform
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The id (UUID) of the customer to connect. | defaults to undefined|
| **platform** | [**&#39;ActiveAgent&#39; | &#39;Facebook&#39; | &#39;GoogleAds&#39; | &#39;TheTradeDesk&#39; | &#39;Pinterest&#39; | &#39;LinkedIn&#39;**]**Array<&#39;ActiveAgent&#39; &#124; &#39;Facebook&#39; &#124; &#39;GoogleAds&#39; &#124; &#39;TheTradeDesk&#39; &#124; &#39;Pinterest&#39; &#124; &#39;LinkedIn&#39;>** | The platform to connect the customer to. If undefined, users will be presented with a list of platforms to choose from. | (optional) defaults to undefined|


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

# **getAllCustomers**
> Array<CustomerDto> getAllCustomers()

Get a list of all customers.

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


const { status, data } = await client.customers.getAllCustomers();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<CustomerDto>**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of customers retrieved successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllCustomersWithPlatforms**
> Array<CustomerWithPlatformsDto> getAllCustomersWithPlatforms()

Get a list of all customers with their connected platforms.

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

const { status, data } = await client.customers.getAllCustomersWithPlatforms(
    customers
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **customers** | **Array&lt;string&gt;** | The ids of the customers to fetch. | (optional) defaults to undefined|


### Return type

**Array<CustomerWithPlatformsDto>**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of customers with connected platforms retrieved successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCustomer**
> CustomerDto getCustomer()

Get a single customer by their id. Returns 404 if the customer does not exist.

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


let id: string; // The id (UUID) of the customer to fetch. (default to undefined)

const { status, data } = await client.customers.getCustomer(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The id (UUID) of the customer to fetch. | defaults to undefined|


### Return type

**CustomerDto**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Customer retrieved successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCustomerWithPlatforms**
> CustomerWithPlatformsDto getCustomerWithPlatforms()

Get a single customer with their connected platforms. Returns 404 if the customer does not exist.

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


let id: string; // The id (UUID) of the customer to fetch with platforms. (default to undefined)

const { status, data } = await client.customers.getCustomerWithPlatforms(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | The id (UUID) of the customer to fetch with platforms. | defaults to undefined|


### Return type

**CustomerWithPlatformsDto**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Customer with connected platforms retrieved successfully. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

