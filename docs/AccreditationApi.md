# AccreditationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**accreditationIndexByRegistryId**](#accreditationindexbyregistryid) | **GET** /api/v1/accreditations/{registryId} | Get accreditations by registry ID|
|[**accreditationStoreByRegistryId**](#accreditationstorebyregistryid) | **POST** /api/v1/accreditations/{registryId} | Create accreditation for a registry|
|[**accreditationUpdateByRegistryId**](#accreditationupdatebyregistryid) | **PUT** /api/v1/accreditations/{id}/registries/{registryId} | Update accreditation for a registry|

# **accreditationIndexByRegistryId**
> AccreditationIndexByRegistryId200Response accreditationIndexByRegistryId()


### Example

```typescript
import {
    AccreditationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AccreditationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)

const { status, data } = await apiInstance.accreditationIndexByRegistryId(
    registryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | ID of the registry | defaults to undefined|


### Return type

**AccreditationIndexByRegistryId200Response**

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

# **accreditationStoreByRegistryId**
> AccreditationStoreByRegistryId201Response accreditationStoreByRegistryId(accreditation)


### Example

```typescript
import {
    AccreditationApi,
    Configuration,
    Accreditation
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AccreditationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let accreditation: Accreditation; //

const { status, data } = await apiInstance.accreditationStoreByRegistryId(
    registryId,
    accreditation
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accreditation** | **Accreditation**|  | |
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

# **accreditationUpdateByRegistryId**
> AccreditationUpdateByRegistryId200Response accreditationUpdateByRegistryId(accreditation)


### Example

```typescript
import {
    AccreditationApi,
    Configuration,
    Accreditation
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AccreditationApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let id: number; //ID of the accreditation (default to undefined)
let accreditation: Accreditation; //

const { status, data } = await apiInstance.accreditationUpdateByRegistryId(
    registryId,
    id,
    accreditation
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accreditation** | **Accreditation**|  | |
| **registryId** | [**number**] | ID of the registry | defaults to undefined|
| **id** | [**number**] | ID of the accreditation | defaults to undefined|


### Return type

**AccreditationUpdateByRegistryId200Response**

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

