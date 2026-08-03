# ProjectHasOrganisationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectHasOrganisationShow**](#projecthasorganisationshow) | **GET** /api/v1/project-organisations/{projectOrganisationId} | Get details of a project-organisation relationship|

# **projectHasOrganisationShow**
> ProjectHasOrganisation projectHasOrganisationShow()


### Example

```typescript
import {
    ProjectHasOrganisationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectHasOrganisationApi(configuration);

let projectOrganisationId: number; //ID of the project-organisation relationship (default to undefined)

const { status, data } = await apiInstance.projectHasOrganisationShow(
    projectOrganisationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectOrganisationId** | [**number**] | ID of the project-organisation relationship | defaults to undefined|


### Return type

**ProjectHasOrganisation**

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
|**404** | Project-organisation relationship not found |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

