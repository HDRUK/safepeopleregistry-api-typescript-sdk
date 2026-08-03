# ProjectUserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectUserShow**](#projectusershow) | **GET** /api/v1/project_users/{id} | Get project user details|

# **projectUserShow**
> CustodianProjectUsersShow200Response projectUserShow()

Returns details for a specific project user

### Example

```typescript
import {
    ProjectUserApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectUserApi(configuration);

let id: number; //ID of the project user (default to undefined)

const { status, data } = await apiInstance.projectUserShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the project user | defaults to undefined|


### Return type

**CustodianProjectUsersShow200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Invalid argument(s) |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

