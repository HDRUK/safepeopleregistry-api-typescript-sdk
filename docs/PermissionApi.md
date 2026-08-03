# PermissionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**permissionDestroy**](#permissiondestroy) | **DELETE** /api/v1/permissions/{id} | Permission@destroy|
|[**permissionIndex**](#permissionindex) | **GET** /api/v1/permissions | Permission@index|
|[**permissionShow**](#permissionshow) | **GET** /api/v1/permissions/{id} | Permission@show|
|[**permissionStore**](#permissionstore) | **POST** /api/v1/permissions | Permission@store|
|[**permissionUpdate**](#permissionupdate) | **PATCH** /api/v1/permissions/{id} | Permission@update|

# **permissionDestroy**
> AffiliationDestroy200Response permissionDestroy()

Delete a Permission entry from the system

### Example

```typescript
import {
    PermissionApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new PermissionApi(configuration);

let id: number; //Permission entry ID (default to undefined)

const { status, data } = await apiInstance.permissionDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Permission entry ID | defaults to undefined|


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
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **permissionIndex**
> PermissionIndex200Response permissionIndex()

Return a list of Permissions

### Example

```typescript
import {
    PermissionApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new PermissionApi(configuration);

const { status, data } = await apiInstance.permissionIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**PermissionIndex200Response**

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

# **permissionShow**
> PermissionIndex200Response permissionShow()

Return a Permission entry by ID

### Example

```typescript
import {
    PermissionApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new PermissionApi(configuration);

let id: number; //Permission entry ID (default to undefined)

const { status, data } = await apiInstance.permissionShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Permission entry ID | defaults to undefined|


### Return type

**PermissionIndex200Response**

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

# **permissionStore**
> AccreditationStoreByRegistryId201Response permissionStore(permissionStoreRequest)

Create a Permission entry

### Example

```typescript
import {
    PermissionApi,
    Configuration,
    PermissionStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new PermissionApi(configuration);

let permissionStoreRequest: PermissionStoreRequest; //Permission definition

const { status, data } = await apiInstance.permissionStore(
    permissionStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **permissionStoreRequest** | **PermissionStoreRequest**| Permission definition | |


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
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **permissionUpdate**
> PermissionUpdate200Response permissionUpdate(permissionStoreRequest)

Update a Permission entry

### Example

```typescript
import {
    PermissionApi,
    Configuration,
    PermissionStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new PermissionApi(configuration);

let id: number; //Permission entry ID (default to undefined)
let permissionStoreRequest: PermissionStoreRequest; //Permission definition

const { status, data } = await apiInstance.permissionUpdate(
    id,
    permissionStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **permissionStoreRequest** | **PermissionStoreRequest**| Permission definition | |
| **id** | [**number**] | Permission entry ID | defaults to undefined|


### Return type

**PermissionUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

