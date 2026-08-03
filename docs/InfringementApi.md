# InfringementApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**infringementIndex**](#infringementindex) | **GET** /api/v1/infringements | Infringement@index|
|[**infringementShow**](#infringementshow) | **GET** /api/v1/infringements/{id} | Infringement@show|
|[**infringementStore**](#infringementstore) | **POST** /api/v1/infringements | Infringement@store|

# **infringementIndex**
> InfringementIndex200Response infringementIndex()

Return a list of Infringements

### Example

```typescript
import {
    InfringementApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new InfringementApi(configuration);

const { status, data } = await apiInstance.infringementIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**InfringementIndex200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **infringementShow**
> InfringementIndex200Response infringementShow()

Return an Infringement entry by ID

### Example

```typescript
import {
    InfringementApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new InfringementApi(configuration);

let id: number; //Infringement entry ID (default to undefined)

const { status, data } = await apiInstance.infringementShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Infringement entry ID | defaults to undefined|


### Return type

**InfringementIndex200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **infringementStore**
> InfringementStore201Response infringementStore(infringementStoreRequest)

Create an Infringement entry

### Example

```typescript
import {
    InfringementApi,
    Configuration,
    InfringementStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new InfringementApi(configuration);

let infringementStoreRequest: InfringementStoreRequest; //Infringement definition

const { status, data } = await apiInstance.infringementStore(
    infringementStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **infringementStoreRequest** | **InfringementStoreRequest**| Infringement definition | |


### Return type

**InfringementStore201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**201** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

