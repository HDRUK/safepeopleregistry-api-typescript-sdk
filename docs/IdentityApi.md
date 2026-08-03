# IdentityApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**identityDestroy**](#identitydestroy) | **DELETE** /api/v1/identities/{id} | Identity@destroy|
|[**identityIndex**](#identityindex) | **GET** /api/v1/identities | Identity@index|
|[**identityShow**](#identityshow) | **GET** /api/v1/identities/{id} | Identity@show|
|[**identityStore**](#identitystore) | **POST** /api/v1/identities | Identity@store|
|[**identityUpdate**](#identityupdate) | **PUT** /api/v1/identities/{id} | Identity@update|

# **identityDestroy**
> AffiliationDestroy200Response identityDestroy()

Delete an Identity entry from the system

### Example

```typescript
import {
    IdentityApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new IdentityApi(configuration);

let id: number; //Identity entry ID (default to undefined)

const { status, data } = await apiInstance.identityDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Identity entry ID | defaults to undefined|


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

# **identityIndex**
> IdentityIndex200Response identityIndex()

Return a list of Identity entries

### Example

```typescript
import {
    IdentityApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new IdentityApi(configuration);

const { status, data } = await apiInstance.identityIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**IdentityIndex200Response**

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

# **identityShow**
> IdentityIndex200Response identityShow()

Return an Identity entry by ID

### Example

```typescript
import {
    IdentityApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new IdentityApi(configuration);

let id: number; //Identity ID (default to undefined)

const { status, data } = await apiInstance.identityShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Identity ID | defaults to undefined|


### Return type

**IdentityIndex200Response**

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

# **identityStore**
> IdentityStore201Response identityStore(identityStoreRequest)

Create a Identity entry

### Example

```typescript
import {
    IdentityApi,
    Configuration,
    IdentityStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new IdentityApi(configuration);

let identityStoreRequest: IdentityStoreRequest; //Identity definition

const { status, data } = await apiInstance.identityStore(
    identityStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityStoreRequest** | **IdentityStoreRequest**| Identity definition | |


### Return type

**IdentityStore201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Success |  -  |
|**404** | Not found response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **identityUpdate**
> IdentityUpdate200Response identityUpdate(identityStoreRequest)

Update a Identity entry

### Example

```typescript
import {
    IdentityApi,
    Configuration,
    IdentityStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new IdentityApi(configuration);

let id: number; //Identity entry ID (default to undefined)
let identityStoreRequest: IdentityStoreRequest; //Identity definition

const { status, data } = await apiInstance.identityUpdate(
    id,
    identityStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityStoreRequest** | **IdentityStoreRequest**| Identity definition | |
| **id** | [**number**] | Identity entry ID | defaults to undefined|


### Return type

**IdentityUpdate200Response**

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

