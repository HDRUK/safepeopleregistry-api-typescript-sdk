# ProjectDetailApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectDetailIndex**](#projectdetailindex) | **GET** /api/v1/project_details | ProjectDetail@index|
|[**projectDetailShow**](#projectdetailshow) | **GET** /api/v1/project_details/{id} | ProjectDetail@show|

# **projectDetailIndex**
> ProjectDetailIndex200Response projectDetailIndex()

Return a list of ProjectDetail

### Example

```typescript
import {
    ProjectDetailApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectDetailApi(configuration);

const { status, data } = await apiInstance.projectDetailIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**ProjectDetailIndex200Response**

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

# **projectDetailShow**
> ProjectDetailIndex200Response projectDetailShow()

Return a ProjectDetail

### Example

```typescript
import {
    ProjectDetailApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectDetailApi(configuration);

let id: number; //ProjectDetail entry ID (default to undefined)

const { status, data } = await apiInstance.projectDetailShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ProjectDetail entry ID | defaults to undefined|


### Return type

**ProjectDetailIndex200Response**

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

