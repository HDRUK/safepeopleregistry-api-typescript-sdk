# ResolutionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**resolutionIndexByRegistryId**](#resolutionindexbyregistryid) | **GET** /api/v1/registries/{registryId}/resolutions | Get resolutions by registry ID|
|[**resolutionStoreByRegistryId**](#resolutionstorebyregistryid) | **POST** /api/v1/registries/{registryId}/resolutions | Create a new resolution for a registry|

# **resolutionIndexByRegistryId**
> Array<Resolution> resolutionIndexByRegistryId()


### Example

```typescript
import {
    ResolutionApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ResolutionApi(configuration);

let registryId: number; //ID of the registry (default to undefined)

const { status, data } = await apiInstance.resolutionIndexByRegistryId(
    registryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | ID of the registry | defaults to undefined|


### Return type

**Array<Resolution>**

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

# **resolutionStoreByRegistryId**
> AccreditationStoreByRegistryId201Response resolutionStoreByRegistryId(resolution)


### Example

```typescript
import {
    ResolutionApi,
    Configuration,
    Resolution
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ResolutionApi(configuration);

let registryId: number; //ID of the registry (default to undefined)
let resolution: Resolution; //

const { status, data } = await apiInstance.resolutionStoreByRegistryId(
    registryId,
    resolution
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **resolution** | **Resolution**|  | |
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

