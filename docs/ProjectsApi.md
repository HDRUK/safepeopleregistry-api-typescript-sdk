# ProjectsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectsDelete**](#projectsdelete) | **DELETE** /api/v1/project_users/{id} | ProjectHasUser@delete|
|[**projectsGetValidatedProjects**](#projectsgetvalidatedprojects) | **GET** /api/v1/projects/user/{registryId}/validated | Project@getValidatedProjects|

# **projectsDelete**
> projectsDelete()

Delete a user from a project

### Example

```typescript
import {
    ProjectsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectsApi(configuration);

let id: number; //ID (default to undefined)

const { status, data } = await apiInstance.projectsDelete(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | success |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | failed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectsGetValidatedProjects**
> OrganisationGetProjects200Response projectsGetValidatedProjects()

Return (approved) projects for a registry (user)

### Example

```typescript
import {
    ProjectsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectsApi(configuration);

let registryId: number; //Registry ID (default to undefined)

const { status, data } = await apiInstance.projectsGetValidatedProjects(
    registryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | Registry ID | defaults to undefined|


### Return type

**OrganisationGetProjects200Response**

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

