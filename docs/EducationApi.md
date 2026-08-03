# EducationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**educationDestroyByRegistryId**](#educationdestroybyregistryid) | **DELETE** /api/v1/registries/{registryId}/educations/{id} | Delete an education record|
|[**educationIndexByRegistryId**](#educationindexbyregistryid) | **GET** /api/v1/educations/registries/{registryId} | Get education records by registry ID|
|[**educationShowByRegistryId**](#educationshowbyregistryid) | **GET** /api/v1/educations/{id}/registries/{registryId} | Get a specific education record by ID and registry ID|
|[**educationStoreByRegistryId**](#educationstorebyregistryid) | **POST** /api/v1/registries/{registryId}/educations | Create a new education record for a registry|
|[**educationUpdateByRegistryId**](#educationupdatebyregistryid) | **PUT** /api/v1/registries/{registryId}/educations/{id} | Update an existing education record|

# **educationDestroyByRegistryId**
> EducationDestroyByRegistryId200Response educationDestroyByRegistryId()


### Example

```typescript
import {
    EducationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EducationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let id: number; //ID of the education record (default to undefined)

const { status, data } = await apiInstance.educationDestroyByRegistryId(
    registryId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | ID of the registry | defaults to undefined|
| **id** | [**number**] | ID of the education record | defaults to undefined|


### Return type

**EducationDestroyByRegistryId200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Deleted |  -  |
|**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **educationIndexByRegistryId**
> Array<Education> educationIndexByRegistryId()


### Example

```typescript
import {
    EducationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EducationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)

const { status, data } = await apiInstance.educationIndexByRegistryId(
    registryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | ID of the registry | defaults to undefined|


### Return type

**Array<Education>**

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **educationShowByRegistryId**
> Education educationShowByRegistryId()


### Example

```typescript
import {
    EducationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EducationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let id: number; //ID of the education record (default to undefined)

const { status, data } = await apiInstance.educationShowByRegistryId(
    registryId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | ID of the registry | defaults to undefined|
| **id** | [**number**] | ID of the education record | defaults to undefined|


### Return type

**Education**

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
|**404** | Education record not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **educationStoreByRegistryId**
> AccreditationStoreByRegistryId201Response educationStoreByRegistryId(education)


### Example

```typescript
import {
    EducationApi,
    Configuration,
    Education
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EducationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let education: Education; //

const { status, data } = await apiInstance.educationStoreByRegistryId(
    registryId,
    education
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **education** | **Education**|  | |
| **registryId** | [**number**] | ID of the registry | defaults to undefined|


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
|**201** | Created |  -  |
|**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **educationUpdateByRegistryId**
> Education educationUpdateByRegistryId(education)


### Example

```typescript
import {
    EducationApi,
    Configuration,
    Education
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EducationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let id: number; //ID of the education record (default to undefined)
let education: Education; //

const { status, data } = await apiInstance.educationUpdateByRegistryId(
    registryId,
    id,
    education
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **education** | **Education**|  | |
| **registryId** | [**number**] | ID of the registry | defaults to undefined|
| **id** | [**number**] | ID of the education record | defaults to undefined|


### Return type

**Education**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Updated |  -  |
|**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

