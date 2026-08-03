# ProjectDetailsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectDetailsDestroy**](#projectdetailsdestroy) | **DELETE** /api/v1/project_details/{id} | ProjectDetails@destroy|
|[**projectDetailsStore**](#projectdetailsstore) | **POST** /api/v1/project_details | ProjectDetails@store|
|[**projectDetailsUpdate**](#projectdetailsupdate) | **PUT** /api/v1/project_details/{id} | ProjectDetails@update|

# **projectDetailsDestroy**
> AffiliationDestroy200Response projectDetailsDestroy()

Delete a ProjectDetail entry from the system

### Example

```typescript
import {
    ProjectDetailsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectDetailsApi(configuration);

let id: number; //ProjectDetails entry ID (default to undefined)

const { status, data } = await apiInstance.projectDetailsDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ProjectDetails entry ID | defaults to undefined|


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

# **projectDetailsStore**
> IdentityStore201Response projectDetailsStore(projectDetail)

Create a ProjectDetail

### Example

```typescript
import {
    ProjectDetailsApi,
    Configuration,
    ProjectDetail
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectDetailsApi(configuration);

let projectDetail: ProjectDetail; //ProjectDetail definition

const { status, data } = await apiInstance.projectDetailsStore(
    projectDetail
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectDetail** | **ProjectDetail**| ProjectDetail definition | |


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
|**404** | Not found response |  -  |
|**201** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectDetailsUpdate**
> ProjectDetailsUpdate200Response projectDetailsUpdate(projectDetail)

Update a ProjectDetail entry

### Example

```typescript
import {
    ProjectDetailsApi,
    Configuration,
    ProjectDetail
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectDetailsApi(configuration);

let id: number; //ProjectDetails entry ID (default to undefined)
let projectDetail: ProjectDetail; //ProjectDetails definition

const { status, data } = await apiInstance.projectDetailsUpdate(
    id,
    projectDetail
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectDetail** | **ProjectDetail**| ProjectDetails definition | |
| **id** | [**number**] | ProjectDetails entry ID | defaults to undefined|


### Return type

**ProjectDetailsUpdate200Response**

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

