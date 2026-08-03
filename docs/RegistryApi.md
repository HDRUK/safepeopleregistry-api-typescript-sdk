# RegistryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**registryDestroy**](#registrydestroy) | **DELETE** /api/v1/registry/{id} | Registry@destroy|
|[**registryIndex**](#registryindex) | **GET** /api/v1/registry | Registry@index|
|[**registryShow**](#registryshow) | **GET** /api/v1/registry/{id} | Registry@show|
|[**registryStore**](#registrystore) | **POST** /api/v1/registry | Registry@store|
|[**registryUpdate**](#registryupdate) | **PUT** /api/v1/registry/{id} | Registry@update|

# **registryDestroy**
> AffiliationDestroy200Response registryDestroy()

Delete a Registry entry from the system

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: number; //Registry entry ID (default to undefined)

const { status, data } = await apiInstance.registryDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Registry entry ID | defaults to undefined|


### Return type

**AffiliationDestroy200Response**

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
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registryIndex**
> RegistryIndex200Response registryIndex()

Return a list of Registry entries

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

const { status, data } = await apiInstance.registryIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**RegistryIndex200Response**

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

# **registryShow**
> RegistryIndex200Response registryShow()

Return a Registry entry by ID

### Example

```typescript
import {
    RegistryApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: number; //Registry entry ID (default to undefined)

const { status, data } = await apiInstance.registryShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Registry entry ID | defaults to undefined|


### Return type

**RegistryIndex200Response**

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

# **registryStore**
> AccreditationStoreByRegistryId201Response registryStore(registry)

Create a Registry entry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    Registry
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let registry: Registry; //Registry definition

const { status, data } = await apiInstance.registryStore(
    registry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registry** | **Registry**| Registry definition | |


### Return type

**AccreditationStoreByRegistryId201Response**

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

# **registryUpdate**
> RegistryUpdate200Response registryUpdate(registry)

Update a Registry entry

### Example

```typescript
import {
    RegistryApi,
    Configuration,
    Registry
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new RegistryApi(configuration);

let id: number; //Registry entry ID (default to undefined)
let registry: Registry; //Registry definition

const { status, data } = await apiInstance.registryUpdate(
    id,
    registry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registry** | **Registry**| Registry definition | |
| **id** | [**number**] | Registry entry ID | defaults to undefined|


### Return type

**RegistryUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

