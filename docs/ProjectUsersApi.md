# ProjectUsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectUsersBulkInviteProjectUsers**](#projectusersbulkinviteprojectusers) | **POST** /api/v1/project_users/bulk | Bulk invite Project Users|

# **projectUsersBulkInviteProjectUsers**
> projectUsersBulkInviteProjectUsers(projectUsersBulkInviteProjectUsersRequest)

Invite multiple users and attach them to a project

### Example

```typescript
import {
    ProjectUsersApi,
    Configuration,
    ProjectUsersBulkInviteProjectUsersRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectUsersApi(configuration);

let projectUsersBulkInviteProjectUsersRequest: ProjectUsersBulkInviteProjectUsersRequest; //

const { status, data } = await apiInstance.projectUsersBulkInviteProjectUsers(
    projectUsersBulkInviteProjectUsersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectUsersBulkInviteProjectUsersRequest** | **ProjectUsersBulkInviteProjectUsersRequest**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

