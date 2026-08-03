# FilesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**filesDownload**](#filesdownload) | **GET** /api/v1/files/{id}/download | Download an uploaded file|
|[**filesShow**](#filesshow) | **GET** /api/v1/files/{id} | Files@show|
|[**filesStore**](#filesstore) | **POST** /api/v1/files | Files@store|

# **filesDownload**
> File filesDownload()

Downloads the specified file

### Example

```typescript
import {
    FilesApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new FilesApi(configuration);

let id: number; //File ID (default to undefined)

const { status, data } = await apiInstance.filesDownload(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | File ID | defaults to undefined|


### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | File downloaded successfully |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | File not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **filesShow**
> FilesShow200Response filesShow()

Gets an uploaded file

### Example

```typescript
import {
    FilesApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new FilesApi(configuration);

let id: number; //File ID (default to undefined)

const { status, data } = await apiInstance.filesShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | File ID | defaults to undefined|


### Return type

**FilesShow200Response**

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
|**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **filesStore**
> AccreditationStoreByRegistryId201Response filesStore()

Uploads a file to the registry

### Example

```typescript
import {
    FilesApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new FilesApi(configuration);

let registryId: number; // (optional) (default to undefined)
let file: File; // (optional) (default to undefined)
let fileType: string; // (optional) (default to undefined)
let entityType: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.filesStore(
    registryId,
    file,
    fileType,
    entityType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] |  | (optional) defaults to undefined|
| **file** | [**File**] |  | (optional) defaults to undefined|
| **fileType** | [**string**] |  | (optional) defaults to undefined|
| **entityType** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AccreditationStoreByRegistryId201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**400** | Bad request |  -  |
|**201** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

